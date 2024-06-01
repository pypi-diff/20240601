# Comparing `tmp/vitaldb-1.4.8-py3-none-any.whl.zip` & `tmp/vitaldb-1.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 56814 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   103238 b- defN 23-Nov-03 00:10 vitaldb/__init__.py
+Zip file size: 57542 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   103353 b- defN 24-Jun-01 00:02 vitaldb/__init__.py
 -rw-rw-rw-  2.0 fat     4653 b- defN 23-Jul-02 09:38 vitaldb/api.py
--rw-rw-rw-  2.0 fat     3305 b- defN 23-Jun-16 07:55 vitaldb/dataset.py
+-rw-rw-rw-  2.0 fat     6431 b- defN 24-Jun-01 00:02 vitaldb/dataset.py
 -rw-rw-rw-  2.0 fat    89543 b- defN 24-May-04 01:12 vitaldb/utils.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      520 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      682 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/RECORD
-9 files, 203126 bytes uncompressed, 55656 bytes compressed:  72.6%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Jun-01 09:35 vitaldb-1.4.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      520 b- defN 24-Jun-01 09:35 vitaldb-1.4.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 09:35 vitaldb-1.4.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Jun-01 09:35 vitaldb-1.4.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      682 b- defN 24-Jun-01 09:35 vitaldb-1.4.9.dist-info/RECORD
+9 files, 206367 bytes uncompressed, 56384 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vitaldb/dataset.py
 Comment: 
 
 Filename: vitaldb/utils.py
 Comment: 
 
-Filename: vitaldb-1.4.8.dist-info/LICENSE
+Filename: vitaldb-1.4.9.dist-info/LICENSE
 Comment: 
 
-Filename: vitaldb-1.4.8.dist-info/METADATA
+Filename: vitaldb-1.4.9.dist-info/METADATA
 Comment: 
 
-Filename: vitaldb-1.4.8.dist-info/WHEEL
+Filename: vitaldb-1.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: vitaldb-1.4.8.dist-info/top_level.txt
+Filename: vitaldb-1.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vitaldb-1.4.8.dist-info/RECORD
+Filename: vitaldb-1.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vitaldb/__init__.py

```diff
@@ -9,16 +9,19 @@
 from .utils import vital_recs
 from .utils import vital_trks
 from .utils import VitalFile
 from .utils import read_csv
 from .utils import read_vital
 from .utils import read_wfdb
 from .utils import read_parquet
+from .dataset import load_clinical_data
+from .dataset import load_lab_data
 from .dataset import load_case
 from .dataset import find_cases
+from .dataset import get_track_names
 
 # tname = 'BIS/BIS'
 # caseids = set()
 # for idx, row in df_trks[df_trks['tname'] == tname].iterrows():
 #     tid = row['tid']
 #     caseid = row['caseid']
 #     maxval = pd.read_csv('https://api.vitaldb.net/' + tid)[tname].max()
```

## vitaldb/dataset.py

```diff
@@ -1,19 +1,68 @@
 import numpy as np
 import pandas as pd
 
 # open dataset trks
+api_url = "https://api.vitaldb.net"
 dftrks = None
+dfci = None
+dflabs = None
+
+def load_clinical_data(caseids=[], params=[]):
+    """Load clinical information for the specified caseIDs and specified parameters into a dataframe.
+
+    Parameters:
+        caseids (list, optional): caseIDs from 1 to 6388. Defaults to [], which returns clinical information of all caseID.
+        params (list, optional): parameter list to filter clinical information. Please refer to "Parameter List" section from vitaldb.net/dataset Overview
+
+    Returns:
+        Dataframe: clinical information.
+    """
+    global dfci
+    if dfci is None:
+        dfci = pd.read_csv(f"{api_url}/cases")
+    
+    res = None
+    if not caseids:
+        res = dfci
+    res = dfci[dfci["caseid"].isin(caseids)]
+    if params:
+        existing_params = [param for param in params if param in dfci.columns]
+        res = res[existing_params]
+    return res
+
+def load_lab_data(caseids=[], params=[]):
+    """Load lab results for the specified caseIDs and specified parameters into a dataframe.
+
+    Parameters:
+        caseids (list, optional): caseIDs from 1 to 6388. Defaults to [], which returns lab results of all caseID.
+        params (list, optional): parameter list to filter lab results. Please refer to "Parameter List" section from vitaldb.net/dataset Overview
+
+    Returns:
+        Dataframe: lab results
+    """
+    global dflabs
+    if dflabs is None:
+        dflabs = pd.read_csv(f"{api_url}/labs")
+    
+    res = None
+    if not caseids:
+        res = dflabs
+    res = dflabs[dflabs["caseid"].isin(caseids)]
+    if params:
+        existing_params = [param for param in params if param in dfci.columns]
+        res = res[existing_params]
+    return res
 
 def load_trk(tid, interval=1):
     if isinstance(tid, list) or isinstance(tid, set) or isinstance(tid, tuple):
         return load_trks(tid, interval)
 
     try:
-        url = 'https://api.vitaldb.net/' + tid
+        url = f"{api_url}/{tid}"
         dtvals = pd.read_csv(url, na_values='-nan(ind)', dtype=np.float32).values
     except:
         return np.empty(0)
 
     if len(dtvals) == 0:
         return np.empty(0)
     
@@ -52,36 +101,68 @@
 
     for i in range(len(tids)):  # copy values
         if trks[i] is not None:
             ret[:len(trks[i]), i] = trks[i]
 
     return ret
 
+def get_track_names(caseids=[]):
+    """Return a list of track names of the specified caseIDs
+
+    Parameters:
+        caseids (list, optional): caseIDs from 1 to 6388. Defaults to [], which returns track names of all caseID.
+
+    Returns:
+        Dataframe: track names by caseID
+    """
+    global dftrks
+    if dftrks is None:
+        dftrks = pd.read_csv(f"{api_url}/trks")
+    
+    return dftrks[dftrks['caseid'].isin(caseids)].groupby('caseid')["tname"].apply(list).reset_index(name="tnames")
 
 def find_cases(track_names):
+    """Return a list of caseID for cases with the given tracklist.
+
+    Parameters:
+        track_names (list or string): a list of track names or a string with track names separated by comma
+
+    Returns:
+        List: caseIDs
+    """
     global dftrks
     if dftrks is None:
-        dftrks = pd.read_csv("https://api.vitaldb.net/trks")
+        dftrks = pd.read_csv(f"{api_url}/trks")
 
     if isinstance(track_names, str):
         if track_names.find(','):
             track_names = track_names.split(',')
         else:
             track_names = [track_names]
 
     return list(set.intersection(*[set(dftrks.loc[dftrks['tname'].str.endswith(dtname), 'caseid']) for dtname in track_names]))
 
 def load_case(caseid, track_names, interval=1):
+    """Load case data with the given track names in a 2D numpy array. Row by time and Column by track. 
+
+    Parameters:
+        caseid (int): caseID from 1 to 6388
+        track_names (list or string):  a list of track names or a string with track names separated by comma
+        interval (int, optional): time interval (= 1 / sample rate). Defaults to 1.
+
+    Returns:
+        ndarray: 2D numpy array. Row by time and Column by track. 
+    """
     global dftrks
 
     if not caseid:
         return None
 
     if dftrks is None:
-        dftrks = pd.read_csv("https://api.vitaldb.net/trks")
+        dftrks = pd.read_csv(f"{api_url}/trks")
 
     if isinstance(track_names, str):
         if track_names.find(','):
             track_names = track_names.split(',')
         else:
             track_names = [track_names]
 
@@ -93,24 +174,30 @@
         else:
             tids.append(None)
     
     return load_trks(tids, interval)
 
 
 if __name__ == '__main__':
-    vals = load_case(858, ['SNUADC/ECG_II', 'SNUADC/PLETH', 'BIS/EEG1_WAV', 'BIS/BIS'], 1/100)     
-    print(vals)
-    quit()
-
-    # caseids = find_cases(['ECG_II'])
-    # print(len(caseids))
+    # print(get_track_names([858, 859, 560]))
     # quit()
-    
-    vals = load_case(1, ['ECG_II', 'ART'])
-    print(vals)
+    # vals = load_case(858, ['SNUADC/ECG_II', 'SNUADC/PLETH', 'BIS/EEG1_WAV', 'BIS/BIS'], 1/100)
+    # print(type(vals))
+    ci = load_clinical_data()
+    print(ci)
+    # labs = load_lab_data([858, 859])
+    # print(labs)
+    # quit()
+
+    caseids = find_cases('ECG_II,PLETH')
+    print(type(caseids))
     quit()
-    vals = load_trks([
-        'eb1e6d9a963d7caab8f00993cd85bf31931b7a32',
-        '29cef7b8fe2cc84e69fd143da510949b3c271314',
-        '829134dd331e867598f17d81c1b31f5be85dddec'
-    ], 60)
-    print(vals)
+    
+    # vals = load_case(1, ['ECG_II', 'ART'])
+    # print(vals)
+    # quit()
+    # vals = load_trks([
+    #     'eb1e6d9a963d7caab8f00993cd85bf31931b7a32',
+    #     '29cef7b8fe2cc84e69fd143da510949b3c271314',
+    #     '829134dd331e867598f17d81c1b31f5be85dddec'
+    # ], 60)
+    # print(vals)
```

## Comparing `vitaldb-1.4.8.dist-info/LICENSE` & `vitaldb-1.4.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vitaldb-1.4.8.dist-info/METADATA` & `vitaldb-1.4.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitaldb
-Version: 1.4.8
+Version: 1.4.9
 Summary: VitalDB Python Libray
 Home-page: https://github.com/vitaldb/vitalutils
 Author: Hyung-Chul Lee
 Author-email: vital@snu.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `vitaldb-1.4.8.dist-info/RECORD` & `vitaldb-1.4.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-vitaldb/__init__.py,sha256=q-AbMSiCgHwv8c1hk2MKGpxVynKtrcJKzuOUHLw3on0,103238
+vitaldb/__init__.py,sha256=UYJ3KQ2Ze2UXLcIO-uxpGtrezFB7dVzp1sWz9_sthtE,103353
 vitaldb/api.py,sha256=Kdmz9GGHSqLrgIPyZX_EnoR0ritjdCiRAWKtsIbpguc,4653
-vitaldb/dataset.py,sha256=qlwphbk8ayfdMdPsQtHZNHfXQPYQtx0yC5QVCn66tVw,3305
+vitaldb/dataset.py,sha256=ovzMIK2i_7BP-qlNS9ixBYK2vNia1Fa3znZz5Py_fsk,6431
 vitaldb/utils.py,sha256=twyahnydSE8kTAEOz6YZjTxzscmhQBzz16LgXvKE_-o,89543
-vitaldb-1.4.8.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
-vitaldb-1.4.8.dist-info/METADATA,sha256=q6R5pN9jOVOAqmqFtGTl8IdeGUbGe5812CdhRsObb0s,520
-vitaldb-1.4.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-vitaldb-1.4.8.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
-vitaldb-1.4.8.dist-info/RECORD,,
+vitaldb-1.4.9.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
+vitaldb-1.4.9.dist-info/METADATA,sha256=dndjcvddKLHvHDOAciDnr1FRDQVvvzQpo0d1Hm9lyQc,520
+vitaldb-1.4.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+vitaldb-1.4.9.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
+vitaldb-1.4.9.dist-info/RECORD,,
```

