# Comparing `tmp/stable-ts-whisperless-2.17.2.tar.gz` & `tmp/stable-ts-whisperless-2.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-whisperless-2.17.2.tar", last modified: Tue May 14 02:23:31 2024, max compression
+gzip compressed data, was "stable-ts-whisperless-2.17.3.tar", last modified: Sat Jun  1 18:16:23 2024, max compression
```

## Comparing `stable-ts-whisperless-2.17.2.tar` & `stable-ts-whisperless-2.17.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.671008 stable-ts-whisperless-2.17.2/
--rw-rw-rw-   0        0        0     1082 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/LICENSE
--rw-rw-rw-   0        0        0    87743 2024-05-14 02:23:31.670008 stable-ts-whisperless-2.17.2/PKG-INFO
--rw-rw-rw-   0        0        0    87342 2024-05-14 00:42:59.000000 stable-ts-whisperless-2.17.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 02:23:31.671008 stable-ts-whisperless-2.17.2/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.669009 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/
--rw-rw-rw-   0        0        0    87743 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.644008 stable-ts-whisperless-2.17.2/stable_whisper/
--rw-rw-rw-   0        0        0      353 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       24 2024-05-14 00:50:46.000000 stable-ts-whisperless-2.17.2/stable_whisper/_version.py
--rw-rw-rw-   0        0        0    70716 2024-05-14 01:52:58.000000 stable-ts-whisperless-2.17.2/stable_whisper/alignment.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.653008 stable-ts-whisperless-2.17.2/stable_whisper/audio/
--rw-rw-rw-   0        0        0    24130 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/__init__.py
--rw-rw-rw-   0        0        0     7657 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/demucs.py
--rw-rw-rw-   0        0        0     3276 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/dfnet.py
--rw-rw-rw-   0        0        0     2952 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/noisereduce.py
--rw-rw-rw-   0        0        0     1977 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/output.py
--rw-rw-rw-   0        0        0     8761 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/utils.py
--rw-rw-rw-   0        0        0     4522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     2047 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/default.py
--rw-rw-rw-   0        0        0    16093 2024-05-14 01:08:23.000000 stable-ts-whisperless-2.17.2/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     2308 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0   103762 2024-05-14 02:04:09.000000 stable-ts-whisperless-2.17.2/stable_whisper/result.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.659010 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/
--rw-rw-rw-   0        0        0    18720 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/nonvad.py
--rw-rw-rw-   0        0        0     2246 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/silero_vad.py
--rw-rw-rw-   0        0        0     4491 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/utils.py
--rw-rw-rw-   0        0        0    24045 2024-05-13 21:51:05.000000 stable-ts-whisperless-2.17.2/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    11983 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2622 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/utils.py
--rw-rw-rw-   0        0        0     4020 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0     9426 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_compatibility.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.667008 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/
--rw-rw-rw-   0        0        0      454 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/__init__.py
--rw-rw-rw-   0        0        0    39229 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/cli.py
--rw-rw-rw-   0        0        0    11231 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/faster_whisper.py
--rw-rw-rw-   0        0        0     9957 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/hf_whisper.py
--rw-rw-rw-   0        0        0    42315 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/original_whisper.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.558727 stable-ts-whisperless-2.17.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/LICENSE
+-rw-rw-rw-   0        0        0    89132 2024-06-01 18:16:23.556725 stable-ts-whisperless-2.17.3/PKG-INFO
+-rw-rw-rw-   0        0        0    88731 2024-05-24 00:32:13.000000 stable-ts-whisperless-2.17.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 18:16:23.558727 stable-ts-whisperless-2.17.3/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.554724 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/
+-rw-rw-rw-   0        0        0    89132 2024-06-01 18:16:22.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2024-06-01 18:16:23.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 18:16:22.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-06-01 18:16:22.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-06-01 18:16:22.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 18:16:22.000000 stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.425973 stable-ts-whisperless-2.17.3/stable_whisper/
+-rw-rw-rw-   0        0        0      353 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       24 2024-06-01 18:03:22.000000 stable-ts-whisperless-2.17.3/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0    70716 2024-05-14 01:52:58.000000 stable-ts-whisperless-2.17.3/stable_whisper/alignment.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.476724 stable-ts-whisperless-2.17.3/stable_whisper/audio/
+-rw-rw-rw-   0        0        0    24130 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/__init__.py
+-rw-rw-rw-   0        0        0     7657 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/demucs.py
+-rw-rw-rw-   0        0        0     3276 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/dfnet.py
+-rw-rw-rw-   0        0        0     2952 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/noisereduce.py
+-rw-rw-rw-   0        0        0     1977 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/output.py
+-rw-rw-rw-   0        0        0     8761 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/audio/utils.py
+-rw-rw-rw-   0        0        0     4522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     2047 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/default.py
+-rw-rw-rw-   0        0        0    16096 2024-05-16 15:57:13.000000 stable-ts-whisperless-2.17.3/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     2308 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0   108321 2024-05-23 23:56:41.000000 stable-ts-whisperless-2.17.3/stable_whisper/result.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.509724 stable-ts-whisperless-2.17.3/stable_whisper/stabilization/
+-rw-rw-rw-   0        0        0    18720 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/stabilization/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/stabilization/nonvad.py
+-rw-rw-rw-   0        0        0     2246 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/stabilization/silero_vad.py
+-rw-rw-rw-   0        0        0     4491 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/stabilization/utils.py
+-rw-rw-rw-   0        0        0    24046 2024-05-24 04:35:24.000000 stable-ts-whisperless-2.17.3/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    11983 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2622 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/utils.py
+-rw-rw-rw-   0        0        0     4020 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0     9426 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_compatibility.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:16:23.552724 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/
+-rw-rw-rw-   0        0        0      454 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/__init__.py
+-rw-rw-rw-   0        0        0    39229 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/cli.py
+-rw-rw-rw-   0        0        0    11231 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/faster_whisper.py
+-rw-rw-rw-   0        0        0     9957 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/hf_whisper.py
+-rw-rw-rw-   0        0        0    42315 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/original_whisper.py
```

### Comparing `stable-ts-whisperless-2.17.2/LICENSE` & `stable-ts-whisperless-2.17.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/PKG-INFO` & `stable-ts-whisperless-2.17.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: stable-ts-whisperless
-Version: 2.17.2
-Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
-Home-page: https://github.com/jianfch/stable-ts
-Author: Jian
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: torch
-Requires-Dist: torchaudio
-Requires-Dist: tqdm
-
 # Stabilizing Timestamps for Whisper
 
 This library modifies [Whisper](https://github.com/openai/whisper) to produce more reliable timestamps and extends its functionality.
 
 https://github.com/jianfch/stable-ts/assets/28970749/7adf0540-3620-4b2b-b2d4-e316906d6dfa
 
 * [Setup](#setup)
@@ -1321,14 +1306,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1347,14 +1334,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1420,14 +1409,42 @@
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
+
+<details>
+<summary>pad()</summary>
+
+        Pad (in-place) timestamps in chronological order.
+
+        Parameters
+        ----------
+        start_pad : float, optional
+            Seconds to pad start timestamps.
+            Each start timestamp will be extended no earlier than the end timestamp of the previous word.
+        end_pad : float, optional
+            Seconds to pad end timestamps.
+            Each end timestamp will be extended no later than the start timestamp of the next word or ``max_end``.
+        max_dur : float, optional
+            Only pad segments or words (``word_level=True``) with duration (in seconds) under or equal to ``max_dur``.
+        max_end : float, optional
+            Timestamp (in seconds) that padded timestamps cannot exceed.
+            Generally used to prevent the last padded end timestamp from exceeding the total duration of the audio.
+        word_level : bool, default False
+            Whether to pad segment timestamps or word timestamps.
+
+        Returns
+        -------
+        stable_whisper.result.WhisperResult
+            The current instance after the changes.
+
+</details>
 
 ### Editing
 The editing methods in stable-ts can be chained with [Regrouping Methods](#regrouping-methods) and used in `regroup()`.
 
 Remove specific instances words or segments:
 ```python
 # Remove first word of the first segment:
```

### Comparing `stable-ts-whisperless-2.17.2/README.md` & `stable-ts-whisperless-2.17.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: stable-ts-whisperless
+Version: 2.17.3
+Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
+Home-page: https://github.com/jianfch/stable-ts
+Author: Jian
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torchaudio
+Requires-Dist: tqdm
+
 # Stabilizing Timestamps for Whisper
 
 This library modifies [Whisper](https://github.com/openai/whisper) to produce more reliable timestamps and extends its functionality.
 
 https://github.com/jianfch/stable-ts/assets/28970749/7adf0540-3620-4b2b-b2d4-e316906d6dfa
 
 * [Setup](#setup)
@@ -1306,14 +1321,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1332,14 +1349,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1405,14 +1424,42 @@
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
+
+<details>
+<summary>pad()</summary>
+
+        Pad (in-place) timestamps in chronological order.
+
+        Parameters
+        ----------
+        start_pad : float, optional
+            Seconds to pad start timestamps.
+            Each start timestamp will be extended no earlier than the end timestamp of the previous word.
+        end_pad : float, optional
+            Seconds to pad end timestamps.
+            Each end timestamp will be extended no later than the start timestamp of the next word or ``max_end``.
+        max_dur : float, optional
+            Only pad segments or words (``word_level=True``) with duration (in seconds) under or equal to ``max_dur``.
+        max_end : float, optional
+            Timestamp (in seconds) that padded timestamps cannot exceed.
+            Generally used to prevent the last padded end timestamp from exceeding the total duration of the audio.
+        word_level : bool, default False
+            Whether to pad segment timestamps or word timestamps.
+
+        Returns
+        -------
+        stable_whisper.result.WhisperResult
+            The current instance after the changes.
+
+</details>
 
 ### Editing
 The editing methods in stable-ts can be chained with [Regrouping Methods](#regrouping-methods) and used in `regroup()`.
 
 Remove specific instances words or segments:
 ```python
 # Remove first word of the first segment:
```

### Comparing `stable-ts-whisperless-2.17.2/setup.py` & `stable-ts-whisperless-2.17.3/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/PKG-INFO` & `stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.17.2
+Version: 2.17.3
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -1321,14 +1321,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1347,14 +1349,16 @@
         max_chars : int, optional
             Maximum number of characters allowed in each segment.
         is_sum_max : bool, default False
             Whether ``max_words`` and ``max_chars`` is applied to the merged segment instead of the individual segments
             to be merged.
         lock : bool, default False
             Whether to prevent future splits/merges from altering changes made by this method.
+        newline : bool, default False
+            Whether to insert a line break between the merged segments.
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
@@ -1420,14 +1424,42 @@
 
         Returns
         -------
         stable_whisper.result.WhisperResult
             The current instance after the changes.
 
 </details>
+
+<details>
+<summary>pad()</summary>
+
+        Pad (in-place) timestamps in chronological order.
+
+        Parameters
+        ----------
+        start_pad : float, optional
+            Seconds to pad start timestamps.
+            Each start timestamp will be extended no earlier than the end timestamp of the previous word.
+        end_pad : float, optional
+            Seconds to pad end timestamps.
+            Each end timestamp will be extended no later than the start timestamp of the next word or ``max_end``.
+        max_dur : float, optional
+            Only pad segments or words (``word_level=True``) with duration (in seconds) under or equal to ``max_dur``.
+        max_end : float, optional
+            Timestamp (in seconds) that padded timestamps cannot exceed.
+            Generally used to prevent the last padded end timestamp from exceeding the total duration of the audio.
+        word_level : bool, default False
+            Whether to pad segment timestamps or word timestamps.
+
+        Returns
+        -------
+        stable_whisper.result.WhisperResult
+            The current instance after the changes.
+
+</details>
 
 ### Editing
 The editing methods in stable-ts can be chained with [Regrouping Methods](#regrouping-methods) and used in `regroup()`.
 
 Remove specific instances words or segments:
 ```python
 # Remove first word of the first segment:
```

### Comparing `stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/SOURCES.txt` & `stable-ts-whisperless-2.17.3/stable_ts_whisperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/alignment.py` & `stable-ts-whisperless-2.17.3/stable_whisper/alignment.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/__init__.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/demucs.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/demucs.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/dfnet.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/dfnet.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/noisereduce.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/noisereduce.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/output.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/audio/utils.py` & `stable-ts-whisperless-2.17.3/stable_whisper/audio/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/decode.py` & `stable-ts-whisperless-2.17.3/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/default.py` & `stable-ts-whisperless-2.17.3/stable_whisper/default.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/non_whisper.py` & `stable-ts-whisperless-2.17.3/stable_whisper/non_whisper.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
             result = WhisperResult(result, force_order=force_order, check_sorted=check_sorted)
         if suppress_silence:
             result.adjust_by_silence(
                 audio, vad,
                 vad_onnx=vad_onnx, vad_threshold=vad_threshold,
                 q_levels=q_levels, k_size=k_size,
                 sample_rate=curr_audio_sr(True), min_word_dur=min_word_dur,
-                word_level=suppress_word_ts, verbose=True,
+                word_level=suppress_word_ts, verbose=verbose,
                 nonspeech_error=nonspeech_error,
                 use_word_position=use_word_position,
                 min_silence_dur=min_silence_dur
             )
             result.set_current_as_orig()
 
         if result.has_words and regroup:
```

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/quantization.py` & `stable-ts-whisperless-2.17.3/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/result.py` & `stable-ts-whisperless-2.17.3/stable_whisper/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,6223 +264,6508 @@
 00001070: 2d3e 2066 6c6f 6174 3a0d 0a20 2020 2020  -> float:..     
 00001080: 2020 2069 6620 6e6f 7420 7365 6c66 2e72     if not self.r
 00001090: 6f75 6e64 5f74 733a 0d0a 2020 2020 2020  ound_ts:..      
 000010a0: 2020 2020 2020 7265 7475 726e 2074 696d        return tim
 000010b0: 6573 7461 6d70 0d0a 2020 2020 2020 2020  estamp..        
 000010c0: 7265 7475 726e 205f 726f 756e 645f 7469  return _round_ti
 000010d0: 6d65 7374 616d 7028 7469 6d65 7374 616d  mestamp(timestam
-000010e0: 7029 0d0a 0d0a 2020 2020 4070 726f 7065  p)....    @prope
-000010f0: 7274 790d 0a20 2020 2064 6566 2073 7461  rty..    def sta
-00001100: 7274 2873 656c 6629 3a0d 0a20 2020 2020  rt(self):..     
-00001110: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00001120: 7374 6172 740d 0a0d 0a20 2020 2040 7072  start....    @pr
-00001130: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-00001140: 656e 6428 7365 6c66 293a 0d0a 2020 2020  end(self):..    
-00001150: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001160: 5f65 6e64 0d0a 0d0a 2020 2020 4073 7461  _end....    @sta
-00001170: 7274 2e73 6574 7465 720d 0a20 2020 2064  rt.setter..    d
-00001180: 6566 2073 7461 7274 2873 656c 662c 2076  ef start(self, v
-00001190: 616c 293a 0d0a 2020 2020 2020 2020 7365  al):..        se
-000011a0: 6c66 2e5f 7374 6172 7420 3d20 7365 6c66  lf._start = self
-000011b0: 2e72 6f75 6e64 2876 616c 290d 0a0d 0a20  .round(val).... 
-000011c0: 2020 2040 656e 642e 7365 7474 6572 0d0a     @end.setter..
-000011d0: 2020 2020 6465 6620 656e 6428 7365 6c66      def end(self
-000011e0: 2c20 7661 6c29 3a0d 0a20 2020 2020 2020  , val):..       
-000011f0: 2073 656c 662e 5f65 6e64 203d 2073 656c   self._end = sel
-00001200: 662e 726f 756e 6428 7661 6c29 0d0a 0d0a  f.round(val)....
-00001210: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00001220: 2020 2064 6566 2073 6567 6d65 6e74 5f69     def segment_i
-00001230: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
-00001240: 2020 7265 7475 726e 204e 6f6e 6520 6966    return None if
-00001250: 2073 656c 662e 7365 676d 656e 7420 6973   self.segment is
-00001260: 204e 6f6e 6520 656c 7365 2073 656c 662e   None else self.
-00001270: 7365 676d 656e 742e 6964 0d0a 0d0a 2020  segment.id....  
-00001280: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00001290: 2064 6566 2064 7572 6174 696f 6e28 7365   def duration(se
-000012a0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-000012b0: 7475 726e 2073 656c 662e 726f 756e 6428  turn self.round(
-000012c0: 7365 6c66 2e65 6e64 202d 2073 656c 662e  self.end - self.
-000012d0: 7374 6172 7429 0d0a 0d0a 2020 2020 6465  start)....    de
-000012e0: 6620 726f 756e 645f 616c 6c5f 7469 6d65  f round_all_time
-000012f0: 7374 616d 7073 2873 656c 6629 3a0d 0a20  stamps(self):.. 
-00001300: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00001310: 7761 726e 2827 6060 2e72 6f75 6e64 5f61  warn('``.round_a
-00001320: 6c6c 5f74 696d 6573 7461 6d70 7328 2960  ll_timestamps()`
-00001330: 6020 6973 2064 6570 7265 6361 7465 6420  ` is deprecated 
-00001340: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
-00001350: 7665 6420 696e 2066 7574 7572 6520 7665  ved in future ve
-00001360: 7273 696f 6e73 2e20 270d 0a20 2020 2020  rsions. '..     
-00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001380: 2027 5573 6520 6060 2e72 6f75 6e64 5f74   'Use ``.round_t
-00001390: 733d 5472 7565 6060 2074 6f20 726f 756e  s=True`` to roun
-000013a0: 6420 7469 6d65 7374 616d 7073 2062 7920  d timestamps by 
-000013b0: 6465 6661 756c 7420 696e 7374 6561 642e  default instead.
-000013c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000013d0: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
-000013e0: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
-000013f0: 2073 656c 662e 726f 756e 645f 7473 203d   self.round_ts =
-00001400: 2054 7275 650d 0a0d 0a20 2020 2064 6566   True....    def
-00001410: 206f 6666 7365 745f 7469 6d65 2873 656c   offset_time(sel
-00001420: 662c 206f 6666 7365 745f 7365 636f 6e64  f, offset_second
-00001430: 733a 2066 6c6f 6174 293a 0d0a 2020 2020  s: float):..    
-00001440: 2020 2020 7365 6c66 2e73 7461 7274 203d      self.start =
-00001450: 2073 656c 662e 7374 6172 7420 2b20 6f66   self.start + of
-00001460: 6673 6574 5f73 6563 6f6e 6473 0d0a 2020  fset_seconds..  
-00001470: 2020 2020 2020 7365 6c66 2e65 6e64 203d        self.end =
-00001480: 2073 656c 662e 656e 6420 2b20 6f66 6673   self.end + offs
-00001490: 6574 5f73 6563 6f6e 6473 0d0a 0d0a 2020  et_seconds....  
-000014a0: 2020 6465 6620 746f 5f64 6963 7428 7365    def to_dict(se
-000014b0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-000014c0: 7475 726e 2064 6963 7428 0d0a 2020 2020  turn dict(..    
-000014d0: 2020 2020 2020 2020 776f 7264 3d73 656c          word=sel
-000014e0: 662e 776f 7264 2c0d 0a20 2020 2020 2020  f.word,..       
-000014f0: 2020 2020 2073 7461 7274 3d73 656c 662e       start=self.
-00001500: 7374 6172 742c 0d0a 2020 2020 2020 2020  start,..        
-00001510: 2020 2020 656e 643d 7365 6c66 2e65 6e64      end=self.end
-00001520: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00001530: 726f 6261 6269 6c69 7479 3d73 656c 662e  robability=self.
-00001540: 7072 6f62 6162 696c 6974 792c 0d0a 2020  probability,..  
-00001550: 2020 2020 2020 2020 2020 746f 6b65 6e73            tokens
-00001560: 3d4e 6f6e 6520 6966 2073 656c 662e 746f  =None if self.to
-00001570: 6b65 6e73 2069 7320 4e6f 6e65 2065 6c73  kens is None els
-00001580: 6520 7365 6c66 2e74 6f6b 656e 732e 636f  e self.tokens.co
-00001590: 7079 2829 0d0a 2020 2020 2020 2020 290d  py()..        ).
-000015a0: 0a0d 0a20 2020 2064 6566 206c 6f63 6b5f  ...    def lock_
-000015b0: 6c65 6674 2873 656c 6629 3a0d 0a20 2020  left(self):..   
-000015c0: 2020 2020 2073 656c 662e 6c65 6674 5f6c       self.left_l
-000015d0: 6f63 6b65 6420 3d20 5472 7565 0d0a 0d0a  ocked = True....
-000015e0: 2020 2020 6465 6620 6c6f 636b 5f72 6967      def lock_rig
-000015f0: 6874 2873 656c 6629 3a0d 0a20 2020 2020  ht(self):..     
-00001600: 2020 2073 656c 662e 7269 6768 745f 6c6f     self.right_lo
-00001610: 636b 6564 203d 2054 7275 650d 0a0d 0a20  cked = True.... 
-00001620: 2020 2064 6566 206c 6f63 6b5f 626f 7468     def lock_both
-00001630: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001640: 2073 656c 662e 6c6f 636b 5f6c 6566 7428   self.lock_left(
-00001650: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00001660: 6c6f 636b 5f72 6967 6874 2829 0d0a 0d0a  lock_right()....
-00001670: 2020 2020 6465 6620 756e 6c6f 636b 5f62      def unlock_b
-00001680: 6f74 6828 7365 6c66 293a 0d0a 2020 2020  oth(self):..    
-00001690: 2020 2020 7365 6c66 2e6c 6566 745f 6c6f      self.left_lo
-000016a0: 636b 6564 203d 2046 616c 7365 0d0a 2020  cked = False..  
-000016b0: 2020 2020 2020 7365 6c66 2e72 6967 6874        self.right
-000016c0: 5f6c 6f63 6b65 6420 3d20 4661 6c73 650d  _locked = False.
-000016d0: 0a0d 0a20 2020 2064 6566 2073 7570 7072  ...    def suppr
-000016e0: 6573 735f 7369 6c65 6e63 6528 7365 6c66  ess_silence(self
-000016f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001700: 2020 2020 2020 2020 2020 2020 7369 6c65              sile
-00001710: 6e74 5f73 7461 7274 733a 206e 702e 6e64  nt_starts: np.nd
-00001720: 6172 7261 792c 0d0a 2020 2020 2020 2020  array,..        
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2073 696c 656e 745f 656e 6473 3a20 6e70   silent_ends: np
-00001750: 2e6e 6461 7272 6179 2c0d 0a20 2020 2020  .ndarray,..     
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
-00001780: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00001790: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2020 6e6f 6e73 7065 6563 685f 6572      nonspeech_er
-000017c0: 726f 723a 2066 6c6f 6174 203d 2030 2e33  ror: float = 0.3
-000017d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000017e0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
-000017f0: 5f65 6e64 3a20 4f70 7469 6f6e 616c 5b62  _end: Optional[b
-00001800: 6f6f 6c5d 203d 2054 7275 6529 3a0d 0a20  ool] = True):.. 
-00001810: 2020 2020 2020 2073 7570 7072 6573 735f         suppress_
-00001820: 7369 6c65 6e63 6528 7365 6c66 2c20 7369  silence(self, si
-00001830: 6c65 6e74 5f73 7461 7274 732c 2073 696c  lent_starts, sil
-00001840: 656e 745f 656e 6473 2c20 6d69 6e5f 776f  ent_ends, min_wo
-00001850: 7264 5f64 7572 2c20 6e6f 6e73 7065 6563  rd_dur, nonspeec
-00001860: 685f 6572 726f 722c 206b 6565 705f 656e  h_error, keep_en
-00001870: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
-00001880: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
-00001890: 6566 2072 6573 6361 6c65 5f74 696d 6528  ef rescale_time(
-000018a0: 7365 6c66 2c20 7363 616c 655f 6661 6374  self, scale_fact
-000018b0: 6f72 3a20 666c 6f61 7429 3a0d 0a20 2020  or: float):..   
-000018c0: 2020 2020 2073 656c 662e 7374 6172 7420       self.start 
-000018d0: 3d20 7365 6c66 2e73 7461 7274 202a 2073  = self.start * s
-000018e0: 6361 6c65 5f66 6163 746f 720d 0a20 2020  cale_factor..   
-000018f0: 2020 2020 2073 656c 662e 656e 6420 3d20       self.end = 
-00001900: 7365 6c66 2e65 6e64 202a 2073 6361 6c65  self.end * scale
-00001910: 5f66 6163 746f 720d 0a0d 0a20 2020 2064  _factor....    d
-00001920: 6566 2063 6c61 6d70 5f6d 6178 2873 656c  ef clamp_max(sel
-00001930: 662c 206d 6178 5f64 7572 3a20 666c 6f61  f, max_dur: floa
-00001940: 742c 2063 6c69 705f 7374 6172 743a 2062  t, clip_start: b
-00001950: 6f6f 6c20 3d20 4661 6c73 652c 2076 6572  ool = False, ver
-00001960: 626f 7365 3a20 626f 6f6c 203d 2046 616c  bose: bool = Fal
-00001970: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
-00001980: 2073 656c 662e 6475 7261 7469 6f6e 203e   self.duration >
-00001990: 206d 6178 5f64 7572 3a0d 0a20 2020 2020   max_dur:..     
-000019a0: 2020 2020 2020 2069 6620 636c 6970 5f73         if clip_s
-000019b0: 7461 7274 3a0d 0a20 2020 2020 2020 2020  tart:..         
-000019c0: 2020 2020 2020 206e 6577 5f73 7461 7274         new_start
-000019d0: 203d 2072 6f75 6e64 2873 656c 662e 656e   = round(self.en
-000019e0: 6420 2d20 6d61 785f 6475 722c 2033 290d  d - max_dur, 3).
-000019f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a00: 2069 6620 7665 7262 6f73 653a 0d0a 2020   if verbose:..  
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 7072 696e 7428 6627 5374 6172 743a    print(f'Start:
-00001a30: 207b 7365 6c66 2e73 7461 7274 7d20 2d3e   {self.start} ->
-00001a40: 207b 6e65 775f 7374 6172 747d 5c6e 456e   {new_start}\nEn
-00001a50: 643a 207b 7365 6c66 2e65 6e64 7d5c 6e54  d: {self.end}\nT
-00001a60: 6578 743a 227b 7365 6c66 2e77 6f72 647d  ext:"{self.word}
-00001a70: 225c 6e27 290d 0a20 2020 2020 2020 2020  "\n')..         
-00001a80: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
-00001a90: 7420 3d20 6e65 775f 7374 6172 740d 0a0d  t = new_start...
-00001aa0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00001ab0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001ac0: 2020 2020 6e65 775f 656e 6420 3d20 726f      new_end = ro
-00001ad0: 756e 6428 7365 6c66 2e73 7461 7274 202b  und(self.start +
-00001ae0: 206d 6178 5f64 7572 2c20 3329 0d0a 2020   max_dur, 3)..  
-00001af0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001b00: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001b20: 7269 6e74 2866 2753 7461 7274 3a20 7b73  rint(f'Start: {s
-00001b30: 656c 662e 7374 6172 747d 5c6e 456e 643a  elf.start}\nEnd:
-00001b40: 207b 7365 6c66 2e65 6e64 7d20 2d3e 207b   {self.end} -> {
-00001b50: 6e65 775f 656e 647d 5c6e 5465 7874 3a22  new_end}\nText:"
-00001b60: 7b73 656c 662e 776f 7264 7d22 5c6e 2729  {self.word}"\n')
-00001b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001b80: 2020 7365 6c66 2e65 6e64 203d 206e 6577    self.end = new
-00001b90: 5f65 6e64 0d0a 0d0a 2020 2020 6465 6620  _end....    def 
-00001ba0: 7365 745f 7365 676d 656e 7428 7365 6c66  set_segment(self
-00001bb0: 2c20 7365 676d 656e 743a 2027 5365 676d  , segment: 'Segm
-00001bc0: 656e 7427 293a 0d0a 2020 2020 2020 2020  ent'):..        
-00001bd0: 7761 726e 696e 6773 2e77 6172 6e28 2760  warnings.warn('`
-00001be0: 602e 7365 745f 7365 676d 656e 7428 6375  `.set_segment(cu
-00001bf0: 7272 656e 745f 7365 676d 656e 745f 696e  rrent_segment_in
-00001c00: 7374 616e 6365 2960 6020 6973 2064 6570  stance)`` is dep
-00001c10: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
-00001c20: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
-00001c30: 7574 7572 6520 7665 7273 696f 6e73 2e27  uture versions.'
-00001c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c50: 2020 2020 2020 2020 2720 5573 6520 6060          ' Use ``
-00001c60: 2e73 6567 6d65 6e74 203d 2063 7572 7265  .segment = curre
-00001c70: 6e74 5f73 6567 6d65 6e74 6060 2069 6e73  nt_segment`` ins
-00001c80: 7465 6164 2e27 2c0d 0a20 2020 2020 2020  tead.',..       
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001ca0: 7461 636b 6c65 7665 6c3d 3229 0d0a 2020  tacklevel=2)..  
-00001cb0: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
-00001cc0: 6e74 203d 2073 6567 6d65 6e74 0d0a 0d0a  nt = segment....
-00001cd0: 2020 2020 6465 6620 6765 745f 7365 676d      def get_segm
-00001ce0: 656e 7428 7365 6c66 2920 2d3e 2055 6e69  ent(self) -> Uni
-00001cf0: 6f6e 5b27 5365 676d 656e 7427 2c20 4e6f  on['Segment', No
-00001d00: 6e65 5d3a 0d0a 2020 2020 2020 2020 2222  ne]:..        ""
-00001d10: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
-00001d20: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
-00001d30: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
-00001d40: 7370 6572 2e72 6573 756c 742e 5365 676d  sper.result.Segm
-00001d50: 656e 7460 2074 6861 7420 7468 6973 2069  ent` that this i
-00001d60: 6e73 7461 6e63 6520 6973 2061 2070 6172  nstance is a par
-00001d70: 7420 6f66 2e0d 0a20 2020 2020 2020 2022  t of...        "
-00001d80: 2222 0d0a 2020 2020 2020 2020 7761 726e  ""..        warn
-00001d90: 696e 6773 2e77 6172 6e28 2760 602e 6765  ings.warn('``.ge
-00001da0: 745f 7365 676d 656e 7428 2960 6020 7769  t_segment()`` wi
-00001db0: 6c6c 2062 6520 7265 6d6f 7665 6420 696e  ll be removed in
-00001dc0: 2066 7574 7572 6520 7665 7273 696f 6e73   future versions
-00001dd0: 2e20 5573 6520 6060 2e73 6567 6d65 6e74  . Use ``.segment
-00001de0: 6060 2069 6e73 7465 6164 2e27 2c0d 0a20  `` instead.',.. 
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 2073 7461 636b 6c65 7665 6c3d       stacklevel=
-00001e10: 3229 0d0a 2020 2020 2020 2020 7265 7475  2)..        retu
-00001e20: 726e 2073 656c 662e 7365 676d 656e 740d  rn self.segment.
-00001e30: 0a0d 0a0d 0a64 6566 205f 776f 7264 735f  .....def _words_
-00001e40: 6279 5f6c 6f63 6b28 776f 7264 733a 204c  by_lock(words: L
-00001e50: 6973 745b 576f 7264 5469 6d69 6e67 5d2c  ist[WordTiming],
-00001e60: 206f 6e6c 795f 7465 7874 3a20 626f 6f6c   only_text: bool
-00001e70: 203d 2046 616c 7365 2c20 696e 636c 7564   = False, includ
-00001e80: 655f 7369 6e67 6c65 3a20 626f 6f6c 203d  e_single: bool =
-00001e90: 2046 616c 7365 293a 0d0a 2020 2020 2222   False):..    ""
-00001ea0: 220d 0a20 2020 2052 6574 7572 6e20 6120  "..    Return a 
-00001eb0: 6e65 7374 6564 206c 6973 7420 6f66 2077  nested list of w
-00001ec0: 6f72 6473 2073 7563 6820 7468 6174 2065  ords such that e
-00001ed0: 6163 6820 7375 626c 6973 7420 636f 6e74  ach sublist cont
-00001ee0: 6169 6e73 2077 6f72 6473 2074 6861 7420  ains words that 
-00001ef0: 6172 6520 6c6f 636b 6564 2074 6f67 6574  are locked toget
-00001f00: 6865 722e 0d0a 2020 2020 2222 220d 0a20  her...    """.. 
-00001f10: 2020 2061 6c6c 5f77 6f72 6473 203d 205b     all_words = [
-00001f20: 5d0d 0a20 2020 2066 6f72 2077 6f72 6420  ]..    for word 
-00001f30: 696e 2077 6f72 6473 3a0d 0a20 2020 2020  in words:..     
-00001f40: 2020 2069 6620 6c65 6e28 616c 6c5f 776f     if len(all_wo
-00001f50: 7264 7329 203d 3d20 3020 6f72 206e 6f74  rds) == 0 or not
-00001f60: 2028 616c 6c5f 776f 7264 735b 2d31 5d5b   (all_words[-1][
-00001f70: 2d31 5d2e 7269 6768 745f 6c6f 636b 6564  -1].right_locked
-00001f80: 206f 7220 776f 7264 2e6c 6566 745f 6c6f   or word.left_lo
-00001f90: 636b 6564 293a 0d0a 2020 2020 2020 2020  cked):..        
-00001fa0: 2020 2020 616c 6c5f 776f 7264 732e 6170      all_words.ap
-00001fb0: 7065 6e64 285b 776f 7264 5d29 0d0a 2020  pend([word])..  
-00001fc0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00001fd0: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
-00001fe0: 6473 5b2d 315d 2e61 7070 656e 6428 776f  ds[-1].append(wo
-00001ff0: 7264 290d 0a20 2020 2069 6620 6f6e 6c79  rd)..    if only
-00002000: 5f74 6578 743a 0d0a 2020 2020 2020 2020  _text:..        
-00002010: 616c 6c5f 776f 7264 7320 3d20 6c69 7374  all_words = list
-00002020: 286d 6170 286c 616d 6264 6120 7773 3a20  (map(lambda ws: 
-00002030: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
-00002040: 773a 2077 2e77 6f72 642c 2077 7329 292c  w: w.word, ws)),
-00002050: 2061 6c6c 5f77 6f72 6473 2929 0d0a 2020   all_words))..  
-00002060: 2020 6966 206e 6f74 2069 6e63 6c75 6465    if not include
-00002070: 5f73 696e 676c 653a 0d0a 2020 2020 2020  _single:..      
-00002080: 2020 616c 6c5f 776f 7264 7320 3d20 5b77    all_words = [w
-00002090: 7320 666f 7220 7773 2069 6e20 616c 6c5f  s for ws in all_
-000020a0: 776f 7264 7320 6966 206c 656e 2877 7329  words if len(ws)
-000020b0: 203e 2031 5d0d 0a20 2020 2072 6574 7572   > 1]..    retur
-000020c0: 6e20 616c 6c5f 776f 7264 730d 0a0d 0a0d  n all_words.....
-000020d0: 0a63 6c61 7373 2053 6567 6d65 6e74 3a0d  .class Segment:.
-000020e0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-000020f0: 745f 5f28 0d0a 2020 2020 2020 2020 2020  t__(..          
-00002100: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00002110: 2020 2020 2073 7461 7274 3a20 4f70 7469       start: Opti
-00002120: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-00002130: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00002140: 2065 6e64 3a20 4f70 7469 6f6e 616c 5b66   end: Optional[f
-00002150: 6c6f 6174 5d20 3d20 4e6f 6e65 2c0d 0a20  loat] = None,.. 
-00002160: 2020 2020 2020 2020 2020 2074 6578 743a             text:
-00002170: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00002180: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00002190: 2020 2020 7365 656b 3a20 4f70 7469 6f6e      seek: Option
-000021a0: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
-000021b0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-000021c0: 6f6b 656e 733a 204c 6973 745b 696e 745d  okens: List[int]
-000021d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-000021e0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-000021f0: 653a 204f 7074 696f 6e61 6c5b 666c 6f61  e: Optional[floa
-00002200: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
-00002210: 2020 2020 2020 2020 6176 675f 6c6f 6770          avg_logp
-00002220: 726f 623a 204f 7074 696f 6e61 6c5b 666c  rob: Optional[fl
-00002230: 6f61 745d 203d 204e 6f6e 652c 0d0a 2020  oat] = None,..  
-00002240: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
-00002250: 7373 696f 6e5f 7261 7469 6f3a 204f 7074  ssion_ratio: Opt
-00002260: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
-00002270: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00002280: 2020 6e6f 5f73 7065 6563 685f 7072 6f62    no_speech_prob
-00002290: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-000022a0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-000022b0: 2020 2020 2020 2077 6f72 6473 3a20 4f70         words: Op
-000022c0: 7469 6f6e 616c 5b55 6e69 6f6e 5b4c 6973  tional[Union[Lis
-000022d0: 745b 576f 7264 5469 6d69 6e67 5d2c 204c  t[WordTiming], L
-000022e0: 6973 745b 6469 6374 5d5d 5d20 3d20 4e6f  ist[dict]]] = No
-000022f0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00002300: 2069 643a 204f 7074 696f 6e61 6c5b 696e   id: Optional[in
-00002310: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
-00002320: 2020 2020 2020 2020 7265 7375 6c74 3a20          result: 
-00002330: 4f70 7469 6f6e 616c 5b22 5768 6973 7065  Optional["Whispe
-00002340: 7252 6573 756c 7422 5d20 3d20 4e6f 6e65  rResult"] = None
-00002350: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00002360: 6f75 6e64 5f74 733a 2062 6f6f 6c20 3d20  ound_ts: bool = 
-00002370: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00002380: 2020 2069 676e 6f72 655f 756e 7573 6564     ignore_unused
-00002390: 5f61 7267 733a 2062 6f6f 6c20 3d20 4661  _args: bool = Fa
-000023a0: 6c73 650d 0a20 2020 2029 3a0d 0a20 2020  lse..    ):..   
-000023b0: 2020 2020 2069 6620 776f 7264 733a 0d0a       if words:..
-000023c0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000023d0: 676e 6f72 655f 756e 7573 6564 5f61 7267  gnore_unused_arg
-000023e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000023f0: 2020 2020 7374 6172 7420 3d20 656e 6420      start = end 
-00002400: 3d20 7465 7874 203d 2074 6f6b 656e 7320  = text = tokens 
-00002410: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00002420: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002430: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-00002440: 7461 7274 206f 7220 656e 6429 2069 7320  tart or end) is 
-00002450: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00002460: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00002470: 6172 6e69 6e67 732e 7761 726e 2827 4172  arnings.warn('Ar
-00002480: 6775 6d65 6e74 7320 666f 7220 6060 7374  guments for ``st
-00002490: 6172 7460 6020 616e 6420 6060 656e 6460  art`` and ``end`
-000024a0: 6020 7769 6c6c 2062 6520 6967 6e6f 7265  ` will be ignore
-000024b0: 6420 270d 0a20 2020 2020 2020 2020 2020  d '..           
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2020 2020 2027 616e 6420 7468 6520         'and the 
-000024e0: 6060 7374 6172 7460 6020 616e 6420 6060  ``start`` and ``
-000024f0: 656e 6460 6020 7769 6c6c 2074 616b 656e  end`` will taken
-00002500: 2066 726f 6d20 7468 6520 6669 7273 7420   from the first 
-00002510: 616e 6420 6c61 7374 2060 6077 6f72 6473  and last ``words
-00002520: 6060 2e27 2c0d 0a20 2020 2020 2020 2020  ``.',..         
-00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002540: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
-00002550: 7665 6c3d 3229 0d0a 2020 2020 2020 2020  vel=2)..        
-00002560: 2020 2020 2020 2020 6966 2074 6578 7420          if text 
-00002570: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-000025a0: 2754 6865 2061 7267 756d 656e 7420 666f  'The argument fo
-000025b0: 7220 6060 7465 7874 6060 2077 696c 6c20  r ``text`` will 
-000025c0: 6265 2069 676e 6f72 6564 2027 0d0a 2020  be ignored '..  
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2761 6e64 2069 7420 7769 6c6c 2061 6c77  'and it will alw
-00002600: 6179 7320 6265 2074 6865 2063 6f6e 6361  ays be the conca
-00002610: 7465 6e61 7469 6f6e 206f 6620 7465 7874  tenation of text
-00002620: 2069 6e20 6060 776f 7264 7360 6027 2c0d   in ``words``',.
-00002630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 2020 2073 7461 636b 6c65 7665 6c3d 3229     stacklevel=2)
-00002660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002670: 2020 6966 2074 6f6b 656e 7320 6973 206e    if tokens is n
-00002680: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00002690: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-000026a0: 726e 696e 6773 2e77 6172 6e28 2754 6865  rnings.warn('The
-000026b0: 2061 7267 756d 656e 7420 666f 7220 6060   argument for ``
-000026c0: 746f 6b65 6e73 6060 2077 696c 6c20 6265  tokens`` will be
-000026d0: 2069 676e 6f72 6564 2027 0d0a 2020 2020   ignored '..    
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00002700: 6e64 2069 7420 7769 6c6c 2061 6c77 6179  nd it will alway
-00002710: 7320 6265 2074 6865 2063 6f6e 6361 7465  s be the concate
-00002720: 6e61 7469 6f6e 206f 6620 746f 6b65 6e73  nation of tokens
-00002730: 2069 6e20 6060 776f 7264 7360 6027 2c0d   in ``words``',.
-00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 2073 7461 636b 6c65 7665 6c3d 3229     stacklevel=2)
-00002770: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00002780: 6f75 6e64 5f74 7320 3d20 726f 756e 645f  ound_ts = round_
-00002790: 7473 0d0a 2020 2020 2020 2020 7365 6c66  ts..        self
-000027a0: 2e5f 6465 6661 756c 745f 7374 6172 7420  ._default_start 
-000027b0: 3d20 7365 6c66 2e72 6f75 6e64 2873 7461  = self.round(sta
-000027c0: 7274 2920 6966 2073 7461 7274 2065 6c73  rt) if start els
-000027d0: 6520 302e 300d 0a20 2020 2020 2020 2073  e 0.0..        s
-000027e0: 656c 662e 5f64 6566 6175 6c74 5f65 6e64  elf._default_end
-000027f0: 203d 2073 656c 662e 726f 756e 6428 656e   = self.round(en
-00002800: 6429 2069 6620 656e 6420 656c 7365 2030  d) if end else 0
-00002810: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
-00002820: 2e5f 6465 6661 756c 745f 7465 7874 203d  ._default_text =
-00002830: 2074 6578 7420 6f72 2027 270d 0a20 2020   text or ''..   
-00002840: 2020 2020 2073 656c 662e 5f64 6566 6175       self._defau
-00002850: 6c74 5f74 6f6b 656e 7320 3d20 746f 6b65  lt_tokens = toke
-00002860: 6e73 206f 7220 5b5d 0d0a 2020 2020 2020  ns or []..      
-00002870: 2020 7365 6c66 2e73 6565 6b20 3d20 7365    self.seek = se
-00002880: 656b 0d0a 2020 2020 2020 2020 7365 6c66  ek..        self
-00002890: 2e74 656d 7065 7261 7475 7265 203d 2074  .temperature = t
-000028a0: 656d 7065 7261 7475 7265 0d0a 2020 2020  emperature..    
-000028b0: 2020 2020 7365 6c66 2e61 7667 5f6c 6f67      self.avg_log
-000028c0: 7072 6f62 203d 2061 7667 5f6c 6f67 7072  prob = avg_logpr
-000028d0: 6f62 0d0a 2020 2020 2020 2020 7365 6c66  ob..        self
-000028e0: 2e63 6f6d 7072 6573 7369 6f6e 5f72 6174  .compression_rat
-000028f0: 696f 203d 2063 6f6d 7072 6573 7369 6f6e  io = compression
-00002900: 5f72 6174 696f 0d0a 2020 2020 2020 2020  _ratio..        
-00002910: 7365 6c66 2e6e 6f5f 7370 6565 6368 5f70  self.no_speech_p
-00002920: 726f 6220 3d20 6e6f 5f73 7065 6563 685f  rob = no_speech_
-00002930: 7072 6f62 0d0a 2020 2020 2020 2020 7365  prob..        se
-00002940: 6c66 2e77 6f72 6473 203d 2077 6f72 6473  lf.words = words
-00002950: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00002960: 662e 776f 7264 7320 616e 6420 6973 696e  f.words and isin
-00002970: 7374 616e 6365 2877 6f72 6473 5b30 5d2c  stance(words[0],
-00002980: 2064 6963 7429 3a0d 0a20 2020 2020 2020   dict):..       
-00002990: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
-000029a0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-000029b0: 2020 2020 2057 6f72 6454 696d 696e 6728       WordTiming(
-000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000029d0: 2020 2020 2020 2a2a 776f 7264 2c0d 0a20        **word,.. 
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2073 6567 6d65 6e74 3d73 656c 662c     segment=self,
-00002a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002a10: 2020 2020 2020 726f 756e 645f 7473 3d73        round_ts=s
-00002a20: 656c 662e 726f 756e 645f 7473 2c0d 0a20  elf.round_ts,.. 
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2069 676e 6f72 655f 756e 7573 6564     ignore_unused
-00002a50: 5f61 7267 733d 5472 7565 0d0a 2020 2020  _args=True..    
-00002a60: 2020 2020 2020 2020 2020 2020 2920 666f              ) fo
-00002a70: 7220 776f 7264 2069 6e20 7365 6c66 2e77  r word in self.w
-00002a80: 6f72 6473 0d0a 2020 2020 2020 2020 2020  ords..          
-00002a90: 2020 5d0d 0a20 2020 2020 2020 2073 656c    ]..        sel
-00002aa0: 662e 6964 203d 2069 640d 0a20 2020 2020  f.id = id..     
-00002ab0: 2020 2073 656c 662e 5f72 6576 6572 7365     self._reverse
-00002ac0: 645f 7465 7874 203d 2046 616c 7365 0d0a  d_text = False..
-00002ad0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00002ae0: 756c 7420 3d20 7265 7375 6c74 0d0a 0d0a  ult = result....
-00002af0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00002b00: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002b10: 2072 6574 7572 6e20 6627 5365 676d 656e   return f'Segmen
-00002b20: 7428 7374 6172 743d 7b73 656c 662e 7374  t(start={self.st
-00002b30: 6172 747d 2c20 656e 643d 7b73 656c 662e  art}, end={self.
-00002b40: 656e 647d 2c20 7465 7874 3d22 7b73 656c  end}, text="{sel
-00002b50: 662e 7465 7874 7d22 2927 0d0a 0d0a 2020  f.text}")'....  
-00002b60: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
-00002b70: 5f28 7365 6c66 2c20 696e 6465 783a 2069  _(self, index: i
-00002b80: 6e74 2920 2d3e 2057 6f72 6454 696d 696e  nt) -> WordTimin
-00002b90: 673a 0d0a 2020 2020 2020 2020 6966 2073  g:..        if s
-00002ba0: 656c 662e 776f 7264 7320 6973 204e 6f6e  elf.words is Non
-00002bb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002bc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00002bd0: 2827 7365 676d 656e 7420 636f 6e74 6169  ('segment contai
-00002be0: 6e73 206e 6f20 776f 7264 7327 290d 0a20  ns no words').. 
-00002bf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00002c00: 6c66 2e77 6f72 6473 5b69 6e64 6578 5d0d  lf.words[index].
-00002c10: 0a0d 0a20 2020 2064 6566 205f 5f64 656c  ...    def __del
-00002c20: 6974 656d 5f5f 2873 656c 662c 2069 6e64  item__(self, ind
-00002c30: 6578 3a20 696e 7429 3a0d 0a20 2020 2020  ex: int):..     
-00002c40: 2020 2069 6620 7365 6c66 2e77 6f72 6473     if self.words
-00002c50: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00002c60: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00002c70: 7565 4572 726f 7228 2773 6567 6d65 6e74  ueError('segment
-00002c80: 2063 6f6e 7461 696e 7320 6e6f 2077 6f72   contains no wor
-00002c90: 6473 2729 0d0a 2020 2020 2020 2020 6465  ds')..        de
-00002ca0: 6c20 7365 6c66 2e77 6f72 6473 5b69 6e64  l self.words[ind
-00002cb0: 6578 5d0d 0a20 2020 2020 2020 2073 656c  ex]..        sel
-00002cc0: 662e 7265 6173 7369 676e 5f69 6473 2869  f.reassign_ids(i
-00002cd0: 6e64 6578 290d 0a0d 0a20 2020 2064 6566  ndex)....    def
-00002ce0: 205f 5f64 6565 7063 6f70 795f 5f28 7365   __deepcopy__(se
-00002cf0: 6c66 2c20 6d65 6d6f 3d4e 6f6e 6529 3a0d  lf, memo=None):.
-00002d00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002d10: 7365 6c66 2e63 6f70 7928 636f 7079 5f77  self.copy(copy_w
-00002d20: 6f72 6473 3d54 7275 652c 2063 6f70 795f  ords=True, copy_
-00002d30: 746f 6b65 6e73 3d54 7275 6529 0d0a 0d0a  tokens=True)....
-00002d40: 2020 2020 6465 6620 5f5f 636f 7079 5f5f      def __copy__
-00002d50: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002d60: 2072 6574 7572 6e20 7365 6c66 2e63 6f70   return self.cop
-00002d70: 7928 290d 0a0d 0a20 2020 2064 6566 2063  y()....    def c
-00002d80: 6f70 7928 0d0a 2020 2020 2020 2020 2020  opy(..          
-00002d90: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00002da0: 2020 2020 206e 6577 5f77 6f72 6473 3a20       new_words: 
-00002db0: 4f70 7469 6f6e 616c 5b4c 6973 745b 576f  Optional[List[Wo
-00002dc0: 7264 5469 6d69 6e67 5d5d 203d 204e 6f6e  rdTiming]] = Non
-00002dd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002de0: 6b65 6570 5f72 6573 756c 743a 2062 6f6f  keep_result: boo
-00002df0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00002e00: 2020 2020 2020 2020 636f 7079 5f77 6f72          copy_wor
-00002e10: 6473 3a20 626f 6f6c 203d 2046 616c 7365  ds: bool = False
-00002e20: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00002e30: 6f70 795f 746f 6b65 6e73 3a20 626f 6f6c  opy_tokens: bool
-00002e40: 203d 2046 616c 7365 0d0a 2020 2020 293a   = False..    ):
-00002e50: 0d0a 2020 2020 2020 2020 6966 206e 6577  ..        if new
-00002e60: 5f77 6f72 6473 2069 7320 4e6f 6e65 3a0d  _words is None:.
-00002e70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002e80: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
-00002e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ea0: 2077 6f72 6473 203d 205b 772e 636f 7079   words = [w.copy
-00002eb0: 2863 6f70 795f 746f 6b65 6e73 3d63 6f70  (copy_tokens=cop
-00002ec0: 795f 746f 6b65 6e73 2920 666f 7220 7720  y_tokens) for w 
-00002ed0: 696e 2073 656c 662e 776f 7264 735d 2069  in self.words] i
-00002ee0: 6620 636f 7079 5f77 6f72 6473 2065 6c73  f copy_words els
-00002ef0: 6520 7365 6c66 2e77 6f72 6473 0d0a 2020  e self.words..  
-00002f00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00002f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f20: 2077 6f72 6473 203d 204e 6f6e 650d 0a20   words = None.. 
-00002f30: 2020 2020 2020 2020 2020 2064 6566 5f73             def_s
-00002f40: 7461 7274 203d 2073 656c 662e 5f64 6566  tart = self._def
-00002f50: 6175 6c74 5f73 7461 7274 0d0a 2020 2020  ault_start..    
-00002f60: 2020 2020 2020 2020 6465 665f 656e 6420          def_end 
-00002f70: 3d20 7365 6c66 2e5f 6465 6661 756c 745f  = self._default_
-00002f80: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-00002f90: 2064 6566 5f74 6578 7420 3d20 7365 6c66   def_text = self
-00002fa0: 2e5f 6465 6661 756c 745f 7465 7874 0d0a  ._default_text..
-00002fb0: 2020 2020 2020 2020 2020 2020 6465 665f              def_
-00002fc0: 746f 6b65 6e73 203d 2073 656c 662e 5f64  tokens = self._d
-00002fd0: 6566 6175 6c74 5f74 6f6b 656e 730d 0a20  efault_tokens.. 
-00002fe0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00002ff0: 2020 2020 2020 2020 2020 776f 7264 7320            words 
-00003000: 3d20 5b77 2e63 6f70 7928 636f 7079 5f74  = [w.copy(copy_t
-00003010: 6f6b 656e 733d 636f 7079 5f74 6f6b 656e  okens=copy_token
-00003020: 7329 2066 6f72 2077 2069 6e20 6e65 775f  s) for w in new_
-00003030: 776f 7264 735d 2069 6620 636f 7079 5f77  words] if copy_w
-00003040: 6f72 6473 2065 6c73 6520 6e65 775f 776f  ords else new_wo
-00003050: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
-00003060: 2064 6566 5f73 7461 7274 203d 2064 6566   def_start = def
-00003070: 5f65 6e64 203d 2064 6566 5f74 6578 7420  _end = def_text 
-00003080: 3d20 6465 665f 746f 6b65 6e73 203d 204e  = def_tokens = N
-00003090: 6f6e 650d 0a20 2020 2020 2020 206e 6577  one..        new
-000030a0: 5f73 6567 203d 2053 6567 6d65 6e74 280d  _seg = Segment(.
-000030b0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-000030c0: 7274 3d64 6566 5f73 7461 7274 2c0d 0a20  rt=def_start,.. 
-000030d0: 2020 2020 2020 2020 2020 2065 6e64 3d64             end=d
-000030e0: 6566 5f65 6e64 2c0d 0a20 2020 2020 2020  ef_end,..       
-000030f0: 2020 2020 2074 6578 743d 6465 665f 7465       text=def_te
-00003100: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-00003110: 2073 6565 6b3d 7365 6c66 2e73 6565 6b2c   seek=self.seek,
-00003120: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-00003130: 6b65 6e73 3d64 6566 5f74 6f6b 656e 732c  kens=def_tokens,
-00003140: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00003150: 6d70 6572 6174 7572 653d 7365 6c66 2e74  mperature=self.t
-00003160: 656d 7065 7261 7475 7265 2c0d 0a20 2020  emperature,..   
-00003170: 2020 2020 2020 2020 2061 7667 5f6c 6f67           avg_log
-00003180: 7072 6f62 3d73 656c 662e 6176 675f 6c6f  prob=self.avg_lo
-00003190: 6770 726f 622c 0d0a 2020 2020 2020 2020  gprob,..        
-000031a0: 2020 2020 636f 6d70 7265 7373 696f 6e5f      compression_
-000031b0: 7261 7469 6f3d 7365 6c66 2e63 6f6d 7072  ratio=self.compr
-000031c0: 6573 7369 6f6e 5f72 6174 696f 2c0d 0a20  ession_ratio,.. 
-000031d0: 2020 2020 2020 2020 2020 206e 6f5f 7370             no_sp
-000031e0: 6565 6368 5f70 726f 623d 7365 6c66 2e6e  eech_prob=self.n
-000031f0: 6f5f 7370 6565 6368 5f70 726f 622c 0d0a  o_speech_prob,..
-00003200: 2020 2020 2020 2020 2020 2020 776f 7264              word
-00003210: 733d 776f 7264 732c 0d0a 2020 2020 2020  s=words,..      
-00003220: 2020 2020 2020 6964 3d73 656c 662e 6964        id=self.id
-00003230: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00003240: 6573 756c 743d 7365 6c66 2e72 6573 756c  esult=self.resul
-00003250: 7420 6966 206b 6565 705f 7265 7375 6c74  t if keep_result
-00003260: 2065 6c73 6520 4e6f 6e65 2c0d 0a20 2020   else None,..   
-00003270: 2020 2020 2020 2020 2072 6f75 6e64 5f74           round_t
-00003280: 733d 7365 6c66 2e72 6f75 6e64 5f74 732c  s=self.round_ts,
-00003290: 0d0a 2020 2020 2020 2020 2020 2020 6967  ..            ig
-000032a0: 6e6f 7265 5f75 6e75 7365 645f 6172 6773  nore_unused_args
-000032b0: 3d54 7275 650d 0a20 2020 2020 2020 2029  =True..        )
-000032c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000032d0: 206e 6577 5f73 6567 0d0a 0d0a 2020 2020   new_seg....    
-000032e0: 6465 6620 726f 756e 6428 7365 6c66 2c20  def round(self, 
-000032f0: 7469 6d65 7374 616d 703a 2066 6c6f 6174  timestamp: float
-00003300: 2920 2d3e 2066 6c6f 6174 3a0d 0a20 2020  ) -> float:..   
-00003310: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00003320: 2e72 6f75 6e64 5f74 733a 0d0a 2020 2020  .round_ts:..    
-00003330: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00003340: 696d 6573 7461 6d70 0d0a 2020 2020 2020  imestamp..      
-00003350: 2020 7265 7475 726e 205f 726f 756e 645f    return _round_
-00003360: 7469 6d65 7374 616d 7028 7469 6d65 7374  timestamp(timest
-00003370: 616d 7029 0d0a 0d0a 2020 2020 6465 6620  amp)....    def 
-00003380: 746f 5f64 6973 706c 6179 5f73 7472 2873  to_display_str(s
-00003390: 656c 662c 206f 6e6c 795f 7365 676d 656e  elf, only_segmen
-000033a0: 743a 2062 6f6f 6c20 3d20 4661 6c73 6529  t: bool = False)
-000033b0: 3a0d 0a20 2020 2020 2020 206c 696e 6520  :..        line 
-000033c0: 3d20 6627 5b7b 666f 726d 6174 5f74 696d  = f'[{format_tim
-000033d0: 6573 7461 6d70 2873 656c 662e 7374 6172  estamp(self.star
-000033e0: 7429 7d20 2d2d 3e20 7b66 6f72 6d61 745f  t)} --> {format_
-000033f0: 7469 6d65 7374 616d 7028 7365 6c66 2e65  timestamp(self.e
-00003400: 6e64 297d 5d20 227b 7365 6c66 2e74 6578  nd)}] "{self.tex
-00003410: 747d 2227 0d0a 2020 2020 2020 2020 6966  t}"'..        if
-00003420: 2073 656c 662e 6861 735f 776f 7264 7320   self.has_words 
-00003430: 616e 6420 6e6f 7420 6f6e 6c79 5f73 6567  and not only_seg
-00003440: 6d65 6e74 3a0d 0a20 2020 2020 2020 2020  ment:..         
-00003450: 2020 206c 696e 6520 2b3d 2027 5c6e 2720     line += '\n' 
-00003460: 2b20 275c 6e27 2e6a 6f69 6e28 0d0a 2020  + '\n'.join(..  
-00003470: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00003480: 2d5b 7b66 6f72 6d61 745f 7469 6d65 7374  -[{format_timest
-00003490: 616d 7028 772e 7374 6172 7429 7d5d 202d  amp(w.start)}] -
-000034a0: 3e20 5b7b 666f 726d 6174 5f74 696d 6573  > [{format_times
-000034b0: 7461 6d70 2877 2e65 6e64 297d 5d20 5c22  tamp(w.end)}] \"
-000034c0: 7b77 2e77 6f72 647d 5c22 2220 666f 7220  {w.word}\"" for 
-000034d0: 7720 696e 2073 656c 662e 776f 7264 730d  w in self.words.
-000034e0: 0a20 2020 2020 2020 2020 2020 2029 202b  .            ) +
-000034f0: 2027 5c6e 270d 0a20 2020 2020 2020 2072   '\n'..        r
-00003500: 6574 7572 6e20 6c69 6e65 0d0a 0d0a 2020  eturn line....  
-00003510: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00003520: 2064 6566 2068 6173 5f77 6f72 6473 2873   def has_words(s
-00003530: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00003540: 6574 7572 6e20 626f 6f6c 2873 656c 662e  eturn bool(self.
-00003550: 776f 7264 7329 0d0a 0d0a 2020 2020 4070  words)....    @p
-00003560: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00003570: 206f 7269 5f68 6173 5f77 6f72 6473 2873   ori_has_words(s
-00003580: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00003590: 6574 7572 6e20 7365 6c66 2e77 6f72 6473  eturn self.words
-000035a0: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 0d0a   is not None....
-000035b0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000035c0: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
-000035d0: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
-000035e0: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
-000035f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00003600: 7572 6e20 7365 6c66 2e77 6f72 6473 5b30  urn self.words[0
-00003610: 5d2e 7374 6172 740d 0a20 2020 2020 2020  ].start..       
-00003620: 2072 6574 7572 6e20 7365 6c66 2e5f 6465   return self._de
-00003630: 6661 756c 745f 7374 6172 740d 0a0d 0a20  fault_start.... 
-00003640: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00003650: 2020 6465 6620 656e 6428 7365 6c66 293a    def end(self):
-00003660: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00003670: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
-00003680: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003690: 2073 656c 662e 776f 7264 735b 2d31 5d2e   self.words[-1].
-000036a0: 656e 640d 0a20 2020 2020 2020 2072 6574  end..        ret
-000036b0: 7572 6e20 7365 6c66 2e5f 6465 6661 756c  urn self._defaul
-000036c0: 745f 656e 640d 0a0d 0a20 2020 2040 7374  t_end....    @st
-000036d0: 6172 742e 7365 7474 6572 0d0a 2020 2020  art.setter..    
-000036e0: 6465 6620 7374 6172 7428 7365 6c66 2c20  def start(self, 
-000036f0: 7661 6c29 3a0d 0a20 2020 2020 2020 2069  val):..        i
-00003700: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
-00003710: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00003720: 656c 662e 776f 7264 735b 305d 2e73 7461  elf.words[0].sta
-00003730: 7274 203d 2076 616c 0d0a 2020 2020 2020  rt = val..      
-00003740: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00003750: 2020 2020 2020 7365 6c66 2e5f 6465 6661        self._defa
-00003760: 756c 745f 7374 6172 7420 3d20 7365 6c66  ult_start = self
-00003770: 2e72 6f75 6e64 2876 616c 290d 0a0d 0a20  .round(val).... 
-00003780: 2020 2040 656e 642e 7365 7474 6572 0d0a     @end.setter..
-00003790: 2020 2020 6465 6620 656e 6428 7365 6c66      def end(self
-000037a0: 2c20 7661 6c29 3a0d 0a20 2020 2020 2020  , val):..       
-000037b0: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
-000037c0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000037d0: 2073 656c 662e 776f 7264 735b 2d31 5d2e   self.words[-1].
-000037e0: 656e 6420 3d20 7661 6c0d 0a20 2020 2020  end = val..     
-000037f0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00003800: 2020 2020 2020 2073 656c 662e 5f64 6566         self._def
-00003810: 6175 6c74 5f65 6e64 203d 2073 656c 662e  ault_end = self.
-00003820: 726f 756e 6428 7661 6c29 0d0a 0d0a 2020  round(val)....  
-00003830: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00003840: 2064 6566 2074 6578 7428 7365 6c66 2920   def text(self) 
-00003850: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-00003860: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
-00003870: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00003880: 2072 6574 7572 6e20 2727 2e6a 6f69 6e28   return ''.join(
-00003890: 776f 7264 2e77 6f72 6420 666f 7220 776f  word.word for wo
-000038a0: 7264 2069 6e20 7365 6c66 2e77 6f72 6473  rd in self.words
-000038b0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000038c0: 6e20 7365 6c66 2e5f 6465 6661 756c 745f  n self._default_
-000038d0: 7465 7874 0d0a 0d0a 2020 2020 4070 726f  text....    @pro
-000038e0: 7065 7274 790d 0a20 2020 2064 6566 2074  perty..    def t
-000038f0: 6f6b 656e 7328 7365 6c66 2920 2d3e 204c  okens(self) -> L
-00003900: 6973 745b 696e 745d 3a0d 0a20 2020 2020  ist[int]:..     
-00003910: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
-00003920: 6f72 6473 2061 6e64 2073 656c 662e 776f  ords and self.wo
-00003930: 7264 735b 305d 2e74 6f6b 656e 733a 0d0a  rds[0].tokens:..
-00003940: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003950: 726e 206c 6973 7428 6368 6169 6e2e 6672  rn list(chain.fr
-00003960: 6f6d 5f69 7465 7261 626c 6528 776f 7264  om_iterable(word
-00003970: 2e74 6f6b 656e 7320 666f 7220 776f 7264  .tokens for word
-00003980: 2069 6e20 7365 6c66 2e77 6f72 6473 2929   in self.words))
-00003990: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000039a0: 2073 656c 662e 5f64 6566 6175 6c74 5f74   self._default_t
-000039b0: 6f6b 656e 730d 0a0d 0a20 2020 2040 7072  okens....    @pr
-000039c0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-000039d0: 6475 7261 7469 6f6e 2873 656c 6629 3a0d  duration(self):.
-000039e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000039f0: 7365 6c66 2e65 6e64 202d 2073 656c 662e  self.end - self.
-00003a00: 7374 6172 740d 0a0d 0a20 2020 2064 6566  start....    def
-00003a10: 2077 6f72 645f 636f 756e 7428 7365 6c66   word_count(self
-00003a20: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00003a30: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-00003a40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003a50: 726e 206c 656e 2873 656c 662e 776f 7264  rn len(self.word
-00003a60: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
-00003a70: 726e 202d 310d 0a0d 0a20 2020 2064 6566  rn -1....    def
-00003a80: 2063 6861 725f 636f 756e 7428 7365 6c66   char_count(self
-00003a90: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00003aa0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-00003ab0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003ac0: 726e 2073 756d 286c 656e 2877 2920 666f  rn sum(len(w) fo
-00003ad0: 7220 7720 696e 2073 656c 662e 776f 7264  r w in self.word
-00003ae0: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
-00003af0: 726e 206c 656e 2873 656c 662e 7465 7874  rn len(self.text
-00003b00: 290d 0a0d 0a20 2020 2064 6566 2061 6464  )....    def add
-00003b10: 2873 656c 662c 206f 7468 6572 3a20 2753  (self, other: 'S
-00003b20: 6567 6d65 6e74 272c 2063 6f70 795f 776f  egment', copy_wo
-00003b30: 7264 733a 2062 6f6f 6c20 3d20 4661 6c73  rds: bool = Fals
-00003b40: 6529 3a0d 0a20 2020 2020 2020 2069 6620  e):..        if 
-00003b50: 7365 6c66 2e6f 7269 5f68 6173 5f77 6f72  self.ori_has_wor
-00003b60: 6473 203d 3d20 6f74 6865 722e 6f72 695f  ds == other.ori_
-00003b70: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
-00003b80: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
-00003b90: 2873 656c 662e 776f 7264 7320 2b20 6f74  (self.words + ot
-00003ba0: 6865 722e 776f 7264 7329 2069 6620 7365  her.words) if se
-00003bb0: 6c66 2e6f 7269 5f68 6173 5f77 6f72 6473  lf.ori_has_words
-00003bc0: 2065 6c73 6520 4e6f 6e65 0d0a 2020 2020   else None..    
-00003bd0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003be0: 2020 2020 2020 2073 656c 665f 7374 6174         self_stat
-00003bf0: 6520 3d20 2777 6974 6827 2069 6620 7365  e = 'with' if se
-00003c00: 6c66 2e6f 7269 5f68 6173 5f77 6f72 6473  lf.ori_has_words
-00003c10: 2065 6c73 6520 2777 6974 686f 7574 270d   else 'without'.
-00003c20: 0a20 2020 2020 2020 2020 2020 206f 7468  .            oth
-00003c30: 6572 5f73 7461 7465 203d 2027 7769 7468  er_state = 'with
-00003c40: 2720 6966 206f 7468 6572 2e6f 7269 5f68  ' if other.ori_h
-00003c50: 6173 5f77 6f72 6473 2065 6c73 6520 2777  as_words else 'w
-00003c60: 6974 686f 7574 270d 0a20 2020 2020 2020  ithout'..       
-00003c70: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00003c80: 4572 726f 7228 6622 4361 6e27 7420 6d65  Error(f"Can't me
-00003c90: 7267 6520 7365 676d 656e 7420 7b73 656c  rge segment {sel
-00003ca0: 665f 7374 6174 657d 2077 6f72 6473 2061  f_state} words a
-00003cb0: 6e64 2061 2073 6567 6d65 6e74 207b 6f74  nd a segment {ot
-00003cc0: 6865 725f 7374 6174 657d 2077 6f72 6473  her_state} words
-00003cd0: 2e22 290d 0a0d 0a20 2020 2020 2020 2073  .")....        s
-00003ce0: 656c 665f 636f 7079 203d 2073 656c 662e  elf_copy = self.
-00003cf0: 636f 7079 2877 6f72 6473 2c20 636f 7079  copy(words, copy
-00003d00: 5f77 6f72 6473 3d63 6f70 795f 776f 7264  _words=copy_word
-00003d10: 7329 0d0a 2020 2020 2020 2020 5f63 6f6d  s)..        _com
-00003d20: 6269 6e65 5f61 7474 7228 7365 6c66 5f63  bine_attr(self_c
-00003d30: 6f70 792c 206f 7468 6572 2c20 2774 656d  opy, other, 'tem
-00003d40: 7065 7261 7475 7265 2729 0d0a 2020 2020  perature')..    
-00003d50: 2020 2020 5f63 6f6d 6269 6e65 5f61 7474      _combine_att
-00003d60: 7228 7365 6c66 5f63 6f70 792c 206f 7468  r(self_copy, oth
-00003d70: 6572 2c20 2761 7667 5f6c 6f67 7072 6f62  er, 'avg_logprob
-00003d80: 2729 0d0a 2020 2020 2020 2020 5f63 6f6d  ')..        _com
-00003d90: 6269 6e65 5f61 7474 7228 7365 6c66 5f63  bine_attr(self_c
-00003da0: 6f70 792c 206f 7468 6572 2c20 2763 6f6d  opy, other, 'com
-00003db0: 7072 6573 7369 6f6e 5f72 6174 696f 2729  pression_ratio')
-00003dc0: 0d0a 2020 2020 2020 2020 5f63 6f6d 6269  ..        _combi
-00003dd0: 6e65 5f61 7474 7228 7365 6c66 5f63 6f70  ne_attr(self_cop
-00003de0: 792c 206f 7468 6572 2c20 276e 6f5f 7370  y, other, 'no_sp
-00003df0: 6565 6368 5f70 726f 6227 290d 0a0d 0a20  eech_prob').... 
-00003e00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00003e10: 6c66 5f63 6f70 790d 0a0d 0a20 2020 2064  lf_copy....    d
-00003e20: 6566 205f 5f61 6464 5f5f 2873 656c 662c  ef __add__(self,
-00003e30: 206f 7468 6572 3a20 2753 6567 6d65 6e74   other: 'Segment
-00003e40: 2729 3a0d 0a20 2020 2020 2020 2072 6574  '):..        ret
-00003e50: 7572 6e20 7365 6c66 2e61 6464 286f 7468  urn self.add(oth
-00003e60: 6572 2c20 636f 7079 5f77 6f72 6473 3d54  er, copy_words=T
-00003e70: 7275 6529 0d0a 0d0a 2020 2020 6465 6620  rue)....    def 
-00003e80: 5f77 6f72 645f 6f70 6572 6174 696f 6e73  _word_operations
-00003e90: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
-00003ea0: 3a20 7374 722c 202a 6172 6773 2c20 2a2a  : str, *args, **
-00003eb0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00003ec0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
-00003ed0: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-00003ee0: 2020 666f 7220 7720 696e 2073 656c 662e    for w in self.
-00003ef0: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
-00003f00: 2020 2020 2020 2020 6765 7461 7474 7228          getattr(
-00003f10: 772c 206f 7065 7261 7469 6f6e 2928 2a61  w, operation)(*a
-00003f20: 7267 732c 202a 2a6b 7761 7267 7329 0d0a  rgs, **kwargs)..
-00003f30: 0d0a 2020 2020 6465 6620 726f 756e 645f  ..    def round_
-00003f40: 616c 6c5f 7469 6d65 7374 616d 7073 2873  all_timestamps(s
-00003f50: 656c 6629 3a0d 0a20 2020 2020 2020 2077  elf):..        w
-00003f60: 6172 6e69 6e67 732e 7761 726e 2827 6060  arnings.warn('``
-00003f70: 2e72 6f75 6e64 5f61 6c6c 5f74 696d 6573  .round_all_times
-00003f80: 7461 6d70 7328 2960 6020 6973 2064 6570  tamps()`` is dep
-00003f90: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
-00003fa0: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
-00003fb0: 7574 7572 6520 7665 7273 696f 6e73 2e20  uture versions. 
-00003fc0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00003fd0: 2020 2020 2020 2020 2027 5573 6520 6060           'Use ``
-00003fe0: 2e72 6f75 6e64 5f74 733d 5472 7565 6060  .round_ts=True``
-00003ff0: 2074 6f20 726f 756e 6420 7469 6d65 7374   to round timest
-00004000: 616d 7073 2062 7920 6465 6661 756c 7420  amps by default 
-00004010: 696e 7374 6561 642e 272c 0d0a 2020 2020  instead.',..    
-00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004030: 2020 7374 6163 6b6c 6576 656c 3d32 290d    stacklevel=2).
-00004040: 0a20 2020 2020 2020 2073 656c 662e 726f  .        self.ro
-00004050: 756e 645f 7473 203d 2054 7275 650d 0a0d  und_ts = True...
-00004060: 0a20 2020 2064 6566 206f 6666 7365 745f  .    def offset_
-00004070: 7469 6d65 2873 656c 662c 206f 6666 7365  time(self, offse
-00004080: 745f 7365 636f 6e64 733a 2066 6c6f 6174  t_seconds: float
-00004090: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-000040a0: 656c 662e 7365 656b 2069 7320 6e6f 7420  elf.seek is not 
-000040b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000040c0: 2020 2073 656c 662e 7365 656b 202b 3d20     self.seek += 
-000040d0: 6f66 6673 6574 5f73 6563 6f6e 6473 0d0a  offset_seconds..
-000040e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000040f0: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
-00004100: 2020 2020 2020 2020 7365 6c66 2e5f 776f          self._wo
-00004110: 7264 5f6f 7065 7261 7469 6f6e 7328 276f  rd_operations('o
-00004120: 6666 7365 745f 7469 6d65 272c 206f 6666  ffset_time', off
-00004130: 7365 745f 7365 636f 6e64 7329 0d0a 2020  set_seconds)..  
-00004140: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00004150: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00004160: 6172 7420 3d20 7365 6c66 2e73 7461 7274  art = self.start
-00004170: 202b 206f 6666 7365 745f 7365 636f 6e64   + offset_second
-00004180: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
-00004190: 656c 662e 656e 6420 3d20 7365 6c66 2e65  elf.end = self.e
-000041a0: 6e64 202b 206f 6666 7365 745f 7365 636f  nd + offset_seco
-000041b0: 6e64 730d 0a0d 0a20 2020 2064 6566 2061  nds....    def a
-000041c0: 6464 5f77 6f72 6473 2873 656c 662c 2069  dd_words(self, i
-000041d0: 6e64 6578 303a 2069 6e74 2c20 696e 6465  ndex0: int, inde
-000041e0: 7831 3a20 696e 742c 2069 6e70 6c61 6365  x1: int, inplace
-000041f0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
-00004200: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00004210: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
-00004220: 2020 2020 2020 2020 2020 6e65 775f 776f            new_wo
-00004230: 7264 203d 2073 656c 662e 776f 7264 735b  rd = self.words[
-00004240: 696e 6465 7830 5d20 2b20 7365 6c66 2e77  index0] + self.w
-00004250: 6f72 6473 5b69 6e64 6578 315d 0d0a 2020  ords[index1]..  
-00004260: 2020 2020 2020 2020 2020 6966 2069 6e70            if inp
-00004270: 6c61 6365 3a0d 0a20 2020 2020 2020 2020  lace:..         
-00004280: 2020 2020 2020 2069 302c 2069 3120 3d20         i0, i1 = 
-00004290: 736f 7274 6564 285b 696e 6465 7830 2c20  sorted([index0, 
-000042a0: 696e 6465 7831 5d29 0d0a 2020 2020 2020  index1])..      
-000042b0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000042c0: 6f72 6473 5b69 305d 203d 206e 6577 5f77  ords[i0] = new_w
-000042d0: 6f72 640d 0a20 2020 2020 2020 2020 2020  ord..           
-000042e0: 2020 2020 2064 656c 2073 656c 662e 776f       del self.wo
-000042f0: 7264 735b 6931 5d0d 0a20 2020 2020 2020  rds[i1]..       
-00004300: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
-00004310: 776f 7264 0d0a 0d0a 2020 2020 6465 6620  word....    def 
-00004320: 7265 7363 616c 655f 7469 6d65 2873 656c  rescale_time(sel
-00004330: 662c 2073 6361 6c65 5f66 6163 746f 723a  f, scale_factor:
-00004340: 2066 6c6f 6174 293a 0d0a 2020 2020 2020   float):..      
-00004350: 2020 6966 2073 656c 662e 7365 656b 2069    if self.seek i
-00004360: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00004370: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00004380: 656b 202a 3d20 7363 616c 655f 6661 6374  ek *= scale_fact
-00004390: 6f72 0d0a 2020 2020 2020 2020 6966 2073  or..        if s
-000043a0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-000043b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000043c0: 2e5f 776f 7264 5f6f 7065 7261 7469 6f6e  ._word_operation
-000043d0: 7328 2772 6573 6361 6c65 5f74 696d 6527  s('rescale_time'
-000043e0: 2c20 7363 616c 655f 6661 6374 6f72 290d  , scale_factor).
-000043f0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00004400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004410: 2e73 7461 7274 203d 2073 656c 662e 7374  .start = self.st
-00004420: 6172 7420 2a20 7363 616c 655f 6661 6374  art * scale_fact
-00004430: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
-00004440: 7365 6c66 2e65 6e64 203d 2073 656c 662e  self.end = self.
-00004450: 656e 6420 2a20 7363 616c 655f 6661 6374  end * scale_fact
-00004460: 6f72 0d0a 0d0a 2020 2020 6465 6620 6170  or....    def ap
-00004470: 706c 795f 6d69 6e5f 6475 7228 7365 6c66  ply_min_dur(self
-00004480: 2c20 6d69 6e5f 6475 723a 2066 6c6f 6174  , min_dur: float
-00004490: 2c20 696e 706c 6163 653a 2062 6f6f 6c20  , inplace: bool 
-000044a0: 3d20 4661 6c73 6529 3a0d 0a20 2020 2020  = False):..     
-000044b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000044c0: 4d65 7267 6520 616e 7920 776f 7264 2077  Merge any word w
-000044d0: 6974 6820 6164 6a61 6365 6e74 2077 6f72  ith adjacent wor
-000044e0: 6420 6966 2069 7473 2064 7572 6174 696f  d if its duratio
-000044f0: 6e20 6973 206c 6573 7320 7468 616e 2060  n is less than `
-00004500: 606d 696e 5f64 7572 6060 2e0d 0a20 2020  `min_dur``...   
-00004510: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004520: 2020 7365 676d 656e 7420 3d20 7365 6c66    segment = self
-00004530: 2069 6620 696e 706c 6163 6520 656c 7365   if inplace else
-00004540: 2064 6565 7063 6f70 7928 7365 6c66 290d   deepcopy(self).
-00004550: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00004560: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
-00004570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004580: 7572 6e20 7365 676d 656e 740d 0a20 2020  urn segment..   
-00004590: 2020 2020 206d 6178 5f69 203d 206c 656e       max_i = len
-000045a0: 2873 6567 6d65 6e74 2e77 6f72 6473 2920  (segment.words) 
-000045b0: 2d20 310d 0a20 2020 2020 2020 2069 6620  - 1..        if 
-000045c0: 6d61 785f 6920 3d3d 2030 3a0d 0a20 2020  max_i == 0:..   
-000045d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000045e0: 7365 676d 656e 740d 0a20 2020 2020 2020  segment..       
-000045f0: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
-00004600: 6564 2872 616e 6765 286c 656e 2873 6567  ed(range(len(seg
-00004610: 6d65 6e74 2e77 6f72 6473 2929 293a 0d0a  ment.words))):..
-00004620: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00004630: 6178 5f69 203d 3d20 303a 0d0a 2020 2020  ax_i == 0:..    
-00004640: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00004650: 6b0d 0a20 2020 2020 2020 2020 2020 2069  k..            i
-00004660: 6620 7365 676d 656e 742e 776f 7264 735b  f segment.words[
-00004670: 695d 2e64 7572 6174 696f 6e20 3c20 6d69  i].duration < mi
-00004680: 6e5f 6475 723a 0d0a 2020 2020 2020 2020  n_dur:..        
-00004690: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
-000046a0: 6d61 785f 693a 0d0a 2020 2020 2020 2020  max_i:..        
-000046b0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
-000046c0: 656e 742e 6164 645f 776f 7264 7328 692d  ent.add_words(i-
-000046d0: 312c 2069 2c20 696e 706c 6163 653d 5472  1, i, inplace=Tr
-000046e0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-000046f0: 2020 2020 2065 6c69 6620 6920 3d3d 2030       elif i == 0
-00004700: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004710: 2020 2020 2020 2073 6567 6d65 6e74 2e61         segment.a
-00004720: 6464 5f77 6f72 6473 2869 2c20 692b 312c  dd_words(i, i+1,
-00004730: 2069 6e70 6c61 6365 3d54 7275 6529 0d0a   inplace=True)..
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00004760: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00004770: 676d 656e 742e 776f 7264 735b 692b 315d  gment.words[i+1]
-00004780: 2e64 7572 6174 696f 6e20 3c20 7365 676d  .duration < segm
-00004790: 656e 742e 776f 7264 735b 692d 315d 2e64  ent.words[i-1].d
-000047a0: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 7365 676d 656e 742e 6164 645f 776f    segment.add_wo
-000047d0: 7264 7328 692d 312c 2069 2c20 696e 706c  rds(i-1, i, inpl
-000047e0: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004800: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004810: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004820: 676d 656e 742e 6164 645f 776f 7264 7328  gment.add_words(
-00004830: 692c 2069 2b31 2c20 696e 706c 6163 653d  i, i+1, inplace=
-00004840: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00004850: 2020 2020 2020 206d 6178 5f69 202d 3d20         max_i -= 
-00004860: 310d 0a20 2020 2020 2020 2072 6574 7572  1..        retur
-00004870: 6e20 7365 676d 656e 740d 0a0d 0a20 2020  n segment....   
-00004880: 2064 6566 205f 746f 5f72 6576 6572 7365   def _to_reverse
-00004890: 5f74 6578 7428 0d0a 2020 2020 2020 2020  _text(..        
-000048a0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-000048b0: 2020 2020 2020 2070 7265 7065 6e64 5f70         prepend_p
-000048c0: 756e 6374 7561 7469 6f6e 733a 204f 7074  unctuations: Opt
-000048d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-000048e0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000048f0: 6170 7065 6e64 5f70 756e 6374 7561 7469  append_punctuati
-00004900: 6f6e 733a 204f 7074 696f 6e61 6c5b 7374  ons: Optional[st
-00004910: 725d 203d 204e 6f6e 652c 0d0a 2020 2020  r] = None,..    
-00004920: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00004930: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00004940: 6120 636f 7079 2077 6974 6820 776f 7264  a copy with word
-00004950: 7320 7265 7665 7273 6564 206f 7264 6572  s reversed order
-00004960: 2070 6572 2073 6567 6d65 6e74 2e0d 0a20   per segment... 
-00004970: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00004980: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00004990: 6e28 2760 605f 746f 5f72 6576 6572 7365  n('``_to_reverse
-000049a0: 5f74 6578 7428 2960 6020 6973 2064 6570  _text()`` is dep
-000049b0: 7265 6361 7465 6420 616e 6420 7769 6c6c  recated and will
-000049c0: 2062 6520 7265 6d6f 7665 6420 696e 2066   be removed in f
-000049d0: 7574 7572 6520 7665 7273 696f 6e73 2e27  uture versions.'
-000049e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000049f0: 2020 2020 2020 2020 2063 6174 6567 6f72           categor
-00004a00: 793d 4465 7072 6563 6174 696f 6e57 6172  y=DeprecationWar
-00004a10: 6e69 6e67 2c20 7374 6163 6b6c 6576 656c  ning, stacklevel
-00004a20: 3d32 290d 0a20 2020 2020 2020 2070 7265  =2)..        pre
-00004a30: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
-00004a40: 7320 3d20 6765 745f 7072 6570 656e 645f  s = get_prepend_
-00004a50: 7075 6e63 7475 6174 696f 6e73 2870 7265  punctuations(pre
-00004a60: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
-00004a70: 7329 0d0a 2020 2020 2020 2020 6966 2070  s)..        if p
-00004a80: 7265 7065 6e64 5f70 756e 6374 7561 7469  repend_punctuati
-00004a90: 6f6e 7320 616e 6420 2720 2720 6e6f 7420  ons and ' ' not 
-00004aa0: 696e 2070 7265 7065 6e64 5f70 756e 6374  in prepend_punct
-00004ab0: 7561 7469 6f6e 733a 0d0a 2020 2020 2020  uations:..      
-00004ac0: 2020 2020 2020 7072 6570 656e 645f 7075        prepend_pu
-00004ad0: 6e63 7475 6174 696f 6e73 202b 3d20 2720  nctuations += ' 
-00004ae0: 270d 0a20 2020 2020 2020 2061 7070 656e  '..        appen
-00004af0: 645f 7075 6e63 7475 6174 696f 6e73 203d  d_punctuations =
-00004b00: 2067 6574 5f61 7070 656e 645f 7075 6e63   get_append_punc
-00004b10: 7475 6174 696f 6e73 2861 7070 656e 645f  tuations(append_
-00004b20: 7075 6e63 7475 6174 696f 6e73 290d 0a20  punctuations).. 
-00004b30: 2020 2020 2020 2073 656c 665f 636f 7079         self_copy
-00004b40: 203d 2073 656c 662e 636f 7079 2863 6f70   = self.copy(cop
-00004b50: 795f 776f 7264 733d 5472 7565 290d 0a20  y_words=True).. 
-00004b60: 2020 2020 2020 2068 6173 5f70 7265 7065         has_prepe
-00004b70: 6e64 203d 2062 6f6f 6c28 7072 6570 656e  nd = bool(prepen
-00004b80: 645f 7075 6e63 7475 6174 696f 6e73 290d  d_punctuations).
-00004b90: 0a20 2020 2020 2020 2068 6173 5f61 7070  .        has_app
-00004ba0: 656e 6420 3d20 626f 6f6c 2861 7070 656e  end = bool(appen
-00004bb0: 645f 7075 6e63 7475 6174 696f 6e73 290d  d_punctuations).
-00004bc0: 0a20 2020 2020 2020 2069 6620 6861 735f  .        if has_
-00004bd0: 7072 6570 656e 6420 6f72 2068 6173 5f61  prepend or has_a
-00004be0: 7070 656e 643a 0d0a 2020 2020 2020 2020  ppend:..        
-00004bf0: 2020 2020 776f 7264 5f6f 626a 7320 3d20      word_objs = 
-00004c00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00004c10: 2020 2073 656c 665f 636f 7079 2e77 6f72     self_copy.wor
-00004c20: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-00004c30: 2020 2020 6966 2073 656c 665f 636f 7079      if self_copy
-00004c40: 2e68 6173 5f77 6f72 6473 2065 6c73 650d  .has_words else.
-00004c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c60: 205b 576f 7264 5469 6d69 6e67 2877 2c20   [WordTiming(w, 
-00004c70: 302c 2031 2c20 3029 2066 6f72 2077 2069  0, 1, 0) for w i
-00004c80: 6e20 7365 6c66 5f63 6f70 792e 7465 7874  n self_copy.text
-00004c90: 2e73 706c 6974 2827 2027 295d 0d0a 2020  .split(' ')]..  
-00004ca0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00004cb0: 2020 2020 2020 2020 2066 6f72 2077 6f72           for wor
-00004cc0: 6420 696e 2077 6f72 645f 6f62 6a73 3a0d  d in word_objs:.
-00004cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ce0: 206e 6577 5f61 7070 656e 6420 3d20 2727   new_append = ''
-00004cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004d00: 2020 6966 2068 6173 5f70 7265 7065 6e64    if has_prepend
-00004d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004d20: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
-00004d30: 7261 6e67 6528 6c65 6e28 776f 7264 2929  range(len(word))
-00004d40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004d50: 2020 2020 2020 2020 2020 2063 6861 7220             char 
-00004d60: 3d20 776f 7264 2e77 6f72 645b 305d 0d0a  = word.word[0]..
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2020 2020 2020 6966 2063 6861 7220          if char 
-00004d90: 696e 2070 7265 7065 6e64 5f70 756e 6374  in prepend_punct
-00004da0: 7561 7469 6f6e 733a 0d0a 2020 2020 2020  uations:..      
-00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dc0: 2020 2020 2020 6e65 775f 6170 7065 6e64        new_append
-00004dd0: 202b 3d20 6368 6172 0d0a 2020 2020 2020   += char..      
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 776f 7264 2e77 6f72 6420        word.word 
-00004e00: 3d20 776f 7264 2e77 6f72 645b 313a 5d0d  = word.word[1:].
-00004e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00004e50: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
-00004e60: 2020 206e 6577 5f70 7265 7065 6e64 203d     new_prepend =
-00004e70: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
-00004e80: 2020 2020 2069 6620 6861 735f 6170 7065       if has_appe
-00004e90: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
-00004ea0: 2020 2020 2020 2020 2066 6f72 205f 2069           for _ i
-00004eb0: 6e20 7261 6e67 6528 6c65 6e28 776f 7264  n range(len(word
-00004ec0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00004ed0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00004ee0: 7220 3d20 776f 7264 2e77 6f72 645b 2d31  r = word.word[-1
-00004ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00004f00: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
-00004f10: 6172 2069 6e20 6170 7065 6e64 5f70 756e  ar in append_pun
-00004f20: 6374 7561 7469 6f6e 733a 0d0a 2020 2020  ctuations:..    
-00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2020 2020 2020 6e65 775f 7072 6570          new_prep
-00004f50: 656e 6420 2b3d 2063 6861 720d 0a20 2020  end += char..   
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2077 6f72 642e 776f           word.wo
-00004f80: 7264 203d 2077 6f72 642e 776f 7264 5b3a  rd = word.word[:
-00004f90: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
-00004fa0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00004fb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
-00004fe0: 2020 2020 2020 2077 6f72 642e 776f 7264         word.word
-00004ff0: 203d 2066 277b 6e65 775f 7072 6570 656e   = f'{new_prepen
-00005000: 647d 7b77 6f72 642e 776f 7264 7d7b 6e65  d}{word.word}{ne
-00005010: 775f 6170 7065 6e64 5b3a 3a2d 315d 7d27  w_append[::-1]}'
-00005020: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00005030: 6c66 5f63 6f70 792e 5f64 6566 6175 6c74  lf_copy._default
-00005040: 5f74 6578 7420 3d20 2727 2e6a 6f69 6e28  _text = ''.join(
-00005050: 772e 776f 7264 2066 6f72 2077 2069 6e20  w.word for w in 
-00005060: 7265 7665 7273 6564 2877 6f72 645f 6f62  reversed(word_ob
-00005070: 6a73 2929 0d0a 0d0a 2020 2020 2020 2020  js))....        
-00005080: 7265 7475 726e 2073 656c 665f 636f 7079  return self_copy
-00005090: 0d0a 0d0a 2020 2020 6465 6620 746f 5f64  ....    def to_d
-000050a0: 6963 7428 7365 6c66 2c20 7265 7665 7273  ict(self, revers
-000050b0: 655f 7465 7874 3a20 556e 696f 6e5b 626f  e_text: Union[bo
-000050c0: 6f6c 2c20 7475 706c 655d 203d 2046 616c  ol, tuple] = Fal
-000050d0: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
-000050e0: 2072 6576 6572 7365 5f74 6578 743a 0d0a   reverse_text:..
-000050f0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-00005100: 696e 6773 2e77 6172 6e28 2760 6072 6576  ings.warn('``rev
-00005110: 6572 7365 5f74 6578 743d 5472 7565 6060  erse_text=True``
-00005120: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
-00005130: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
-00005140: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
-00005150: 7369 6f6e 732e 2027 0d0a 2020 2020 2020  sions. '..      
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 2752 544c 2074 6578 7420 706c      'RTL text pl
-00005180: 6179 6261 636b 2069 7373 7565 7320 6172  ayback issues ar
-00005190: 6520 6361 7573 6564 2062 7920 7468 6520  e caused by the 
-000051a0: 7669 6465 6f20 706c 6179 6572 2069 6e63  video player inc
-000051b0: 6f72 7265 6374 6c79 2070 6172 7369 6e67  orrectly parsing
-000051c0: 2074 6167 7320 270d 0a20 2020 2020 2020   tags '..       
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2020 2027 286e 6f74 653a 2074 6167 7320     '(note: tags 
-000051f0: 636f 6d65 2066 726f 6d20 6060 7365 676d  come from ``segm
-00005200: 656e 745f 6c65 7665 6c3d 5472 7565 202b  ent_level=True +
-00005210: 2077 6f72 645f 6c65 7665 6c3d 5472 7565   word_level=True
-00005220: 6060 292e 2729 0d0a 2020 2020 2020 2020  ``).')..        
-00005230: 2020 2020 7365 676d 656e 7420 3d20 7365      segment = se
-00005240: 6c66 2e5f 746f 5f72 6576 6572 7365 5f74  lf._to_reverse_t
-00005250: 6578 7428 2a28 7265 7665 7273 655f 7465  ext(*(reverse_te
-00005260: 7874 2069 6620 7265 7665 7273 655f 7465  xt if reverse_te
-00005270: 7874 2065 6c73 6520 5b5d 2929 0d0a 2020  xt else []))..  
-00005280: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00005290: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
-000052a0: 203d 2073 656c 660d 0a0d 0a20 2020 2020   = self....     
-000052b0: 2020 2073 6567 5f64 6963 7420 3d20 6469     seg_dict = di
-000052c0: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
-000052d0: 2073 7461 7274 3d73 6567 6d65 6e74 2e73   start=segment.s
-000052e0: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
-000052f0: 2020 2065 6e64 3d73 6567 6d65 6e74 2e65     end=segment.e
-00005300: 6e64 2c0d 0a20 2020 2020 2020 2020 2020  nd,..           
-00005310: 2074 6578 743d 7365 676d 656e 742e 7465   text=segment.te
-00005320: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-00005330: 2073 6565 6b3d 7365 676d 656e 742e 7365   seek=segment.se
-00005340: 656b 2c0d 0a20 2020 2020 2020 2020 2020  ek,..           
-00005350: 2074 6f6b 656e 733d 4e6f 6e65 2069 6620   tokens=None if 
-00005360: 7365 676d 656e 742e 746f 6b65 6e73 2069  segment.tokens i
-00005370: 7320 4e6f 6e65 2065 6c73 6520 7365 676d  s None else segm
-00005380: 656e 742e 746f 6b65 6e73 2e63 6f70 7928  ent.tokens.copy(
-00005390: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000053a0: 7465 6d70 6572 6174 7572 653d 7365 676d  temperature=segm
-000053b0: 656e 742e 7465 6d70 6572 6174 7572 652c  ent.temperature,
-000053c0: 0d0a 2020 2020 2020 2020 2020 2020 6176  ..            av
-000053d0: 675f 6c6f 6770 726f 623d 7365 676d 656e  g_logprob=segmen
-000053e0: 742e 6176 675f 6c6f 6770 726f 622c 0d0a  t.avg_logprob,..
-000053f0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00005400: 7265 7373 696f 6e5f 7261 7469 6f3d 7365  ression_ratio=se
-00005410: 676d 656e 742e 636f 6d70 7265 7373 696f  gment.compressio
-00005420: 6e5f 7261 7469 6f2c 0d0a 2020 2020 2020  n_ratio,..      
-00005430: 2020 2020 2020 6e6f 5f73 7065 6563 685f        no_speech_
-00005440: 7072 6f62 3d73 6567 6d65 6e74 2e6e 6f5f  prob=segment.no_
-00005450: 7370 6565 6368 5f70 726f 622c 0d0a 2020  speech_prob,..  
-00005460: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
-00005470: 2020 2069 6620 7365 676d 656e 742e 6861     if segment.ha
-00005480: 735f 776f 7264 733a 0d0a 2020 2020 2020  s_words:..      
-00005490: 2020 2020 2020 7365 675f 6469 6374 5b27        seg_dict['
-000054a0: 776f 7264 7327 5d20 3d20 5b77 2e74 6f5f  words'] = [w.to_
-000054b0: 6469 6374 2829 2066 6f72 2077 2069 6e20  dict() for w in 
-000054c0: 7365 676d 656e 742e 776f 7264 735d 0d0a  segment.words]..
-000054d0: 2020 2020 2020 2020 656c 6966 2073 6567          elif seg
-000054e0: 6d65 6e74 2e6f 7269 5f68 6173 5f77 6f72  ment.ori_has_wor
-000054f0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00005500: 2073 6567 5f64 6963 745b 2777 6f72 6473   seg_dict['words
-00005510: 275d 203d 205b 5d0d 0a20 2020 2020 2020  '] = []..       
-00005520: 2069 6620 7265 7665 7273 655f 7465 7874   if reverse_text
-00005530: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00005540: 6567 5f64 6963 745b 2772 6576 6572 7365  eg_dict['reverse
-00005550: 645f 7465 7874 275d 203d 2054 7275 650d  d_text'] = True.
-00005560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005570: 7365 675f 6469 6374 0d0a 0d0a 2020 2020  seg_dict....    
-00005580: 6465 6620 776f 7264 735f 6279 5f6c 6f63  def words_by_loc
-00005590: 6b28 7365 6c66 2c20 6f6e 6c79 5f74 6578  k(self, only_tex
-000055a0: 743a 2062 6f6f 6c20 3d20 5472 7565 2c20  t: bool = True, 
-000055b0: 696e 636c 7564 655f 7369 6e67 6c65 3a20  include_single: 
-000055c0: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
-000055d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000055e0: 776f 7264 735f 6279 5f6c 6f63 6b28 7365  words_by_lock(se
-000055f0: 6c66 2e77 6f72 6473 2c20 6f6e 6c79 5f74  lf.words, only_t
-00005600: 6578 743d 6f6e 6c79 5f74 6578 742c 2069  ext=only_text, i
-00005610: 6e63 6c75 6465 5f73 696e 676c 653d 696e  nclude_single=in
-00005620: 636c 7564 655f 7369 6e67 6c65 290d 0a0d  clude_single)...
-00005630: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00005640: 2020 2020 6465 6620 6c65 6674 5f6c 6f63      def left_loc
-00005650: 6b65 6428 7365 6c66 293a 0d0a 2020 2020  ked(self):..    
-00005660: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
-00005670: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
-00005680: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00005690: 776f 7264 735b 305d 2e6c 6566 745f 6c6f  words[0].left_lo
-000056a0: 636b 6564 0d0a 2020 2020 2020 2020 7265  cked..        re
-000056b0: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
-000056c0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-000056d0: 2064 6566 2072 6967 6874 5f6c 6f63 6b65   def right_locke
-000056e0: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
-000056f0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
-00005700: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-00005710: 2020 7265 7475 726e 2073 656c 662e 776f    return self.wo
-00005720: 7264 735b 2d31 5d2e 7269 6768 745f 6c6f  rds[-1].right_lo
-00005730: 636b 6564 0d0a 2020 2020 2020 2020 7265  cked..        re
-00005740: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
-00005750: 2020 6465 6620 6c6f 636b 5f6c 6566 7428    def lock_left(
-00005760: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00005770: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
-00005780: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005790: 7365 6c66 2e77 6f72 6473 5b30 5d2e 6c6f  self.words[0].lo
-000057a0: 636b 5f6c 6566 7428 290d 0a0d 0a20 2020  ck_left()....   
-000057b0: 2064 6566 206c 6f63 6b5f 7269 6768 7428   def lock_right(
-000057c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000057d0: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
-000057e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000057f0: 7365 6c66 2e77 6f72 6473 5b2d 315d 2e6c  self.words[-1].l
-00005800: 6f63 6b5f 7269 6768 7428 290d 0a0d 0a20  ock_right().... 
-00005810: 2020 2064 6566 206c 6f63 6b5f 626f 7468     def lock_both
-00005820: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00005830: 2073 656c 662e 6c6f 636b 5f6c 6566 7428   self.lock_left(
-00005840: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00005850: 6c6f 636b 5f72 6967 6874 2829 0d0a 0d0a  lock_right()....
-00005860: 2020 2020 6465 6620 756e 6c6f 636b 5f61      def unlock_a
-00005870: 6c6c 5f77 6f72 6473 2873 656c 6629 3a0d  ll_words(self):.
-00005880: 0a20 2020 2020 2020 2073 656c 662e 5f77  .        self._w
-00005890: 6f72 645f 6f70 6572 6174 696f 6e73 2827  ord_operations('
-000058a0: 756e 6c6f 636b 5f62 6f74 6827 290d 0a0d  unlock_both')...
-000058b0: 0a20 2020 2064 6566 2072 6561 7373 6967  .    def reassig
-000058c0: 6e5f 6964 7328 7365 6c66 2c20 7374 6172  n_ids(self, star
-000058d0: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
-000058e0: 203d 204e 6f6e 6529 3a0d 0a20 2020 2020   = None):..     
-000058f0: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
-00005900: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
-00005910: 2020 2066 6f72 2069 2c20 776f 7264 2069     for i, word i
-00005920: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
-00005930: 2e77 6f72 6473 5b73 7461 7274 3a5d 2c20  .words[start:], 
-00005940: 7374 6172 7420 6f72 2030 293a 0d0a 2020  start or 0):..  
-00005950: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-00005960: 7264 2e73 6567 6d65 6e74 203d 2073 656c  rd.segment = sel
-00005970: 660d 0a20 2020 2020 2020 2020 2020 2020  f..             
-00005980: 2020 2077 6f72 642e 6964 203d 2069 0d0a     word.id = i..
-00005990: 0d0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-000059a0: 5f73 6567 5f77 6974 685f 776f 7264 7328  _seg_with_words(
-000059b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000059c0: 7761 726e 696e 6773 2e77 6172 6e28 2741  warnings.warn('A
-000059d0: 7474 7269 6275 7465 7320 7468 6174 2072  ttributes that r
-000059e0: 6571 7569 7265 6420 7570 6461 7469 6e67  equired updating
-000059f0: 2061 7265 206e 6f77 2070 726f 7065 7274   are now propert
-00005a00: 6965 7320 6261 7365 6420 6f6e 2074 6865  ies based on the
-00005a10: 2060 6077 6f72 6473 6060 2065 7863 6570   ``words`` excep
-00005a20: 7420 666f 7220 6060 6964 6060 2e20 270d  t for ``id``. '.
-00005a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a40: 2020 2020 2020 2027 6060 7570 6461 7465         '``update
-00005a50: 5f73 6567 5f77 6974 685f 776f 7264 7328  _seg_with_words(
-00005a60: 2960 6020 6973 2064 6570 7265 6361 7465  )`` is deprecate
-00005a70: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
-00005a80: 6d6f 7665 6420 696e 2066 7574 7572 6520  moved in future 
-00005a90: 7665 7273 696f 6e73 2e20 270d 0a20 2020  versions. '..   
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2027 5573 6520 6060 2e72 6561 7373     'Use ``.reass
-00005ac0: 6967 6e5f 6964 7328 2960 6020 746f 206d  ign_ids()`` to m
-00005ad0: 616e 7561 6c6c 7920 7570 6461 7465 2069  anually update i
-00005ae0: 6473 272c 0d0a 2020 2020 2020 2020 2020  ds',..          
-00005af0: 2020 2020 2020 2020 2020 2020 7374 6163              stac
-00005b00: 6b6c 6576 656c 3d32 290d 0a20 2020 2020  klevel=2)..     
-00005b10: 2020 2073 656c 662e 7265 6173 7369 676e     self.reassign
-00005b20: 5f69 6473 2829 0d0a 0d0a 2020 2020 6465  _ids()....    de
-00005b30: 6620 7375 7070 7265 7373 5f73 696c 656e  f suppress_silen
-00005b40: 6365 2873 656c 662c 0d0a 2020 2020 2020  ce(self,..      
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2073 696c 656e 745f 7374 6172 7473     silent_starts
-00005b70: 3a20 6e70 2e6e 6461 7272 6179 2c0d 0a20  : np.ndarray,.. 
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2020 2020 2020 2020 7369 6c65 6e74 5f65          silent_e
-00005ba0: 6e64 733a 206e 702e 6e64 6172 7261 792c  nds: np.ndarray,
-00005bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bc0: 2020 2020 2020 2020 2020 206d 696e 5f77             min_w
-00005bd0: 6f72 645f 6475 723a 204f 7074 696f 6e61  ord_dur: Optiona
-00005be0: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
-00005bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005c00: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
-00005c10: 6c65 7665 6c3a 2062 6f6f 6c20 3d20 5472  level: bool = Tr
-00005c20: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00005c30: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00005c40: 6e73 7065 6563 685f 6572 726f 723a 2066  nspeech_error: f
-00005c50: 6c6f 6174 203d 2030 2e33 2c0d 0a20 2020  loat = 0.3,..   
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 2020 7573 655f 776f 7264 5f70        use_word_p
-00005c80: 6f73 6974 696f 6e3a 2062 6f6f 6c20 3d20  osition: bool = 
-00005c90: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-00005ca0: 6d69 6e5f 776f 7264 5f64 7572 203d 2067  min_word_dur = g
-00005cb0: 6574 5f6d 696e 5f77 6f72 645f 6475 7228  et_min_word_dur(
-00005cc0: 6d69 6e5f 776f 7264 5f64 7572 290d 0a20  min_word_dur).. 
-00005cd0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00005ce0: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
-00005cf0: 2020 2020 2020 2065 6e64 696e 675f 7075         ending_pu
-00005d00: 6e63 7475 6174 696f 6e73 203d 2067 6574  nctuations = get
-00005d10: 5f61 7070 656e 645f 7075 6e63 7475 6174  _append_punctuat
-00005d20: 696f 6e73 2829 0d0a 2020 2020 2020 2020  ions()..        
-00005d30: 2020 2020 776f 7264 7320 3d20 7365 6c66      words = self
-00005d40: 2e77 6f72 6473 2069 6620 776f 7264 5f6c  .words if word_l
-00005d50: 6576 656c 206f 7220 6c65 6e28 7365 6c66  evel or len(self
-00005d60: 2e77 6f72 6473 2920 3d3d 2031 2065 6c73  .words) == 1 els
-00005d70: 6520 5b73 656c 662e 776f 7264 735b 305d  e [self.words[0]
-00005d80: 2c20 7365 6c66 2e77 6f72 6473 5b2d 315d  , self.words[-1]
-00005d90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-00005da0: 6f72 2069 2c20 7720 696e 2065 6e75 6d65  or i, w in enume
-00005db0: 7261 7465 2877 6f72 6473 2c20 3129 3a0d  rate(words, 1):.
-00005dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005dd0: 2069 6620 7573 655f 776f 7264 5f70 6f73   if use_word_pos
-00005de0: 6974 696f 6e3a 0d0a 2020 2020 2020 2020  ition:..        
-00005df0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
-00005e00: 5f65 6e64 203d 206e 6f74 2028 772e 776f  _end = not (w.wo
-00005e10: 7264 5b2d 315d 2069 6e20 656e 6469 6e67  rd[-1] in ending
-00005e20: 5f70 756e 6374 7561 7469 6f6e 7320 6f72  _punctuations or
-00005e30: 2069 203d 3d20 6c65 6e28 776f 7264 7329   i == len(words)
-00005e40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005e50: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00005e60: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
-00005e70: 6570 5f65 6e64 203d 204e 6f6e 650d 0a20  ep_end = None.. 
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00005e90: 2e73 7570 7072 6573 735f 7369 6c65 6e63  .suppress_silenc
-00005ea0: 6528 7369 6c65 6e74 5f73 7461 7274 732c  e(silent_starts,
-00005eb0: 2073 696c 656e 745f 656e 6473 2c20 6d69   silent_ends, mi
-00005ec0: 6e5f 776f 7264 5f64 7572 2c20 6e6f 6e73  n_word_dur, nons
-00005ed0: 7065 6563 685f 6572 726f 722c 206b 6565  peech_error, kee
-00005ee0: 705f 656e 6429 0d0a 2020 2020 2020 2020  p_end)..        
-00005ef0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00005f00: 2020 2073 7570 7072 6573 735f 7369 6c65     suppress_sile
-00005f10: 6e63 6528 7365 6c66 2c0d 0a20 2020 2020  nce(self,..     
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 2020 2020 7369 6c65 6e74 5f73          silent_s
-00005f40: 7461 7274 732c 0d0a 2020 2020 2020 2020  tarts,..        
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2073 696c 656e 745f 656e 6473       silent_ends
-00005f70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 6d69 6e5f 776f 7264 5f64 7572 2c0d 0a20  min_word_dur,.. 
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 2020 2020 6e6f 6e73              nons
-00005fc0: 7065 6563 685f 6572 726f 7229 0d0a 0d0a  peech_error)....
-00005fd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005fe0: 656c 660d 0a0d 0a20 2020 2064 6566 2067  elf....    def g
-00005ff0: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
-00006000: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-00006010: 2020 6c6f 636b 6564 5f69 6e64 6963 6573    locked_indices
-00006020: 203d 205b 690d 0a20 2020 2020 2020 2020   = [i..         
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2066 6f72 2069 2c20 286c 6566 742c 2072   for i, (left, r
-00006050: 6967 6874 2920 696e 2065 6e75 6d65 7261  ight) in enumera
-00006060: 7465 287a 6970 2873 656c 662e 776f 7264  te(zip(self.word
-00006070: 735b 313a 5d2c 2073 656c 662e 776f 7264  s[1:], self.word
-00006080: 735b 3a2d 315d 2929 0d0a 2020 2020 2020  s[:-1]))..      
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 6966 206c 6566 742e 6c65 6674      if left.left
-000060b0: 5f6c 6f63 6b65 6420 6f72 2072 6967 6874  _locked or right
-000060c0: 2e72 6967 6874 5f6c 6f63 6b65 645d 0d0a  .right_locked]..
-000060d0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-000060e0: 6f63 6b65 645f 696e 6469 6365 730d 0a0d  ocked_indices...
-000060f0: 0a20 2020 2064 6566 2067 6574 5f67 6170  .    def get_gap
-00006100: 7328 7365 6c66 2c20 6173 5f6e 6461 7272  s(self, as_ndarr
-00006110: 6179 3d46 616c 7365 293a 0d0a 2020 2020  ay=False):..    
-00006120: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
-00006130: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
-00006140: 2020 2020 735f 7473 203d 206e 702e 6172      s_ts = np.ar
-00006150: 7261 7928 5b77 2e73 7461 7274 2066 6f72  ray([w.start for
-00006160: 2077 2069 6e20 7365 6c66 2e77 6f72 6473   w in self.words
-00006170: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00006180: 655f 7473 203d 206e 702e 6172 7261 7928  e_ts = np.array(
-00006190: 5b77 2e65 6e64 2066 6f72 2077 2069 6e20  [w.end for w in 
-000061a0: 7365 6c66 2e77 6f72 6473 5d29 0d0a 2020  self.words])..  
-000061b0: 2020 2020 2020 2020 2020 6761 7020 3d20            gap = 
-000061c0: 735f 7473 5b31 3a5d 202d 2065 5f74 735b  s_ts[1:] - e_ts[
-000061d0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
-000061e0: 2020 7265 7475 726e 2067 6170 2069 6620    return gap if 
-000061f0: 6173 5f6e 6461 7272 6179 2065 6c73 6520  as_ndarray else 
-00006200: 6761 702e 746f 6c69 7374 2829 0d0a 2020  gap.tolist()..  
-00006210: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
-00006220: 0a0d 0a20 2020 2064 6566 2067 6574 5f67  ...    def get_g
-00006230: 6170 5f69 6e64 6963 6573 2873 656c 662c  ap_indices(self,
-00006240: 206d 6178 5f67 6170 3a20 666c 6f61 7420   max_gap: float 
-00006250: 3d20 302e 3129 3a20 2023 2066 6f72 2073  = 0.1):  # for s
-00006260: 706c 6974 7469 6e67 0d0a 2020 2020 2020  plitting..      
-00006270: 2020 6966 206e 6f74 2073 656c 662e 6861    if not self.ha
-00006280: 735f 776f 7264 7320 6f72 206c 656e 2873  s_words or len(s
-00006290: 656c 662e 776f 7264 7329 203c 2032 3a0d  elf.words) < 2:.
-000062a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000062b0: 7572 6e20 5b5d 0d0a 2020 2020 2020 2020  urn []..        
-000062c0: 6966 206d 6178 5f67 6170 2069 7320 4e6f  if max_gap is No
-000062d0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000062e0: 206d 6178 5f67 6170 203d 2030 0d0a 2020   max_gap = 0..  
-000062f0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00006300: 2873 656c 662e 6765 745f 6761 7073 2854  (self.get_gaps(T
-00006310: 7275 6529 203e 206d 6178 5f67 6170 292e  rue) > max_gap).
-00006320: 6e6f 6e7a 6572 6f28 295b 305d 2e74 6f6c  nonzero()[0].tol
-00006330: 6973 7428 290d 0a20 2020 2020 2020 2072  ist()..        r
-00006340: 6574 7572 6e20 736f 7274 6564 2873 6574  eturn sorted(set
-00006350: 2869 6e64 6963 6573 2920 2d20 7365 7428  (indices) - set(
-00006360: 7365 6c66 2e67 6574 5f6c 6f63 6b65 645f  self.get_locked_
-00006370: 696e 6469 6365 7328 2929 290d 0a0d 0a20  indices())).... 
-00006380: 2020 2064 6566 2067 6574 5f70 756e 6374     def get_punct
-00006390: 7561 7469 6f6e 5f69 6e64 6963 6573 2873  uation_indices(s
-000063a0: 656c 662c 2070 756e 6374 7561 7469 6f6e  elf, punctuation
-000063b0: 3a20 556e 696f 6e5b 4c69 7374 5b73 7472  : Union[List[str
-000063c0: 5d2c 204c 6973 745b 5475 706c 655b 7374  ], List[Tuple[st
-000063d0: 722c 2073 7472 5d5d 2c20 7374 725d 293a  r, str]], str]):
-000063e0: 2020 2320 666f 7220 7370 6c69 7474 696e    # for splittin
-000063f0: 670d 0a20 2020 2020 2020 2069 6620 6e6f  g..        if no
-00006400: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
-00006410: 206f 7220 6c65 6e28 7365 6c66 2e77 6f72   or len(self.wor
-00006420: 6473 2920 3c20 323a 0d0a 2020 2020 2020  ds) < 2:..      
-00006430: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
-00006440: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00006450: 7374 616e 6365 2870 756e 6374 7561 7469  stance(punctuati
-00006460: 6f6e 2c20 7374 7229 3a0d 0a20 2020 2020  on, str):..     
-00006470: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
-00006480: 6f6e 203d 205b 7075 6e63 7475 6174 696f  on = [punctuatio
-00006490: 6e5d 0d0a 2020 2020 2020 2020 696e 6469  n]..        indi
-000064a0: 6365 7320 3d20 5b5d 0d0a 2020 2020 2020  ces = []..      
-000064b0: 2020 666f 7220 7020 696e 2070 756e 6374    for p in punct
-000064c0: 7561 7469 6f6e 3a0d 0a20 2020 2020 2020  uation:..       
-000064d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000064e0: 6365 2870 2c20 7374 7229 3a0d 0a20 2020  ce(p, str):..   
-000064f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006500: 2069 2c20 7320 696e 2065 6e75 6d65 7261   i, s in enumera
-00006510: 7465 2873 656c 662e 776f 7264 735b 3a2d  te(self.words[:-
-00006520: 315d 293a 0d0a 2020 2020 2020 2020 2020  1]):..          
-00006530: 2020 2020 2020 2020 2020 6966 2073 2e77            if s.w
-00006540: 6f72 642e 656e 6473 7769 7468 2870 293a  ord.endswith(p):
-00006550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006560: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00006570: 732e 6170 7065 6e64 2869 290d 0a20 2020  s.append(i)..   
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2065 6c69 6620 6920 213d 2030 2061 6e64   elif i != 0 and
-000065a0: 2073 2e77 6f72 642e 7374 6172 7473 7769   s.word.startswi
-000065b0: 7468 2870 293a 0d0a 2020 2020 2020 2020  th(p):..        
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 696e 6469 6365 732e 6170 7065 6e64 2869  indices.append(i
-000065e0: 2d31 290d 0a20 2020 2020 2020 2020 2020  -1)..           
-000065f0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00006600: 2020 2020 2020 2020 656e 6469 6e67 2c20          ending, 
-00006610: 6265 6769 6e6e 696e 6720 3d20 700d 0a20  beginning = p.. 
-00006620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006630: 6e64 6963 6573 2e65 7874 656e 6428 5b69  ndices.extend([i
-00006640: 2066 6f72 2069 2c20 2877 302c 2077 3129   for i, (w0, w1)
-00006650: 2069 6e20 656e 756d 6572 6174 6528 7a69   in enumerate(zi
-00006660: 7028 7365 6c66 2e77 6f72 6473 5b3a 2d31  p(self.words[:-1
-00006670: 5d2c 2073 656c 662e 776f 7264 735b 313a  ], self.words[1:
-00006680: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066a0: 2020 2020 2069 6620 7730 2e77 6f72 642e       if w0.word.
-000066b0: 656e 6473 7769 7468 2865 6e64 696e 6729  endswith(ending)
-000066c0: 2061 6e64 2077 312e 776f 7264 2e73 7461   and w1.word.sta
-000066d0: 7274 7377 6974 6828 6265 6769 6e6e 696e  rtswith(beginnin
-000066e0: 6729 5d29 0d0a 0d0a 2020 2020 2020 2020  g)])....        
-000066f0: 7265 7475 726e 2073 6f72 7465 6428 7365  return sorted(se
-00006700: 7428 696e 6469 6365 7329 202d 2073 6574  t(indices) - set
-00006710: 2873 656c 662e 6765 745f 6c6f 636b 6564  (self.get_locked
-00006720: 5f69 6e64 6963 6573 2829 2929 0d0a 0d0a  _indices()))....
-00006730: 2020 2020 6465 6620 6765 745f 6c65 6e67      def get_leng
-00006740: 7468 5f69 6e64 6963 6573 2873 656c 662c  th_indices(self,
-00006750: 206d 6178 5f63 6861 7273 3a20 696e 7420   max_chars: int 
-00006760: 3d20 4e6f 6e65 2c20 6d61 785f 776f 7264  = None, max_word
-00006770: 733a 2069 6e74 203d 204e 6f6e 652c 2065  s: int = None, e
-00006780: 7665 6e5f 7370 6c69 743a 2062 6f6f 6c20  ven_split: bool 
-00006790: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 696e 636c 7564 655f 6c6f 636b      include_lock
-000067c0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
-000067d0: 0d0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
-000067e0: 7370 6c69 7474 696e 670d 0a20 2020 2020  splitting..     
-000067f0: 2020 2069 6620 6e6f 7420 7365 6c66 2e68     if not self.h
-00006800: 6173 5f77 6f72 6473 206f 7220 286d 6178  as_words or (max
-00006810: 5f63 6861 7273 2069 7320 4e6f 6e65 2061  _chars is None a
-00006820: 6e64 206d 6178 5f77 6f72 6473 2069 7320  nd max_words is 
-00006830: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-00006840: 2020 2020 7265 7475 726e 205b 5d0d 0a20      return [].. 
-00006850: 2020 2020 2020 2061 7373 6572 7420 6d61         assert ma
-00006860: 785f 6368 6172 7320 213d 2030 2061 6e64  x_chars != 0 and
-00006870: 206d 6178 5f77 6f72 6473 2021 3d20 302c   max_words != 0,
-00006880: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
-00006890: 6627 6d61 785f 6368 6172 7320 616e 6420  f'max_chars and 
-000068a0: 6d61 785f 776f 7264 7320 6d75 7374 2062  max_words must b
-000068b0: 6520 6772 6561 7465 7220 302c 2062 7574  e greater 0, but
-000068c0: 2067 6f74 207b 6d61 785f 6368 6172 737d   got {max_chars}
-000068d0: 2061 6e64 207b 6d61 785f 776f 7264 737d   and {max_words}
-000068e0: 270d 0a20 2020 2020 2020 2069 6620 6c65  '..        if le
-000068f0: 6e28 7365 6c66 2e77 6f72 6473 2920 3c20  n(self.words) < 
-00006900: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-00006910: 7265 7475 726e 205b 5d0d 0a20 2020 2020  return []..     
-00006920: 2020 2069 6e64 6963 6573 203d 205b 5d0d     indices = [].
-00006930: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-00006940: 5f73 706c 6974 3a0d 0a20 2020 2020 2020  _split:..       
-00006950: 2020 2020 2063 6861 725f 636f 756e 7420       char_count 
-00006960: 3d20 2d31 2069 6620 6d61 785f 6368 6172  = -1 if max_char
-00006970: 7320 6973 204e 6f6e 6520 656c 7365 2073  s is None else s
-00006980: 756d 286d 6170 286c 656e 2c20 7365 6c66  um(map(len, self
-00006990: 2e77 6f72 6473 2929 0d0a 2020 2020 2020  .words))..      
-000069a0: 2020 2020 2020 776f 7264 5f63 6f75 6e74        word_count
-000069b0: 203d 202d 3120 6966 206d 6178 5f77 6f72   = -1 if max_wor
-000069c0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-000069d0: 6c65 6e28 7365 6c66 2e77 6f72 6473 290d  len(self.words).
-000069e0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000069f0: 6565 645f 6368 6172 7320 3d20 6d61 785f  eed_chars = max_
-00006a00: 6368 6172 7320 6973 206e 6f74 204e 6f6e  chars is not Non
-00006a10: 6520 616e 6420 6368 6172 5f63 6f75 6e74  e and char_count
-00006a20: 203e 206d 6178 5f63 6861 7273 0d0a 2020   > max_chars..  
-00006a30: 2020 2020 2020 2020 2020 6578 6365 6564            exceed
-00006a40: 5f77 6f72 6473 203d 206d 6178 5f77 6f72  _words = max_wor
-00006a50: 6473 2069 7320 6e6f 7420 4e6f 6e65 2061  ds is not None a
-00006a60: 6e64 2077 6f72 645f 636f 756e 7420 3e20  nd word_count > 
-00006a70: 6d61 785f 776f 7264 730d 0a20 2020 2020  max_words..     
-00006a80: 2020 2020 2020 2069 6620 6578 6365 6564         if exceed
-00006a90: 5f63 6861 7273 3a0d 0a20 2020 2020 2020  _chars:..       
-00006aa0: 2020 2020 2020 2020 2073 706c 6974 7320           splits 
-00006ab0: 3d20 6e70 2e63 6569 6c28 6368 6172 5f63  = np.ceil(char_c
-00006ac0: 6f75 6e74 202f 206d 6178 5f63 6861 7273  ount / max_chars
-00006ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006ae0: 2020 2063 6861 7273 5f70 6572 5f73 706c     chars_per_spl
-00006af0: 6974 203d 2063 6861 725f 636f 756e 7420  it = char_count 
-00006b00: 2f20 7370 6c69 7473 0d0a 2020 2020 2020  / splits..      
-00006b10: 2020 2020 2020 2020 2020 6375 6d5f 6368            cum_ch
-00006b20: 6172 5f63 6f75 6e74 203d 206e 702e 6375  ar_count = np.cu
-00006b30: 6d73 756d 285b 6c65 6e28 772e 776f 7264  msum([len(w.word
-00006b40: 2920 666f 7220 7720 696e 2073 656c 662e  ) for w in self.
-00006b50: 776f 7264 735b 3a2d 315d 5d29 0d0a 2020  words[:-1]])..  
-00006b60: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006b70: 6469 6365 7320 3d20 5b0d 0a20 2020 2020  dices = [..     
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00006b90: 6e70 2e61 6273 2863 756d 5f63 6861 725f  np.abs(cum_char_
-00006ba0: 636f 756e 742d 2869 2a63 6861 7273 5f70  count-(i*chars_p
-00006bb0: 6572 5f73 706c 6974 2929 292e 6172 676d  er_split))).argm
-00006bc0: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
-00006bd0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00006be0: 696e 2072 616e 6765 2831 2c20 696e 7428  in range(1, int(
-00006bf0: 7370 6c69 7473 2929 0d0a 2020 2020 2020  splits))..      
-00006c00: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-00006c10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006c20: 6d61 785f 776f 7264 7320 6973 206e 6f74  max_words is not
-00006c30: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00006c40: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00006c50: 6564 5f77 6f72 6473 203d 2061 6e79 286a  ed_words = any(j
-00006c60: 2d69 2b31 203e 206d 6178 5f77 6f72 6473  -i+1 > max_words
-00006c70: 2066 6f72 2069 2c20 6a20 696e 207a 6970   for i, j in zip
-00006c80: 285b 305d 2b69 6e64 6963 6573 2c20 696e  ([0]+indices, in
-00006c90: 6469 6365 732b 5b6c 656e 2873 656c 662e  dices+[len(self.
-00006ca0: 776f 7264 7329 5d29 290d 0a0d 0a20 2020  words)]))....   
-00006cb0: 2020 2020 2020 2020 2069 6620 6578 6365           if exce
-00006cc0: 6564 5f77 6f72 6473 3a0d 0a20 2020 2020  ed_words:..     
-00006cd0: 2020 2020 2020 2020 2020 2073 706c 6974             split
-00006ce0: 7320 3d20 6e70 2e63 6569 6c28 776f 7264  s = np.ceil(word
-00006cf0: 5f63 6f75 6e74 202f 206d 6178 5f77 6f72  _count / max_wor
-00006d00: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00006d10: 2020 2020 2077 6f72 6473 5f70 6572 5f73       words_per_s
-00006d20: 706c 6974 203d 2077 6f72 645f 636f 756e  plit = word_coun
-00006d30: 7420 2f20 7370 6c69 7473 0d0a 2020 2020  t / splits..    
-00006d40: 2020 2020 2020 2020 2020 2020 6375 6d5f              cum_
-00006d50: 776f 7264 5f63 6f75 6e74 203d 206e 702e  word_count = np.
-00006d60: 6172 7261 7928 7261 6e67 6528 312c 206c  array(range(1, l
-00006d70: 656e 2873 656c 662e 776f 7264 7329 2b31  en(self.words)+1
-00006d80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006d90: 2020 2020 696e 6469 6365 7320 3d20 5b0d      indices = [.
-00006da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006db0: 2020 2020 206e 702e 6162 7328 6375 6d5f       np.abs(cum_
-00006dc0: 776f 7264 5f63 6f75 6e74 2d28 692a 776f  word_count-(i*wo
-00006dd0: 7264 735f 7065 725f 7370 6c69 7429 292e  rds_per_split)).
-00006de0: 6172 676d 696e 2829 0d0a 2020 2020 2020  argmin()..      
-00006df0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00006e00: 7220 6920 696e 2072 616e 6765 2831 2c20  r i in range(1, 
-00006e10: 696e 7428 7370 6c69 7473 2929 0d0a 2020  int(splits))..  
-00006e20: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
-00006e30: 0a0d 0a20 2020 2020 2020 2065 6c73 653a  ...        else:
-00006e40: 0d0a 2020 2020 2020 2020 2020 2020 6375  ..            cu
-00006e50: 7272 5f77 6f72 6473 203d 2030 0d0a 2020  rr_words = 0..  
-00006e60: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
-00006e70: 6861 7273 203d 2030 0d0a 2020 2020 2020  hars = 0..      
-00006e80: 2020 2020 2020 6c6f 636b 6564 5f69 6e64        locked_ind
-00006e90: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
-00006ea0: 2020 2020 2020 2069 6620 696e 636c 7564         if includ
-00006eb0: 655f 6c6f 636b 3a0d 0a20 2020 2020 2020  e_lock:..       
-00006ec0: 2020 2020 2020 2020 206c 6f63 6b65 645f           locked_
-00006ed0: 696e 6469 6365 7320 3d20 7365 6c66 2e67  indices = self.g
-00006ee0: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
-00006ef0: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00006f00: 2066 6f72 2069 2c20 776f 7264 2069 6e20   for i, word in 
-00006f10: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
-00006f20: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
-00006f30: 2020 2020 2020 2020 6375 7272 5f77 6f72          curr_wor
-00006f40: 6473 202b 3d20 310d 0a20 2020 2020 2020  ds += 1..       
-00006f50: 2020 2020 2020 2020 2063 7572 725f 6368           curr_ch
-00006f60: 6172 7320 2b3d 206c 656e 2877 6f72 6429  ars += len(word)
-00006f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006f80: 2020 6966 2069 2021 3d20 303a 0d0a 2020    if i != 0:..  
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2020 6966 2028 0d0a 2020 2020 2020 2020    if (..        
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 6d61 785f 6368 6172 7320 6973      max_chars is
-00006fd0: 206e 6f74 204e 6f6e 6520 616e 6420 6375   not None and cu
-00006fe0: 7272 5f63 6861 7273 203e 206d 6178 5f63  rr_chars > max_c
-00006ff0: 6861 7273 0d0a 2020 2020 2020 2020 2020  hars..          
-00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007010: 2020 6f72 0d0a 2020 2020 2020 2020 2020    or..          
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 6d61 785f 776f 7264 7320 6973 206e    max_words is n
-00007040: 6f74 204e 6f6e 6520 616e 6420 6375 7272  ot None and curr
-00007050: 5f77 6f72 6473 203e 206d 6178 5f77 6f72  _words > max_wor
-00007060: 6473 0d0a 2020 2020 2020 2020 2020 2020  ds..            
-00007070: 2020 2020 2020 2020 2920 616e 6420 692d          ) and i-
-00007080: 3120 6e6f 7420 696e 206c 6f63 6b65 645f  1 not in locked_
-00007090: 696e 6469 6365 733a 0d0a 2020 2020 2020  indices:..      
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 696e 6469 6365 732e 6170 7065 6e64    indices.append
-000070c0: 2869 2d31 290d 0a20 2020 2020 2020 2020  (i-1)..         
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000070e0: 7572 725f 776f 7264 7320 3d20 310d 0a20  urr_words = 1.. 
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007100: 2020 2020 2020 2063 7572 725f 6368 6172         curr_char
-00007110: 7320 3d20 6c65 6e28 776f 7264 290d 0a20  s = len(word).. 
-00007120: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
-00007130: 6469 6365 730d 0a0d 0a20 2020 2064 6566  dices....    def
-00007140: 2067 6574 5f64 7572 6174 696f 6e5f 696e   get_duration_in
-00007150: 6469 6365 7328 7365 6c66 2c20 6d61 785f  dices(self, max_
-00007160: 6475 723a 2066 6c6f 6174 2c20 6576 656e  dur: float, even
-00007170: 5f73 706c 6974 3a20 626f 6f6c 203d 2054  _split: bool = T
-00007180: 7275 652c 2069 6e63 6c75 6465 5f6c 6f63  rue, include_loc
-00007190: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 6529  k: bool = False)
-000071a0: 3a0d 0a20 2020 2020 2020 2069 6620 6e6f  :..        if no
-000071b0: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
-000071c0: 206f 7220 2874 6f74 616c 5f64 7572 6174   or (total_durat
-000071d0: 696f 6e20 3a3d 206e 702e 7375 6d28 5b77  ion := np.sum([w
-000071e0: 2e64 7572 6174 696f 6e20 666f 7220 7720  .duration for w 
-000071f0: 696e 2073 656c 662e 776f 7264 735d 2929  in self.words]))
-00007200: 203c 3d20 6d61 785f 6475 723a 0d0a 2020   <= max_dur:..  
-00007210: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007220: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
-00007230: 6576 656e 5f73 706c 6974 3a0d 0a20 2020  even_split:..   
-00007240: 2020 2020 2020 2020 2073 706c 6974 7320           splits 
-00007250: 3d20 6e70 2e63 6569 6c28 746f 7461 6c5f  = np.ceil(total_
-00007260: 6475 7261 7469 6f6e 202f 206d 6178 5f64  duration / max_d
-00007270: 7572 290d 0a20 2020 2020 2020 2020 2020  ur)..           
-00007280: 2064 7572 5f70 6572 5f73 706c 6974 203d   dur_per_split =
-00007290: 2074 6f74 616c 5f64 7572 6174 696f 6e20   total_duration 
-000072a0: 2f20 7370 6c69 7473 0d0a 2020 2020 2020  / splits..      
-000072b0: 2020 2020 2020 6375 6d5f 6475 7220 3d20        cum_dur = 
-000072c0: 6e70 2e63 756d 7375 6d28 5b77 2e64 7572  np.cumsum([w.dur
-000072d0: 6174 696f 6e20 666f 7220 7720 696e 2073  ation for w in s
-000072e0: 656c 662e 776f 7264 735b 3a2d 315d 5d29  elf.words[:-1]])
-000072f0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00007300: 6469 6365 7320 3d20 5b0d 0a20 2020 2020  dices = [..     
-00007310: 2020 2020 2020 2020 2020 2028 6e70 2e61             (np.a
-00007320: 6273 2863 756d 5f64 7572 202d 2028 6920  bs(cum_dur - (i 
-00007330: 2a20 6475 725f 7065 725f 7370 6c69 7429  * dur_per_split)
-00007340: 2929 2e61 7267 6d69 6e28 290d 0a20 2020  )).argmin()..   
-00007350: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00007360: 2069 2069 6e20 7261 6e67 6528 312c 2069   i in range(1, i
-00007370: 6e74 2873 706c 6974 7329 290d 0a20 2020  nt(splits))..   
-00007380: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00007390: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000073a0: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-000073b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000073c0: 2063 7572 725f 746f 7461 6c5f 6475 7220   curr_total_dur 
-000073d0: 3d20 302e 300d 0a20 2020 2020 2020 2020  = 0.0..         
-000073e0: 2020 206c 6f63 6b65 645f 696e 6469 6365     locked_indice
-000073f0: 7320 3d20 7365 6c66 2e67 6574 5f6c 6f63  s = self.get_loc
-00007400: 6b65 645f 696e 6469 6365 7328 2920 6966  ked_indices() if
-00007410: 2069 6e63 6c75 6465 5f6c 6f63 6b20 656c   include_lock el
-00007420: 7365 205b 5d0d 0a20 2020 2020 2020 2020  se []..         
-00007430: 2020 2066 6f72 2069 2c20 776f 7264 2069     for i, word i
-00007440: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
-00007450: 2e77 6f72 6473 293a 0d0a 2020 2020 2020  .words):..      
-00007460: 2020 2020 2020 2020 2020 6375 7272 5f74            curr_t
-00007470: 6f74 616c 5f64 7572 202b 3d20 776f 7264  otal_dur += word
-00007480: 2e64 7572 6174 696f 6e0d 0a20 2020 2020  .duration..     
-00007490: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-000074a0: 213d 2030 3a0d 0a20 2020 2020 2020 2020  != 0:..         
-000074b0: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
-000074c0: 7272 5f74 6f74 616c 5f64 7572 203e 206d  rr_total_dur > m
-000074d0: 6178 5f64 7572 2061 6e64 2069 202d 2031  ax_dur and i - 1
-000074e0: 206e 6f74 2069 6e20 6c6f 636b 6564 5f69   not in locked_i
-000074f0: 6e64 6963 6573 3a0d 0a20 2020 2020 2020  ndices:..       
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 2069 6e64 6963 6573 2e61 7070 656e 6428   indices.append(
-00007520: 6920 2d20 3129 0d0a 2020 2020 2020 2020  i - 1)..        
-00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 6375 7272 5f74 6f74 616c 5f64 7572 203d  curr_total_dur =
-00007550: 2077 6f72 642e 6475 7261 7469 6f6e 0d0a   word.duration..
-00007560: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00007570: 6e64 6963 6573 0d0a 0d0a 2020 2020 6465  ndices....    de
-00007580: 6620 7370 6c69 7428 7365 6c66 2c20 696e  f split(self, in
-00007590: 6469 6365 733a 204c 6973 745b 696e 745d  dices: List[int]
-000075a0: 293a 0d0a 2020 2020 2020 2020 6966 206c  ):..        if l
-000075b0: 656e 2869 6e64 6963 6573 2920 3d3d 2030  en(indices) == 0
-000075c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000075d0: 6574 7572 6e20 5b5d 0d0a 2020 2020 2020  eturn []..      
-000075e0: 2020 6966 2069 6e64 6963 6573 5b2d 315d    if indices[-1]
-000075f0: 2021 3d20 6c65 6e28 7365 6c66 2e77 6f72   != len(self.wor
-00007600: 6473 2920 2d20 313a 0d0a 2020 2020 2020  ds) - 1:..      
-00007610: 2020 2020 2020 696e 6469 6365 732e 6170        indices.ap
-00007620: 7065 6e64 286c 656e 2873 656c 662e 776f  pend(len(self.wo
-00007630: 7264 7329 202d 2031 290d 0a20 2020 2020  rds) - 1)..     
-00007640: 2020 2073 6567 5f63 6f70 6965 7320 3d20     seg_copies = 
-00007650: 5b5d 0d0a 2020 2020 2020 2020 7072 6576  []..        prev
-00007660: 5f69 203d 2030 0d0a 2020 2020 2020 2020  _i = 0..        
-00007670: 666f 7220 6920 696e 2069 6e64 6963 6573  for i in indices
-00007680: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00007690: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-000076a0: 2020 206e 6577 5f77 6f72 6473 203d 2073     new_words = s
-000076b0: 656c 662e 776f 7264 735b 7072 6576 5f69  elf.words[prev_i
-000076c0: 3a69 5d0d 0a20 2020 2020 2020 2020 2020  :i]..           
-000076d0: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
-000076e0: 636f 7079 286e 6577 5f77 6f72 6473 2c20  copy(new_words, 
-000076f0: 636f 7079 5f77 6f72 6473 3d46 616c 7365  copy_words=False
-00007700: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00007710: 6567 5f63 6f70 6965 732e 6170 7065 6e64  eg_copies.append
-00007720: 286e 6577 5f73 6567 290d 0a20 2020 2020  (new_seg)..     
-00007730: 2020 2020 2020 2070 7265 765f 6920 3d20         prev_i = 
-00007740: 690d 0a20 2020 2020 2020 2072 6574 7572  i..        retur
-00007750: 6e20 7365 675f 636f 7069 6573 0d0a 0d0a  n seg_copies....
-00007760: 2020 2020 6465 6620 7365 745f 7265 7375      def set_resu
-00007770: 6c74 2873 656c 662c 2072 6573 756c 743a  lt(self, result:
-00007780: 2027 5768 6973 7065 7252 6573 756c 7427   'WhisperResult'
-00007790: 293a 0d0a 2020 2020 2020 2020 7761 726e  ):..        warn
-000077a0: 696e 6773 2e77 6172 6e28 2760 602e 7365  ings.warn('``.se
-000077b0: 745f 7265 7375 6c74 2863 7572 7265 6e74  t_result(current
-000077c0: 5f72 6573 756c 745f 696e 7374 616e 6365  _result_instance
-000077d0: 2960 6020 6973 2064 6570 7265 6361 7465  )`` is deprecate
-000077e0: 6420 616e 6420 7769 6c6c 2062 6520 7265  d and will be re
-000077f0: 6d6f 7665 6420 696e 2066 7574 7572 6520  moved in future 
-00007800: 7665 7273 696f 6e73 2e20 270d 0a20 2020  versions. '..   
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2027 5573 6520 6060 2e72 6573 756c     'Use ``.resul
-00007830: 7420 3d20 6375 7272 656e 745f 7265 7375  t = current_resu
-00007840: 6c74 5f69 6e73 7461 6e63 6560 6020 696e  lt_instance`` in
-00007850: 7374 6561 642e 272c 0d0a 2020 2020 2020  stead.',..      
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 7374 6163 6b6c 6576 656c 3d32 290d 0a20  stacklevel=2).. 
-00007880: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
-00007890: 6c74 203d 2072 6573 756c 740d 0a0d 0a20  lt = result.... 
-000078a0: 2020 2064 6566 2067 6574 5f72 6573 756c     def get_resul
-000078b0: 7428 7365 6c66 2920 2d3e 2055 6e69 6f6e  t(self) -> Union
-000078c0: 5b27 5768 6973 7065 7252 6573 756c 7427  ['WhisperResult'
-000078d0: 2c20 4e6f 6e65 5d3a 0d0a 2020 2020 2020  , None]:..      
-000078e0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
-000078f0: 6574 7572 6e20 6f75 7465 7220 696e 7374  eturn outer inst
-00007900: 616e 6365 206f 6620 3a63 6c61 7373 3a60  ance of :class:`
-00007910: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
-00007920: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
-00007930: 756c 7460 2074 6861 7420 6060 7365 6c66  ult` that ``self
-00007940: 6060 2069 7320 6120 7061 7274 206f 662e  `` is a part of.
-00007950: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00007960: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-00007970: 7761 726e 2827 6060 2e67 6574 5f72 6573  warn('``.get_res
-00007980: 756c 7428 2960 6020 7769 6c6c 2062 6520  ult()`` will be 
-00007990: 7265 6d6f 7665 6420 696e 2066 7574 7572  removed in futur
-000079a0: 6520 7665 7273 696f 6e73 2e20 5573 6520  e versions. Use 
-000079b0: 6060 2e72 6573 756c 7460 6020 696e 7374  ``.result`` inst
-000079c0: 6561 642e 272c 0d0a 2020 2020 2020 2020  ead.',..        
-000079d0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-000079e0: 6163 6b6c 6576 656c 3d32 290d 0a20 2020  acklevel=2)..   
-000079f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007a00: 2e72 6573 756c 740d 0a0d 0a0d 0a63 6c61  .result......cla
-00007a10: 7373 2057 6869 7370 6572 5265 7375 6c74  ss WhisperResult
-00007a20: 3a0d 0a0d 0a20 2020 2064 6566 205f 5f69  :....    def __i
-00007a30: 6e69 745f 5f28 0d0a 2020 2020 2020 2020  nit__(..        
-00007a40: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-00007a50: 2020 2020 2020 2072 6573 756c 743a 2055         result: U
-00007a60: 6e69 6f6e 5b73 7472 2c20 6469 6374 2c20  nion[str, dict, 
-00007a70: 6c69 7374 5d2c 0d0a 2020 2020 2020 2020  list],..        
-00007a80: 2020 2020 666f 7263 655f 6f72 6465 723a      force_order:
-00007a90: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00007aa0: 2020 2020 2020 2020 2020 2020 6368 6563              chec
-00007ab0: 6b5f 736f 7274 6564 3a20 556e 696f 6e5b  k_sorted: Union[
-00007ac0: 626f 6f6c 2c20 7374 725d 203d 2054 7275  bool, str] = Tru
-00007ad0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00007ae0: 7368 6f77 5f75 6e73 6f72 7465 643a 2062  show_unsorted: b
-00007af0: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
-00007b00: 293a 0d0a 2020 2020 2020 2020 7265 7375  ):..        resu
-00007b10: 6c74 2c20 7365 6c66 2e70 6174 6820 3d20  lt, self.path = 
-00007b20: 7365 6c66 2e5f 7374 616e 6461 7264 697a  self._standardiz
-00007b30: 655f 7265 7375 6c74 2872 6573 756c 7429  e_result(result)
-00007b40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00007b50: 7269 5f64 6963 7420 3d20 7265 7375 6c74  ri_dict = result
-00007b60: 2e67 6574 2827 6f72 695f 6469 6374 2729  .get('ori_dict')
-00007b70: 206f 7220 7265 7375 6c74 0d0a 2020 2020   or result..    
-00007b80: 2020 2020 7365 6c66 2e6c 616e 6775 6167      self.languag
-00007b90: 6520 3d20 7365 6c66 2e6f 7269 5f64 6963  e = self.ori_dic
-00007ba0: 742e 6765 7428 276c 616e 6775 6167 6527  t.get('language'
-00007bb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007bc0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-00007bd0: 203d 2072 6573 756c 742e 6765 7428 2772   = result.get('r
-00007be0: 6567 726f 7570 5f68 6973 746f 7279 272c  egroup_history',
-00007bf0: 2027 2729 0d0a 2020 2020 2020 2020 7365   '')..        se
-00007c00: 6c66 2e5f 6e6f 6e73 7065 6563 685f 7365  lf._nonspeech_se
-00007c10: 6374 696f 6e73 203d 2072 6573 756c 742e  ctions = result.
-00007c20: 6765 7428 276e 6f6e 7370 6565 6368 5f73  get('nonspeech_s
-00007c30: 6563 7469 6f6e 7327 2c20 5b5d 290d 0a20  ections', []).. 
-00007c40: 2020 2020 2020 2073 6567 6d65 6e74 7320         segments 
-00007c50: 3d20 2872 6573 756c 742e 6765 7428 2773  = (result.get('s
-00007c60: 6567 6d65 6e74 7327 2c20 7365 6c66 2e6f  egments', self.o
-00007c70: 7269 5f64 6963 742e 6765 7428 2773 6567  ri_dict.get('seg
-00007c80: 6d65 6e74 7327 2929 206f 7220 7b7d 292e  ments')) or {}).
-00007c90: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00007ca0: 7365 6c66 2e73 6567 6d65 6e74 7320 3d20  self.segments = 
-00007cb0: 5b53 6567 6d65 6e74 282a 2a73 2c20 6967  [Segment(**s, ig
-00007cc0: 6e6f 7265 5f75 6e75 7365 645f 6172 6773  nore_unused_args
-00007cd0: 3d54 7275 6529 2066 6f72 2073 2069 6e20  =True) for s in 
-00007ce0: 7365 676d 656e 7473 5d20 6966 2073 6567  segments] if seg
-00007cf0: 6d65 6e74 7320 656c 7365 205b 5d0d 0a20  ments else [].. 
-00007d00: 2020 2020 2020 2073 656c 662e 5f66 6f72         self._for
-00007d10: 6365 645f 6f72 6465 7220 3d20 666f 7263  ced_order = forc
-00007d20: 655f 6f72 6465 720d 0a20 2020 2020 2020  e_order..       
-00007d30: 2069 6620 7365 6c66 2e5f 666f 7263 6564   if self._forced
-00007d40: 5f6f 7264 6572 3a0d 0a20 2020 2020 2020  _order:..       
-00007d50: 2020 2020 2073 656c 662e 666f 7263 655f       self.force_
-00007d60: 6f72 6465 7228 290d 0a20 2020 2020 2020  order()..       
-00007d70: 2073 656c 662e 7261 6973 655f 666f 725f   self.raise_for_
-00007d80: 756e 736f 7274 6564 2863 6865 636b 5f73  unsorted(check_s
-00007d90: 6f72 7465 642c 2073 686f 775f 756e 736f  orted, show_unso
-00007da0: 7274 6564 290d 0a20 2020 2020 2020 2073  rted)..        s
-00007db0: 656c 662e 7265 6d6f 7665 5f6e 6f5f 776f  elf.remove_no_wo
-00007dc0: 7264 5f73 6567 6d65 6e74 7328 616e 7928  rd_segments(any(
-00007dd0: 7365 672e 6861 735f 776f 7264 7320 666f  seg.has_words fo
-00007de0: 7220 7365 6720 696e 2073 656c 662e 7365  r seg in self.se
-00007df0: 676d 656e 7473 2929 0d0a 0d0a 2020 2020  gments))....    
-00007e00: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
-00007e10: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
-00007e20: 2920 2d3e 2053 6567 6d65 6e74 3a0d 0a20  ) -> Segment:.. 
-00007e30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00007e40: 6c66 2e73 6567 6d65 6e74 735b 696e 6465  lf.segments[inde
-00007e50: 785d 0d0a 0d0a 2020 2020 6465 6620 5f5f  x]....    def __
-00007e60: 6465 6c69 7465 6d5f 5f28 7365 6c66 2c20  delitem__(self, 
-00007e70: 696e 6465 783a 2069 6e74 293a 0d0a 2020  index: int):..  
-00007e80: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
-00007e90: 6567 6d65 6e74 735b 696e 6465 785d 0d0a  egments[index]..
-00007ea0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00007eb0: 7373 6967 6e5f 6964 7328 5472 7565 2c20  ssign_ids(True, 
-00007ec0: 7374 6172 743d 696e 6465 7829 0d0a 0d0a  start=index)....
-00007ed0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00007ee0: 2020 2064 6566 2064 7572 6174 696f 6e28     def duration(
-00007ef0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00007f00: 6966 206e 6f74 2073 656c 662e 7365 676d  if not self.segm
-00007f10: 656e 7473 3a0d 0a20 2020 2020 2020 2020  ents:..         
-00007f20: 2020 2072 6574 7572 6e20 302e 300d 0a20     return 0.0.. 
-00007f30: 2020 2020 2020 2072 6574 7572 6e20 5f72         return _r
-00007f40: 6f75 6e64 5f74 696d 6573 7461 6d70 2873  ound_timestamp(s
-00007f50: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
-00007f60: 2e65 6e64 202d 2073 656c 662e 7365 676d  .end - self.segm
-00007f70: 656e 7473 5b30 5d2e 7374 6172 7429 0d0a  ents[0].start)..
-00007f80: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00007f90: 686f 640d 0a20 2020 2064 6566 205f 7374  hod..    def _st
-00007fa0: 616e 6461 7264 697a 655f 7265 7375 6c74  andardize_result
-00007fb0: 2872 6573 756c 743a 2055 6e69 6f6e 5b73  (result: Union[s
-00007fc0: 7472 2c20 6469 6374 2c20 4c69 7374 5b64  tr, dict, List[d
-00007fd0: 6963 745d 2c20 4c69 7374 5b4c 6973 745b  ict], List[List[
-00007fe0: 6469 6374 5d5d 5d29 202d 3e20 5475 706c  dict]]]) -> Tupl
-00007ff0: 655b 6469 6374 2c20 556e 696f 6e5b 7374  e[dict, Union[st
-00008000: 722c 204e 6f6e 655d 5d3a 0d0a 2020 2020  r, None]]:..    
-00008010: 2020 2020 7061 7468 203d 204e 6f6e 650d      path = None.
-00008020: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00008030: 7374 616e 6365 2872 6573 756c 742c 2073  stance(result, s
-00008040: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
-00008050: 2020 7061 7468 203d 2072 6573 756c 740d    path = result.
-00008060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00008070: 756c 7420 3d20 6c6f 6164 5f72 6573 756c  ult = load_resul
-00008080: 7428 7061 7468 290d 0a20 2020 2020 2020  t(path)..       
-00008090: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-000080a0: 6573 756c 742c 2064 6963 7429 3a0d 0a20  esult, dict):.. 
-000080b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000080c0: 6e20 7265 7375 6c74 2c20 7061 7468 0d0a  n result, path..
-000080d0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-000080e0: 7369 6e73 7461 6e63 6528 7265 7375 6c74  sinstance(result
-000080f0: 2c20 6c69 7374 293a 0d0a 2020 2020 2020  , list):..      
-00008100: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00008110: 4572 726f 7228 6627 4578 7065 6374 2072  Error(f'Expect r
-00008120: 6573 756c 7420 746f 2062 6520 6c69 7374  esult to be list
-00008130: 2062 7574 2067 6f74 207b 7479 7065 2872   but got {type(r
-00008140: 6573 756c 7429 7d27 290d 0a20 2020 2020  esult)}')..     
-00008150: 2020 2069 6620 6e6f 7420 7265 7375 6c74     if not result
-00008160: 206f 7220 6e6f 7420 7265 7375 6c74 5b30   or not result[0
-00008170: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-00008180: 7265 7475 726e 207b 7d2c 2070 6174 680d  return {}, path.
-00008190: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-000081a0: 7374 616e 6365 2872 6573 756c 745b 305d  stance(result[0]
-000081b0: 2c20 6c69 7374 293a 0d0a 2020 2020 2020  , list):..      
-000081c0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-000081d0: 6e73 7461 6e63 6528 7265 7375 6c74 5b30  nstance(result[0
-000081e0: 5d5b 305d 2c20 6469 6374 293a 0d0a 2020  ][0], dict):..  
-000081f0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00008200: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00008210: 6564 4572 726f 7228 6627 476f 7420 6c69  edError(f'Got li
-00008220: 7374 206f 6620 6c69 7374 206f 6620 7b74  st of list of {t
-00008230: 7970 6528 7265 7375 6c74 5b30 5d29 7d20  ype(result[0])} 
-00008240: 6275 7420 6578 7065 6374 7320 6c69 7374  but expects list
-00008250: 206f 6620 6c69 7374 206f 6620 6469 6374   of list of dict
-00008260: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00008270: 7265 7375 6c74 203d 2064 6963 7428 0d0a  result = dict(..
-00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 7365 676d 656e 7473 3d5b 0d0a 2020 2020  segments=[..    
-000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000082d0: 7461 7274 3d77 6f72 6473 5b30 5d5b 2773  tart=words[0]['s
-000082e0: 7461 7274 275d 2c0d 0a20 2020 2020 2020  tart'],..       
-000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008300: 2065 6e64 3d77 6f72 6473 5b2d 315d 5b27   end=words[-1]['
-00008310: 656e 6427 5d2c 0d0a 2020 2020 2020 2020  end'],..        
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 7465 7874 3d27 272e 6a6f 696e 2877 5b27  text=''.join(w['
-00008340: 776f 7264 275d 2066 6f72 2077 2069 6e20  word'] for w in 
-00008350: 776f 7264 7329 2c0d 0a20 2020 2020 2020  words),..       
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2077 6f72 6473 3d77 6f72 6473 0d0a 2020   words=words..  
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-000083a0: 2020 2020 2020 2020 2066 6f72 2077 6f72           for wor
-000083b0: 6473 2069 6e20 7265 7375 6c74 2069 6620  ds in result if 
-000083c0: 776f 7264 730d 0a20 2020 2020 2020 2020  words..         
-000083d0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-000083e0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
-000083f0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00008400: 6365 2872 6573 756c 745b 305d 2c20 6469  ce(result[0], di
-00008410: 6374 293a 0d0a 2020 2020 2020 2020 2020  ct):..          
-00008420: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00008430: 7365 676d 656e 7473 3d72 6573 756c 7429  segments=result)
-00008440: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00008450: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00008460: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00008470: 6445 7272 6f72 2866 2747 6f74 206c 6973  dError(f'Got lis
-00008480: 7420 6f66 207b 7479 7065 2872 6573 756c  t of {type(resul
-00008490: 745b 305d 297d 2062 7574 2065 7870 6563  t[0])} but expec
-000084a0: 7473 206c 6973 7420 6f66 206c 6973 742f  ts list of list/
-000084b0: 6469 6374 2729 0d0a 2020 2020 2020 2020  dict')..        
-000084c0: 7265 7475 726e 2072 6573 756c 742c 2070  return result, p
-000084d0: 6174 680d 0a0d 0a20 2020 2064 6566 2066  ath....    def f
-000084e0: 6f72 6365 5f6f 7264 6572 2873 656c 6629  orce_order(self)
-000084f0: 3a0d 0a20 2020 2020 2020 2070 7265 765f  :..        prev_
-00008500: 7473 5f65 6e64 203d 2030 0d0a 2020 2020  ts_end = 0..    
-00008510: 2020 2020 7469 6d65 7374 616d 7073 203d      timestamps =
-00008520: 2073 656c 662e 616c 6c5f 776f 7264 735f   self.all_words_
-00008530: 6f72 5f73 6567 6d65 6e74 7328 290d 0a20  or_segments().. 
-00008540: 2020 2020 2020 2066 6f72 2069 2c20 7473         for i, ts
-00008550: 2069 6e20 656e 756d 6572 6174 6528 7469   in enumerate(ti
-00008560: 6d65 7374 616d 7073 2c20 3129 3a0d 0a20  mestamps, 1):.. 
-00008570: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
-00008580: 2e73 7461 7274 203c 2070 7265 765f 7473  .start < prev_ts
-00008590: 5f65 6e64 3a0d 0a20 2020 2020 2020 2020  _end:..         
-000085a0: 2020 2020 2020 2074 732e 7374 6172 7420         ts.start 
-000085b0: 3d20 7072 6576 5f74 735f 656e 640d 0a20  = prev_ts_end.. 
-000085c0: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
-000085d0: 2e73 7461 7274 203e 2074 732e 656e 643a  .start > ts.end:
-000085e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000085f0: 2020 6966 2070 7265 765f 7473 5f65 6e64    if prev_ts_end
-00008600: 203e 2074 732e 656e 643a 0d0a 2020 2020   > ts.end:..    
-00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 7761 726e 696e 6773 2e77 6172 6e28 274d  warnings.warn('M
-00008630: 756c 7469 706c 6520 636f 6e73 6563 7574  ultiple consecut
-00008640: 6976 6520 7469 6d65 7374 616d 7073 2061  ive timestamps a
-00008650: 7265 206f 7574 206f 6620 6f72 6465 722e  re out of order.
-00008660: 2053 6f6d 6520 7061 7274 7320 7769 6c6c   Some parts will
-00008670: 2068 6176 6520 6e6f 2064 7572 6174 696f   have no duratio
-00008680: 6e2e 2729 0d0a 2020 2020 2020 2020 2020  n.')..          
-00008690: 2020 2020 2020 2020 2020 7473 2e73 7461            ts.sta
-000086a0: 7274 203d 2074 732e 656e 640d 0a20 2020  rt = ts.end..   
-000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086c0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-000086d0: 692d 322c 202d 312c 202d 3129 3a0d 0a20  i-2, -1, -1):.. 
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2020 2020 2020 2069 6620 7469 6d65 7374         if timest
-00008700: 616d 7073 5b6a 5d2e 656e 6420 3e20 7473  amps[j].end > ts
-00008710: 2e65 6e64 3a0d 0a20 2020 2020 2020 2020  .end:..         
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2074 696d 6573 7461 6d70 735b 6a5d     timestamps[j]
-00008740: 2e65 6e64 203d 2074 732e 656e 640d 0a20  .end = ts.end.. 
-00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008760: 2020 2020 2020 2069 6620 7469 6d65 7374         if timest
-00008770: 616d 7073 5b6a 5d2e 7374 6172 7420 3e20  amps[j].start > 
-00008780: 7473 2e65 6e64 3a0d 0a20 2020 2020 2020  ts.end:..       
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 2074 696d 6573 7461 6d70 735b       timestamps[
-000087b0: 6a5d 2e73 7461 7274 203d 2074 732e 656e  j].start = ts.en
-000087c0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-000087d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000087e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000087f0: 2074 732e 7374 6172 7420 213d 2070 7265   ts.start != pre
-00008800: 765f 7473 5f65 6e64 3a0d 0a20 2020 2020  v_ts_end:..     
-00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008820: 2020 2074 732e 7374 6172 7420 3d20 7072     ts.start = pr
-00008830: 6576 5f74 735f 656e 640d 0a20 2020 2020  ev_ts_end..     
-00008840: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008850: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00008860: 2020 2020 2020 2020 2020 2020 2020 7473                ts
-00008870: 2e65 6e64 203d 2074 732e 7374 6172 7420  .end = ts.start 
-00008880: 6966 2069 203d 3d20 6c65 6e28 7469 6d65  if i == len(time
-00008890: 7374 616d 7073 2920 656c 7365 2074 696d  stamps) else tim
-000088a0: 6573 7461 6d70 735b 695d 2e73 7461 7274  estamps[i].start
-000088b0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-000088c0: 6576 5f74 735f 656e 6420 3d20 7473 2e65  ev_ts_end = ts.e
-000088d0: 6e64 0d0a 0d0a 2020 2020 6465 6620 7261  nd....    def ra
-000088e0: 6973 655f 666f 725f 756e 736f 7274 6564  ise_for_unsorted
-000088f0: 2873 656c 662c 2063 6865 636b 5f73 6f72  (self, check_sor
-00008900: 7465 643a 2055 6e69 6f6e 5b62 6f6f 6c2c  ted: Union[bool,
-00008910: 2073 7472 5d20 3d20 5472 7565 2c20 7368   str] = True, sh
-00008920: 6f77 5f75 6e73 6f72 7465 643a 2062 6f6f  ow_unsorted: boo
-00008930: 6c20 3d20 5472 7565 293a 0d0a 2020 2020  l = True):..    
-00008940: 2020 2020 6966 2063 6865 636b 5f73 6f72      if check_sor
-00008950: 7465 6420 6973 2046 616c 7365 3a0d 0a20  ted is False:.. 
-00008960: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008970: 6e0d 0a20 2020 2020 2020 2061 6c6c 5f70  n..        all_p
-00008980: 6172 7473 203d 2073 656c 662e 616c 6c5f  arts = self.all_
-00008990: 776f 7264 735f 6f72 5f73 6567 6d65 6e74  words_or_segment
-000089a0: 7328 290d 0a20 2020 2020 2020 2069 6620  s()..        if 
-000089b0: 6e6f 7420 616c 6c5f 7061 7274 733a 0d0a  not all_parts:..
-000089c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000089d0: 726e 0d0a 2020 2020 2020 2020 6973 5f77  rn..        is_w
-000089e0: 6f72 6420 3d20 6973 696e 7374 616e 6365  ord = isinstance
-000089f0: 2861 6c6c 5f70 6172 7473 5b30 5d2c 2057  (all_parts[0], W
-00008a00: 6f72 6454 696d 696e 6729 0d0a 2020 2020  ordTiming)..    
-00008a10: 2020 2020 7469 6d65 7374 616d 7073 203d      timestamps =
-00008a20: 206e 702e 6172 7261 7928 6c69 7374 2863   np.array(list(c
-00008a30: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
-00008a40: 6c65 2828 702e 7374 6172 742c 2070 2e65  le((p.start, p.e
-00008a50: 6e64 2920 666f 7220 7020 696e 2061 6c6c  nd) for p in all
-00008a60: 5f70 6172 7473 2929 290d 0a20 2020 2020  _parts)))..     
-00008a70: 2020 2069 6620 6c65 6e28 7469 6d65 7374     if len(timest
-00008a80: 616d 7073 2920 3e20 3120 616e 6420 2875  amps) > 1 and (u
-00008a90: 6e73 6f72 7465 645f 6d61 736b 203a 3d20  nsorted_mask := 
-00008aa0: 7469 6d65 7374 616d 7073 5b3a 2d31 5d20  timestamps[:-1] 
-00008ab0: 3e20 7469 6d65 7374 616d 7073 5b31 3a5d  > timestamps[1:]
-00008ac0: 292e 616e 7928 293a 0d0a 2020 2020 2020  ).any():..      
-00008ad0: 2020 2020 2020 6966 2073 686f 775f 756e        if show_un
-00008ae0: 736f 7274 6564 3a0d 0a20 2020 2020 2020  sorted:..       
-00008af0: 2020 2020 2020 2020 2064 6566 2067 6574           def get
-00008b00: 5f70 6172 745f 696e 666f 2869 6478 293a  _part_info(idx):
-00008b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008b20: 2020 2020 2020 6375 7272 5f70 6172 7420        curr_part 
-00008b30: 3d20 616c 6c5f 7061 7274 735b 6964 785d  = all_parts[idx]
-00008b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008b50: 2020 2020 2020 7365 675f 6964 203d 2063        seg_id = c
-00008b60: 7572 725f 7061 7274 2e73 6567 6d65 6e74  urr_part.segment
-00008b70: 5f69 6420 6966 2069 735f 776f 7264 2065  _id if is_word e
-00008b80: 6c73 6520 6375 7272 5f70 6172 742e 6964  lse curr_part.id
-00008b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008ba0: 2020 2020 2020 776f 7264 5f69 645f 7374        word_id_st
-00008bb0: 7220 3d20 6627 576f 7264 2049 443a 207b  r = f'Word ID: {
-00008bc0: 6375 7272 5f70 6172 742e 6964 7d5c 6e27  curr_part.id}\n'
-00008bd0: 2069 6620 6973 5f77 6f72 6420 656c 7365   if is_word else
-00008be0: 2027 270d 0a20 2020 2020 2020 2020 2020   ''..           
-00008bf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008c00: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00008c10: 2020 2020 2020 2020 2020 2066 2753 6567             f'Seg
-00008c20: 6d65 6e74 2049 443a 207b 7365 675f 6964  ment ID: {seg_id
-00008c30: 7d5c 6e7b 776f 7264 5f69 645f 7374 727d  }\n{word_id_str}
-00008c40: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00008c50: 2020 2020 2020 2020 2020 2066 2753 7461             f'Sta
-00008c60: 7274 3a20 7b63 7572 725f 7061 7274 2e73  rt: {curr_part.s
-00008c70: 7461 7274 7d5c 6e45 6e64 3a20 7b63 7572  tart}\nEnd: {cur
-00008c80: 725f 7061 7274 2e65 6e64 7d5c 6e27 0d0a  r_part.end}\n'..
-00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ca0: 2020 2020 2020 2020 6627 5465 7874 3a20          f'Text: 
-00008cb0: 227b 6375 7272 5f70 6172 742e 776f 7264  "{curr_part.word
-00008cc0: 2069 6620 6973 5f77 6f72 6420 656c 7365   if is_word else
-00008cd0: 2063 7572 725f 7061 7274 2e74 6578 747d   curr_part.text}
-00008ce0: 2227 0d0a 2020 2020 2020 2020 2020 2020  "'..            
-00008cf0: 2020 2020 2020 2020 292c 2063 7572 725f          ), curr_
-00008d00: 7061 7274 2e73 7461 7274 2c20 6375 7272  part.start, curr
-00008d10: 5f70 6172 742e 656e 640d 0a0d 0a20 2020  _part.end....   
-00008d20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00008d30: 2069 2c20 756e 736f 7274 6564 2069 6e20   i, unsorted in 
-00008d40: 656e 756d 6572 6174 6528 756e 736f 7274  enumerate(unsort
-00008d50: 6564 5f6d 6173 6b2c 2032 293a 0d0a 2020  ed_mask, 2):..  
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 6966 2075 6e73 6f72 7465 643a 0d0a    if unsorted:..
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 2020 2020 776f 7264 5f69 6420          word_id 
-00008da0: 3d20 692f 2f32 2d31 0d0a 2020 2020 2020  = i//2-1..      
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 2020 7061 7274 5f69 6e66 6f2c 2073 7461    part_info, sta
-00008dd0: 7274 2c20 656e 6420 3d20 6765 745f 7061  rt, end = get_pa
-00008de0: 7274 5f69 6e66 6f28 776f 7264 5f69 6429  rt_info(word_id)
-00008df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008e00: 2020 2020 2020 2020 2020 6966 2069 2025            if i %
-00008e10: 2032 203d 3d20 313a 0d0a 2020 2020 2020   2 == 1:..      
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2020 6e65 7874 5f69 6e66 6f2c        next_info,
-00008e40: 206e 6578 745f 7374 6172 742c 205f 203d   next_start, _ =
-00008e50: 2067 6574 5f70 6172 745f 696e 666f 2877   get_part_info(w
-00008e60: 6f72 645f 6964 2b31 290d 0a20 2020 2020  ord_id+1)..     
-00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e80: 2020 2020 2020 2070 6172 745f 696e 666f         part_info
-00008e90: 202b 3d20 6627 5c6e 436f 6e66 6c69 6374   += f'\nConflict
-00008ea0: 3a20 656e 6420 287b 656e 647d 2920 3e20  : end ({end}) > 
-00008eb0: 6e65 7874 2073 7461 7274 2028 7b6e 6578  next start ({nex
-00008ec0: 745f 7374 6172 747d 295c 6e7b 6e65 7874  t_start})\n{next
-00008ed0: 5f69 6e66 6f7d 270d 0a20 2020 2020 2020  _info}'..       
-00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ef0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 2020 7061 7274 5f69 6e66 6f20 2b3d      part_info +=
-00008f20: 2066 275c 6e43 6f6e 666c 6963 743a 2073   f'\nConflict: s
-00008f30: 7461 7274 2028 7b73 7461 7274 7d29 203e  tart ({start}) >
-00008f40: 2065 6e64 2028 7b65 6e64 7d29 270d 0a20   end ({end})'.. 
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f60: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
-00008f70: 745f 696e 666f 2c20 656e 643d 275c 6e5c  t_info, end='\n\
-00008f80: 6e27 290d 0a0d 0a20 2020 2020 2020 2020  n')....         
-00008f90: 2020 2064 6174 6120 3d20 7365 6c66 2e74     data = self.t
-00008fa0: 6f5f 6469 6374 2829 0d0a 2020 2020 2020  o_dict()..      
-00008fb0: 2020 2020 2020 6966 2063 6865 636b 5f73        if check_s
-00008fc0: 6f72 7465 6420 6973 2054 7275 653a 0d0a  orted is True:..
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 7261 6973 6520 556e 736f 7274 6564 4578  raise UnsortedEx
-00008ff0: 6365 7074 696f 6e28 6461 7461 3d64 6174  ception(data=dat
-00009000: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
-00009010: 7761 726e 696e 6773 2e77 6172 6e28 2754  warnings.warn('T
-00009020: 696d 6573 7461 6d70 7320 6172 6520 6e6f  imestamps are no
-00009030: 7420 696e 2061 7363 656e 6469 6e67 206f  t in ascending o
-00009040: 7264 6572 2e20 270d 0a20 2020 2020 2020  rder. '..       
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 2027 4966 2064 6174 6120 6973 2070     'If data is p
-00009070: 726f 6475 6365 6420 6279 2053 7461 626c  roduced by Stabl
-00009080: 652d 7473 2c20 706c 6561 7365 2073 7562  e-ts, please sub
-00009090: 6d69 7420 616e 2069 7373 7565 2077 6974  mit an issue wit
-000090a0: 6820 7468 6520 7361 7665 6420 6461 7461  h the saved data
-000090b0: 2e27 290d 0a20 2020 2020 2020 2020 2020  .')..           
-000090c0: 2073 6176 655f 6173 5f6a 736f 6e28 6461   save_as_json(da
-000090d0: 7461 2c20 6368 6563 6b5f 736f 7274 6564  ta, check_sorted
-000090e0: 290d 0a0d 0a20 2020 2064 6566 2075 7064  )....    def upd
-000090f0: 6174 655f 616c 6c5f 7365 6773 5f77 6974  ate_all_segs_wit
-00009100: 685f 776f 7264 7328 7365 6c66 293a 0d0a  h_words(self):..
-00009110: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00009120: 2e77 6172 6e28 2741 7474 7269 6275 7465  .warn('Attribute
-00009130: 7320 7468 6174 2072 6571 7569 7265 6420  s that required 
-00009140: 7570 6461 7469 6e67 2061 7265 206e 6f77  updating are now
-00009150: 2070 726f 7065 7274 6965 7320 6261 7365   properties base
-00009160: 6420 6f6e 2074 6865 2060 6077 6f72 6473  d on the ``words
-00009170: 6060 2065 7863 6570 7420 666f 7220 6060  `` except for ``
-00009180: 6964 6060 2e20 270d 0a20 2020 2020 2020  id``. '..       
-00009190: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000091a0: 6060 7570 6461 7465 5f61 6c6c 5f73 6567  ``update_all_seg
-000091b0: 735f 7769 7468 5f77 6f72 6473 2829 6060  s_with_words()``
-000091c0: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
-000091d0: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
-000091e0: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
-000091f0: 7369 6f6e 732e 2027 0d0a 2020 2020 2020  sions. '..      
+000010e0: 7029 0d0a 0d0a 2020 2020 6465 6620 746f  p)....    def to
+000010f0: 5f64 6973 706c 6179 5f73 7472 2873 656c  _display_str(sel
+00001100: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00001110: 7572 6e20 6622 5b7b 666f 726d 6174 5f74  urn f"[{format_t
+00001120: 696d 6573 7461 6d70 2873 656c 662e 7374  imestamp(self.st
+00001130: 6172 7429 7d5d 202d 3e20 5b7b 666f 726d  art)}] -> [{form
+00001140: 6174 5f74 696d 6573 7461 6d70 2873 656c  at_timestamp(sel
+00001150: 662e 656e 6429 7d5d 205c 227b 7365 6c66  f.end)}] \"{self
+00001160: 2e77 6f72 647d 5c22 220d 0a0d 0a20 2020  .word}\""....   
+00001170: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00001180: 6465 6620 7374 6172 7428 7365 6c66 293a  def start(self):
+00001190: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000011a0: 2073 656c 662e 5f73 7461 7274 0d0a 0d0a   self._start....
+000011b0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000011c0: 2020 2064 6566 2065 6e64 2873 656c 6629     def end(self)
+000011d0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000011e0: 6e20 7365 6c66 2e5f 656e 640d 0a0d 0a20  n self._end.... 
+000011f0: 2020 2040 7374 6172 742e 7365 7474 6572     @start.setter
+00001200: 0d0a 2020 2020 6465 6620 7374 6172 7428  ..    def start(
+00001210: 7365 6c66 2c20 7661 6c29 3a0d 0a20 2020  self, val):..   
+00001220: 2020 2020 2073 656c 662e 5f73 7461 7274       self._start
+00001230: 203d 2073 656c 662e 726f 756e 6428 7661   = self.round(va
+00001240: 6c29 0d0a 0d0a 2020 2020 4065 6e64 2e73  l)....    @end.s
+00001250: 6574 7465 720d 0a20 2020 2064 6566 2065  etter..    def e
+00001260: 6e64 2873 656c 662c 2076 616c 293a 0d0a  nd(self, val):..
+00001270: 2020 2020 2020 2020 7365 6c66 2e5f 656e          self._en
+00001280: 6420 3d20 7365 6c66 2e72 6f75 6e64 2876  d = self.round(v
+00001290: 616c 290d 0a0d 0a20 2020 2040 7072 6f70  al)....    @prop
+000012a0: 6572 7479 0d0a 2020 2020 6465 6620 7365  erty..    def se
+000012b0: 676d 656e 745f 6964 2873 656c 6629 3a0d  gment_id(self):.
+000012c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000012d0: 4e6f 6e65 2069 6620 7365 6c66 2e73 6567  None if self.seg
+000012e0: 6d65 6e74 2069 7320 4e6f 6e65 2065 6c73  ment is None els
+000012f0: 6520 7365 6c66 2e73 6567 6d65 6e74 2e69  e self.segment.i
+00001300: 640d 0a0d 0a20 2020 2040 7072 6f70 6572  d....    @proper
+00001310: 7479 0d0a 2020 2020 6465 6620 6475 7261  ty..    def dura
+00001320: 7469 6f6e 2873 656c 6629 3a0d 0a20 2020  tion(self):..   
+00001330: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00001340: 2e72 6f75 6e64 2873 656c 662e 656e 6420  .round(self.end 
+00001350: 2d20 7365 6c66 2e73 7461 7274 290d 0a0d  - self.start)...
+00001360: 0a20 2020 2064 6566 2072 6f75 6e64 5f61  .    def round_a
+00001370: 6c6c 5f74 696d 6573 7461 6d70 7328 7365  ll_timestamps(se
+00001380: 6c66 293a 0d0a 2020 2020 2020 2020 7761  lf):..        wa
+00001390: 726e 696e 6773 2e77 6172 6e28 2760 602e  rnings.warn('``.
+000013a0: 726f 756e 645f 616c 6c5f 7469 6d65 7374  round_all_timest
+000013b0: 616d 7073 2829 6060 2069 7320 6465 7072  amps()`` is depr
+000013c0: 6563 6174 6564 2061 6e64 2077 696c 6c20  ecated and will 
+000013d0: 6265 2072 656d 6f76 6564 2069 6e20 6675  be removed in fu
+000013e0: 7475 7265 2076 6572 7369 6f6e 732e 2027  ture versions. '
+000013f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001400: 2020 2020 2020 2020 2755 7365 2060 602e          'Use ``.
+00001410: 726f 756e 645f 7473 3d54 7275 6560 6020  round_ts=True`` 
+00001420: 746f 2072 6f75 6e64 2074 696d 6573 7461  to round timesta
+00001430: 6d70 7320 6279 2064 6566 6175 6c74 2069  mps by default i
+00001440: 6e73 7465 6164 2e27 2c0d 0a20 2020 2020  nstead.',..     
+00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001460: 2073 7461 636b 6c65 7665 6c3d 3229 0d0a   stacklevel=2)..
+00001470: 2020 2020 2020 2020 7365 6c66 2e72 6f75          self.rou
+00001480: 6e64 5f74 7320 3d20 5472 7565 0d0a 0d0a  nd_ts = True....
+00001490: 2020 2020 6465 6620 6f66 6673 6574 5f74      def offset_t
+000014a0: 696d 6528 7365 6c66 2c20 6f66 6673 6574  ime(self, offset
+000014b0: 5f73 6563 6f6e 6473 3a20 666c 6f61 7429  _seconds: float)
+000014c0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+000014d0: 7374 6172 7420 3d20 7365 6c66 2e73 7461  start = self.sta
+000014e0: 7274 202b 206f 6666 7365 745f 7365 636f  rt + offset_seco
+000014f0: 6e64 730d 0a20 2020 2020 2020 2073 656c  nds..        sel
+00001500: 662e 656e 6420 3d20 7365 6c66 2e65 6e64  f.end = self.end
+00001510: 202b 206f 6666 7365 745f 7365 636f 6e64   + offset_second
+00001520: 730d 0a0d 0a20 2020 2064 6566 2074 6f5f  s....    def to_
+00001530: 6469 6374 2873 656c 6629 3a0d 0a20 2020  dict(self):..   
+00001540: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
+00001550: 280d 0a20 2020 2020 2020 2020 2020 2077  (..            w
+00001560: 6f72 643d 7365 6c66 2e77 6f72 642c 0d0a  ord=self.word,..
+00001570: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00001580: 743d 7365 6c66 2e73 7461 7274 2c0d 0a20  t=self.start,.. 
+00001590: 2020 2020 2020 2020 2020 2065 6e64 3d73             end=s
+000015a0: 656c 662e 656e 642c 0d0a 2020 2020 2020  elf.end,..      
+000015b0: 2020 2020 2020 7072 6f62 6162 696c 6974        probabilit
+000015c0: 793d 7365 6c66 2e70 726f 6261 6269 6c69  y=self.probabili
+000015d0: 7479 2c0d 0a20 2020 2020 2020 2020 2020  ty,..           
+000015e0: 2074 6f6b 656e 733d 4e6f 6e65 2069 6620   tokens=None if 
+000015f0: 7365 6c66 2e74 6f6b 656e 7320 6973 204e  self.tokens is N
+00001600: 6f6e 6520 656c 7365 2073 656c 662e 746f  one else self.to
+00001610: 6b65 6e73 2e63 6f70 7928 290d 0a20 2020  kens.copy()..   
+00001620: 2020 2020 2029 0d0a 0d0a 2020 2020 6465       )....    de
+00001630: 6620 6c6f 636b 5f6c 6566 7428 7365 6c66  f lock_left(self
+00001640: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00001650: 2e6c 6566 745f 6c6f 636b 6564 203d 2054  .left_locked = T
+00001660: 7275 650d 0a0d 0a20 2020 2064 6566 206c  rue....    def l
+00001670: 6f63 6b5f 7269 6768 7428 7365 6c66 293a  ock_right(self):
+00001680: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+00001690: 6967 6874 5f6c 6f63 6b65 6420 3d20 5472  ight_locked = Tr
+000016a0: 7565 0d0a 0d0a 2020 2020 6465 6620 6c6f  ue....    def lo
+000016b0: 636b 5f62 6f74 6828 7365 6c66 293a 0d0a  ck_both(self):..
+000016c0: 2020 2020 2020 2020 7365 6c66 2e6c 6f63          self.loc
+000016d0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
+000016e0: 2020 7365 6c66 2e6c 6f63 6b5f 7269 6768    self.lock_righ
+000016f0: 7428 290d 0a0d 0a20 2020 2064 6566 2075  t()....    def u
+00001700: 6e6c 6f63 6b5f 626f 7468 2873 656c 6629  nlock_both(self)
+00001710: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+00001720: 6c65 6674 5f6c 6f63 6b65 6420 3d20 4661  left_locked = Fa
+00001730: 6c73 650d 0a20 2020 2020 2020 2073 656c  lse..        sel
+00001740: 662e 7269 6768 745f 6c6f 636b 6564 203d  f.right_locked =
+00001750: 2046 616c 7365 0d0a 0d0a 2020 2020 6465   False....    de
+00001760: 6620 7375 7070 7265 7373 5f73 696c 656e  f suppress_silen
+00001770: 6365 2873 656c 662c 0d0a 2020 2020 2020  ce(self,..      
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 2020 2073 696c 656e 745f 7374 6172 7473     silent_starts
+000017a0: 3a20 6e70 2e6e 6461 7272 6179 2c0d 0a20  : np.ndarray,.. 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 2020 2020 7369 6c65 6e74 5f65          silent_e
+000017d0: 6e64 733a 206e 702e 6e64 6172 7261 792c  nds: np.ndarray,
+000017e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017f0: 2020 2020 2020 2020 2020 206d 696e 5f77             min_w
+00001800: 6f72 645f 6475 723a 204f 7074 696f 6e61  ord_dur: Optiona
+00001810: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
+00001820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001830: 2020 2020 2020 2020 2020 206e 6f6e 7370             nonsp
+00001840: 6565 6368 5f65 7272 6f72 3a20 666c 6f61  eech_error: floa
+00001850: 7420 3d20 302e 332c 0d0a 2020 2020 2020  t = 0.3,..      
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 206b 6565 705f 656e 643a 204f 7074     keep_end: Opt
+00001880: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
+00001890: 7565 293a 0d0a 2020 2020 2020 2020 7375  ue):..        su
+000018a0: 7070 7265 7373 5f73 696c 656e 6365 2873  ppress_silence(s
+000018b0: 656c 662c 2073 696c 656e 745f 7374 6172  elf, silent_star
+000018c0: 7473 2c20 7369 6c65 6e74 5f65 6e64 732c  ts, silent_ends,
+000018d0: 206d 696e 5f77 6f72 645f 6475 722c 206e   min_word_dur, n
+000018e0: 6f6e 7370 6565 6368 5f65 7272 6f72 2c20  onspeech_error, 
+000018f0: 6b65 6570 5f65 6e64 290d 0a20 2020 2020  keep_end)..     
+00001900: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
+00001910: 0d0a 2020 2020 6465 6620 7265 7363 616c  ..    def rescal
+00001920: 655f 7469 6d65 2873 656c 662c 2073 6361  e_time(self, sca
+00001930: 6c65 5f66 6163 746f 723a 2066 6c6f 6174  le_factor: float
+00001940: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00001950: 2e73 7461 7274 203d 2073 656c 662e 7374  .start = self.st
+00001960: 6172 7420 2a20 7363 616c 655f 6661 6374  art * scale_fact
+00001970: 6f72 0d0a 2020 2020 2020 2020 7365 6c66  or..        self
+00001980: 2e65 6e64 203d 2073 656c 662e 656e 6420  .end = self.end 
+00001990: 2a20 7363 616c 655f 6661 6374 6f72 0d0a  * scale_factor..
+000019a0: 0d0a 2020 2020 6465 6620 636c 616d 705f  ..    def clamp_
+000019b0: 6d61 7828 7365 6c66 2c20 6d61 785f 6475  max(self, max_du
+000019c0: 723a 2066 6c6f 6174 2c20 636c 6970 5f73  r: float, clip_s
+000019d0: 7461 7274 3a20 626f 6f6c 203d 2046 616c  tart: bool = Fal
+000019e0: 7365 2c20 7665 7262 6f73 653a 2062 6f6f  se, verbose: boo
+000019f0: 6c20 3d20 4661 6c73 6529 3a0d 0a20 2020  l = False):..   
+00001a00: 2020 2020 2069 6620 7365 6c66 2e64 7572       if self.dur
+00001a10: 6174 696f 6e20 3e20 6d61 785f 6475 723a  ation > max_dur:
+00001a20: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001a30: 2063 6c69 705f 7374 6172 743a 0d0a 2020   clip_start:..  
+00001a40: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00001a50: 775f 7374 6172 7420 3d20 726f 756e 6428  w_start = round(
+00001a60: 7365 6c66 2e65 6e64 202d 206d 6178 5f64  self.end - max_d
+00001a70: 7572 2c20 3329 0d0a 2020 2020 2020 2020  ur, 3)..        
+00001a80: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00001a90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001aa0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00001ab0: 2753 7461 7274 3a20 7b73 656c 662e 7374  'Start: {self.st
+00001ac0: 6172 747d 202d 3e20 7b6e 6577 5f73 7461  art} -> {new_sta
+00001ad0: 7274 7d5c 6e45 6e64 3a20 7b73 656c 662e  rt}\nEnd: {self.
+00001ae0: 656e 647d 5c6e 5465 7874 3a22 7b73 656c  end}\nText:"{sel
+00001af0: 662e 776f 7264 7d22 5c6e 2729 0d0a 2020  f.word}"\n')..  
+00001b00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001b10: 6c66 2e73 7461 7274 203d 206e 6577 5f73  lf.start = new_s
+00001b20: 7461 7274 0d0a 0d0a 2020 2020 2020 2020  tart....        
+00001b30: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001b40: 2020 2020 2020 2020 2020 206e 6577 5f65             new_e
+00001b50: 6e64 203d 2072 6f75 6e64 2873 656c 662e  nd = round(self.
+00001b60: 7374 6172 7420 2b20 6d61 785f 6475 722c  start + max_dur,
+00001b70: 2033 290d 0a20 2020 2020 2020 2020 2020   3)..           
+00001b80: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+00001b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ba0: 2020 2020 2020 7072 696e 7428 6627 5374        print(f'St
+00001bb0: 6172 743a 207b 7365 6c66 2e73 7461 7274  art: {self.start
+00001bc0: 7d5c 6e45 6e64 3a20 7b73 656c 662e 656e  }\nEnd: {self.en
+00001bd0: 647d 202d 3e20 7b6e 6577 5f65 6e64 7d5c  d} -> {new_end}\
+00001be0: 6e54 6578 743a 227b 7365 6c66 2e77 6f72  nText:"{self.wor
+00001bf0: 647d 225c 6e27 290d 0a20 2020 2020 2020  d}"\n')..       
+00001c00: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
+00001c10: 6420 3d20 6e65 775f 656e 640d 0a0d 0a20  d = new_end.... 
+00001c20: 2020 2064 6566 2073 6574 5f73 6567 6d65     def set_segme
+00001c30: 6e74 2873 656c 662c 2073 6567 6d65 6e74  nt(self, segment
+00001c40: 3a20 2753 6567 6d65 6e74 2729 3a0d 0a20  : 'Segment'):.. 
+00001c50: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00001c60: 7761 726e 2827 6060 2e73 6574 5f73 6567  warn('``.set_seg
+00001c70: 6d65 6e74 2863 7572 7265 6e74 5f73 6567  ment(current_seg
+00001c80: 6d65 6e74 5f69 6e73 7461 6e63 6529 6060  ment_instance)``
+00001c90: 2069 7320 6465 7072 6563 6174 6564 2061   is deprecated a
+00001ca0: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
+00001cb0: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
+00001cc0: 7369 6f6e 732e 270d 0a20 2020 2020 2020  sions.'..       
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001ce0: 2055 7365 2060 602e 7365 676d 656e 7420   Use ``.segment 
+00001cf0: 3d20 6375 7272 656e 745f 7365 676d 656e  = current_segmen
+00001d00: 7460 6020 696e 7374 6561 642e 272c 0d0a  t`` instead.',..
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 7374 6163 6b6c 6576 656c        stacklevel
+00001d30: 3d32 290d 0a20 2020 2020 2020 2073 656c  =2)..        sel
+00001d40: 662e 7365 676d 656e 7420 3d20 7365 676d  f.segment = segm
+00001d50: 656e 740d 0a0d 0a20 2020 2064 6566 2067  ent....    def g
+00001d60: 6574 5f73 6567 6d65 6e74 2873 656c 6629  et_segment(self)
+00001d70: 202d 3e20 556e 696f 6e5b 2753 6567 6d65   -> Union['Segme
+00001d80: 6e74 272c 204e 6f6e 655d 3a0d 0a20 2020  nt', None]:..   
+00001d90: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00001da0: 2020 5265 7475 726e 2069 6e73 7461 6e63    Return instanc
+00001db0: 6520 6f66 203a 636c 6173 733a 6073 7461  e of :class:`sta
+00001dc0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+00001dd0: 6c74 2e53 6567 6d65 6e74 6020 7468 6174  lt.Segment` that
+00001de0: 2074 6869 7320 696e 7374 616e 6365 2069   this instance i
+00001df0: 7320 6120 7061 7274 206f 662e 0d0a 2020  s a part of...  
+00001e00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001e10: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+00001e20: 2827 6060 2e67 6574 5f73 6567 6d65 6e74  ('``.get_segment
+00001e30: 2829 6060 2077 696c 6c20 6265 2072 656d  ()`` will be rem
+00001e40: 6f76 6564 2069 6e20 6675 7475 7265 2076  oved in future v
+00001e50: 6572 7369 6f6e 732e 2055 7365 2060 602e  ersions. Use ``.
+00001e60: 7365 676d 656e 7460 6020 696e 7374 6561  segment`` instea
+00001e70: 642e 272c 0d0a 2020 2020 2020 2020 2020  d.',..          
+00001e80: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+00001e90: 6b6c 6576 656c 3d32 290d 0a20 2020 2020  klevel=2)..     
+00001ea0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+00001eb0: 6567 6d65 6e74 0d0a 0d0a 0d0a 6465 6620  egment......def 
+00001ec0: 5f77 6f72 6473 5f62 795f 6c6f 636b 2877  _words_by_lock(w
+00001ed0: 6f72 6473 3a20 4c69 7374 5b57 6f72 6454  ords: List[WordT
+00001ee0: 696d 696e 675d 2c20 6f6e 6c79 5f74 6578  iming], only_tex
+00001ef0: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
+00001f00: 2069 6e63 6c75 6465 5f73 696e 676c 653a   include_single:
+00001f10: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00001f20: 0a20 2020 2022 2222 0d0a 2020 2020 5265  .    """..    Re
+00001f30: 7475 726e 2061 206e 6573 7465 6420 6c69  turn a nested li
+00001f40: 7374 206f 6620 776f 7264 7320 7375 6368  st of words such
+00001f50: 2074 6861 7420 6561 6368 2073 7562 6c69   that each subli
+00001f60: 7374 2063 6f6e 7461 696e 7320 776f 7264  st contains word
+00001f70: 7320 7468 6174 2061 7265 206c 6f63 6b65  s that are locke
+00001f80: 6420 746f 6765 7468 6572 2e0d 0a20 2020  d together...   
+00001f90: 2022 2222 0d0a 2020 2020 616c 6c5f 776f   """..    all_wo
+00001fa0: 7264 7320 3d20 5b5d 0d0a 2020 2020 666f  rds = []..    fo
+00001fb0: 7220 776f 7264 2069 6e20 776f 7264 733a  r word in words:
+00001fc0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00001fd0: 2861 6c6c 5f77 6f72 6473 2920 3d3d 2030  (all_words) == 0
+00001fe0: 206f 7220 6e6f 7420 2861 6c6c 5f77 6f72   or not (all_wor
+00001ff0: 6473 5b2d 315d 5b2d 315d 2e72 6967 6874  ds[-1][-1].right
+00002000: 5f6c 6f63 6b65 6420 6f72 2077 6f72 642e  _locked or word.
+00002010: 6c65 6674 5f6c 6f63 6b65 6429 3a0d 0a20  left_locked):.. 
+00002020: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
+00002030: 6f72 6473 2e61 7070 656e 6428 5b77 6f72  ords.append([wor
+00002040: 645d 290d 0a20 2020 2020 2020 2065 6c73  d])..        els
+00002050: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002060: 616c 6c5f 776f 7264 735b 2d31 5d2e 6170  all_words[-1].ap
+00002070: 7065 6e64 2877 6f72 6429 0d0a 2020 2020  pend(word)..    
+00002080: 6966 206f 6e6c 795f 7465 7874 3a0d 0a20  if only_text:.. 
+00002090: 2020 2020 2020 2061 6c6c 5f77 6f72 6473         all_words
+000020a0: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
+000020b0: 6461 2077 733a 206c 6973 7428 6d61 7028  da ws: list(map(
+000020c0: 6c61 6d62 6461 2077 3a20 772e 776f 7264  lambda w: w.word
+000020d0: 2c20 7773 2929 2c20 616c 6c5f 776f 7264  , ws)), all_word
+000020e0: 7329 290d 0a20 2020 2069 6620 6e6f 7420  s))..    if not 
+000020f0: 696e 636c 7564 655f 7369 6e67 6c65 3a0d  include_single:.
+00002100: 0a20 2020 2020 2020 2061 6c6c 5f77 6f72  .        all_wor
+00002110: 6473 203d 205b 7773 2066 6f72 2077 7320  ds = [ws for ws 
+00002120: 696e 2061 6c6c 5f77 6f72 6473 2069 6620  in all_words if 
+00002130: 6c65 6e28 7773 2920 3e20 315d 0d0a 2020  len(ws) > 1]..  
+00002140: 2020 7265 7475 726e 2061 6c6c 5f77 6f72    return all_wor
+00002150: 6473 0d0a 0d0a 0d0a 636c 6173 7320 5365  ds......class Se
+00002160: 676d 656e 743a 0d0a 0d0a 2020 2020 6465  gment:....    de
+00002170: 6620 5f5f 696e 6974 5f5f 280d 0a20 2020  f __init__(..   
+00002180: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+00002190: 2020 2020 2020 2020 2020 2020 7374 6172              star
+000021a0: 743a 204f 7074 696f 6e61 6c5b 666c 6f61  t: Optional[floa
+000021b0: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
+000021c0: 2020 2020 2020 2020 656e 643a 204f 7074          end: Opt
+000021d0: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+000021e0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+000021f0: 2020 7465 7874 3a20 4f70 7469 6f6e 616c    text: Optional
+00002200: 5b73 7472 5d20 3d20 4e6f 6e65 2c0d 0a20  [str] = None,.. 
+00002210: 2020 2020 2020 2020 2020 2073 6565 6b3a             seek:
+00002220: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00002230: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00002240: 2020 2020 2020 746f 6b65 6e73 3a20 4c69        tokens: Li
+00002250: 7374 5b69 6e74 5d20 3d20 4e6f 6e65 2c0d  st[int] = None,.
+00002260: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00002270: 7065 7261 7475 7265 3a20 4f70 7469 6f6e  perature: Option
+00002280: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
+00002290: 2c0d 0a20 2020 2020 2020 2020 2020 2061  ,..            a
+000022a0: 7667 5f6c 6f67 7072 6f62 3a20 4f70 7469  vg_logprob: Opti
+000022b0: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+000022c0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+000022d0: 2063 6f6d 7072 6573 7369 6f6e 5f72 6174   compression_rat
+000022e0: 696f 3a20 4f70 7469 6f6e 616c 5b66 6c6f  io: Optional[flo
+000022f0: 6174 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  at] = None,..   
+00002300: 2020 2020 2020 2020 206e 6f5f 7370 6565           no_spee
+00002310: 6368 5f70 726f 623a 204f 7074 696f 6e61  ch_prob: Optiona
+00002320: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
+00002330: 0d0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+00002340: 7264 733a 204f 7074 696f 6e61 6c5b 556e  rds: Optional[Un
+00002350: 696f 6e5b 4c69 7374 5b57 6f72 6454 696d  ion[List[WordTim
+00002360: 696e 675d 2c20 4c69 7374 5b64 6963 745d  ing], List[dict]
+00002370: 5d5d 203d 204e 6f6e 652c 0d0a 2020 2020  ]] = None,..    
+00002380: 2020 2020 2020 2020 6964 3a20 4f70 7469          id: Opti
+00002390: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000023a0: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+000023b0: 6573 756c 743a 204f 7074 696f 6e61 6c5b  esult: Optional[
+000023c0: 2257 6869 7370 6572 5265 7375 6c74 225d  "WhisperResult"]
+000023d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+000023e0: 2020 2020 2020 726f 756e 645f 7473 3a20        round_ts: 
+000023f0: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
+00002400: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+00002410: 5f75 6e75 7365 645f 6172 6773 3a20 626f  _unused_args: bo
+00002420: 6f6c 203d 2046 616c 7365 0d0a 2020 2020  ol = False..    
+00002430: 293a 0d0a 2020 2020 2020 2020 6966 2077  ):..        if w
+00002440: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+00002450: 2020 2069 6620 6967 6e6f 7265 5f75 6e75     if ignore_unu
+00002460: 7365 645f 6172 6773 3a0d 0a20 2020 2020  sed_args:..     
+00002470: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00002480: 203d 2065 6e64 203d 2074 6578 7420 3d20   = end = text = 
+00002490: 746f 6b65 6e73 203d 204e 6f6e 650d 0a20  tokens = None.. 
+000024a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000024b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000024c0: 2020 6966 2028 7374 6172 7420 6f72 2065    if (start or e
+000024d0: 6e64 2920 6973 206e 6f74 204e 6f6e 653a  nd) is not None:
+000024e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000024f0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00002500: 6172 6e28 2741 7267 756d 656e 7473 2066  arn('Arguments f
+00002510: 6f72 2060 6073 7461 7274 6060 2061 6e64  or ``start`` and
+00002520: 2060 6065 6e64 6060 2077 696c 6c20 6265   ``end`` will be
+00002530: 2069 676e 6f72 6564 2027 0d0a 2020 2020   ignored '..    
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+00002560: 6e64 2074 6865 2060 6073 7461 7274 6060  nd the ``start``
+00002570: 2061 6e64 2060 6065 6e64 6060 2077 696c   and ``end`` wil
+00002580: 6c20 7461 6b65 6e20 6672 6f6d 2074 6865  l taken from the
+00002590: 2066 6972 7374 2061 6e64 206c 6173 7420   first and last 
+000025a0: 6060 776f 7264 7360 602e 272c 0d0a 2020  ``words``.',..  
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 7374 6163 6b6c 6576 656c 3d32 290d 0a20  stacklevel=2).. 
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000025f0: 6620 7465 7874 2069 7320 6e6f 7420 4e6f  f text is not No
+00002600: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002610: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00002620: 732e 7761 726e 2827 5468 6520 6172 6775  s.warn('The argu
+00002630: 6d65 6e74 2066 6f72 2060 6074 6578 7460  ment for ``text`
+00002640: 6020 7769 6c6c 2062 6520 6967 6e6f 7265  ` will be ignore
+00002650: 6420 270d 0a20 2020 2020 2020 2020 2020  d '..           
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 2027 616e 6420 6974 2077         'and it w
+00002680: 696c 6c20 616c 7761 7973 2062 6520 7468  ill always be th
+00002690: 6520 636f 6e63 6174 656e 6174 696f 6e20  e concatenation 
+000026a0: 6f66 2074 6578 7420 696e 2060 6077 6f72  of text in ``wor
+000026b0: 6473 6060 272c 0d0a 2020 2020 2020 2020  ds``',..        
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
+000026e0: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
+000026f0: 2020 2020 2020 2020 2069 6620 746f 6b65           if toke
+00002700: 6e73 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ns is not None:.
+00002710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002720: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00002730: 726e 2827 5468 6520 6172 6775 6d65 6e74  rn('The argument
+00002740: 2066 6f72 2060 6074 6f6b 656e 7360 6020   for ``tokens`` 
+00002750: 7769 6c6c 2062 6520 6967 6e6f 7265 6420  will be ignored 
+00002760: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 2020 2020 2027 616e 6420 6974 2077 696c       'and it wil
+00002790: 6c20 616c 7761 7973 2062 6520 7468 6520  l always be the 
+000027a0: 636f 6e63 6174 656e 6174 696f 6e20 6f66  concatenation of
+000027b0: 2074 6f6b 656e 7320 696e 2060 6077 6f72   tokens in ``wor
+000027c0: 6473 6060 272c 0d0a 2020 2020 2020 2020  ds``',..        
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
+000027f0: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
+00002800: 2073 656c 662e 726f 756e 645f 7473 203d   self.round_ts =
+00002810: 2072 6f75 6e64 5f74 730d 0a20 2020 2020   round_ts..     
+00002820: 2020 2073 656c 662e 5f64 6566 6175 6c74     self._default
+00002830: 5f73 7461 7274 203d 2073 656c 662e 726f  _start = self.ro
+00002840: 756e 6428 7374 6172 7429 2069 6620 7374  und(start) if st
+00002850: 6172 7420 656c 7365 2030 2e30 0d0a 2020  art else 0.0..  
+00002860: 2020 2020 2020 7365 6c66 2e5f 6465 6661        self._defa
+00002870: 756c 745f 656e 6420 3d20 7365 6c66 2e72  ult_end = self.r
+00002880: 6f75 6e64 2865 6e64 2920 6966 2065 6e64  ound(end) if end
+00002890: 2065 6c73 6520 302e 300d 0a20 2020 2020   else 0.0..     
+000028a0: 2020 2073 656c 662e 5f64 6566 6175 6c74     self._default
+000028b0: 5f74 6578 7420 3d20 7465 7874 206f 7220  _text = text or 
+000028c0: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
+000028d0: 2e5f 6465 6661 756c 745f 746f 6b65 6e73  ._default_tokens
+000028e0: 203d 2074 6f6b 656e 7320 6f72 205b 5d0d   = tokens or [].
+000028f0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00002900: 656b 203d 2073 6565 6b0d 0a20 2020 2020  ek = seek..     
+00002910: 2020 2073 656c 662e 7465 6d70 6572 6174     self.temperat
+00002920: 7572 6520 3d20 7465 6d70 6572 6174 7572  ure = temperatur
+00002930: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00002940: 6176 675f 6c6f 6770 726f 6220 3d20 6176  avg_logprob = av
+00002950: 675f 6c6f 6770 726f 620d 0a20 2020 2020  g_logprob..     
+00002960: 2020 2073 656c 662e 636f 6d70 7265 7373     self.compress
+00002970: 696f 6e5f 7261 7469 6f20 3d20 636f 6d70  ion_ratio = comp
+00002980: 7265 7373 696f 6e5f 7261 7469 6f0d 0a20  ression_ratio.. 
+00002990: 2020 2020 2020 2073 656c 662e 6e6f 5f73         self.no_s
+000029a0: 7065 6563 685f 7072 6f62 203d 206e 6f5f  peech_prob = no_
+000029b0: 7370 6565 6368 5f70 726f 620d 0a20 2020  speech_prob..   
+000029c0: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
+000029d0: 3d20 776f 7264 730d 0a20 2020 2020 2020  = words..       
+000029e0: 2069 6620 7365 6c66 2e77 6f72 6473 2061   if self.words a
+000029f0: 6e64 2069 7369 6e73 7461 6e63 6528 776f  nd isinstance(wo
+00002a00: 7264 735b 305d 2c20 6469 6374 293a 0d0a  rds[0], dict):..
+00002a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002a20: 2e77 6f72 6473 203d 205b 0d0a 2020 2020  .words = [..    
+00002a30: 2020 2020 2020 2020 2020 2020 576f 7264              Word
+00002a40: 5469 6d69 6e67 280d 0a20 2020 2020 2020  Timing(..       
+00002a50: 2020 2020 2020 2020 2020 2020 202a 2a77               **w
+00002a60: 6f72 642c 0d0a 2020 2020 2020 2020 2020  ord,..          
+00002a70: 2020 2020 2020 2020 2020 7365 676d 656e            segmen
+00002a80: 743d 7365 6c66 2c0d 0a20 2020 2020 2020  t=self,..       
+00002a90: 2020 2020 2020 2020 2020 2020 2072 6f75               rou
+00002aa0: 6e64 5f74 733d 7365 6c66 2e72 6f75 6e64  nd_ts=self.round
+00002ab0: 5f74 732c 0d0a 2020 2020 2020 2020 2020  _ts,..          
+00002ac0: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+00002ad0: 5f75 6e75 7365 645f 6172 6773 3d54 7275  _unused_args=Tru
+00002ae0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00002af0: 2020 2029 2066 6f72 2077 6f72 6420 696e     ) for word in
+00002b00: 2073 656c 662e 776f 7264 730d 0a20 2020   self.words..   
+00002b10: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00002b20: 2020 2020 7365 6c66 2e69 6420 3d20 6964      self.id = id
+00002b30: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00002b40: 7265 7665 7273 6564 5f74 6578 7420 3d20  reversed_text = 
+00002b50: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
+00002b60: 656c 662e 7265 7375 6c74 203d 2072 6573  elf.result = res
+00002b70: 756c 740d 0a0d 0a20 2020 2064 6566 205f  ult....    def _
+00002b80: 5f72 6570 725f 5f28 7365 6c66 293a 0d0a  _repr__(self):..
+00002b90: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00002ba0: 2753 6567 6d65 6e74 2873 7461 7274 3d7b  'Segment(start={
+00002bb0: 7365 6c66 2e73 7461 7274 7d2c 2065 6e64  self.start}, end
+00002bc0: 3d7b 7365 6c66 2e65 6e64 7d2c 2074 6578  ={self.end}, tex
+00002bd0: 743d 227b 7365 6c66 2e74 6578 747d 2229  t="{self.text}")
+00002be0: 270d 0a0d 0a20 2020 2064 6566 205f 5f67  '....    def __g
+00002bf0: 6574 6974 656d 5f5f 2873 656c 662c 2069  etitem__(self, i
+00002c00: 6e64 6578 3a20 696e 7429 202d 3e20 576f  ndex: int) -> Wo
+00002c10: 7264 5469 6d69 6e67 3a0d 0a20 2020 2020  rdTiming:..     
+00002c20: 2020 2069 6620 7365 6c66 2e77 6f72 6473     if self.words
+00002c30: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002c40: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00002c50: 7565 4572 726f 7228 2773 6567 6d65 6e74  ueError('segment
+00002c60: 2063 6f6e 7461 696e 7320 6e6f 2077 6f72   contains no wor
+00002c70: 6473 2729 0d0a 2020 2020 2020 2020 7265  ds')..        re
+00002c80: 7475 726e 2073 656c 662e 776f 7264 735b  turn self.words[
+00002c90: 696e 6465 785d 0d0a 0d0a 2020 2020 6465  index]....    de
+00002ca0: 6620 5f5f 6465 6c69 7465 6d5f 5f28 7365  f __delitem__(se
+00002cb0: 6c66 2c20 696e 6465 783a 2069 6e74 293a  lf, index: int):
+00002cc0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00002cd0: 662e 776f 7264 7320 6973 204e 6f6e 653a  f.words is None:
+00002ce0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00002cf0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00002d00: 7365 676d 656e 7420 636f 6e74 6169 6e73  segment contains
+00002d10: 206e 6f20 776f 7264 7327 290d 0a20 2020   no words')..   
+00002d20: 2020 2020 2064 656c 2073 656c 662e 776f       del self.wo
+00002d30: 7264 735b 696e 6465 785d 0d0a 2020 2020  rds[index]..    
+00002d40: 2020 2020 7365 6c66 2e72 6561 7373 6967      self.reassig
+00002d50: 6e5f 6964 7328 696e 6465 7829 0d0a 0d0a  n_ids(index)....
+00002d60: 2020 2020 6465 6620 5f5f 6465 6570 636f      def __deepco
+00002d70: 7079 5f5f 2873 656c 662c 206d 656d 6f3d  py__(self, memo=
+00002d80: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00002d90: 7265 7475 726e 2073 656c 662e 636f 7079  return self.copy
+00002da0: 2863 6f70 795f 776f 7264 733d 5472 7565  (copy_words=True
+00002db0: 2c20 636f 7079 5f74 6f6b 656e 733d 5472  , copy_tokens=Tr
+00002dc0: 7565 290d 0a0d 0a20 2020 2064 6566 205f  ue)....    def _
+00002dd0: 5f63 6f70 795f 5f28 7365 6c66 293a 0d0a  _copy__(self):..
+00002de0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002df0: 656c 662e 636f 7079 2829 0d0a 0d0a 2020  elf.copy()....  
+00002e00: 2020 6465 6620 636f 7079 280d 0a20 2020    def copy(..   
+00002e10: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+00002e20: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00002e30: 776f 7264 733a 204f 7074 696f 6e61 6c5b  words: Optional[
+00002e40: 4c69 7374 5b57 6f72 6454 696d 696e 675d  List[WordTiming]
+00002e50: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+00002e60: 2020 2020 2020 206b 6565 705f 7265 7375         keep_resu
+00002e70: 6c74 3a20 626f 6f6c 203d 2046 616c 7365  lt: bool = False
+00002e80: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00002e90: 6f70 795f 776f 7264 733a 2062 6f6f 6c20  opy_words: bool 
+00002ea0: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00002eb0: 2020 2020 2020 636f 7079 5f74 6f6b 656e        copy_token
+00002ec0: 733a 2062 6f6f 6c20 3d20 4661 6c73 650d  s: bool = False.
+00002ed0: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
+00002ee0: 2069 6620 6e65 775f 776f 7264 7320 6973   if new_words is
+00002ef0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00002f00: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
+00002f10: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00002f20: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
+00002f30: 5b77 2e63 6f70 7928 636f 7079 5f74 6f6b  [w.copy(copy_tok
+00002f40: 656e 733d 636f 7079 5f74 6f6b 656e 7329  ens=copy_tokens)
+00002f50: 2066 6f72 2077 2069 6e20 7365 6c66 2e77   for w in self.w
+00002f60: 6f72 6473 5d20 6966 2063 6f70 795f 776f  ords] if copy_wo
+00002f70: 7264 7320 656c 7365 2073 656c 662e 776f  rds else self.wo
+00002f80: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
+00002f90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00002fa0: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
+00002fb0: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00002fc0: 2020 6465 665f 7374 6172 7420 3d20 7365    def_start = se
+00002fd0: 6c66 2e5f 6465 6661 756c 745f 7374 6172  lf._default_star
+00002fe0: 740d 0a20 2020 2020 2020 2020 2020 2064  t..            d
+00002ff0: 6566 5f65 6e64 203d 2073 656c 662e 5f64  ef_end = self._d
+00003000: 6566 6175 6c74 5f65 6e64 0d0a 2020 2020  efault_end..    
+00003010: 2020 2020 2020 2020 6465 665f 7465 7874          def_text
+00003020: 203d 2073 656c 662e 5f64 6566 6175 6c74   = self._default
+00003030: 5f74 6578 740d 0a20 2020 2020 2020 2020  _text..         
+00003040: 2020 2064 6566 5f74 6f6b 656e 7320 3d20     def_tokens = 
+00003050: 7365 6c66 2e5f 6465 6661 756c 745f 746f  self._default_to
+00003060: 6b65 6e73 0d0a 2020 2020 2020 2020 656c  kens..        el
+00003070: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00003080: 2077 6f72 6473 203d 205b 772e 636f 7079   words = [w.copy
+00003090: 2863 6f70 795f 746f 6b65 6e73 3d63 6f70  (copy_tokens=cop
+000030a0: 795f 746f 6b65 6e73 2920 666f 7220 7720  y_tokens) for w 
+000030b0: 696e 206e 6577 5f77 6f72 6473 5d20 6966  in new_words] if
+000030c0: 2063 6f70 795f 776f 7264 7320 656c 7365   copy_words else
+000030d0: 206e 6577 5f77 6f72 6473 0d0a 2020 2020   new_words..    
+000030e0: 2020 2020 2020 2020 6465 665f 7374 6172          def_star
+000030f0: 7420 3d20 6465 665f 656e 6420 3d20 6465  t = def_end = de
+00003100: 665f 7465 7874 203d 2064 6566 5f74 6f6b  f_text = def_tok
+00003110: 656e 7320 3d20 4e6f 6e65 0d0a 2020 2020  ens = None..    
+00003120: 2020 2020 6e65 775f 7365 6720 3d20 5365      new_seg = Se
+00003130: 676d 656e 7428 0d0a 2020 2020 2020 2020  gment(..        
+00003140: 2020 2020 7374 6172 743d 6465 665f 7374      start=def_st
+00003150: 6172 742c 0d0a 2020 2020 2020 2020 2020  art,..          
+00003160: 2020 656e 643d 6465 665f 656e 642c 0d0a    end=def_end,..
+00003170: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00003180: 3d64 6566 5f74 6578 742c 0d0a 2020 2020  =def_text,..    
+00003190: 2020 2020 2020 2020 7365 656b 3d73 656c          seek=sel
+000031a0: 662e 7365 656b 2c0d 0a20 2020 2020 2020  f.seek,..       
+000031b0: 2020 2020 2074 6f6b 656e 733d 6465 665f       tokens=def_
+000031c0: 746f 6b65 6e73 2c0d 0a20 2020 2020 2020  tokens,..       
+000031d0: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
+000031e0: 3d73 656c 662e 7465 6d70 6572 6174 7572  =self.temperatur
+000031f0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00003200: 6176 675f 6c6f 6770 726f 623d 7365 6c66  avg_logprob=self
+00003210: 2e61 7667 5f6c 6f67 7072 6f62 2c0d 0a20  .avg_logprob,.. 
+00003220: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
+00003230: 6573 7369 6f6e 5f72 6174 696f 3d73 656c  ession_ratio=sel
+00003240: 662e 636f 6d70 7265 7373 696f 6e5f 7261  f.compression_ra
+00003250: 7469 6f2c 0d0a 2020 2020 2020 2020 2020  tio,..          
+00003260: 2020 6e6f 5f73 7065 6563 685f 7072 6f62    no_speech_prob
+00003270: 3d73 656c 662e 6e6f 5f73 7065 6563 685f  =self.no_speech_
+00003280: 7072 6f62 2c0d 0a20 2020 2020 2020 2020  prob,..         
+00003290: 2020 2077 6f72 6473 3d77 6f72 6473 2c0d     words=words,.
+000032a0: 0a20 2020 2020 2020 2020 2020 2069 643d  .            id=
+000032b0: 7365 6c66 2e69 642c 0d0a 2020 2020 2020  self.id,..      
+000032c0: 2020 2020 2020 7265 7375 6c74 3d73 656c        result=sel
+000032d0: 662e 7265 7375 6c74 2069 6620 6b65 6570  f.result if keep
+000032e0: 5f72 6573 756c 7420 656c 7365 204e 6f6e  _result else Non
+000032f0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00003300: 726f 756e 645f 7473 3d73 656c 662e 726f  round_ts=self.ro
+00003310: 756e 645f 7473 2c0d 0a20 2020 2020 2020  und_ts,..       
+00003320: 2020 2020 2069 676e 6f72 655f 756e 7573       ignore_unus
+00003330: 6564 5f61 7267 733d 5472 7565 0d0a 2020  ed_args=True..  
+00003340: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00003350: 2072 6574 7572 6e20 6e65 775f 7365 670d   return new_seg.
+00003360: 0a0d 0a20 2020 2064 6566 2072 6f75 6e64  ...    def round
+00003370: 2873 656c 662c 2074 696d 6573 7461 6d70  (self, timestamp
+00003380: 3a20 666c 6f61 7429 202d 3e20 666c 6f61  : float) -> floa
+00003390: 743a 0d0a 2020 2020 2020 2020 6966 206e  t:..        if n
+000033a0: 6f74 2073 656c 662e 726f 756e 645f 7473  ot self.round_ts
+000033b0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000033c0: 6574 7572 6e20 7469 6d65 7374 616d 700d  eturn timestamp.
+000033d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000033e0: 5f72 6f75 6e64 5f74 696d 6573 7461 6d70  _round_timestamp
+000033f0: 2874 696d 6573 7461 6d70 290d 0a0d 0a20  (timestamp).... 
+00003400: 2020 2064 6566 2074 6f5f 6469 7370 6c61     def to_displa
+00003410: 795f 7374 7228 7365 6c66 2c20 6f6e 6c79  y_str(self, only
+00003420: 5f73 6567 6d65 6e74 3a20 626f 6f6c 203d  _segment: bool =
+00003430: 2046 616c 7365 293a 0d0a 2020 2020 2020   False):..      
+00003440: 2020 6c69 6e65 203d 2066 275b 7b66 6f72    line = f'[{for
+00003450: 6d61 745f 7469 6d65 7374 616d 7028 7365  mat_timestamp(se
+00003460: 6c66 2e73 7461 7274 297d 202d 2d3e 207b  lf.start)} --> {
+00003470: 666f 726d 6174 5f74 696d 6573 7461 6d70  format_timestamp
+00003480: 2873 656c 662e 656e 6429 7d5d 2022 7b73  (self.end)}] "{s
+00003490: 656c 662e 7465 7874 7d22 270d 0a20 2020  elf.text}"'..   
+000034a0: 2020 2020 2069 6620 7365 6c66 2e68 6173       if self.has
+000034b0: 5f77 6f72 6473 2061 6e64 206e 6f74 206f  _words and not o
+000034c0: 6e6c 795f 7365 676d 656e 743a 0d0a 2020  nly_segment:..  
+000034d0: 2020 2020 2020 2020 2020 6c69 6e65 202b            line +
+000034e0: 3d20 275c 6e27 202b 2027 5c6e 272e 6a6f  = '\n' + '\n'.jo
+000034f0: 696e 280d 0a20 2020 2020 2020 2020 2020  in(..           
+00003500: 2020 2020 2066 222d 7b77 2e74 6f5f 6469       f"-{w.to_di
+00003510: 7370 6c61 795f 7374 7228 297d 2220 666f  splay_str()}" fo
+00003520: 7220 7720 696e 2073 656c 662e 776f 7264  r w in self.word
+00003530: 730d 0a20 2020 2020 2020 2020 2020 2029  s..            )
+00003540: 202b 2027 5c6e 270d 0a20 2020 2020 2020   + '\n'..       
+00003550: 2072 6574 7572 6e20 6c69 6e65 0d0a 0d0a   return line....
+00003560: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00003570: 2020 2064 6566 2068 6173 5f77 6f72 6473     def has_words
+00003580: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00003590: 2072 6574 7572 6e20 626f 6f6c 2873 656c   return bool(sel
+000035a0: 662e 776f 7264 7329 0d0a 0d0a 2020 2020  f.words)....    
+000035b0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+000035c0: 6566 206f 7269 5f68 6173 5f77 6f72 6473  ef ori_has_words
+000035d0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000035e0: 2072 6574 7572 6e20 7365 6c66 2e77 6f72   return self.wor
+000035f0: 6473 2069 7320 6e6f 7420 4e6f 6e65 0d0a  ds is not None..
+00003600: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00003610: 0a20 2020 2064 6566 2073 7461 7274 2873  .    def start(s
+00003620: 656c 6629 3a0d 0a20 2020 2020 2020 2069  elf):..        i
+00003630: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
+00003640: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00003650: 6574 7572 6e20 7365 6c66 2e77 6f72 6473  eturn self.words
+00003660: 5b30 5d2e 7374 6172 740d 0a20 2020 2020  [0].start..     
+00003670: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00003680: 6465 6661 756c 745f 7374 6172 740d 0a0d  default_start...
+00003690: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+000036a0: 2020 2020 6465 6620 656e 6428 7365 6c66      def end(self
+000036b0: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
+000036c0: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
+000036d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000036e0: 726e 2073 656c 662e 776f 7264 735b 2d31  rn self.words[-1
+000036f0: 5d2e 656e 640d 0a20 2020 2020 2020 2072  ].end..        r
+00003700: 6574 7572 6e20 7365 6c66 2e5f 6465 6661  eturn self._defa
+00003710: 756c 745f 656e 640d 0a0d 0a20 2020 2040  ult_end....    @
+00003720: 7374 6172 742e 7365 7474 6572 0d0a 2020  start.setter..  
+00003730: 2020 6465 6620 7374 6172 7428 7365 6c66    def start(self
+00003740: 2c20 7661 6c29 3a0d 0a20 2020 2020 2020  , val):..       
+00003750: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
+00003760: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00003770: 2073 656c 662e 776f 7264 735b 305d 2e73   self.words[0].s
+00003780: 7461 7274 203d 2076 616c 0d0a 2020 2020  tart = val..    
+00003790: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000037a0: 2020 2020 2020 2020 7365 6c66 2e5f 6465          self._de
+000037b0: 6661 756c 745f 7374 6172 7420 3d20 7365  fault_start = se
+000037c0: 6c66 2e72 6f75 6e64 2876 616c 290d 0a0d  lf.round(val)...
+000037d0: 0a20 2020 2040 656e 642e 7365 7474 6572  .    @end.setter
+000037e0: 0d0a 2020 2020 6465 6620 656e 6428 7365  ..    def end(se
+000037f0: 6c66 2c20 7661 6c29 3a0d 0a20 2020 2020  lf, val):..     
+00003800: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
+00003810: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+00003820: 2020 2073 656c 662e 776f 7264 735b 2d31     self.words[-1
+00003830: 5d2e 656e 6420 3d20 7661 6c0d 0a20 2020  ].end = val..   
+00003840: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+00003850: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+00003860: 6566 6175 6c74 5f65 6e64 203d 2073 656c  efault_end = sel
+00003870: 662e 726f 756e 6428 7661 6c29 0d0a 0d0a  f.round(val)....
+00003880: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00003890: 2020 2064 6566 2074 6578 7428 7365 6c66     def text(self
+000038a0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000038b0: 2020 2069 6620 7365 6c66 2e68 6173 5f77     if self.has_w
+000038c0: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+000038d0: 2020 2072 6574 7572 6e20 2727 2e6a 6f69     return ''.joi
+000038e0: 6e28 776f 7264 2e77 6f72 6420 666f 7220  n(word.word for 
+000038f0: 776f 7264 2069 6e20 7365 6c66 2e77 6f72  word in self.wor
+00003900: 6473 290d 0a20 2020 2020 2020 2072 6574  ds)..        ret
+00003910: 7572 6e20 7365 6c66 2e5f 6465 6661 756c  urn self._defaul
+00003920: 745f 7465 7874 0d0a 0d0a 2020 2020 4070  t_text....    @p
+00003930: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00003940: 2074 6f6b 656e 7328 7365 6c66 2920 2d3e   tokens(self) ->
+00003950: 204c 6973 745b 696e 745d 3a0d 0a20 2020   List[int]:..   
+00003960: 2020 2020 2069 6620 7365 6c66 2e68 6173       if self.has
+00003970: 5f77 6f72 6473 2061 6e64 2073 656c 662e  _words and self.
+00003980: 776f 7264 735b 305d 2e74 6f6b 656e 733a  words[0].tokens:
+00003990: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000039a0: 7475 726e 206c 6973 7428 6368 6169 6e2e  turn list(chain.
+000039b0: 6672 6f6d 5f69 7465 7261 626c 6528 776f  from_iterable(wo
+000039c0: 7264 2e74 6f6b 656e 7320 666f 7220 776f  rd.tokens for wo
+000039d0: 7264 2069 6e20 7365 6c66 2e77 6f72 6473  rd in self.words
+000039e0: 2929 0d0a 2020 2020 2020 2020 7265 7475  ))..        retu
+000039f0: 726e 2073 656c 662e 5f64 6566 6175 6c74  rn self._default
+00003a00: 5f74 6f6b 656e 730d 0a0d 0a20 2020 2040  _tokens....    @
+00003a10: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00003a20: 6620 6475 7261 7469 6f6e 2873 656c 6629  f duration(self)
+00003a30: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00003a40: 6e20 7365 6c66 2e65 6e64 202d 2073 656c  n self.end - sel
+00003a50: 662e 7374 6172 740d 0a0d 0a20 2020 2064  f.start....    d
+00003a60: 6566 2077 6f72 645f 636f 756e 7428 7365  ef word_count(se
+00003a70: 6c66 293a 0d0a 2020 2020 2020 2020 6966  lf):..        if
+00003a80: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
+00003a90: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00003aa0: 7475 726e 206c 656e 2873 656c 662e 776f  turn len(self.wo
+00003ab0: 7264 7329 0d0a 2020 2020 2020 2020 7265  rds)..        re
+00003ac0: 7475 726e 202d 310d 0a0d 0a20 2020 2064  turn -1....    d
+00003ad0: 6566 2063 6861 725f 636f 756e 7428 7365  ef char_count(se
+00003ae0: 6c66 293a 0d0a 2020 2020 2020 2020 6966  lf):..        if
+00003af0: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
+00003b00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00003b10: 7475 726e 2073 756d 286c 656e 2877 2920  turn sum(len(w) 
+00003b20: 666f 7220 7720 696e 2073 656c 662e 776f  for w in self.wo
+00003b30: 7264 7329 0d0a 2020 2020 2020 2020 7265  rds)..        re
+00003b40: 7475 726e 206c 656e 2873 656c 662e 7465  turn len(self.te
+00003b50: 7874 290d 0a0d 0a20 2020 2064 6566 2061  xt)....    def a
+00003b60: 6464 2873 656c 662c 206f 7468 6572 3a20  dd(self, other: 
+00003b70: 2753 6567 6d65 6e74 272c 2063 6f70 795f  'Segment', copy_
+00003b80: 776f 7264 733a 2062 6f6f 6c20 3d20 4661  words: bool = Fa
+00003b90: 6c73 652c 206e 6577 6c69 6e65 3a20 626f  lse, newline: bo
+00003ba0: 6f6c 203d 2046 616c 7365 293a 0d0a 2020  ol = False):..  
+00003bb0: 2020 2020 2020 6966 2073 656c 662e 6f72        if self.or
+00003bc0: 695f 6861 735f 776f 7264 7320 3d3d 206f  i_has_words == o
+00003bd0: 7468 6572 2e6f 7269 5f68 6173 5f77 6f72  ther.ori_has_wor
+00003be0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00003bf0: 2077 6f72 6473 203d 2028 7365 6c66 2e77   words = (self.w
+00003c00: 6f72 6473 202b 206f 7468 6572 2e77 6f72  ords + other.wor
+00003c10: 6473 2920 6966 2073 656c 662e 6f72 695f  ds) if self.ori_
+00003c20: 6861 735f 776f 7264 7320 656c 7365 204e  has_words else N
+00003c30: 6f6e 650d 0a20 2020 2020 2020 2065 6c73  one..        els
+00003c40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003c50: 7365 6c66 5f73 7461 7465 203d 2027 7769  self_state = 'wi
+00003c60: 7468 2720 6966 2073 656c 662e 6f72 695f  th' if self.ori_
+00003c70: 6861 735f 776f 7264 7320 656c 7365 2027  has_words else '
+00003c80: 7769 7468 6f75 7427 0d0a 2020 2020 2020  without'..      
+00003c90: 2020 2020 2020 6f74 6865 725f 7374 6174        other_stat
+00003ca0: 6520 3d20 2777 6974 6827 2069 6620 6f74  e = 'with' if ot
+00003cb0: 6865 722e 6f72 695f 6861 735f 776f 7264  her.ori_has_word
+00003cc0: 7320 656c 7365 2027 7769 7468 6f75 7427  s else 'without'
+00003cd0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00003ce0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00003cf0: 2243 616e 2774 206d 6572 6765 2073 6567  "Can't merge seg
+00003d00: 6d65 6e74 207b 7365 6c66 5f73 7461 7465  ment {self_state
+00003d10: 7d20 776f 7264 7320 616e 6420 6120 7365  } words and a se
+00003d20: 676d 656e 7420 7b6f 7468 6572 5f73 7461  gment {other_sta
+00003d30: 7465 7d20 776f 7264 732e 2229 0d0a 0d0a  te} words.")....
+00003d40: 2020 2020 2020 2020 7365 6c66 5f63 6f70          self_cop
+00003d50: 7920 3d20 7365 6c66 2e63 6f70 7928 776f  y = self.copy(wo
+00003d60: 7264 732c 2063 6f70 795f 776f 7264 733d  rds, copy_words=
+00003d70: 636f 7079 5f77 6f72 6473 290d 0a20 2020  copy_words)..   
+00003d80: 2020 2020 205f 636f 6d62 696e 655f 6174       _combine_at
+00003d90: 7472 2873 656c 665f 636f 7079 2c20 6f74  tr(self_copy, ot
+00003da0: 6865 722c 2027 7465 6d70 6572 6174 7572  her, 'temperatur
+00003db0: 6527 290d 0a20 2020 2020 2020 205f 636f  e')..        _co
+00003dc0: 6d62 696e 655f 6174 7472 2873 656c 665f  mbine_attr(self_
+00003dd0: 636f 7079 2c20 6f74 6865 722c 2027 6176  copy, other, 'av
+00003de0: 675f 6c6f 6770 726f 6227 290d 0a20 2020  g_logprob')..   
+00003df0: 2020 2020 205f 636f 6d62 696e 655f 6174       _combine_at
+00003e00: 7472 2873 656c 665f 636f 7079 2c20 6f74  tr(self_copy, ot
+00003e10: 6865 722c 2027 636f 6d70 7265 7373 696f  her, 'compressio
+00003e20: 6e5f 7261 7469 6f27 290d 0a20 2020 2020  n_ratio')..     
+00003e30: 2020 205f 636f 6d62 696e 655f 6174 7472     _combine_attr
+00003e40: 2873 656c 665f 636f 7079 2c20 6f74 6865  (self_copy, othe
+00003e50: 722c 2027 6e6f 5f73 7065 6563 685f 7072  r, 'no_speech_pr
+00003e60: 6f62 2729 0d0a 0d0a 2020 2020 2020 2020  ob')....        
+00003e70: 7365 6c66 5f63 6f70 792e 5f64 6566 6175  self_copy._defau
+00003e80: 6c74 5f65 6e64 203d 206f 7468 6572 2e5f  lt_end = other._
+00003e90: 6465 6661 756c 745f 656e 640d 0a20 2020  default_end..   
+00003ea0: 2020 2020 2073 656c 665f 636f 7079 2e5f       self_copy._
+00003eb0: 6465 6661 756c 745f 7465 7874 202b 3d20  default_text += 
+00003ec0: 6f74 6865 722e 5f64 6566 6175 6c74 5f74  other._default_t
+00003ed0: 6578 740d 0a20 2020 2020 2020 2073 656c  ext..        sel
+00003ee0: 665f 636f 7079 2e5f 6465 6661 756c 745f  f_copy._default_
+00003ef0: 746f 6b65 6e73 202b 3d20 6f74 6865 722e  tokens += other.
+00003f00: 5f64 6566 6175 6c74 5f74 6f6b 656e 730d  _default_tokens.
+00003f10: 0a0d 0a20 2020 2020 2020 2069 6620 6e65  ...        if ne
+00003f20: 776c 696e 653a 0d0a 2020 2020 2020 2020  wline:..        
+00003f30: 2020 2020 6966 2073 656c 665f 636f 7079      if self_copy
+00003f40: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
+00003f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003f60: 6e6f 7420 7365 6c66 5f63 6f70 792e 776f  not self_copy.wo
+00003f70: 7264 735b 6c65 6e28 7365 6c66 2e77 6f72  rds[len(self.wor
+00003f80: 6473 292d 315d 2e77 6f72 642e 656e 6473  ds)-1].word.ends
+00003f90: 7769 7468 2827 5c6e 2729 3a0d 0a20 2020  with('\n'):..   
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 2073 656c 665f 636f 7079 2e77 6f72 6473   self_copy.words
+00003fc0: 5b6c 656e 2873 656c 662e 776f 7264 7329  [len(self.words)
+00003fd0: 2d31 5d2e 776f 7264 202b 3d20 275c 6e27  -1].word += '\n'
+00003fe0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00003ff0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00004000: 2020 2020 2069 6620 7365 6c66 5f63 6f70       if self_cop
+00004010: 792e 7465 7874 5b6c 656e 2873 656c 662e  y.text[len(self.
+00004020: 7465 7874 292d 315d 2021 3d20 275c 6e27  text)-1] != '\n'
+00004030: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004040: 2020 2020 2020 2073 656c 665f 636f 7079         self_copy
+00004050: 2e5f 6465 6661 756c 745f 7465 7874 203d  ._default_text =
+00004060: 2073 656c 665f 636f 7079 2e74 6578 745b   self_copy.text[
+00004070: 3a6c 656e 2873 656c 662e 7465 7874 295d  :len(self.text)]
+00004080: 202b 2027 5c6e 2720 2b20 7365 6c66 5f63   + '\n' + self_c
+00004090: 6f70 792e 7465 7874 5b6c 656e 2873 656c  opy.text[len(sel
+000040a0: 662e 7465 7874 293a 5d0d 0a0d 0a20 2020  f.text):]....   
+000040b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000040c0: 5f63 6f70 790d 0a0d 0a20 2020 2064 6566  _copy....    def
+000040d0: 205f 5f61 6464 5f5f 2873 656c 662c 206f   __add__(self, o
+000040e0: 7468 6572 3a20 2753 6567 6d65 6e74 2729  ther: 'Segment')
+000040f0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00004100: 6e20 7365 6c66 2e61 6464 286f 7468 6572  n self.add(other
+00004110: 2c20 636f 7079 5f77 6f72 6473 3d54 7275  , copy_words=Tru
+00004120: 6529 0d0a 0d0a 2020 2020 6465 6620 5f77  e)....    def _w
+00004130: 6f72 645f 6f70 6572 6174 696f 6e73 2873  ord_operations(s
+00004140: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
+00004150: 7374 722c 202a 6172 6773 2c20 2a2a 6b77  str, *args, **kw
+00004160: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00004170: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
+00004180: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004190: 666f 7220 7720 696e 2073 656c 662e 776f  for w in self.wo
+000041a0: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+000041b0: 2020 2020 2020 6765 7461 7474 7228 772c        getattr(w,
+000041c0: 206f 7065 7261 7469 6f6e 2928 2a61 7267   operation)(*arg
+000041d0: 732c 202a 2a6b 7761 7267 7329 0d0a 0d0a  s, **kwargs)....
+000041e0: 2020 2020 6465 6620 726f 756e 645f 616c      def round_al
+000041f0: 6c5f 7469 6d65 7374 616d 7073 2873 656c  l_timestamps(sel
+00004200: 6629 3a0d 0a20 2020 2020 2020 2077 6172  f):..        war
+00004210: 6e69 6e67 732e 7761 726e 2827 6060 2e72  nings.warn('``.r
+00004220: 6f75 6e64 5f61 6c6c 5f74 696d 6573 7461  ound_all_timesta
+00004230: 6d70 7328 2960 6020 6973 2064 6570 7265  mps()`` is depre
+00004240: 6361 7465 6420 616e 6420 7769 6c6c 2062  cated and will b
+00004250: 6520 7265 6d6f 7665 6420 696e 2066 7574  e removed in fut
+00004260: 7572 6520 7665 7273 696f 6e73 2e20 270d  ure versions. '.
+00004270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004280: 2020 2020 2020 2027 5573 6520 6060 2e72         'Use ``.r
+00004290: 6f75 6e64 5f74 733d 5472 7565 6060 2074  ound_ts=True`` t
+000042a0: 6f20 726f 756e 6420 7469 6d65 7374 616d  o round timestam
+000042b0: 7073 2062 7920 6465 6661 756c 7420 696e  ps by default in
+000042c0: 7374 6561 642e 272c 0d0a 2020 2020 2020  stead.',..      
+000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042e0: 7374 6163 6b6c 6576 656c 3d32 290d 0a20  stacklevel=2).. 
+000042f0: 2020 2020 2020 2073 656c 662e 726f 756e         self.roun
+00004300: 645f 7473 203d 2054 7275 650d 0a0d 0a20  d_ts = True.... 
+00004310: 2020 2064 6566 206f 6666 7365 745f 7469     def offset_ti
+00004320: 6d65 2873 656c 662c 206f 6666 7365 745f  me(self, offset_
+00004330: 7365 636f 6e64 733a 2066 6c6f 6174 293a  seconds: float):
+00004340: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00004350: 662e 7365 656b 2069 7320 6e6f 7420 4e6f  f.seek is not No
+00004360: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00004370: 2073 656c 662e 7365 656b 202b 3d20 6f66   self.seek += of
+00004380: 6673 6574 5f73 6563 6f6e 6473 0d0a 2020  fset_seconds..  
+00004390: 2020 2020 2020 6966 2073 656c 662e 6861        if self.ha
+000043a0: 735f 776f 7264 733a 0d0a 2020 2020 2020  s_words:..      
+000043b0: 2020 2020 2020 7365 6c66 2e5f 776f 7264        self._word
+000043c0: 5f6f 7065 7261 7469 6f6e 7328 276f 6666  _operations('off
+000043d0: 7365 745f 7469 6d65 272c 206f 6666 7365  set_time', offse
+000043e0: 745f 7365 636f 6e64 7329 0d0a 2020 2020  t_seconds)..    
+000043f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00004400: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
+00004410: 7420 3d20 7365 6c66 2e73 7461 7274 202b  t = self.start +
+00004420: 206f 6666 7365 745f 7365 636f 6e64 730d   offset_seconds.
+00004430: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004440: 662e 656e 6420 3d20 7365 6c66 2e65 6e64  f.end = self.end
+00004450: 202b 206f 6666 7365 745f 7365 636f 6e64   + offset_second
+00004460: 730d 0a0d 0a20 2020 2064 6566 2061 6464  s....    def add
+00004470: 5f77 6f72 6473 2873 656c 662c 2069 6e64  _words(self, ind
+00004480: 6578 303a 2069 6e74 2c20 696e 6465 7831  ex0: int, index1
+00004490: 3a20 696e 742c 2069 6e70 6c61 6365 3a20  : int, inplace: 
+000044a0: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
+000044b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000044c0: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
+000044d0: 2020 2020 2020 2020 6e65 775f 776f 7264          new_word
+000044e0: 203d 2073 656c 662e 776f 7264 735b 696e   = self.words[in
+000044f0: 6465 7830 5d20 2b20 7365 6c66 2e77 6f72  dex0] + self.wor
+00004500: 6473 5b69 6e64 6578 315d 0d0a 2020 2020  ds[index1]..    
+00004510: 2020 2020 2020 2020 6966 2069 6e70 6c61          if inpla
+00004520: 6365 3a0d 0a20 2020 2020 2020 2020 2020  ce:..           
+00004530: 2020 2020 2069 302c 2069 3120 3d20 736f       i0, i1 = so
+00004540: 7274 6564 285b 696e 6465 7830 2c20 696e  rted([index0, in
+00004550: 6465 7831 5d29 0d0a 2020 2020 2020 2020  dex1])..        
+00004560: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+00004570: 6473 5b69 305d 203d 206e 6577 5f77 6f72  ds[i0] = new_wor
+00004580: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00004590: 2020 2064 656c 2073 656c 662e 776f 7264     del self.word
+000045a0: 735b 6931 5d0d 0a20 2020 2020 2020 2020  s[i1]..         
+000045b0: 2020 2072 6574 7572 6e20 6e65 775f 776f     return new_wo
+000045c0: 7264 0d0a 0d0a 2020 2020 6465 6620 7265  rd....    def re
+000045d0: 7363 616c 655f 7469 6d65 2873 656c 662c  scale_time(self,
+000045e0: 2073 6361 6c65 5f66 6163 746f 723a 2066   scale_factor: f
+000045f0: 6c6f 6174 293a 0d0a 2020 2020 2020 2020  loat):..        
+00004600: 6966 2073 656c 662e 7365 656b 2069 7320  if self.seek is 
+00004610: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00004620: 2020 2020 2020 2073 656c 662e 7365 656b         self.seek
+00004630: 202a 3d20 7363 616c 655f 6661 6374 6f72   *= scale_factor
+00004640: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00004650: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
+00004660: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00004670: 776f 7264 5f6f 7065 7261 7469 6f6e 7328  word_operations(
+00004680: 2772 6573 6361 6c65 5f74 696d 6527 2c20  'rescale_time', 
+00004690: 7363 616c 655f 6661 6374 6f72 290d 0a20  scale_factor).. 
+000046a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000046b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000046c0: 7461 7274 203d 2073 656c 662e 7374 6172  tart = self.star
+000046d0: 7420 2a20 7363 616c 655f 6661 6374 6f72  t * scale_factor
+000046e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000046f0: 6c66 2e65 6e64 203d 2073 656c 662e 656e  lf.end = self.en
+00004700: 6420 2a20 7363 616c 655f 6661 6374 6f72  d * scale_factor
+00004710: 0d0a 0d0a 2020 2020 6465 6620 6170 706c  ....    def appl
+00004720: 795f 6d69 6e5f 6475 7228 7365 6c66 2c20  y_min_dur(self, 
+00004730: 6d69 6e5f 6475 723a 2066 6c6f 6174 2c20  min_dur: float, 
+00004740: 696e 706c 6163 653a 2062 6f6f 6c20 3d20  inplace: bool = 
+00004750: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00004760: 2022 2222 0d0a 2020 2020 2020 2020 4d65   """..        Me
+00004770: 7267 6520 616e 7920 776f 7264 2077 6974  rge any word wit
+00004780: 6820 6164 6a61 6365 6e74 2077 6f72 6420  h adjacent word 
+00004790: 6966 2069 7473 2064 7572 6174 696f 6e20  if its duration 
+000047a0: 6973 206c 6573 7320 7468 616e 2060 606d  is less than ``m
+000047b0: 696e 5f64 7572 6060 2e0d 0a20 2020 2020  in_dur``...     
+000047c0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000047d0: 7365 676d 656e 7420 3d20 7365 6c66 2069  segment = self i
+000047e0: 6620 696e 706c 6163 6520 656c 7365 2064  f inplace else d
+000047f0: 6565 7063 6f70 7928 7365 6c66 290d 0a20  eepcopy(self).. 
+00004800: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00004810: 6c66 2e68 6173 5f77 6f72 6473 3a0d 0a20  lf.has_words:.. 
+00004820: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004830: 6e20 7365 676d 656e 740d 0a20 2020 2020  n segment..     
+00004840: 2020 206d 6178 5f69 203d 206c 656e 2873     max_i = len(s
+00004850: 6567 6d65 6e74 2e77 6f72 6473 2920 2d20  egment.words) - 
+00004860: 310d 0a20 2020 2020 2020 2069 6620 6d61  1..        if ma
+00004870: 785f 6920 3d3d 2030 3a0d 0a20 2020 2020  x_i == 0:..     
+00004880: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00004890: 676d 656e 740d 0a20 2020 2020 2020 2066  gment..        f
+000048a0: 6f72 2069 2069 6e20 7265 7665 7273 6564  or i in reversed
+000048b0: 2872 616e 6765 286c 656e 2873 6567 6d65  (range(len(segme
+000048c0: 6e74 2e77 6f72 6473 2929 293a 0d0a 2020  nt.words))):..  
+000048d0: 2020 2020 2020 2020 2020 6966 206d 6178            if max
+000048e0: 5f69 203d 3d20 303a 0d0a 2020 2020 2020  _i == 0:..      
+000048f0: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00004900: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004910: 7365 676d 656e 742e 776f 7264 735b 695d  segment.words[i]
+00004920: 2e64 7572 6174 696f 6e20 3c20 6d69 6e5f  .duration < min_
+00004930: 6475 723a 0d0a 2020 2020 2020 2020 2020  dur:..          
+00004940: 2020 2020 2020 6966 2069 203d 3d20 6d61        if i == ma
+00004950: 785f 693a 0d0a 2020 2020 2020 2020 2020  x_i:..          
+00004960: 2020 2020 2020 2020 2020 7365 676d 656e            segmen
+00004970: 742e 6164 645f 776f 7264 7328 692d 312c  t.add_words(i-1,
+00004980: 2069 2c20 696e 706c 6163 653d 5472 7565   i, inplace=True
+00004990: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000049a0: 2020 2065 6c69 6620 6920 3d3d 2030 3a0d     elif i == 0:.
+000049b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049c0: 2020 2020 2073 6567 6d65 6e74 2e61 6464       segment.add
+000049d0: 5f77 6f72 6473 2869 2c20 692b 312c 2069  _words(i, i+1, i
+000049e0: 6e70 6c61 6365 3d54 7275 6529 0d0a 2020  nplace=True)..  
+000049f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00004a00: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00004a10: 2020 2020 2020 2020 2069 6620 7365 676d           if segm
+00004a20: 656e 742e 776f 7264 735b 692b 315d 2e64  ent.words[i+1].d
+00004a30: 7572 6174 696f 6e20 3c20 7365 676d 656e  uration < segmen
+00004a40: 742e 776f 7264 735b 692d 315d 2e64 7572  t.words[i-1].dur
+00004a50: 6174 696f 6e3a 0d0a 2020 2020 2020 2020  ation:..        
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 7365 676d 656e 742e 6164 645f 776f 7264  segment.add_word
+00004a80: 7328 692d 312c 2069 2c20 696e 706c 6163  s(i-1, i, inplac
+00004a90: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00004aa0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00004ab0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004ac0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+00004ad0: 656e 742e 6164 645f 776f 7264 7328 692c  ent.add_words(i,
+00004ae0: 2069 2b31 2c20 696e 706c 6163 653d 5472   i+1, inplace=Tr
+00004af0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00004b00: 2020 2020 206d 6178 5f69 202d 3d20 310d       max_i -= 1.
+00004b10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004b20: 7365 676d 656e 740d 0a0d 0a20 2020 2064  segment....    d
+00004b30: 6566 205f 746f 5f72 6576 6572 7365 5f74  ef _to_reverse_t
+00004b40: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
+00004b50: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00004b60: 2020 2020 2070 7265 7065 6e64 5f70 756e       prepend_pun
+00004b70: 6374 7561 7469 6f6e 733a 204f 7074 696f  ctuations: Optio
+00004b80: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00004b90: 0d0a 2020 2020 2020 2020 2020 2020 6170  ..            ap
+00004ba0: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
+00004bb0: 733a 204f 7074 696f 6e61 6c5b 7374 725d  s: Optional[str]
+00004bc0: 203d 204e 6f6e 652c 0d0a 2020 2020 293a   = None,..    ):
+00004bd0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00004be0: 2020 2020 2020 2052 6574 7572 6e20 6120         Return a 
+00004bf0: 636f 7079 2077 6974 6820 776f 7264 7320  copy with words 
+00004c00: 7265 7665 7273 6564 206f 7264 6572 2070  reversed order p
+00004c10: 6572 2073 6567 6d65 6e74 2e0d 0a20 2020  er segment...   
+00004c20: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004c30: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00004c40: 2760 605f 746f 5f72 6576 6572 7365 5f74  '``_to_reverse_t
+00004c50: 6578 7428 2960 6020 6973 2064 6570 7265  ext()`` is depre
+00004c60: 6361 7465 6420 616e 6420 7769 6c6c 2062  cated and will b
+00004c70: 6520 7265 6d6f 7665 6420 696e 2066 7574  e removed in fut
+00004c80: 7572 6520 7665 7273 696f 6e73 2e27 2c0d  ure versions.',.
+00004c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ca0: 2020 2020 2020 2063 6174 6567 6f72 793d         category=
+00004cb0: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+00004cc0: 6e67 2c20 7374 6163 6b6c 6576 656c 3d32  ng, stacklevel=2
+00004cd0: 290d 0a20 2020 2020 2020 2070 7265 7065  )..        prepe
+00004ce0: 6e64 5f70 756e 6374 7561 7469 6f6e 7320  nd_punctuations 
+00004cf0: 3d20 6765 745f 7072 6570 656e 645f 7075  = get_prepend_pu
+00004d00: 6e63 7475 6174 696f 6e73 2870 7265 7065  nctuations(prepe
+00004d10: 6e64 5f70 756e 6374 7561 7469 6f6e 7329  nd_punctuations)
+00004d20: 0d0a 2020 2020 2020 2020 6966 2070 7265  ..        if pre
+00004d30: 7065 6e64 5f70 756e 6374 7561 7469 6f6e  pend_punctuation
+00004d40: 7320 616e 6420 2720 2720 6e6f 7420 696e  s and ' ' not in
+00004d50: 2070 7265 7065 6e64 5f70 756e 6374 7561   prepend_punctua
+00004d60: 7469 6f6e 733a 0d0a 2020 2020 2020 2020  tions:..        
+00004d70: 2020 2020 7072 6570 656e 645f 7075 6e63      prepend_punc
+00004d80: 7475 6174 696f 6e73 202b 3d20 2720 270d  tuations += ' '.
+00004d90: 0a20 2020 2020 2020 2061 7070 656e 645f  .        append_
+00004da0: 7075 6e63 7475 6174 696f 6e73 203d 2067  punctuations = g
+00004db0: 6574 5f61 7070 656e 645f 7075 6e63 7475  et_append_punctu
+00004dc0: 6174 696f 6e73 2861 7070 656e 645f 7075  ations(append_pu
+00004dd0: 6e63 7475 6174 696f 6e73 290d 0a20 2020  nctuations)..   
+00004de0: 2020 2020 2073 656c 665f 636f 7079 203d       self_copy =
+00004df0: 2073 656c 662e 636f 7079 2863 6f70 795f   self.copy(copy_
+00004e00: 776f 7264 733d 5472 7565 290d 0a20 2020  words=True)..   
+00004e10: 2020 2020 2068 6173 5f70 7265 7065 6e64       has_prepend
+00004e20: 203d 2062 6f6f 6c28 7072 6570 656e 645f   = bool(prepend_
+00004e30: 7075 6e63 7475 6174 696f 6e73 290d 0a20  punctuations).. 
+00004e40: 2020 2020 2020 2068 6173 5f61 7070 656e         has_appen
+00004e50: 6420 3d20 626f 6f6c 2861 7070 656e 645f  d = bool(append_
+00004e60: 7075 6e63 7475 6174 696f 6e73 290d 0a20  punctuations).. 
+00004e70: 2020 2020 2020 2069 6620 6861 735f 7072         if has_pr
+00004e80: 6570 656e 6420 6f72 2068 6173 5f61 7070  epend or has_app
+00004e90: 656e 643a 0d0a 2020 2020 2020 2020 2020  end:..          
+00004ea0: 2020 776f 7264 5f6f 626a 7320 3d20 280d    word_objs = (.
+00004eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ec0: 2073 656c 665f 636f 7079 2e77 6f72 6473   self_copy.words
+00004ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ee0: 2020 6966 2073 656c 665f 636f 7079 2e68    if self_copy.h
+00004ef0: 6173 5f77 6f72 6473 2065 6c73 650d 0a20  as_words else.. 
+00004f00: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00004f10: 576f 7264 5469 6d69 6e67 2877 2c20 302c  WordTiming(w, 0,
+00004f20: 2031 2c20 3029 2066 6f72 2077 2069 6e20   1, 0) for w in 
+00004f30: 7365 6c66 5f63 6f70 792e 7465 7874 2e73  self_copy.text.s
+00004f40: 706c 6974 2827 2027 295d 0d0a 2020 2020  plit(' ')]..    
+00004f50: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00004f60: 2020 2020 2020 2066 6f72 2077 6f72 6420         for word 
+00004f70: 696e 2077 6f72 645f 6f62 6a73 3a0d 0a20  in word_objs:.. 
+00004f80: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00004f90: 6577 5f61 7070 656e 6420 3d20 2727 0d0a  ew_append = ''..
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 6966 2068 6173 5f70 7265 7065 6e64 3a0d  if has_prepend:.
+00004fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fd0: 2020 2020 2066 6f72 205f 2069 6e20 7261       for _ in ra
+00004fe0: 6e67 6528 6c65 6e28 776f 7264 2929 3a0d  nge(len(word)):.
+00004ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005000: 2020 2020 2020 2020 2063 6861 7220 3d20           char = 
+00005010: 776f 7264 2e77 6f72 645b 305d 0d0a 2020  word.word[0]..  
+00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005030: 2020 2020 2020 6966 2063 6861 7220 696e        if char in
+00005040: 2070 7265 7065 6e64 5f70 756e 6374 7561   prepend_punctua
+00005050: 7469 6f6e 733a 0d0a 2020 2020 2020 2020  tions:..        
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 2020 6e65 775f 6170 7065 6e64 202b      new_append +
+00005080: 3d20 6368 6172 0d0a 2020 2020 2020 2020  = char..        
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 776f 7264 2e77 6f72 6420 3d20      word.word = 
+000050b0: 776f 7264 2e77 6f72 645b 313a 5d0d 0a20  word.word[1:].. 
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00005100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005110: 206e 6577 5f70 7265 7065 6e64 203d 2027   new_prepend = '
+00005120: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00005130: 2020 2069 6620 6861 735f 6170 7065 6e64     if has_append
+00005140: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005150: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
+00005160: 7261 6e67 6528 6c65 6e28 776f 7264 2929  range(len(word))
+00005170: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005180: 2020 2020 2020 2020 2020 2063 6861 7220             char 
+00005190: 3d20 776f 7264 2e77 6f72 645b 2d31 5d0d  = word.word[-1].
+000051a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051b0: 2020 2020 2020 2020 2069 6620 6368 6172           if char
+000051c0: 2069 6e20 6170 7065 6e64 5f70 756e 6374   in append_punct
+000051d0: 7561 7469 6f6e 733a 0d0a 2020 2020 2020  uations:..      
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 2020 2020 6e65 775f 7072 6570 656e        new_prepen
+00005200: 6420 2b3d 2063 6861 720d 0a20 2020 2020  d += char..     
+00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2020 2020 2020 2077 6f72 642e 776f 7264         word.word
+00005230: 203d 2077 6f72 642e 776f 7264 5b3a 2d31   = word.word[:-1
+00005240: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005250: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00005260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005270: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00005280: 6561 6b0d 0a20 2020 2020 2020 2020 2020  eak..           
+00005290: 2020 2020 2077 6f72 642e 776f 7264 203d       word.word =
+000052a0: 2066 277b 6e65 775f 7072 6570 656e 647d   f'{new_prepend}
+000052b0: 7b77 6f72 642e 776f 7264 7d7b 6e65 775f  {word.word}{new_
+000052c0: 6170 7065 6e64 5b3a 3a2d 315d 7d27 0d0a  append[::-1]}'..
+000052d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000052e0: 5f63 6f70 792e 5f64 6566 6175 6c74 5f74  _copy._default_t
+000052f0: 6578 7420 3d20 2727 2e6a 6f69 6e28 772e  ext = ''.join(w.
+00005300: 776f 7264 2066 6f72 2077 2069 6e20 7265  word for w in re
+00005310: 7665 7273 6564 2877 6f72 645f 6f62 6a73  versed(word_objs
+00005320: 2929 0d0a 0d0a 2020 2020 2020 2020 7265  ))....        re
+00005330: 7475 726e 2073 656c 665f 636f 7079 0d0a  turn self_copy..
+00005340: 0d0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
+00005350: 7428 7365 6c66 2c20 7265 7665 7273 655f  t(self, reverse_
+00005360: 7465 7874 3a20 556e 696f 6e5b 626f 6f6c  text: Union[bool
+00005370: 2c20 7475 706c 655d 203d 2046 616c 7365  , tuple] = False
+00005380: 293a 0d0a 2020 2020 2020 2020 6966 2072  ):..        if r
+00005390: 6576 6572 7365 5f74 6578 743a 0d0a 2020  everse_text:..  
+000053a0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+000053b0: 6773 2e77 6172 6e28 2760 6072 6576 6572  gs.warn('``rever
+000053c0: 7365 5f74 6578 743d 5472 7565 6060 2069  se_text=True`` i
+000053d0: 7320 6465 7072 6563 6174 6564 2061 6e64  s deprecated and
+000053e0: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
+000053f0: 2069 6e20 6675 7475 7265 2076 6572 7369   in future versi
+00005400: 6f6e 732e 2027 0d0a 2020 2020 2020 2020  ons. '..        
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 2752 544c 2074 6578 7420 706c 6179    'RTL text play
+00005430: 6261 636b 2069 7373 7565 7320 6172 6520  back issues are 
+00005440: 6361 7573 6564 2062 7920 7468 6520 7669  caused by the vi
+00005450: 6465 6f20 706c 6179 6572 2069 6e63 6f72  deo player incor
+00005460: 7265 6374 6c79 2070 6172 7369 6e67 2074  rectly parsing t
+00005470: 6167 7320 270d 0a20 2020 2020 2020 2020  ags '..         
+00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005490: 2027 286e 6f74 653a 2074 6167 7320 636f   '(note: tags co
+000054a0: 6d65 2066 726f 6d20 6060 7365 676d 656e  me from ``segmen
+000054b0: 745f 6c65 7665 6c3d 5472 7565 202b 2077  t_level=True + w
+000054c0: 6f72 645f 6c65 7665 6c3d 5472 7565 6060  ord_level=True``
+000054d0: 292e 2729 0d0a 2020 2020 2020 2020 2020  ).')..          
+000054e0: 2020 7365 676d 656e 7420 3d20 7365 6c66    segment = self
+000054f0: 2e5f 746f 5f72 6576 6572 7365 5f74 6578  ._to_reverse_tex
+00005500: 7428 2a28 7265 7665 7273 655f 7465 7874  t(*(reverse_text
+00005510: 2069 6620 7265 7665 7273 655f 7465 7874   if reverse_text
+00005520: 2065 6c73 6520 5b5d 2929 0d0a 2020 2020   else []))..    
+00005530: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00005540: 2020 2020 2020 2073 6567 6d65 6e74 203d         segment =
+00005550: 2073 656c 660d 0a0d 0a20 2020 2020 2020   self....       
+00005560: 2073 6567 5f64 6963 7420 3d20 6469 6374   seg_dict = dict
+00005570: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+00005580: 7461 7274 3d73 6567 6d65 6e74 2e73 7461  tart=segment.sta
+00005590: 7274 2c0d 0a20 2020 2020 2020 2020 2020  rt,..           
+000055a0: 2065 6e64 3d73 6567 6d65 6e74 2e65 6e64   end=segment.end
+000055b0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+000055c0: 6578 743d 7365 676d 656e 742e 7465 7874  ext=segment.text
+000055d0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+000055e0: 6565 6b3d 7365 676d 656e 742e 7365 656b  eek=segment.seek
+000055f0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00005600: 6f6b 656e 733d 4e6f 6e65 2069 6620 7365  okens=None if se
+00005610: 676d 656e 742e 746f 6b65 6e73 2069 7320  gment.tokens is 
+00005620: 4e6f 6e65 2065 6c73 6520 7365 676d 656e  None else segmen
+00005630: 742e 746f 6b65 6e73 2e63 6f70 7928 292c  t.tokens.copy(),
+00005640: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+00005650: 6d70 6572 6174 7572 653d 7365 676d 656e  mperature=segmen
+00005660: 742e 7465 6d70 6572 6174 7572 652c 0d0a  t.temperature,..
+00005670: 2020 2020 2020 2020 2020 2020 6176 675f              avg_
+00005680: 6c6f 6770 726f 623d 7365 676d 656e 742e  logprob=segment.
+00005690: 6176 675f 6c6f 6770 726f 622c 0d0a 2020  avg_logprob,..  
+000056a0: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
+000056b0: 7373 696f 6e5f 7261 7469 6f3d 7365 676d  ssion_ratio=segm
+000056c0: 656e 742e 636f 6d70 7265 7373 696f 6e5f  ent.compression_
+000056d0: 7261 7469 6f2c 0d0a 2020 2020 2020 2020  ratio,..        
+000056e0: 2020 2020 6e6f 5f73 7065 6563 685f 7072      no_speech_pr
+000056f0: 6f62 3d73 6567 6d65 6e74 2e6e 6f5f 7370  ob=segment.no_sp
+00005700: 6565 6368 5f70 726f 622c 0d0a 2020 2020  eech_prob,..    
+00005710: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00005720: 2069 6620 7365 676d 656e 742e 6861 735f   if segment.has_
+00005730: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
+00005740: 2020 2020 7365 675f 6469 6374 5b27 776f      seg_dict['wo
+00005750: 7264 7327 5d20 3d20 5b77 2e74 6f5f 6469  rds'] = [w.to_di
+00005760: 6374 2829 2066 6f72 2077 2069 6e20 7365  ct() for w in se
+00005770: 676d 656e 742e 776f 7264 735d 0d0a 2020  gment.words]..  
+00005780: 2020 2020 2020 656c 6966 2073 6567 6d65        elif segme
+00005790: 6e74 2e6f 7269 5f68 6173 5f77 6f72 6473  nt.ori_has_words
+000057a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000057b0: 6567 5f64 6963 745b 2777 6f72 6473 275d  eg_dict['words']
+000057c0: 203d 205b 5d0d 0a20 2020 2020 2020 2069   = []..        i
+000057d0: 6620 7265 7665 7273 655f 7465 7874 3a0d  f reverse_text:.
+000057e0: 0a20 2020 2020 2020 2020 2020 2073 6567  .            seg
+000057f0: 5f64 6963 745b 2772 6576 6572 7365 645f  _dict['reversed_
+00005800: 7465 7874 275d 203d 2054 7275 650d 0a20  text'] = True.. 
+00005810: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00005820: 675f 6469 6374 0d0a 0d0a 2020 2020 6465  g_dict....    de
+00005830: 6620 776f 7264 735f 6279 5f6c 6f63 6b28  f words_by_lock(
+00005840: 7365 6c66 2c20 6f6e 6c79 5f74 6578 743a  self, only_text:
+00005850: 2062 6f6f 6c20 3d20 5472 7565 2c20 696e   bool = True, in
+00005860: 636c 7564 655f 7369 6e67 6c65 3a20 626f  clude_single: bo
+00005870: 6f6c 203d 2046 616c 7365 293a 0d0a 2020  ol = False):..  
+00005880: 2020 2020 2020 7265 7475 726e 205f 776f        return _wo
+00005890: 7264 735f 6279 5f6c 6f63 6b28 7365 6c66  rds_by_lock(self
+000058a0: 2e77 6f72 6473 2c20 6f6e 6c79 5f74 6578  .words, only_tex
+000058b0: 743d 6f6e 6c79 5f74 6578 742c 2069 6e63  t=only_text, inc
+000058c0: 6c75 6465 5f73 696e 676c 653d 696e 636c  lude_single=incl
+000058d0: 7564 655f 7369 6e67 6c65 290d 0a0d 0a20  ude_single).... 
+000058e0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+000058f0: 2020 6465 6620 6c65 6674 5f6c 6f63 6b65    def left_locke
+00005900: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
+00005910: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
+00005920: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+00005930: 2020 7265 7475 726e 2073 656c 662e 776f    return self.wo
+00005940: 7264 735b 305d 2e6c 6566 745f 6c6f 636b  rds[0].left_lock
+00005950: 6564 0d0a 2020 2020 2020 2020 7265 7475  ed..        retu
+00005960: 726e 2046 616c 7365 0d0a 0d0a 2020 2020  rn False....    
+00005970: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00005980: 6566 2072 6967 6874 5f6c 6f63 6b65 6428  ef right_locked(
+00005990: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000059a0: 6966 2073 656c 662e 6861 735f 776f 7264  if self.has_word
+000059b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000059c0: 7265 7475 726e 2073 656c 662e 776f 7264  return self.word
+000059d0: 735b 2d31 5d2e 7269 6768 745f 6c6f 636b  s[-1].right_lock
+000059e0: 6564 0d0a 2020 2020 2020 2020 7265 7475  ed..        retu
+000059f0: 726e 2046 616c 7365 0d0a 0d0a 2020 2020  rn False....    
+00005a00: 6465 6620 6c6f 636b 5f6c 6566 7428 7365  def lock_left(se
+00005a10: 6c66 293a 0d0a 2020 2020 2020 2020 6966  lf):..        if
+00005a20: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
+00005a30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005a40: 6c66 2e77 6f72 6473 5b30 5d2e 6c6f 636b  lf.words[0].lock
+00005a50: 5f6c 6566 7428 290d 0a0d 0a20 2020 2064  _left()....    d
+00005a60: 6566 206c 6f63 6b5f 7269 6768 7428 7365  ef lock_right(se
+00005a70: 6c66 293a 0d0a 2020 2020 2020 2020 6966  lf):..        if
+00005a80: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
+00005a90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005aa0: 6c66 2e77 6f72 6473 5b2d 315d 2e6c 6f63  lf.words[-1].loc
+00005ab0: 6b5f 7269 6768 7428 290d 0a0d 0a20 2020  k_right()....   
+00005ac0: 2064 6566 206c 6f63 6b5f 626f 7468 2873   def lock_both(s
+00005ad0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00005ae0: 656c 662e 6c6f 636b 5f6c 6566 7428 290d  elf.lock_left().
+00005af0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+00005b00: 636b 5f72 6967 6874 2829 0d0a 0d0a 2020  ck_right()....  
+00005b10: 2020 6465 6620 756e 6c6f 636b 5f61 6c6c    def unlock_all
+00005b20: 5f77 6f72 6473 2873 656c 6629 3a0d 0a20  _words(self):.. 
+00005b30: 2020 2020 2020 2073 656c 662e 5f77 6f72         self._wor
+00005b40: 645f 6f70 6572 6174 696f 6e73 2827 756e  d_operations('un
+00005b50: 6c6f 636b 5f62 6f74 6827 290d 0a0d 0a20  lock_both').... 
+00005b60: 2020 2064 6566 2072 6561 7373 6967 6e5f     def reassign_
+00005b70: 6964 7328 7365 6c66 2c20 7374 6172 743a  ids(self, start:
+00005b80: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00005b90: 204e 6f6e 6529 3a0d 0a20 2020 2020 2020   None):..       
+00005ba0: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
+00005bb0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00005bc0: 2066 6f72 2069 2c20 776f 7264 2069 6e20   for i, word in 
+00005bd0: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
+00005be0: 6f72 6473 5b73 7461 7274 3a5d 2c20 7374  ords[start:], st
+00005bf0: 6172 7420 6f72 2030 293a 0d0a 2020 2020  art or 0):..    
+00005c00: 2020 2020 2020 2020 2020 2020 776f 7264              word
+00005c10: 2e73 6567 6d65 6e74 203d 2073 656c 660d  .segment = self.
+00005c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c30: 2077 6f72 642e 6964 203d 2069 0d0a 0d0a   word.id = i....
+00005c40: 2020 2020 6465 6620 7570 6461 7465 5f73      def update_s
+00005c50: 6567 5f77 6974 685f 776f 7264 7328 7365  eg_with_words(se
+00005c60: 6c66 293a 0d0a 2020 2020 2020 2020 7761  lf):..        wa
+00005c70: 726e 696e 6773 2e77 6172 6e28 2741 7474  rnings.warn('Att
+00005c80: 7269 6275 7465 7320 7468 6174 2072 6571  ributes that req
+00005c90: 7569 7265 6420 7570 6461 7469 6e67 2061  uired updating a
+00005ca0: 7265 206e 6f77 2070 726f 7065 7274 6965  re now propertie
+00005cb0: 7320 6261 7365 6420 6f6e 2074 6865 2060  s based on the `
+00005cc0: 6077 6f72 6473 6060 2065 7863 6570 7420  `words`` except 
+00005cd0: 666f 7220 6060 6964 6060 2e20 270d 0a20  for ``id``. '.. 
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 2020 2027 6060 7570 6461 7465 5f73       '``update_s
+00005d00: 6567 5f77 6974 685f 776f 7264 7328 2960  eg_with_words()`
+00005d10: 6020 6973 2064 6570 7265 6361 7465 6420  ` is deprecated 
+00005d20: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
+00005d30: 7665 6420 696e 2066 7574 7572 6520 7665  ved in future ve
+00005d40: 7273 696f 6e73 2e20 270d 0a20 2020 2020  rsions. '..     
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2027 5573 6520 6060 2e72 6561 7373 6967   'Use ``.reassig
+00005d70: 6e5f 6964 7328 2960 6020 746f 206d 616e  n_ids()`` to man
+00005d80: 7561 6c6c 7920 7570 6461 7465 2069 6473  ually update ids
+00005d90: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005da0: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
+00005db0: 6576 656c 3d32 290d 0a20 2020 2020 2020  evel=2)..       
+00005dc0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
+00005dd0: 6473 2829 0d0a 0d0a 2020 2020 6465 6620  ds()....    def 
+00005de0: 7375 7070 7265 7373 5f73 696c 656e 6365  suppress_silence
+00005df0: 2873 656c 662c 0d0a 2020 2020 2020 2020  (self,..        
+00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 2073 696c 656e 745f 7374 6172 7473 3a20   silent_starts: 
+00005e20: 6e70 2e6e 6461 7272 6179 2c0d 0a20 2020  np.ndarray,..   
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 2020 7369 6c65 6e74 5f65 6e64        silent_end
+00005e50: 733a 206e 702e 6e64 6172 7261 792c 0d0a  s: np.ndarray,..
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2020 2020 2020 2020 206d 696e 5f77 6f72           min_wor
+00005e80: 645f 6475 723a 204f 7074 696f 6e61 6c5b  d_dur: Optional[
+00005e90: 666c 6f61 745d 203d 204e 6f6e 652c 0d0a  float] = None,..
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 2020 2020 2077 6f72 645f 6c65           word_le
+00005ec0: 7665 6c3a 2062 6f6f 6c20 3d20 5472 7565  vel: bool = True
+00005ed0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005ee0: 2020 2020 2020 2020 2020 2020 6e6f 6e73              nons
+00005ef0: 7065 6563 685f 6572 726f 723a 2066 6c6f  peech_error: flo
+00005f00: 6174 203d 2030 2e33 2c0d 0a20 2020 2020  at = 0.3,..     
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 7573 655f 776f 7264 5f70 6f73      use_word_pos
+00005f30: 6974 696f 6e3a 2062 6f6f 6c20 3d20 5472  ition: bool = Tr
+00005f40: 7565 293a 0d0a 2020 2020 2020 2020 6d69  ue):..        mi
+00005f50: 6e5f 776f 7264 5f64 7572 203d 2067 6574  n_word_dur = get
+00005f60: 5f6d 696e 5f77 6f72 645f 6475 7228 6d69  _min_word_dur(mi
+00005f70: 6e5f 776f 7264 5f64 7572 290d 0a20 2020  n_word_dur)..   
+00005f80: 2020 2020 2069 6620 7365 6c66 2e68 6173       if self.has
+00005f90: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
+00005fa0: 2020 2020 2065 6e64 696e 675f 7075 6e63       ending_punc
+00005fb0: 7475 6174 696f 6e73 203d 2067 6574 5f61  tuations = get_a
+00005fc0: 7070 656e 645f 7075 6e63 7475 6174 696f  ppend_punctuatio
+00005fd0: 6e73 2829 0d0a 2020 2020 2020 2020 2020  ns()..          
+00005fe0: 2020 776f 7264 7320 3d20 7365 6c66 2e77    words = self.w
+00005ff0: 6f72 6473 2069 6620 776f 7264 5f6c 6576  ords if word_lev
+00006000: 656c 206f 7220 6c65 6e28 7365 6c66 2e77  el or len(self.w
+00006010: 6f72 6473 2920 3d3d 2031 2065 6c73 6520  ords) == 1 else 
+00006020: 5b73 656c 662e 776f 7264 735b 305d 2c20  [self.words[0], 
+00006030: 7365 6c66 2e77 6f72 6473 5b2d 315d 5d0d  self.words[-1]].
+00006040: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00006050: 2069 2c20 7720 696e 2065 6e75 6d65 7261   i, w in enumera
+00006060: 7465 2877 6f72 6473 2c20 3129 3a0d 0a20  te(words, 1):.. 
+00006070: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006080: 6620 7573 655f 776f 7264 5f70 6f73 6974  f use_word_posit
+00006090: 696f 6e3a 0d0a 2020 2020 2020 2020 2020  ion:..          
+000060a0: 2020 2020 2020 2020 2020 6b65 6570 5f65            keep_e
+000060b0: 6e64 203d 206e 6f74 2028 772e 776f 7264  nd = not (w.word
+000060c0: 5b2d 315d 2069 6e20 656e 6469 6e67 5f70  [-1] in ending_p
+000060d0: 756e 6374 7561 7469 6f6e 7320 6f72 2069  unctuations or i
+000060e0: 203d 3d20 6c65 6e28 776f 7264 7329 290d   == len(words)).
+000060f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006100: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00006110: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
+00006120: 5f65 6e64 203d 204e 6f6e 650d 0a20 2020  _end = None..   
+00006130: 2020 2020 2020 2020 2020 2020 2077 2e73               w.s
+00006140: 7570 7072 6573 735f 7369 6c65 6e63 6528  uppress_silence(
+00006150: 7369 6c65 6e74 5f73 7461 7274 732c 2073  silent_starts, s
+00006160: 696c 656e 745f 656e 6473 2c20 6d69 6e5f  ilent_ends, min_
+00006170: 776f 7264 5f64 7572 2c20 6e6f 6e73 7065  word_dur, nonspe
+00006180: 6563 685f 6572 726f 722c 206b 6565 705f  ech_error, keep_
+00006190: 656e 6429 0d0a 2020 2020 2020 2020 656c  end)..        el
+000061a0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000061b0: 2073 7570 7072 6573 735f 7369 6c65 6e63   suppress_silenc
+000061c0: 6528 7365 6c66 2c0d 0a20 2020 2020 2020  e(self,..       
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 2020 2020 2020 7369 6c65 6e74 5f73 7461        silent_sta
+000061f0: 7274 732c 0d0a 2020 2020 2020 2020 2020  rts,..          
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2073 696c 656e 745f 656e 6473 2c0d     silent_ends,.
+00006220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006230: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00006240: 6e5f 776f 7264 5f64 7572 2c0d 0a20 2020  n_word_dur,..   
+00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006260: 2020 2020 2020 2020 2020 6e6f 6e73 7065            nonspe
+00006270: 6563 685f 6572 726f 7229 0d0a 0d0a 2020  ech_error)....  
+00006280: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00006290: 660d 0a0d 0a20 2020 2064 6566 2067 6574  f....    def get
+000062a0: 5f6c 6f63 6b65 645f 696e 6469 6365 7328  _locked_indices(
+000062b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000062c0: 6c6f 636b 6564 5f69 6e64 6963 6573 203d  locked_indices =
+000062d0: 205b 690d 0a20 2020 2020 2020 2020 2020   [i..           
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000062f0: 6f72 2069 2c20 286c 6566 742c 2072 6967  or i, (left, rig
+00006300: 6874 2920 696e 2065 6e75 6d65 7261 7465  ht) in enumerate
+00006310: 287a 6970 2873 656c 662e 776f 7264 735b  (zip(self.words[
+00006320: 313a 5d2c 2073 656c 662e 776f 7264 735b  1:], self.words[
+00006330: 3a2d 315d 2929 0d0a 2020 2020 2020 2020  :-1]))..        
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 6966 206c 6566 742e 6c65 6674 5f6c    if left.left_l
+00006360: 6f63 6b65 6420 6f72 2072 6967 6874 2e72  ocked or right.r
+00006370: 6967 6874 5f6c 6f63 6b65 645d 0d0a 2020  ight_locked]..  
+00006380: 2020 2020 2020 7265 7475 726e 206c 6f63        return loc
+00006390: 6b65 645f 696e 6469 6365 730d 0a0d 0a20  ked_indices.... 
+000063a0: 2020 2064 6566 2067 6574 5f67 6170 7328     def get_gaps(
+000063b0: 7365 6c66 2c20 6173 5f6e 6461 7272 6179  self, as_ndarray
+000063c0: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+000063d0: 2020 6966 2073 656c 662e 6861 735f 776f    if self.has_wo
+000063e0: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+000063f0: 2020 735f 7473 203d 206e 702e 6172 7261    s_ts = np.arra
+00006400: 7928 5b77 2e73 7461 7274 2066 6f72 2077  y([w.start for w
+00006410: 2069 6e20 7365 6c66 2e77 6f72 6473 5d29   in self.words])
+00006420: 0d0a 2020 2020 2020 2020 2020 2020 655f  ..            e_
+00006430: 7473 203d 206e 702e 6172 7261 7928 5b77  ts = np.array([w
+00006440: 2e65 6e64 2066 6f72 2077 2069 6e20 7365  .end for w in se
+00006450: 6c66 2e77 6f72 6473 5d29 0d0a 2020 2020  lf.words])..    
+00006460: 2020 2020 2020 2020 6761 7020 3d20 735f          gap = s_
+00006470: 7473 5b31 3a5d 202d 2065 5f74 735b 3a2d  ts[1:] - e_ts[:-
+00006480: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
+00006490: 7265 7475 726e 2067 6170 2069 6620 6173  return gap if as
+000064a0: 5f6e 6461 7272 6179 2065 6c73 6520 6761  _ndarray else ga
+000064b0: 702e 746f 6c69 7374 2829 0d0a 2020 2020  p.tolist()..    
+000064c0: 2020 2020 7265 7475 726e 205b 5d0d 0a0d      return []...
+000064d0: 0a20 2020 2064 6566 2067 6574 5f67 6170  .    def get_gap
+000064e0: 5f69 6e64 6963 6573 2873 656c 662c 206d  _indices(self, m
+000064f0: 6178 5f67 6170 3a20 666c 6f61 7420 3d20  ax_gap: float = 
+00006500: 302e 3129 3a20 2023 2066 6f72 2073 706c  0.1):  # for spl
+00006510: 6974 7469 6e67 0d0a 2020 2020 2020 2020  itting..        
+00006520: 6966 206e 6f74 2073 656c 662e 6861 735f  if not self.has_
+00006530: 776f 7264 7320 6f72 206c 656e 2873 656c  words or len(sel
+00006540: 662e 776f 7264 7329 203c 2032 3a0d 0a20  f.words) < 2:.. 
+00006550: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006560: 6e20 5b5d 0d0a 2020 2020 2020 2020 6966  n []..        if
+00006570: 206d 6178 5f67 6170 2069 7320 4e6f 6e65   max_gap is None
+00006580: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
+00006590: 6178 5f67 6170 203d 2030 0d0a 2020 2020  ax_gap = 0..    
+000065a0: 2020 2020 696e 6469 6365 7320 3d20 2873      indices = (s
+000065b0: 656c 662e 6765 745f 6761 7073 2854 7275  elf.get_gaps(Tru
+000065c0: 6529 203e 206d 6178 5f67 6170 292e 6e6f  e) > max_gap).no
+000065d0: 6e7a 6572 6f28 295b 305d 2e74 6f6c 6973  nzero()[0].tolis
+000065e0: 7428 290d 0a20 2020 2020 2020 2072 6574  t()..        ret
+000065f0: 7572 6e20 736f 7274 6564 2873 6574 2869  urn sorted(set(i
+00006600: 6e64 6963 6573 2920 2d20 7365 7428 7365  ndices) - set(se
+00006610: 6c66 2e67 6574 5f6c 6f63 6b65 645f 696e  lf.get_locked_in
+00006620: 6469 6365 7328 2929 290d 0a0d 0a20 2020  dices()))....   
+00006630: 2064 6566 2067 6574 5f70 756e 6374 7561   def get_punctua
+00006640: 7469 6f6e 5f69 6e64 6963 6573 2873 656c  tion_indices(sel
+00006650: 662c 2070 756e 6374 7561 7469 6f6e 3a20  f, punctuation: 
+00006660: 556e 696f 6e5b 4c69 7374 5b73 7472 5d2c  Union[List[str],
+00006670: 204c 6973 745b 5475 706c 655b 7374 722c   List[Tuple[str,
+00006680: 2073 7472 5d5d 2c20 7374 725d 293a 2020   str]], str]):  
+00006690: 2320 666f 7220 7370 6c69 7474 696e 670d  # for splitting.
+000066a0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000066b0: 7365 6c66 2e68 6173 5f77 6f72 6473 206f  self.has_words o
+000066c0: 7220 6c65 6e28 7365 6c66 2e77 6f72 6473  r len(self.words
+000066d0: 2920 3c20 323a 0d0a 2020 2020 2020 2020  ) < 2:..        
+000066e0: 2020 2020 7265 7475 726e 205b 5d0d 0a20      return [].. 
+000066f0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00006700: 616e 6365 2870 756e 6374 7561 7469 6f6e  ance(punctuation
+00006710: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
+00006720: 2020 2020 2070 756e 6374 7561 7469 6f6e       punctuation
+00006730: 203d 205b 7075 6e63 7475 6174 696f 6e5d   = [punctuation]
+00006740: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
+00006750: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00006760: 666f 7220 7020 696e 2070 756e 6374 7561  for p in punctua
+00006770: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
+00006780: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00006790: 2870 2c20 7374 7229 3a0d 0a20 2020 2020  (p, str):..     
+000067a0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000067b0: 2c20 7320 696e 2065 6e75 6d65 7261 7465  , s in enumerate
+000067c0: 2873 656c 662e 776f 7264 735b 3a2d 315d  (self.words[:-1]
+000067d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000067e0: 2020 2020 2020 2020 6966 2073 2e77 6f72          if s.wor
+000067f0: 642e 656e 6473 7769 7468 2870 293a 0d0a  d.endswith(p):..
+00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006810: 2020 2020 2020 2020 696e 6469 6365 732e          indices.
+00006820: 6170 7065 6e64 2869 290d 0a20 2020 2020  append(i)..     
+00006830: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00006840: 6c69 6620 6920 213d 2030 2061 6e64 2073  lif i != 0 and s
+00006850: 2e77 6f72 642e 7374 6172 7473 7769 7468  .word.startswith
+00006860: 2870 293a 0d0a 2020 2020 2020 2020 2020  (p):..          
+00006870: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00006880: 6469 6365 732e 6170 7065 6e64 2869 2d31  dices.append(i-1
+00006890: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000068a0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000068b0: 2020 2020 2020 656e 6469 6e67 2c20 6265        ending, be
+000068c0: 6769 6e6e 696e 6720 3d20 700d 0a20 2020  ginning = p..   
+000068d0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+000068e0: 6963 6573 2e65 7874 656e 6428 5b69 2066  ices.extend([i f
+000068f0: 6f72 2069 2c20 2877 302c 2077 3129 2069  or i, (w0, w1) i
+00006900: 6e20 656e 756d 6572 6174 6528 7a69 7028  n enumerate(zip(
+00006910: 7365 6c66 2e77 6f72 6473 5b3a 2d31 5d2c  self.words[:-1],
+00006920: 2073 656c 662e 776f 7264 735b 313a 5d29   self.words[1:])
+00006930: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2069 6620 7730 2e77 6f72 642e 656e     if w0.word.en
+00006960: 6473 7769 7468 2865 6e64 696e 6729 2061  dswith(ending) a
+00006970: 6e64 2077 312e 776f 7264 2e73 7461 7274  nd w1.word.start
+00006980: 7377 6974 6828 6265 6769 6e6e 696e 6729  swith(beginning)
+00006990: 5d29 0d0a 0d0a 2020 2020 2020 2020 7265  ])....        re
+000069a0: 7475 726e 2073 6f72 7465 6428 7365 7428  turn sorted(set(
+000069b0: 696e 6469 6365 7329 202d 2073 6574 2873  indices) - set(s
+000069c0: 656c 662e 6765 745f 6c6f 636b 6564 5f69  elf.get_locked_i
+000069d0: 6e64 6963 6573 2829 2929 0d0a 0d0a 2020  ndices()))....  
+000069e0: 2020 6465 6620 6765 745f 6c65 6e67 7468    def get_length
+000069f0: 5f69 6e64 6963 6573 2873 656c 662c 206d  _indices(self, m
+00006a00: 6178 5f63 6861 7273 3a20 696e 7420 3d20  ax_chars: int = 
+00006a10: 4e6f 6e65 2c20 6d61 785f 776f 7264 733a  None, max_words:
+00006a20: 2069 6e74 203d 204e 6f6e 652c 2065 7665   int = None, eve
+00006a30: 6e5f 7370 6c69 743a 2062 6f6f 6c20 3d20  n_split: bool = 
+00006a40: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 696e 636c 7564 655f 6c6f 636b 3a20    include_lock: 
+00006a70: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
+00006a80: 2020 2020 2020 2020 2320 666f 7220 7370          # for sp
+00006a90: 6c69 7474 696e 670d 0a20 2020 2020 2020  litting..       
+00006aa0: 2069 6620 6e6f 7420 7365 6c66 2e68 6173   if not self.has
+00006ab0: 5f77 6f72 6473 206f 7220 286d 6178 5f63  _words or (max_c
+00006ac0: 6861 7273 2069 7320 4e6f 6e65 2061 6e64  hars is None and
+00006ad0: 206d 6178 5f77 6f72 6473 2069 7320 4e6f   max_words is No
+00006ae0: 6e65 293a 0d0a 2020 2020 2020 2020 2020  ne):..          
+00006af0: 2020 7265 7475 726e 205b 5d0d 0a20 2020    return []..   
+00006b00: 2020 2020 2061 7373 6572 7420 6d61 785f       assert max_
+00006b10: 6368 6172 7320 213d 2030 2061 6e64 206d  chars != 0 and m
+00006b20: 6178 5f77 6f72 6473 2021 3d20 302c 205c  ax_words != 0, \
+00006b30: 0d0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+00006b40: 6d61 785f 6368 6172 7320 616e 6420 6d61  max_chars and ma
+00006b50: 785f 776f 7264 7320 6d75 7374 2062 6520  x_words must be 
+00006b60: 6772 6561 7465 7220 302c 2062 7574 2067  greater 0, but g
+00006b70: 6f74 207b 6d61 785f 6368 6172 737d 2061  ot {max_chars} a
+00006b80: 6e64 207b 6d61 785f 776f 7264 737d 270d  nd {max_words}'.
+00006b90: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00006ba0: 7365 6c66 2e77 6f72 6473 2920 3c20 323a  self.words) < 2:
+00006bb0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006bc0: 7475 726e 205b 5d0d 0a20 2020 2020 2020  turn []..       
+00006bd0: 2069 6e64 6963 6573 203d 205b 5d0d 0a20   indices = [].. 
+00006be0: 2020 2020 2020 2069 6620 6576 656e 5f73         if even_s
+00006bf0: 706c 6974 3a0d 0a20 2020 2020 2020 2020  plit:..         
+00006c00: 2020 2063 6861 725f 636f 756e 7420 3d20     char_count = 
+00006c10: 2d31 2069 6620 6d61 785f 6368 6172 7320  -1 if max_chars 
+00006c20: 6973 204e 6f6e 6520 656c 7365 2073 756d  is None else sum
+00006c30: 286d 6170 286c 656e 2c20 7365 6c66 2e77  (map(len, self.w
+00006c40: 6f72 6473 2929 0d0a 2020 2020 2020 2020  ords))..        
+00006c50: 2020 2020 776f 7264 5f63 6f75 6e74 203d      word_count =
+00006c60: 202d 3120 6966 206d 6178 5f77 6f72 6473   -1 if max_words
+00006c70: 2069 7320 4e6f 6e65 2065 6c73 6520 6c65   is None else le
+00006c80: 6e28 7365 6c66 2e77 6f72 6473 290d 0a20  n(self.words).. 
+00006c90: 2020 2020 2020 2020 2020 2065 7863 6565             excee
+00006ca0: 645f 6368 6172 7320 3d20 6d61 785f 6368  d_chars = max_ch
+00006cb0: 6172 7320 6973 206e 6f74 204e 6f6e 6520  ars is not None 
+00006cc0: 616e 6420 6368 6172 5f63 6f75 6e74 203e  and char_count >
+00006cd0: 206d 6178 5f63 6861 7273 0d0a 2020 2020   max_chars..    
+00006ce0: 2020 2020 2020 2020 6578 6365 6564 5f77          exceed_w
+00006cf0: 6f72 6473 203d 206d 6178 5f77 6f72 6473  ords = max_words
+00006d00: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00006d10: 2077 6f72 645f 636f 756e 7420 3e20 6d61   word_count > ma
+00006d20: 785f 776f 7264 730d 0a20 2020 2020 2020  x_words..       
+00006d30: 2020 2020 2069 6620 6578 6365 6564 5f63       if exceed_c
+00006d40: 6861 7273 3a0d 0a20 2020 2020 2020 2020  hars:..         
+00006d50: 2020 2020 2020 2073 706c 6974 7320 3d20         splits = 
+00006d60: 6e70 2e63 6569 6c28 6368 6172 5f63 6f75  np.ceil(char_cou
+00006d70: 6e74 202f 206d 6178 5f63 6861 7273 290d  nt / max_chars).
+00006d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d90: 2063 6861 7273 5f70 6572 5f73 706c 6974   chars_per_split
+00006da0: 203d 2063 6861 725f 636f 756e 7420 2f20   = char_count / 
+00006db0: 7370 6c69 7473 0d0a 2020 2020 2020 2020  splits..        
+00006dc0: 2020 2020 2020 2020 6375 6d5f 6368 6172          cum_char
+00006dd0: 5f63 6f75 6e74 203d 206e 702e 6375 6d73  _count = np.cums
+00006de0: 756d 285b 6c65 6e28 772e 776f 7264 2920  um([len(w.word) 
+00006df0: 666f 7220 7720 696e 2073 656c 662e 776f  for w in self.wo
+00006e00: 7264 735b 3a2d 315d 5d29 0d0a 2020 2020  rds[:-1]])..    
+00006e10: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+00006e20: 6365 7320 3d20 5b0d 0a20 2020 2020 2020  ces = [..       
+00006e30: 2020 2020 2020 2020 2020 2020 2028 6e70               (np
+00006e40: 2e61 6273 2863 756d 5f63 6861 725f 636f  .abs(cum_char_co
+00006e50: 756e 742d 2869 2a63 6861 7273 5f70 6572  unt-(i*chars_per
+00006e60: 5f73 706c 6974 2929 292e 6172 676d 696e  _split))).argmin
+00006e70: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00006e80: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00006e90: 2072 616e 6765 2831 2c20 696e 7428 7370   range(1, int(sp
+00006ea0: 6c69 7473 2929 0d0a 2020 2020 2020 2020  lits))..        
+00006eb0: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+00006ec0: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
+00006ed0: 785f 776f 7264 7320 6973 206e 6f74 204e  x_words is not N
+00006ee0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00006ef0: 2020 2020 2020 2020 2020 6578 6365 6564            exceed
+00006f00: 5f77 6f72 6473 203d 2061 6e79 286a 2d69  _words = any(j-i
+00006f10: 2b31 203e 206d 6178 5f77 6f72 6473 2066  +1 > max_words f
+00006f20: 6f72 2069 2c20 6a20 696e 207a 6970 285b  or i, j in zip([
+00006f30: 305d 2b69 6e64 6963 6573 2c20 696e 6469  0]+indices, indi
+00006f40: 6365 732b 5b6c 656e 2873 656c 662e 776f  ces+[len(self.wo
+00006f50: 7264 7329 5d29 290d 0a0d 0a20 2020 2020  rds)]))....     
+00006f60: 2020 2020 2020 2069 6620 6578 6365 6564         if exceed
+00006f70: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
+00006f80: 2020 2020 2020 2020 2073 706c 6974 7320           splits 
+00006f90: 3d20 6e70 2e63 6569 6c28 776f 7264 5f63  = np.ceil(word_c
+00006fa0: 6f75 6e74 202f 206d 6178 5f77 6f72 6473  ount / max_words
+00006fb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006fc0: 2020 2077 6f72 6473 5f70 6572 5f73 706c     words_per_spl
+00006fd0: 6974 203d 2077 6f72 645f 636f 756e 7420  it = word_count 
+00006fe0: 2f20 7370 6c69 7473 0d0a 2020 2020 2020  / splits..      
+00006ff0: 2020 2020 2020 2020 2020 6375 6d5f 776f            cum_wo
+00007000: 7264 5f63 6f75 6e74 203d 206e 702e 6172  rd_count = np.ar
+00007010: 7261 7928 7261 6e67 6528 312c 206c 656e  ray(range(1, len
+00007020: 2873 656c 662e 776f 7264 7329 2b31 2929  (self.words)+1))
+00007030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007040: 2020 696e 6469 6365 7320 3d20 5b0d 0a20    indices = [.. 
+00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007060: 2020 206e 702e 6162 7328 6375 6d5f 776f     np.abs(cum_wo
+00007070: 7264 5f63 6f75 6e74 2d28 692a 776f 7264  rd_count-(i*word
+00007080: 735f 7065 725f 7370 6c69 7429 292e 6172  s_per_split)).ar
+00007090: 676d 696e 2829 0d0a 2020 2020 2020 2020  gmin()..        
+000070a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000070b0: 6920 696e 2072 616e 6765 2831 2c20 696e  i in range(1, in
+000070c0: 7428 7370 6c69 7473 2929 0d0a 2020 2020  t(splits))..    
+000070d0: 2020 2020 2020 2020 2020 2020 5d0d 0a0d              ]...
+000070e0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+000070f0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00007100: 5f77 6f72 6473 203d 2030 0d0a 2020 2020  _words = 0..    
+00007110: 2020 2020 2020 2020 6375 7272 5f63 6861          curr_cha
+00007120: 7273 203d 2030 0d0a 2020 2020 2020 2020  rs = 0..        
+00007130: 2020 2020 6c6f 636b 6564 5f69 6e64 6963      locked_indic
+00007140: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00007150: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
+00007160: 6c6f 636b 3a0d 0a20 2020 2020 2020 2020  lock:..         
+00007170: 2020 2020 2020 206c 6f63 6b65 645f 696e         locked_in
+00007180: 6469 6365 7320 3d20 7365 6c66 2e67 6574  dices = self.get
+00007190: 5f6c 6f63 6b65 645f 696e 6469 6365 7328  _locked_indices(
+000071a0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+000071b0: 6f72 2069 2c20 776f 7264 2069 6e20 656e  or i, word in en
+000071c0: 756d 6572 6174 6528 7365 6c66 2e77 6f72  umerate(self.wor
+000071d0: 6473 293a 0d0a 2020 2020 2020 2020 2020  ds):..          
+000071e0: 2020 2020 2020 6375 7272 5f77 6f72 6473        curr_words
+000071f0: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
+00007200: 2020 2020 2020 2063 7572 725f 6368 6172         curr_char
+00007210: 7320 2b3d 206c 656e 2877 6f72 6429 0d0a  s += len(word)..
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 6966 2069 2021 3d20 303a 0d0a 2020 2020  if i != 0:..    
+00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007250: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 6d61 785f 6368 6172 7320 6973 206e    max_chars is n
+00007280: 6f74 204e 6f6e 6520 616e 6420 6375 7272  ot None and curr
+00007290: 5f63 6861 7273 203e 206d 6178 5f63 6861  _chars > max_cha
+000072a0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 6d61 785f 776f 7264 7320 6973 206e 6f74  max_words is not
+000072f0: 204e 6f6e 6520 616e 6420 6375 7272 5f77   None and curr_w
+00007300: 6f72 6473 203e 206d 6178 5f77 6f72 6473  ords > max_words
+00007310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007320: 2020 2020 2020 2920 616e 6420 692d 3120        ) and i-1 
+00007330: 6e6f 7420 696e 206c 6f63 6b65 645f 696e  not in locked_in
+00007340: 6469 6365 733a 0d0a 2020 2020 2020 2020  dices:..        
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 696e 6469 6365 732e 6170 7065 6e64 2869  indices.append(i
+00007370: 2d31 290d 0a20 2020 2020 2020 2020 2020  -1)..           
+00007380: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00007390: 725f 776f 7264 7320 3d20 310d 0a20 2020  r_words = 1..   
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 2020 2020 2063 7572 725f 6368 6172 7320       curr_chars 
+000073c0: 3d20 6c65 6e28 776f 7264 290d 0a20 2020  = len(word)..   
+000073d0: 2020 2020 2072 6574 7572 6e20 696e 6469       return indi
+000073e0: 6365 730d 0a0d 0a20 2020 2064 6566 2067  ces....    def g
+000073f0: 6574 5f64 7572 6174 696f 6e5f 696e 6469  et_duration_indi
+00007400: 6365 7328 7365 6c66 2c20 6d61 785f 6475  ces(self, max_du
+00007410: 723a 2066 6c6f 6174 2c20 6576 656e 5f73  r: float, even_s
+00007420: 706c 6974 3a20 626f 6f6c 203d 2054 7275  plit: bool = Tru
+00007430: 652c 2069 6e63 6c75 6465 5f6c 6f63 6b3a  e, include_lock:
+00007440: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
+00007450: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007460: 7365 6c66 2e68 6173 5f77 6f72 6473 206f  self.has_words o
+00007470: 7220 2874 6f74 616c 5f64 7572 6174 696f  r (total_duratio
+00007480: 6e20 3a3d 206e 702e 7375 6d28 5b77 2e64  n := np.sum([w.d
+00007490: 7572 6174 696f 6e20 666f 7220 7720 696e  uration for w in
+000074a0: 2073 656c 662e 776f 7264 735d 2929 203c   self.words])) <
+000074b0: 3d20 6d61 785f 6475 723a 0d0a 2020 2020  = max_dur:..    
+000074c0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+000074d0: 5d0d 0a20 2020 2020 2020 2069 6620 6576  ]..        if ev
+000074e0: 656e 5f73 706c 6974 3a0d 0a20 2020 2020  en_split:..     
+000074f0: 2020 2020 2020 2073 706c 6974 7320 3d20         splits = 
+00007500: 6e70 2e63 6569 6c28 746f 7461 6c5f 6475  np.ceil(total_du
+00007510: 7261 7469 6f6e 202f 206d 6178 5f64 7572  ration / max_dur
+00007520: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00007530: 7572 5f70 6572 5f73 706c 6974 203d 2074  ur_per_split = t
+00007540: 6f74 616c 5f64 7572 6174 696f 6e20 2f20  otal_duration / 
+00007550: 7370 6c69 7473 0d0a 2020 2020 2020 2020  splits..        
+00007560: 2020 2020 6375 6d5f 6475 7220 3d20 6e70      cum_dur = np
+00007570: 2e63 756d 7375 6d28 5b77 2e64 7572 6174  .cumsum([w.durat
+00007580: 696f 6e20 666f 7220 7720 696e 2073 656c  ion for w in sel
+00007590: 662e 776f 7264 735b 3a2d 315d 5d29 0d0a  f.words[:-1]])..
+000075a0: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+000075b0: 6365 7320 3d20 5b0d 0a20 2020 2020 2020  ces = [..       
+000075c0: 2020 2020 2020 2020 2028 6e70 2e61 6273           (np.abs
+000075d0: 2863 756d 5f64 7572 202d 2028 6920 2a20  (cum_dur - (i * 
+000075e0: 6475 725f 7065 725f 7370 6c69 7429 2929  dur_per_split)))
+000075f0: 2e61 7267 6d69 6e28 290d 0a20 2020 2020  .argmin()..     
+00007600: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00007610: 2069 6e20 7261 6e67 6528 312c 2069 6e74   in range(1, int
+00007620: 2873 706c 6974 7329 290d 0a20 2020 2020  (splits))..     
+00007630: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00007640: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00007650: 2020 2020 2069 6e64 6963 6573 203d 205b       indices = [
+00007660: 5d0d 0a20 2020 2020 2020 2020 2020 2063  ]..            c
+00007670: 7572 725f 746f 7461 6c5f 6475 7220 3d20  urr_total_dur = 
+00007680: 302e 300d 0a20 2020 2020 2020 2020 2020  0.0..           
+00007690: 206c 6f63 6b65 645f 696e 6469 6365 7320   locked_indices 
+000076a0: 3d20 7365 6c66 2e67 6574 5f6c 6f63 6b65  = self.get_locke
+000076b0: 645f 696e 6469 6365 7328 2920 6966 2069  d_indices() if i
+000076c0: 6e63 6c75 6465 5f6c 6f63 6b20 656c 7365  nclude_lock else
+000076d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000076e0: 2066 6f72 2069 2c20 776f 7264 2069 6e20   for i, word in 
+000076f0: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
+00007700: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
+00007710: 2020 2020 2020 2020 6375 7272 5f74 6f74          curr_tot
+00007720: 616c 5f64 7572 202b 3d20 776f 7264 2e64  al_dur += word.d
+00007730: 7572 6174 696f 6e0d 0a20 2020 2020 2020  uration..       
+00007740: 2020 2020 2020 2020 2069 6620 6920 213d           if i !=
+00007750: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00007760: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+00007770: 5f74 6f74 616c 5f64 7572 203e 206d 6178  _total_dur > max
+00007780: 5f64 7572 2061 6e64 2069 202d 2031 206e  _dur and i - 1 n
+00007790: 6f74 2069 6e20 6c6f 636b 6564 5f69 6e64  ot in locked_ind
+000077a0: 6963 6573 3a0d 0a20 2020 2020 2020 2020  ices:..         
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000077c0: 6e64 6963 6573 2e61 7070 656e 6428 6920  ndices.append(i 
+000077d0: 2d20 3129 0d0a 2020 2020 2020 2020 2020  - 1)..          
+000077e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000077f0: 7272 5f74 6f74 616c 5f64 7572 203d 2077  rr_total_dur = w
+00007800: 6f72 642e 6475 7261 7469 6f6e 0d0a 2020  ord.duration..  
+00007810: 2020 2020 2020 7265 7475 726e 2069 6e64        return ind
+00007820: 6963 6573 0d0a 0d0a 2020 2020 6465 6620  ices....    def 
+00007830: 7370 6c69 7428 7365 6c66 2c20 696e 6469  split(self, indi
+00007840: 6365 733a 204c 6973 745b 696e 745d 293a  ces: List[int]):
+00007850: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00007860: 2869 6e64 6963 6573 2920 3d3d 2030 3a0d  (indices) == 0:.
+00007870: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007880: 7572 6e20 5b5d 0d0a 2020 2020 2020 2020  urn []..        
+00007890: 6966 2069 6e64 6963 6573 5b2d 315d 2021  if indices[-1] !
+000078a0: 3d20 6c65 6e28 7365 6c66 2e77 6f72 6473  = len(self.words
+000078b0: 2920 2d20 313a 0d0a 2020 2020 2020 2020  ) - 1:..        
+000078c0: 2020 2020 696e 6469 6365 732e 6170 7065      indices.appe
+000078d0: 6e64 286c 656e 2873 656c 662e 776f 7264  nd(len(self.word
+000078e0: 7329 202d 2031 290d 0a20 2020 2020 2020  s) - 1)..       
+000078f0: 2073 6567 5f63 6f70 6965 7320 3d20 5b5d   seg_copies = []
+00007900: 0d0a 2020 2020 2020 2020 7072 6576 5f69  ..        prev_i
+00007910: 203d 2030 0d0a 2020 2020 2020 2020 666f   = 0..        fo
+00007920: 7220 6920 696e 2069 6e64 6963 6573 3a0d  r i in indices:.
+00007930: 0a20 2020 2020 2020 2020 2020 2069 202b  .            i +
+00007940: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+00007950: 206e 6577 5f77 6f72 6473 203d 2073 656c   new_words = sel
+00007960: 662e 776f 7264 735b 7072 6576 5f69 3a69  f.words[prev_i:i
+00007970: 5d0d 0a20 2020 2020 2020 2020 2020 206e  ]..            n
+00007980: 6577 5f73 6567 203d 2073 656c 662e 636f  ew_seg = self.co
+00007990: 7079 286e 6577 5f77 6f72 6473 2c20 636f  py(new_words, co
+000079a0: 7079 5f77 6f72 6473 3d46 616c 7365 290d  py_words=False).
+000079b0: 0a20 2020 2020 2020 2020 2020 2073 6567  .            seg
+000079c0: 5f63 6f70 6965 732e 6170 7065 6e64 286e  _copies.append(n
+000079d0: 6577 5f73 6567 290d 0a20 2020 2020 2020  ew_seg)..       
+000079e0: 2020 2020 2070 7265 765f 6920 3d20 690d       prev_i = i.
+000079f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007a00: 7365 675f 636f 7069 6573 0d0a 0d0a 2020  seg_copies....  
+00007a10: 2020 6465 6620 7365 745f 7265 7375 6c74    def set_result
+00007a20: 2873 656c 662c 2072 6573 756c 743a 2027  (self, result: '
+00007a30: 5768 6973 7065 7252 6573 756c 7427 293a  WhisperResult'):
+00007a40: 0d0a 2020 2020 2020 2020 7761 726e 696e  ..        warnin
+00007a50: 6773 2e77 6172 6e28 2760 602e 7365 745f  gs.warn('``.set_
+00007a60: 7265 7375 6c74 2863 7572 7265 6e74 5f72  result(current_r
+00007a70: 6573 756c 745f 696e 7374 616e 6365 2960  esult_instance)`
+00007a80: 6020 6973 2064 6570 7265 6361 7465 6420  ` is deprecated 
+00007a90: 616e 6420 7769 6c6c 2062 6520 7265 6d6f  and will be remo
+00007aa0: 7665 6420 696e 2066 7574 7572 6520 7665  ved in future ve
+00007ab0: 7273 696f 6e73 2e20 270d 0a20 2020 2020  rsions. '..     
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 2027 5573 6520 6060 2e72 6573 756c 7420   'Use ``.result 
+00007ae0: 3d20 6375 7272 656e 745f 7265 7375 6c74  = current_result
+00007af0: 5f69 6e73 7461 6e63 6560 6020 696e 7374  _instance`` inst
+00007b00: 6561 642e 272c 0d0a 2020 2020 2020 2020  ead.',..        
+00007b10: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00007b20: 6163 6b6c 6576 656c 3d32 290d 0a20 2020  acklevel=2)..   
+00007b30: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+00007b40: 203d 2072 6573 756c 740d 0a0d 0a20 2020   = result....   
+00007b50: 2064 6566 2067 6574 5f72 6573 756c 7428   def get_result(
+00007b60: 7365 6c66 2920 2d3e 2055 6e69 6f6e 5b27  self) -> Union['
+00007b70: 5768 6973 7065 7252 6573 756c 7427 2c20  WhisperResult', 
+00007b80: 4e6f 6e65 5d3a 0d0a 2020 2020 2020 2020  None]:..        
+00007b90: 2222 220d 0a20 2020 2020 2020 2052 6574  """..        Ret
+00007ba0: 7572 6e20 6f75 7465 7220 696e 7374 616e  urn outer instan
+00007bb0: 6365 206f 6620 3a63 6c61 7373 3a60 7374  ce of :class:`st
+00007bc0: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+00007bd0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+00007be0: 7460 2074 6861 7420 6060 7365 6c66 6060  t` that ``self``
+00007bf0: 2069 7320 6120 7061 7274 206f 662e 0d0a   is a part of...
+00007c00: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00007c10: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00007c20: 726e 2827 6060 2e67 6574 5f72 6573 756c  rn('``.get_resul
+00007c30: 7428 2960 6020 7769 6c6c 2062 6520 7265  t()`` will be re
+00007c40: 6d6f 7665 6420 696e 2066 7574 7572 6520  moved in future 
+00007c50: 7665 7273 696f 6e73 2e20 5573 6520 6060  versions. Use ``
+00007c60: 2e72 6573 756c 7460 6020 696e 7374 6561  .result`` instea
+00007c70: 642e 272c 0d0a 2020 2020 2020 2020 2020  d.',..          
+00007c80: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+00007c90: 6b6c 6576 656c 3d32 290d 0a20 2020 2020  klevel=2)..     
+00007ca0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
+00007cb0: 6573 756c 740d 0a0d 0a0d 0a63 6c61 7373  esult......class
+00007cc0: 2057 6869 7370 6572 5265 7375 6c74 3a0d   WhisperResult:.
+00007cd0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+00007ce0: 745f 5f28 0d0a 2020 2020 2020 2020 2020  t__(..          
+00007cf0: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00007d00: 2020 2020 2072 6573 756c 743a 2055 6e69       result: Uni
+00007d10: 6f6e 5b73 7472 2c20 6469 6374 2c20 6c69  on[str, dict, li
+00007d20: 7374 5d2c 0d0a 2020 2020 2020 2020 2020  st],..          
+00007d30: 2020 666f 7263 655f 6f72 6465 723a 2062    force_order: b
+00007d40: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00007d50: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
+00007d60: 736f 7274 6564 3a20 556e 696f 6e5b 626f  sorted: Union[bo
+00007d70: 6f6c 2c20 7374 725d 203d 2054 7275 652c  ol, str] = True,
+00007d80: 0d0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
+00007d90: 6f77 5f75 6e73 6f72 7465 643a 2062 6f6f  ow_unsorted: boo
+00007da0: 6c20 3d20 5472 7565 0d0a 2020 2020 293a  l = True..    ):
+00007db0: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00007dc0: 2c20 7365 6c66 2e70 6174 6820 3d20 7365  , self.path = se
+00007dd0: 6c66 2e5f 7374 616e 6461 7264 697a 655f  lf._standardize_
+00007de0: 7265 7375 6c74 2872 6573 756c 7429 0d0a  result(result)..
+00007df0: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
+00007e00: 5f64 6963 7420 3d20 7265 7375 6c74 2e67  _dict = result.g
+00007e10: 6574 2827 6f72 695f 6469 6374 2729 206f  et('ori_dict') o
+00007e20: 7220 7265 7375 6c74 0d0a 2020 2020 2020  r result..      
+00007e30: 2020 7365 6c66 2e6c 616e 6775 6167 6520    self.language 
+00007e40: 3d20 7365 6c66 2e6f 7269 5f64 6963 742e  = self.ori_dict.
+00007e50: 6765 7428 276c 616e 6775 6167 6527 290d  get('language').
+00007e60: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00007e70: 6567 726f 7570 5f68 6973 746f 7279 203d  egroup_history =
+00007e80: 2072 6573 756c 742e 6765 7428 2772 6567   result.get('reg
+00007e90: 726f 7570 5f68 6973 746f 7279 272c 2027  roup_history', '
+00007ea0: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
+00007eb0: 2e5f 6e6f 6e73 7065 6563 685f 7365 6374  ._nonspeech_sect
+00007ec0: 696f 6e73 203d 2072 6573 756c 742e 6765  ions = result.ge
+00007ed0: 7428 276e 6f6e 7370 6565 6368 5f73 6563  t('nonspeech_sec
+00007ee0: 7469 6f6e 7327 2c20 5b5d 290d 0a20 2020  tions', [])..   
+00007ef0: 2020 2020 2073 6567 6d65 6e74 7320 3d20       segments = 
+00007f00: 2872 6573 756c 742e 6765 7428 2773 6567  (result.get('seg
+00007f10: 6d65 6e74 7327 2c20 7365 6c66 2e6f 7269  ments', self.ori
+00007f20: 5f64 6963 742e 6765 7428 2773 6567 6d65  _dict.get('segme
+00007f30: 6e74 7327 2929 206f 7220 7b7d 292e 636f  nts')) or {}).co
+00007f40: 7079 2829 0d0a 2020 2020 2020 2020 7365  py()..        se
+00007f50: 6c66 2e73 6567 6d65 6e74 7320 3d20 5b53  lf.segments = [S
+00007f60: 6567 6d65 6e74 282a 2a73 2c20 6967 6e6f  egment(**s, igno
+00007f70: 7265 5f75 6e75 7365 645f 6172 6773 3d54  re_unused_args=T
+00007f80: 7275 6529 2066 6f72 2073 2069 6e20 7365  rue) for s in se
+00007f90: 676d 656e 7473 5d20 6966 2073 6567 6d65  gments] if segme
+00007fa0: 6e74 7320 656c 7365 205b 5d0d 0a20 2020  nts else []..   
+00007fb0: 2020 2020 2073 656c 662e 5f66 6f72 6365       self._force
+00007fc0: 645f 6f72 6465 7220 3d20 666f 7263 655f  d_order = force_
+00007fd0: 6f72 6465 720d 0a20 2020 2020 2020 2069  order..        i
+00007fe0: 6620 7365 6c66 2e5f 666f 7263 6564 5f6f  f self._forced_o
+00007ff0: 7264 6572 3a0d 0a20 2020 2020 2020 2020  rder:..         
+00008000: 2020 2073 656c 662e 666f 7263 655f 6f72     self.force_or
+00008010: 6465 7228 290d 0a20 2020 2020 2020 2073  der()..        s
+00008020: 656c 662e 7261 6973 655f 666f 725f 756e  elf.raise_for_un
+00008030: 736f 7274 6564 2863 6865 636b 5f73 6f72  sorted(check_sor
+00008040: 7465 642c 2073 686f 775f 756e 736f 7274  ted, show_unsort
+00008050: 6564 290d 0a20 2020 2020 2020 2073 656c  ed)..        sel
+00008060: 662e 7265 6d6f 7665 5f6e 6f5f 776f 7264  f.remove_no_word
+00008070: 5f73 6567 6d65 6e74 7328 616e 7928 7365  _segments(any(se
+00008080: 672e 6861 735f 776f 7264 7320 666f 7220  g.has_words for 
+00008090: 7365 6720 696e 2073 656c 662e 7365 676d  seg in self.segm
+000080a0: 656e 7473 2929 0d0a 0d0a 2020 2020 6465  ents))....    de
+000080b0: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
+000080c0: 6c66 2c20 696e 6465 783a 2069 6e74 2920  lf, index: int) 
+000080d0: 2d3e 2053 6567 6d65 6e74 3a0d 0a20 2020  -> Segment:..   
+000080e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000080f0: 2e73 6567 6d65 6e74 735b 696e 6465 785d  .segments[index]
+00008100: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6465  ....    def __de
+00008110: 6c69 7465 6d5f 5f28 7365 6c66 2c20 696e  litem__(self, in
+00008120: 6465 783a 2069 6e74 293a 0d0a 2020 2020  dex: int):..    
+00008130: 2020 2020 6465 6c20 7365 6c66 2e73 6567      del self.seg
+00008140: 6d65 6e74 735b 696e 6465 785d 0d0a 2020  ments[index]..  
+00008150: 2020 2020 2020 7365 6c66 2e72 6561 7373        self.reass
+00008160: 6967 6e5f 6964 7328 5472 7565 2c20 7374  ign_ids(True, st
+00008170: 6172 743d 696e 6465 7829 0d0a 0d0a 2020  art=index)....  
+00008180: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00008190: 2064 6566 2064 7572 6174 696f 6e28 7365   def duration(se
+000081a0: 6c66 293a 0d0a 2020 2020 2020 2020 6966  lf):..        if
+000081b0: 206e 6f74 2073 656c 662e 7365 676d 656e   not self.segmen
+000081c0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+000081d0: 2072 6574 7572 6e20 302e 300d 0a20 2020   return 0.0..   
+000081e0: 2020 2020 2072 6574 7572 6e20 5f72 6f75       return _rou
+000081f0: 6e64 5f74 696d 6573 7461 6d70 2873 656c  nd_timestamp(sel
+00008200: 662e 7365 676d 656e 7473 5b2d 315d 2e65  f.segments[-1].e
+00008210: 6e64 202d 2073 656c 662e 7365 676d 656e  nd - self.segmen
+00008220: 7473 5b30 5d2e 7374 6172 7429 0d0a 0d0a  ts[0].start)....
+00008230: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00008240: 640d 0a20 2020 2064 6566 205f 7374 616e  d..    def _stan
+00008250: 6461 7264 697a 655f 7265 7375 6c74 2872  dardize_result(r
+00008260: 6573 756c 743a 2055 6e69 6f6e 5b73 7472  esult: Union[str
+00008270: 2c20 6469 6374 2c20 4c69 7374 5b64 6963  , dict, List[dic
+00008280: 745d 2c20 4c69 7374 5b4c 6973 745b 6469  t], List[List[di
+00008290: 6374 5d5d 5d29 202d 3e20 5475 706c 655b  ct]]]) -> Tuple[
+000082a0: 6469 6374 2c20 556e 696f 6e5b 7374 722c  dict, Union[str,
+000082b0: 204e 6f6e 655d 5d3a 0d0a 2020 2020 2020   None]]:..      
+000082c0: 2020 7061 7468 203d 204e 6f6e 650d 0a20    path = None.. 
+000082d0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000082e0: 616e 6365 2872 6573 756c 742c 2073 7472  ance(result, str
+000082f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00008300: 7061 7468 203d 2072 6573 756c 740d 0a20  path = result.. 
+00008310: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00008320: 7420 3d20 6c6f 6164 5f72 6573 756c 7428  t = load_result(
+00008330: 7061 7468 290d 0a20 2020 2020 2020 2069  path)..        i
+00008340: 6620 6973 696e 7374 616e 6365 2872 6573  f isinstance(res
+00008350: 756c 742c 2064 6963 7429 3a0d 0a20 2020  ult, dict):..   
+00008360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008370: 7265 7375 6c74 2c20 7061 7468 0d0a 2020  result, path..  
+00008380: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00008390: 6e73 7461 6e63 6528 7265 7375 6c74 2c20  nstance(result, 
+000083a0: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+000083b0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+000083c0: 726f 7228 6627 4578 7065 6374 2072 6573  ror(f'Expect res
+000083d0: 756c 7420 746f 2062 6520 6c69 7374 2062  ult to be list b
+000083e0: 7574 2067 6f74 207b 7479 7065 2872 6573  ut got {type(res
+000083f0: 756c 7429 7d27 290d 0a20 2020 2020 2020  ult)}')..       
+00008400: 2069 6620 6e6f 7420 7265 7375 6c74 206f   if not result o
+00008410: 7220 6e6f 7420 7265 7375 6c74 5b30 5d3a  r not result[0]:
+00008420: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00008430: 7475 726e 207b 7d2c 2070 6174 680d 0a20  turn {}, path.. 
+00008440: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00008450: 616e 6365 2872 6573 756c 745b 305d 2c20  ance(result[0], 
+00008460: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+00008470: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00008480: 7461 6e63 6528 7265 7375 6c74 5b30 5d5b  tance(result[0][
+00008490: 305d 2c20 6469 6374 293a 0d0a 2020 2020  0], dict):..    
+000084a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000084b0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+000084c0: 4572 726f 7228 6627 476f 7420 6c69 7374  Error(f'Got list
+000084d0: 206f 6620 6c69 7374 206f 6620 7b74 7970   of list of {typ
+000084e0: 6528 7265 7375 6c74 5b30 5d29 7d20 6275  e(result[0])} bu
+000084f0: 7420 6578 7065 6374 7320 6c69 7374 206f  t expects list o
+00008500: 6620 6c69 7374 206f 6620 6469 6374 2729  f list of dict')
+00008510: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00008520: 7375 6c74 203d 2064 6963 7428 0d0a 2020  sult = dict(..  
+00008530: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008540: 676d 656e 7473 3d5b 0d0a 2020 2020 2020  gments=[..      
+00008550: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00008560: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
+00008570: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00008580: 7274 3d77 6f72 6473 5b30 5d5b 2773 7461  rt=words[0]['sta
+00008590: 7274 275d 2c0d 0a20 2020 2020 2020 2020  rt'],..         
+000085a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000085b0: 6e64 3d77 6f72 6473 5b2d 315d 5b27 656e  nd=words[-1]['en
+000085c0: 6427 5d2c 0d0a 2020 2020 2020 2020 2020  d'],..          
+000085d0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+000085e0: 7874 3d27 272e 6a6f 696e 2877 5b27 776f  xt=''.join(w['wo
+000085f0: 7264 275d 2066 6f72 2077 2069 6e20 776f  rd'] for w in wo
+00008600: 7264 7329 2c0d 0a20 2020 2020 2020 2020  rds),..         
+00008610: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00008620: 6f72 6473 3d77 6f72 6473 0d0a 2020 2020  ords=words..    
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008650: 2020 2020 2020 2066 6f72 2077 6f72 6473         for words
+00008660: 2069 6e20 7265 7375 6c74 2069 6620 776f   in result if wo
+00008670: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
+00008680: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+00008690: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+000086a0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000086b0: 2872 6573 756c 745b 305d 2c20 6469 6374  (result[0], dict
+000086c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000086d0: 7265 7375 6c74 203d 2064 6963 7428 7365  result = dict(se
+000086e0: 676d 656e 7473 3d72 6573 756c 7429 0d0a  gments=result)..
+000086f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00008700: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00008710: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00008720: 7272 6f72 2866 2747 6f74 206c 6973 7420  rror(f'Got list 
+00008730: 6f66 207b 7479 7065 2872 6573 756c 745b  of {type(result[
+00008740: 305d 297d 2062 7574 2065 7870 6563 7473  0])} but expects
+00008750: 206c 6973 7420 6f66 206c 6973 742f 6469   list of list/di
+00008760: 6374 2729 0d0a 2020 2020 2020 2020 7265  ct')..        re
+00008770: 7475 726e 2072 6573 756c 742c 2070 6174  turn result, pat
+00008780: 680d 0a0d 0a20 2020 2064 6566 2066 6f72  h....    def for
+00008790: 6365 5f6f 7264 6572 2873 656c 6629 3a0d  ce_order(self):.
+000087a0: 0a20 2020 2020 2020 2070 7265 765f 7473  .        prev_ts
+000087b0: 5f65 6e64 203d 2030 0d0a 2020 2020 2020  _end = 0..      
+000087c0: 2020 7469 6d65 7374 616d 7073 203d 2073    timestamps = s
+000087d0: 656c 662e 616c 6c5f 776f 7264 735f 6f72  elf.all_words_or
+000087e0: 5f73 6567 6d65 6e74 7328 290d 0a20 2020  _segments()..   
+000087f0: 2020 2020 2066 6f72 2069 2c20 7473 2069       for i, ts i
+00008800: 6e20 656e 756d 6572 6174 6528 7469 6d65  n enumerate(time
+00008810: 7374 616d 7073 2c20 3129 3a0d 0a20 2020  stamps, 1):..   
+00008820: 2020 2020 2020 2020 2069 6620 7473 2e73           if ts.s
+00008830: 7461 7274 203c 2070 7265 765f 7473 5f65  tart < prev_ts_e
+00008840: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
+00008850: 2020 2020 2074 732e 7374 6172 7420 3d20       ts.start = 
+00008860: 7072 6576 5f74 735f 656e 640d 0a20 2020  prev_ts_end..   
+00008870: 2020 2020 2020 2020 2069 6620 7473 2e73           if ts.s
+00008880: 7461 7274 203e 2074 732e 656e 643a 0d0a  tart > ts.end:..
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 6966 2070 7265 765f 7473 5f65 6e64 203e  if prev_ts_end >
+000088b0: 2074 732e 656e 643a 0d0a 2020 2020 2020   ts.end:..      
+000088c0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+000088d0: 726e 696e 6773 2e77 6172 6e28 274d 756c  rnings.warn('Mul
+000088e0: 7469 706c 6520 636f 6e73 6563 7574 6976  tiple consecutiv
+000088f0: 6520 7469 6d65 7374 616d 7073 2061 7265  e timestamps are
+00008900: 206f 7574 206f 6620 6f72 6465 722e 2053   out of order. S
+00008910: 6f6d 6520 7061 7274 7320 7769 6c6c 2068  ome parts will h
+00008920: 6176 6520 6e6f 2064 7572 6174 696f 6e2e  ave no duration.
+00008930: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00008940: 2020 2020 2020 2020 7473 2e73 7461 7274          ts.start
+00008950: 203d 2074 732e 656e 640d 0a20 2020 2020   = ts.end..     
+00008960: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00008970: 6f72 206a 2069 6e20 7261 6e67 6528 692d  or j in range(i-
+00008980: 322c 202d 312c 202d 3129 3a0d 0a20 2020  2, -1, -1):..   
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 2020 2069 6620 7469 6d65 7374 616d       if timestam
+000089b0: 7073 5b6a 5d2e 656e 6420 3e20 7473 2e65  ps[j].end > ts.e
+000089c0: 6e64 3a0d 0a20 2020 2020 2020 2020 2020  nd:..           
+000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089e0: 2074 696d 6573 7461 6d70 735b 6a5d 2e65   timestamps[j].e
+000089f0: 6e64 203d 2074 732e 656e 640d 0a20 2020  nd = ts.end..   
+00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a10: 2020 2020 2069 6620 7469 6d65 7374 616d       if timestam
+00008a20: 7073 5b6a 5d2e 7374 6172 7420 3e20 7473  ps[j].start > ts
+00008a30: 2e65 6e64 3a0d 0a20 2020 2020 2020 2020  .end:..         
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2074 696d 6573 7461 6d70 735b 6a5d     timestamps[j]
+00008a60: 2e73 7461 7274 203d 2074 732e 656e 640d  .start = ts.end.
+00008a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a80: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00008a90: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00008aa0: 732e 7374 6172 7420 213d 2070 7265 765f  s.start != prev_
+00008ab0: 7473 5f65 6e64 3a0d 0a20 2020 2020 2020  ts_end:..       
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2074 732e 7374 6172 7420 3d20 7072 6576   ts.start = prev
+00008ae0: 5f74 735f 656e 640d 0a20 2020 2020 2020  _ts_end..       
+00008af0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00008b00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00008b10: 2020 2020 2020 2020 2020 2020 7473 2e65              ts.e
+00008b20: 6e64 203d 2074 732e 7374 6172 7420 6966  nd = ts.start if
+00008b30: 2069 203d 3d20 6c65 6e28 7469 6d65 7374   i == len(timest
+00008b40: 616d 7073 2920 656c 7365 2074 696d 6573  amps) else times
+00008b50: 7461 6d70 735b 695d 2e73 7461 7274 0d0a  tamps[i].start..
+00008b60: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00008b70: 5f74 735f 656e 6420 3d20 7473 2e65 6e64  _ts_end = ts.end
+00008b80: 0d0a 0d0a 2020 2020 6465 6620 7261 6973  ....    def rais
+00008b90: 655f 666f 725f 756e 736f 7274 6564 2873  e_for_unsorted(s
+00008ba0: 656c 662c 2063 6865 636b 5f73 6f72 7465  elf, check_sorte
+00008bb0: 643a 2055 6e69 6f6e 5b62 6f6f 6c2c 2073  d: Union[bool, s
+00008bc0: 7472 5d20 3d20 5472 7565 2c20 7368 6f77  tr] = True, show
+00008bd0: 5f75 6e73 6f72 7465 643a 2062 6f6f 6c20  _unsorted: bool 
+00008be0: 3d20 5472 7565 293a 0d0a 2020 2020 2020  = True):..      
+00008bf0: 2020 6966 2063 6865 636b 5f73 6f72 7465    if check_sorte
+00008c00: 6420 6973 2046 616c 7365 3a0d 0a20 2020  d is False:..   
+00008c10: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+00008c20: 0a20 2020 2020 2020 2061 6c6c 5f70 6172  .        all_par
+00008c30: 7473 203d 2073 656c 662e 616c 6c5f 776f  ts = self.all_wo
+00008c40: 7264 735f 6f72 5f73 6567 6d65 6e74 7328  rds_or_segments(
+00008c50: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+00008c60: 7420 616c 6c5f 7061 7274 733a 0d0a 2020  t all_parts:..  
+00008c70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008c80: 0d0a 2020 2020 2020 2020 6973 5f77 6f72  ..        is_wor
+00008c90: 6420 3d20 6973 696e 7374 616e 6365 2861  d = isinstance(a
+00008ca0: 6c6c 5f70 6172 7473 5b30 5d2c 2057 6f72  ll_parts[0], Wor
+00008cb0: 6454 696d 696e 6729 0d0a 2020 2020 2020  dTiming)..      
+00008cc0: 2020 7469 6d65 7374 616d 7073 203d 206e    timestamps = n
+00008cd0: 702e 6172 7261 7928 6c69 7374 2863 6861  p.array(list(cha
+00008ce0: 696e 2e66 726f 6d5f 6974 6572 6162 6c65  in.from_iterable
+00008cf0: 2828 702e 7374 6172 742c 2070 2e65 6e64  ((p.start, p.end
+00008d00: 2920 666f 7220 7020 696e 2061 6c6c 5f70  ) for p in all_p
+00008d10: 6172 7473 2929 290d 0a20 2020 2020 2020  arts)))..       
+00008d20: 2069 6620 6c65 6e28 7469 6d65 7374 616d   if len(timestam
+00008d30: 7073 2920 3e20 3120 616e 6420 2875 6e73  ps) > 1 and (uns
+00008d40: 6f72 7465 645f 6d61 736b 203a 3d20 7469  orted_mask := ti
+00008d50: 6d65 7374 616d 7073 5b3a 2d31 5d20 3e20  mestamps[:-1] > 
+00008d60: 7469 6d65 7374 616d 7073 5b31 3a5d 292e  timestamps[1:]).
+00008d70: 616e 7928 293a 0d0a 2020 2020 2020 2020  any():..        
+00008d80: 2020 2020 6966 2073 686f 775f 756e 736f      if show_unso
+00008d90: 7274 6564 3a0d 0a20 2020 2020 2020 2020  rted:..         
+00008da0: 2020 2020 2020 2064 6566 2067 6574 5f70         def get_p
+00008db0: 6172 745f 696e 666f 2869 6478 293a 0d0a  art_info(idx):..
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 2020 2020 6375 7272 5f70 6172 7420 3d20      curr_part = 
+00008de0: 616c 6c5f 7061 7274 735b 6964 785d 0d0a  all_parts[idx]..
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2020 2020 7365 675f 6964 203d 2063 7572      seg_id = cur
+00008e10: 725f 7061 7274 2e73 6567 6d65 6e74 5f69  r_part.segment_i
+00008e20: 6420 6966 2069 735f 776f 7264 2065 6c73  d if is_word els
+00008e30: 6520 6375 7272 5f70 6172 742e 6964 0d0a  e curr_part.id..
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 2020 2020 776f 7264 5f69 645f 7374 7220      word_id_str 
+00008e60: 3d20 6627 576f 7264 2049 443a 207b 6375  = f'Word ID: {cu
+00008e70: 7272 5f70 6172 742e 6964 7d5c 6e27 2069  rr_part.id}\n' i
+00008e80: 6620 6973 5f77 6f72 6420 656c 7365 2027  f is_word else '
+00008e90: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+00008ea0: 2020 2020 2020 2072 6574 7572 6e20 280d         return (.
+00008eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ec0: 2020 2020 2020 2020 2066 2753 6567 6d65           f'Segme
+00008ed0: 6e74 2049 443a 207b 7365 675f 6964 7d5c  nt ID: {seg_id}\
+00008ee0: 6e7b 776f 7264 5f69 645f 7374 727d 270d  n{word_id_str}'.
+00008ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008f00: 2020 2020 2020 2020 2066 2753 7461 7274           f'Start
+00008f10: 3a20 7b63 7572 725f 7061 7274 2e73 7461  : {curr_part.sta
+00008f20: 7274 7d5c 6e45 6e64 3a20 7b63 7572 725f  rt}\nEnd: {curr_
+00008f30: 7061 7274 2e65 6e64 7d5c 6e27 0d0a 2020  part.end}\n'..  
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 2020 2020 2020 6627 5465 7874 3a20 227b        f'Text: "{
+00008f60: 6375 7272 5f70 6172 742e 776f 7264 2069  curr_part.word i
+00008f70: 6620 6973 5f77 6f72 6420 656c 7365 2063  f is_word else c
+00008f80: 7572 725f 7061 7274 2e74 6578 747d 2227  urr_part.text}"'
+00008f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008fa0: 2020 2020 2020 292c 2063 7572 725f 7061        ), curr_pa
+00008fb0: 7274 2e73 7461 7274 2c20 6375 7272 5f70  rt.start, curr_p
+00008fc0: 6172 742e 656e 640d 0a0d 0a20 2020 2020  art.end....     
+00008fd0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00008fe0: 2c20 756e 736f 7274 6564 2069 6e20 656e  , unsorted in en
+00008ff0: 756d 6572 6174 6528 756e 736f 7274 6564  umerate(unsorted
+00009000: 5f6d 6173 6b2c 2032 293a 0d0a 2020 2020  _mask, 2):..    
+00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009020: 6966 2075 6e73 6f72 7465 643a 0d0a 2020  if unsorted:..  
+00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009040: 2020 2020 2020 776f 7264 5f69 6420 3d20        word_id = 
+00009050: 692f 2f32 2d31 0d0a 2020 2020 2020 2020  i//2-1..        
+00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009070: 7061 7274 5f69 6e66 6f2c 2073 7461 7274  part_info, start
+00009080: 2c20 656e 6420 3d20 6765 745f 7061 7274  , end = get_part
+00009090: 5f69 6e66 6f28 776f 7264 5f69 6429 0d0a  _info(word_id)..
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 2020 2020 2020 2020 6966 2069 2025 2032          if i % 2
+000090c0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090e0: 2020 2020 6e65 7874 5f69 6e66 6f2c 206e      next_info, n
+000090f0: 6578 745f 7374 6172 742c 205f 203d 2067  ext_start, _ = g
+00009100: 6574 5f70 6172 745f 696e 666f 2877 6f72  et_part_info(wor
+00009110: 645f 6964 2b31 290d 0a20 2020 2020 2020  d_id+1)..       
+00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009130: 2020 2020 2070 6172 745f 696e 666f 202b       part_info +
+00009140: 3d20 6627 5c6e 436f 6e66 6c69 6374 3a20  = f'\nConflict: 
+00009150: 656e 6420 287b 656e 647d 2920 3e20 6e65  end ({end}) > ne
+00009160: 7874 2073 7461 7274 2028 7b6e 6578 745f  xt start ({next_
+00009170: 7374 6172 747d 295c 6e7b 6e65 7874 5f69  start})\n{next_i
+00009180: 6e66 6f7d 270d 0a20 2020 2020 2020 2020  nfo}'..         
+00009190: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000091a0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091c0: 2020 7061 7274 5f69 6e66 6f20 2b3d 2066    part_info += f
+000091d0: 275c 6e43 6f6e 666c 6963 743a 2073 7461  '\nConflict: sta
+000091e0: 7274 2028 7b73 7461 7274 7d29 203e 2065  rt ({start}) > e
+000091f0: 6e64 2028 7b65 6e64 7d29 270d 0a20 2020  nd ({end})'..   
 00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 2755 7365 2060 602e 7265 6173 7369 676e  'Use ``.reassign
-00009220: 5f69 6473 2829 6060 2074 6f20 6d61 6e75  _ids()`` to manu
-00009230: 616c 6c79 2075 7064 6174 6520 6964 7327  ally update ids'
-00009240: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009250: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
-00009260: 7665 6c3d 3229 0d0a 2020 2020 2020 2020  vel=2)..        
-00009270: 7365 6c66 2e72 6561 7373 6967 6e5f 6964  self.reassign_id
-00009280: 7328 290d 0a0d 0a20 2020 2064 6566 2075  s()....    def u
-00009290: 7064 6174 655f 6e6f 6e73 7065 6563 685f  pdate_nonspeech_
-000092a0: 7365 6374 696f 6e73 2873 656c 662c 2073  sections(self, s
-000092b0: 696c 656e 745f 7374 6172 7473 2c20 7369  ilent_starts, si
-000092c0: 6c65 6e74 5f65 6e64 7329 3a0d 0a20 2020  lent_ends):..   
-000092d0: 2020 2020 2073 656c 662e 5f6e 6f6e 7370       self._nonsp
-000092e0: 6565 6368 5f73 6563 7469 6f6e 7320 3d20  eech_sections = 
-000092f0: 5b0d 0a20 2020 2020 2020 2020 2020 2064  [..            d
-00009300: 6963 7428 7374 6172 743d 726f 756e 6428  ict(start=round(
-00009310: 732c 2033 292c 2065 6e64 3d72 6f75 6e64  s, 3), end=round
-00009320: 2865 2c20 3329 2920 666f 7220 732c 2065  (e, 3)) for s, e
-00009330: 2069 6e20 7a69 7028 7369 6c65 6e74 5f73   in zip(silent_s
-00009340: 7461 7274 732c 2073 696c 656e 745f 656e  tarts, silent_en
-00009350: 6473 290d 0a20 2020 2020 2020 205d 0d0a  ds)..        ]..
-00009360: 0d0a 2020 2020 6465 6620 6164 645f 7365  ..    def add_se
-00009370: 676d 656e 7473 2873 656c 662c 2069 6e64  gments(self, ind
-00009380: 6578 303a 2069 6e74 2c20 696e 6465 7831  ex0: int, index1
-00009390: 3a20 696e 742c 2069 6e70 6c61 6365 3a20  : int, inplace: 
-000093a0: 626f 6f6c 203d 2046 616c 7365 2c20 6c6f  bool = False, lo
-000093b0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-000093c0: 293a 0d0a 2020 2020 2020 2020 6e65 775f  ):..        new_
-000093d0: 7365 6720 3d20 7365 6c66 2e73 6567 6d65  seg = self.segme
-000093e0: 6e74 735b 696e 6465 7830 5d2e 6164 6428  nts[index0].add(
-000093f0: 7365 6c66 2e73 6567 6d65 6e74 735b 696e  self.segments[in
-00009400: 6465 7831 5d2c 2063 6f70 795f 776f 7264  dex1], copy_word
-00009410: 733d 4661 6c73 6529 0d0a 2020 2020 2020  s=False)..      
-00009420: 2020 6966 206c 6f63 6b20 616e 6420 7365    if lock and se
-00009430: 6c66 2e73 6567 6d65 6e74 735b 696e 6465  lf.segments[inde
-00009440: 7830 5d2e 6861 735f 776f 7264 733a 0d0a  x0].has_words:..
-00009450: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
-00009460: 5f69 6478 203d 206c 656e 2873 656c 662e  _idx = len(self.
-00009470: 7365 676d 656e 7473 5b69 6e64 6578 305d  segments[index0]
-00009480: 2e77 6f72 6473 290d 0a20 2020 2020 2020  .words)..       
-00009490: 2020 2020 206e 6577 5f73 6567 2e77 6f72       new_seg.wor
-000094a0: 6473 5b6c 6f63 6b5f 6964 7820 2d20 315d  ds[lock_idx - 1]
-000094b0: 2e6c 6f63 6b5f 7269 6768 7428 290d 0a20  .lock_right().. 
-000094c0: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-000094d0: 636b 5f69 6478 203c 206c 656e 286e 6577  ck_idx < len(new
-000094e0: 5f73 6567 2e77 6f72 6473 293a 0d0a 2020  _seg.words):..  
-000094f0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00009500: 775f 7365 672e 776f 7264 735b 6c6f 636b  w_seg.words[lock
-00009510: 5f69 6478 5d2e 6c6f 636b 5f6c 6566 7428  _idx].lock_left(
-00009520: 290d 0a20 2020 2020 2020 2069 6620 696e  )..        if in
-00009530: 706c 6163 653a 0d0a 2020 2020 2020 2020  place:..        
-00009540: 2020 2020 6930 2c20 6931 203d 2073 6f72      i0, i1 = sor
-00009550: 7465 6428 5b69 6e64 6578 302c 2069 6e64  ted([index0, ind
-00009560: 6578 315d 290d 0a20 2020 2020 2020 2020  ex1])..         
-00009570: 2020 2073 656c 662e 7365 676d 656e 7473     self.segments
-00009580: 5b69 305d 203d 206e 6577 5f73 6567 0d0a  [i0] = new_seg..
-00009590: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-000095a0: 7365 6c66 2e73 6567 6d65 6e74 735b 6931  self.segments[i1
-000095b0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-000095c0: 6e20 6e65 775f 7365 670d 0a0d 0a20 2020  n new_seg....   
-000095d0: 2064 6566 2072 6573 6361 6c65 5f74 696d   def rescale_tim
-000095e0: 6528 7365 6c66 2c20 7363 616c 655f 6661  e(self, scale_fa
-000095f0: 6374 6f72 3a20 666c 6f61 7429 3a0d 0a20  ctor: float):.. 
-00009600: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
-00009610: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
-00009620: 2020 2020 2020 2020 2020 2020 732e 7265              s.re
-00009630: 7363 616c 655f 7469 6d65 2873 6361 6c65  scale_time(scale
-00009640: 5f66 6163 746f 7229 0d0a 0d0a 2020 2020  _factor)....    
-00009650: 6465 6620 6170 706c 795f 6d69 6e5f 6475  def apply_min_du
-00009660: 7228 7365 6c66 2c20 6d69 6e5f 6475 723a  r(self, min_dur:
-00009670: 2066 6c6f 6174 2c20 696e 706c 6163 653a   float, inplace:
-00009680: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
-00009690: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000096a0: 2020 2020 2020 4d65 7267 6520 616e 7920        Merge any 
-000096b0: 776f 7264 2f73 6567 6d65 6e74 2077 6974  word/segment wit
-000096c0: 6820 6164 6a61 6365 6e74 2077 6f72 642f  h adjacent word/
-000096d0: 7365 676d 656e 7420 6966 2069 7473 2064  segment if its d
-000096e0: 7572 6174 696f 6e20 6973 206c 6573 7320  uration is less 
-000096f0: 7468 616e 2060 606d 696e 5f64 7572 6060  than ``min_dur``
-00009700: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00009710: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00009720: 2073 656c 6620 6966 2069 6e70 6c61 6365   self if inplace
-00009730: 2065 6c73 6520 6465 6570 636f 7079 2873   else deepcopy(s
-00009740: 656c 6629 0d0a 2020 2020 2020 2020 6d61  elf)..        ma
-00009750: 785f 6920 3d20 6c65 6e28 7265 7375 6c74  x_i = len(result
-00009760: 2e73 6567 6d65 6e74 7329 202d 2031 0d0a  .segments) - 1..
-00009770: 2020 2020 2020 2020 6966 206d 6178 5f69          if max_i
-00009780: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-00009790: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000097a0: 740d 0a20 2020 2020 2020 2066 6f72 2069  t..        for i
-000097b0: 2069 6e20 7265 7665 7273 6564 2872 616e   in reversed(ran
-000097c0: 6765 286c 656e 2872 6573 756c 742e 7365  ge(len(result.se
-000097d0: 676d 656e 7473 2929 293a 0d0a 2020 2020  gments))):..    
-000097e0: 2020 2020 2020 2020 6966 206d 6178 5f69          if max_i
-000097f0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-00009800: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-00009810: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00009820: 7375 6c74 2e73 6567 6d65 6e74 735b 695d  sult.segments[i]
-00009830: 2e64 7572 6174 696f 6e20 3c20 6d69 6e5f  .duration < min_
-00009840: 6475 723a 0d0a 2020 2020 2020 2020 2020  dur:..          
-00009850: 2020 2020 2020 6966 2069 203d 3d20 6d61        if i == ma
-00009860: 785f 693a 0d0a 2020 2020 2020 2020 2020  x_i:..          
-00009870: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00009880: 2e61 6464 5f73 6567 6d65 6e74 7328 692d  .add_segments(i-
-00009890: 312c 2069 2c20 696e 706c 6163 653d 5472  1, i, inplace=Tr
-000098a0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-000098b0: 2020 2020 2065 6c69 6620 6920 3d3d 2030       elif i == 0
-000098c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000098d0: 2020 2020 2020 2072 6573 756c 742e 6164         result.ad
-000098e0: 645f 7365 676d 656e 7473 2869 2c20 692b  d_segments(i, i+
-000098f0: 312c 2069 6e70 6c61 6365 3d54 7275 6529  1, inplace=True)
-00009900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009910: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00009920: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009930: 7265 7375 6c74 2e73 6567 6d65 6e74 735b  result.segments[
-00009940: 692b 315d 2e64 7572 6174 696f 6e20 3c20  i+1].duration < 
-00009950: 7265 7375 6c74 2e73 6567 6d65 6e74 735b  result.segments[
-00009960: 692d 315d 2e64 7572 6174 696f 6e3a 0d0a  i-1].duration:..
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2020 2020 2020 2020 7265 7375 6c74 2e61          result.a
-00009990: 6464 5f73 6567 6d65 6e74 7328 692d 312c  dd_segments(i-1,
-000099a0: 2069 2c20 696e 706c 6163 653d 5472 7565   i, inplace=True
-000099b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000099c0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 7265 7375 6c74 2e61 6464        result.add
-000099f0: 5f73 6567 6d65 6e74 7328 692c 2069 2b31  _segments(i, i+1
-00009a00: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
-00009a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009a20: 206d 6178 5f69 202d 3d20 310d 0a20 2020   max_i -= 1..   
-00009a30: 2020 2020 2072 6573 756c 742e 7265 6173       result.reas
-00009a40: 7369 676e 5f69 6473 2829 0d0a 2020 2020  sign_ids()..    
-00009a50: 2020 2020 666f 7220 7320 696e 2072 6573      for s in res
-00009a60: 756c 742e 7365 676d 656e 7473 3a0d 0a20  ult.segments:.. 
-00009a70: 2020 2020 2020 2020 2020 2073 2e61 7070             s.app
-00009a80: 6c79 5f6d 696e 5f64 7572 286d 696e 5f64  ly_min_dur(min_d
-00009a90: 7572 2c20 696e 706c 6163 653d 5472 7565  ur, inplace=True
-00009aa0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00009ab0: 6e20 7265 7375 6c74 0d0a 0d0a 2020 2020  n result....    
-00009ac0: 6465 6620 6f66 6673 6574 5f74 696d 6528  def offset_time(
-00009ad0: 7365 6c66 2c20 6f66 6673 6574 5f73 6563  self, offset_sec
-00009ae0: 6f6e 6473 3a20 666c 6f61 7429 3a0d 0a20  onds: float):.. 
-00009af0: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
-00009b00: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
-00009b10: 2020 2020 2020 2020 2020 2020 732e 6f66              s.of
-00009b20: 6673 6574 5f74 696d 6528 6f66 6673 6574  fset_time(offset
-00009b30: 5f73 6563 6f6e 6473 290d 0a0d 0a20 2020  _seconds)....   
-00009b40: 2064 6566 2073 7570 7072 6573 735f 7369   def suppress_si
-00009b50: 6c65 6e63 6528 0d0a 2020 2020 2020 2020  lence(..        
-00009b60: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-00009b70: 2020 2020 2020 2073 696c 656e 745f 7374         silent_st
-00009b80: 6172 7473 3a20 6e70 2e6e 6461 7272 6179  arts: np.ndarray
-00009b90: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00009ba0: 696c 656e 745f 656e 6473 3a20 6e70 2e6e  ilent_ends: np.n
-00009bb0: 6461 7272 6179 2c0d 0a20 2020 2020 2020  darray,..       
-00009bc0: 2020 2020 206d 696e 5f77 6f72 645f 6475       min_word_du
-00009bd0: 723a 204f 7074 696f 6e61 6c5b 666c 6f61  r: Optional[floa
-00009be0: 745d 203d 204e 6f6e 652c 0d0a 2020 2020  t] = None,..    
-00009bf0: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
-00009c00: 656c 3a20 626f 6f6c 203d 2054 7275 652c  el: bool = True,
-00009c10: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
-00009c20: 6e73 7065 6563 685f 6572 726f 723a 2066  nspeech_error: f
-00009c30: 6c6f 6174 203d 2030 2e33 2c0d 0a20 2020  loat = 0.3,..   
-00009c40: 2020 2020 2020 2020 2075 7365 5f77 6f72           use_wor
-00009c50: 645f 706f 7369 7469 6f6e 3a20 626f 6f6c  d_position: bool
-00009c60: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-00009c70: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
-00009c80: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
-00009c90: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
-00009ca0: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
-00009cb0: 2222 220d 0a20 2020 2020 2020 204d 6f76  """..        Mov
-00009cc0: 6520 616e 7920 7374 6172 742f 656e 6420  e any start/end 
-00009cd0: 7469 6d65 7374 616d 7073 2069 6e20 7369  timestamps in si
-00009ce0: 6c65 6e63 6520 7061 7274 7320 6f66 2061  lence parts of a
-00009cf0: 7564 696f 2074 6f20 7468 6520 626f 756e  udio to the boun
-00009d00: 6461 7269 6573 206f 6620 7468 6520 7369  daries of the si
-00009d10: 6c65 6e63 652e 0d0a 0d0a 2020 2020 2020  lence.....      
-00009d20: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00009d30: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00009d40: 0d0a 2020 2020 2020 2020 7369 6c65 6e74  ..        silent
-00009d50: 5f73 7461 7274 7320 3a20 6e75 6d70 792e  _starts : numpy.
-00009d60: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
-00009d70: 2020 2020 2041 6e20 6172 7261 7920 7374       An array st
-00009d80: 6172 7469 6e67 2074 696d 6573 7461 6d70  arting timestamp
-00009d90: 7320 6f66 2073 696c 656e 7420 7365 6374  s of silent sect
-00009da0: 696f 6e73 206f 6620 6175 6469 6f2e 0d0a  ions of audio...
-00009db0: 2020 2020 2020 2020 7369 6c65 6e74 5f65          silent_e
-00009dc0: 6e64 7320 3a20 6e75 6d70 792e 6e64 6172  nds : numpy.ndar
-00009dd0: 7261 790d 0a20 2020 2020 2020 2020 2020  ray..           
-00009de0: 2041 6e20 6172 7261 7920 656e 6469 6e67   An array ending
-00009df0: 2074 696d 6573 7461 6d70 7320 6f66 2073   timestamps of s
-00009e00: 696c 656e 7420 7365 6374 696f 6e73 206f  ilent sections o
-00009e10: 6620 6175 6469 6f2e 0d0a 2020 2020 2020  f audio...      
-00009e20: 2020 6d69 6e5f 776f 7264 5f64 7572 203a    min_word_dur :
-00009e30: 2066 6c6f 6174 206f 7220 4e6f 6e65 2c20   float or None, 
-00009e40: 6465 6661 756c 7420 4e6f 6e65 206d 6561  default None mea
-00009e50: 6e69 6e67 2075 7365 2060 6073 7461 626c  ning use ``stabl
-00009e60: 655f 7768 6973 7065 722e 6465 6661 756c  e_whisper.defaul
-00009e70: 742e 4445 4641 554c 545f 5641 4c55 4553  t.DEFAULT_VALUES
-00009e80: 6060 0d0a 2020 2020 2020 2020 2020 2020  ``..            
-00009e90: 5368 6f72 7465 7374 2064 7572 6174 696f  Shortest duratio
-00009ea0: 6e20 6561 6368 2077 6f72 6420 6973 2061  n each word is a
-00009eb0: 6c6c 6f77 6564 2074 6f20 7265 6163 6820  llowed to reach 
-00009ec0: 666f 7220 6164 6a75 7374 6d65 6e74 732e  for adjustments.
-00009ed0: 0d0a 2020 2020 2020 2020 776f 7264 5f6c  ..        word_l
-00009ee0: 6576 656c 203a 2062 6f6f 6c2c 2064 6566  evel : bool, def
-00009ef0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-00009f00: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00009f10: 746f 2073 6574 7469 6e67 7320 746f 2077  to settings to w
-00009f20: 6f72 6420 6c65 7665 6c20 7469 6d65 7374  ord level timest
-00009f30: 616d 7073 2e0d 0a20 2020 2020 2020 206e  amps...        n
-00009f40: 6f6e 7370 6565 6368 5f65 7272 6f72 203a  onspeech_error :
-00009f50: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-00009f60: 302e 330d 0a20 2020 2020 2020 2020 2020  0.3..           
-00009f70: 2052 656c 6174 6976 6520 6572 726f 7220   Relative error 
-00009f80: 6f66 206e 6f6e 2d73 7065 6563 6820 7365  of non-speech se
-00009f90: 6374 696f 6e73 2074 6861 7420 6170 7065  ctions that appe
-00009fa0: 6172 2069 6e20 6265 7477 6565 6e20 6120  ar in between a 
-00009fb0: 776f 7264 2066 6f72 2061 646a 7573 746d  word for adjustm
-00009fc0: 656e 7473 2e0d 0a20 2020 2020 2020 2075  ents...        u
-00009fd0: 7365 5f77 6f72 645f 706f 7369 7469 6f6e  se_word_position
-00009fe0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00009ff0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-0000a000: 2020 2057 6865 7468 6572 2074 6f20 7573     Whether to us
-0000a010: 6520 706f 7369 7469 6f6e 206f 6620 7468  e position of th
-0000a020: 6520 776f 7264 2069 6e20 6974 7320 7365  e word in its se
-0000a030: 676d 656e 7420 746f 2064 6574 6572 6d69  gment to determi
-0000a040: 6e65 2077 6865 7468 6572 2074 6f20 6b65  ne whether to ke
-0000a050: 6570 2065 6e64 206f 7220 7374 6172 7420  ep end or start 
-0000a060: 7469 6d65 7374 616d 7073 2069 660d 0a20  timestamps if.. 
-0000a070: 2020 2020 2020 2020 2020 2061 646a 7573             adjus
-0000a080: 746d 656e 7473 2061 7265 2072 6571 7569  tments are requi
-0000a090: 7265 642e 2049 6620 6974 2069 7320 7468  red. If it is th
-0000a0a0: 6520 6669 7273 7420 776f 7264 2c20 6b65  e first word, ke
-0000a0b0: 6570 2065 6e64 2e20 456c 7365 2069 6620  ep end. Else if 
-0000a0c0: 6974 2069 7320 7468 6520 6c61 7374 2077  it is the last w
-0000a0d0: 6f72 642c 206b 6565 7020 7468 6520 7374  ord, keep the st
-0000a0e0: 6172 742e 0d0a 2020 2020 2020 2020 7665  art...        ve
-0000a0f0: 7262 6f73 6520 3a20 626f 6f6c 2c20 6465  rbose : bool, de
-0000a100: 6661 756c 7420 5472 7565 0d0a 2020 2020  fault True..    
-0000a110: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-0000a120: 746f 2075 7365 2070 726f 6772 6573 7362  to use progressb
-0000a130: 6172 2074 6f20 7368 6f77 2070 726f 6772  ar to show progr
-0000a140: 6573 732e 0d0a 0d0a 2020 2020 2020 2020  ess.....        
-0000a150: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-0000a160: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0000a170: 2020 7374 6162 6c65 5f77 6869 7370 6572    stable_whisper
-0000a180: 2e72 6573 756c 742e 5768 6973 7065 7252  .result.WhisperR
-0000a190: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
-0000a1a0: 2020 2054 6865 2063 7572 7265 6e74 2069     The current i
-0000a1b0: 6e73 7461 6e63 6520 6166 7465 7220 7468  nstance after th
-0000a1c0: 6520 6368 616e 6765 732e 0d0a 2020 2020  e changes...    
-0000a1d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0000a1e0: 206d 696e 5f77 6f72 645f 6475 7220 3d20   min_word_dur = 
-0000a1f0: 6765 745f 6d69 6e5f 776f 7264 5f64 7572  get_min_word_dur
-0000a200: 286d 696e 5f77 6f72 645f 6475 7229 0d0a  (min_word_dur)..
-0000a210: 2020 2020 2020 2020 6d61 785f 7473 203d          max_ts =
-0000a220: 2073 656c 662e 7365 676d 656e 7473 5b2d   self.segments[-
-0000a230: 315d 2e65 6e64 2069 6620 7365 6c66 2e73  1].end if self.s
-0000a240: 6567 6d65 6e74 7320 656c 7365 2030 0d0a  egments else 0..
-0000a250: 2020 2020 2020 2020 7769 7468 2074 7164          with tqd
-0000a260: 6d28 746f 7461 6c3d 6d61 785f 7473 2c20  m(total=max_ts, 
-0000a270: 756e 6974 3d27 7365 6327 2c20 6469 7361  unit='sec', disa
-0000a280: 626c 653d 6e6f 7420 7665 7262 6f73 652c  ble=not verbose,
-0000a290: 2064 6573 633d 2741 646a 7573 746d 656e   desc='Adjustmen
-0000a2a0: 7427 2920 6173 2074 7164 6d5f 7062 6172  t') as tqdm_pbar
-0000a2b0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-0000a2c0: 6f72 2073 2069 6e20 7365 6c66 2e73 6567  or s in self.seg
-0000a2d0: 6d65 6e74 733a 0d0a 2020 2020 2020 2020  ments:..        
-0000a2e0: 2020 2020 2020 2020 732e 7375 7070 7265          s.suppre
-0000a2f0: 7373 5f73 696c 656e 6365 280d 0a20 2020  ss_silence(..   
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 2073 696c 656e 745f 7374 6172 7473 2c0d   silent_starts,.
-0000a320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a330: 2020 2020 2073 696c 656e 745f 656e 6473       silent_ends
-0000a340: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a350: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
-0000a360: 6475 722c 0d0a 2020 2020 2020 2020 2020  dur,..          
-0000a370: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
-0000a380: 6576 656c 3d77 6f72 645f 6c65 7665 6c2c  evel=word_level,
-0000a390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a3a0: 2020 2020 2020 6e6f 6e73 7065 6563 685f        nonspeech_
-0000a3b0: 6572 726f 723d 6e6f 6e73 7065 6563 685f  error=nonspeech_
-0000a3c0: 6572 726f 722c 0d0a 2020 2020 2020 2020  error,..        
-0000a3d0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
-0000a3e0: 776f 7264 5f70 6f73 6974 696f 6e3d 7573  word_position=us
-0000a3f0: 655f 776f 7264 5f70 6f73 6974 696f 6e0d  e_word_position.
-0000a400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a410: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0000a420: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
-0000a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a440: 2020 2020 2074 7164 6d5f 7062 6172 2e75       tqdm_pbar.u
-0000a450: 7064 6174 6528 732e 656e 6420 2d20 7471  pdate(s.end - tq
-0000a460: 646d 5f70 6261 722e 6e29 0d0a 2020 2020  dm_pbar.n)..    
-0000a470: 2020 2020 2020 2020 7471 646d 5f70 6261          tqdm_pba
-0000a480: 722e 7570 6461 7465 2874 7164 6d5f 7062  r.update(tqdm_pb
-0000a490: 6172 2e74 6f74 616c 202d 2074 7164 6d5f  ar.total - tqdm_
-0000a4a0: 7062 6172 2e6e 290d 0a0d 0a20 2020 2020  pbar.n)....     
-0000a4b0: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
-0000a4c0: 0d0a 2020 2020 6465 6620 6164 6a75 7374  ..    def adjust
-0000a4d0: 5f62 795f 7369 6c65 6e63 6528 0d0a 2020  _by_silence(..  
-0000a4e0: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-0000a4f0: 0a20 2020 2020 2020 2020 2020 2061 7564  .            aud
-0000a500: 696f 3a20 556e 696f 6e5b 746f 7263 682e  io: Union[torch.
-0000a510: 5465 6e73 6f72 2c20 6e70 2e6e 6461 7272  Tensor, np.ndarr
-0000a520: 6179 2c20 7374 722c 2062 7974 6573 5d2c  ay, str, bytes],
-0000a530: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000a540: 643a 2062 6f6f 6c20 3d20 4661 6c73 652c  d: bool = False,
-0000a550: 0d0a 2020 2020 2020 2020 2020 2020 2a2c  ..            *,
-0000a560: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-0000a570: 7262 6f73 653a 2028 626f 6f6c 2c20 4e6f  rbose: (bool, No
-0000a580: 6e65 2920 3d20 4661 6c73 652c 0d0a 2020  ne) = False,..  
-0000a590: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-0000a5a0: 5f72 6174 653a 2069 6e74 203d 204e 6f6e  _rate: int = Non
-0000a5b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000a5c0: 7661 645f 6f6e 6e78 3a20 626f 6f6c 203d  vad_onnx: bool =
-0000a5d0: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-0000a5e0: 2020 2020 2076 6164 5f74 6872 6573 686f       vad_thresho
-0000a5f0: 6c64 3a20 666c 6f61 7420 3d20 302e 3335  ld: float = 0.35
-0000a600: 2c0d 0a20 2020 2020 2020 2020 2020 2071  ,..            q
-0000a610: 5f6c 6576 656c 733a 2069 6e74 203d 2032  _levels: int = 2
-0000a620: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-0000a630: 6b5f 7369 7a65 3a20 696e 7420 3d20 352c  k_size: int = 5,
-0000a640: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0000a650: 6e5f 776f 7264 5f64 7572 3a20 4f70 7469  n_word_dur: Opti
-0000a660: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-0000a670: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-0000a680: 206d 696e 5f73 696c 656e 6365 5f64 7572   min_silence_dur
-0000a690: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-0000a6a0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-0000a6b0: 2020 2020 2020 2077 6f72 645f 6c65 7665         word_leve
-0000a6c0: 6c3a 2062 6f6f 6c20 3d20 5472 7565 2c0d  l: bool = True,.
-0000a6d0: 0a20 2020 2020 2020 2020 2020 206e 6f6e  .            non
-0000a6e0: 7370 6565 6368 5f65 7272 6f72 3a20 666c  speech_error: fl
-0000a6f0: 6f61 7420 3d20 302e 332c 0d0a 2020 2020  oat = 0.3,..    
-0000a700: 2020 2020 2020 2020 7573 655f 776f 7264          use_word
-0000a710: 5f70 6f73 6974 696f 6e3a 2062 6f6f 6c20  _position: bool 
-0000a720: 3d20 5472 7565 0d0a 0d0a 2020 2020 2920  = True....    ) 
-0000a730: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
-0000a740: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
-0000a750: 0d0a 2020 2020 2020 2020 4164 6a75 7374  ..        Adjust
-0000a760: 2074 696d 6573 7461 6d70 7320 6261 7365   timestamps base
-0000a770: 206f 6e20 6465 7465 6374 6564 2073 7065   on detected spe
-0000a780: 6563 6820 6761 7073 2e0d 0a0d 0a20 2020  ech gaps.....   
-0000a790: 2020 2020 2054 6869 7320 6973 206d 6574       This is met
-0000a7a0: 686f 6420 636f 6d62 696e 6573 203a 6d65  hod combines :me
-0000a7b0: 7468 3a60 7374 6162 6c65 5f77 6869 7370  th:`stable_whisp
-0000a7c0: 6572 2e72 6573 756c 742e 5768 6973 7065  er.result.Whispe
-0000a7d0: 7252 6573 756c 742e 7375 7070 7265 7373  rResult.suppress
-0000a7e0: 5f73 696c 656e 6365 6020 7769 7468 2073  _silence` with s
-0000a7f0: 696c 656e 6365 2064 6574 6563 7469 6f6e  ilence detection
-0000a800: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-0000a810: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
-0000a820: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-0000a830: 2020 2020 2061 7564 696f 203a 2073 7472       audio : str
-0000a840: 206f 7220 6e75 6d70 792e 6e64 6172 7261   or numpy.ndarra
-0000a850: 7920 6f72 2074 6f72 6368 2e54 656e 736f  y or torch.Tenso
-0000a860: 7220 6f72 2062 7974 6573 0d0a 2020 2020  r or bytes..    
-0000a870: 2020 2020 2020 2020 5061 7468 2f55 524c          Path/URL
-0000a880: 2074 6f20 7468 6520 6175 6469 6f20 6669   to the audio fi
-0000a890: 6c65 2c20 7468 6520 6175 6469 6f20 7761  le, the audio wa
-0000a8a0: 7665 666f 726d 2c20 6f72 2062 7974 6573  veform, or bytes
-0000a8b0: 206f 6620 6175 6469 6f20 6669 6c65 2e0d   of audio file..
-0000a8c0: 0a20 2020 2020 2020 2076 6164 203a 2062  .        vad : b
-0000a8d0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-0000a8e0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000a8f0: 5768 6574 6865 7220 746f 2075 7365 2053  Whether to use S
-0000a900: 696c 6572 6f20 5641 4420 746f 2067 656e  ilero VAD to gen
-0000a910: 6572 6174 6520 7469 6d65 7374 616d 7020  erate timestamp 
-0000a920: 7375 7070 7265 7373 696f 6e20 6d61 736b  suppression mask
-0000a930: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
-0000a940: 696c 6572 6f20 5641 4420 7265 7175 6972  ilero VAD requir
-0000a950: 6573 2050 7954 6f72 6368 2031 2e31 322e  es PyTorch 1.12.
-0000a960: 302b 2e20 4f66 6669 6369 616c 2072 6570  0+. Official rep
-0000a970: 6f2c 2068 7474 7073 3a2f 2f67 6974 6875  o, https://githu
-0000a980: 622e 636f 6d2f 736e 616b 6572 7334 2f73  b.com/snakers4/s
-0000a990: 696c 6572 6f2d 7661 642e 0d0a 2020 2020  ilero-vad...    
-0000a9a0: 2020 2020 7665 7262 6f73 6520 3a20 626f      verbose : bo
-0000a9b0: 6f6c 206f 7220 4e6f 6e65 2c20 6465 6661  ol or None, defa
-0000a9c0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
-0000a9d0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-0000a9e0: 6f20 7573 6520 7072 6f67 7265 7373 6261  o use progressba
-0000a9f0: 7220 746f 2073 686f 7720 7072 6f67 7265  r to show progre
-0000aa00: 7373 2e0d 0a20 2020 2020 2020 2020 2020  ss...           
-0000aa10: 2049 6620 6060 7661 6420 3d20 5472 7565   If ``vad = True
-0000aa20: 6060 2061 6e64 2060 6046 616c 7365 6060  `` and ``False``
-0000aa30: 2c20 6d75 7465 206d 6573 7361 6765 7320  , mute messages 
-0000aa40: 6162 6f75 7420 6869 7474 696e 6720 6c6f  about hitting lo
-0000aa50: 6361 6c20 6361 6368 6573 2e0d 0a20 2020  cal caches...   
-0000aa60: 2020 2020 2020 2020 204e 6f74 6520 7468           Note th
-0000aa70: 6174 2074 6865 206d 6573 7361 6765 2061  at the message a
-0000aa80: 626f 7574 2066 6972 7374 2064 6f77 6e6c  bout first downl
-0000aa90: 6f61 6420 6361 6e6e 6f74 2062 6520 6d75  oad cannot be mu
-0000aaa0: 7465 642e 0d0a 2020 2020 2020 2020 7361  ted...        sa
-0000aab0: 6d70 6c65 5f72 6174 6520 3a20 696e 742c  mple_rate : int,
-0000aac0: 2064 6566 6175 6c74 204e 6f6e 652c 206d   default None, m
-0000aad0: 6561 6e69 6e67 2060 6077 6869 7370 6572  eaning ``whisper
-0000aae0: 2e61 7564 696f 2e53 414d 504c 455f 5241  .audio.SAMPLE_RA
-0000aaf0: 5445 6060 2c20 3136 6b48 5a0d 0a20 2020  TE``, 16kHZ..   
-0000ab00: 2020 2020 2020 2020 2054 6865 2073 616d           The sam
-0000ab10: 706c 6520 7261 7465 206f 6620 6060 6175  ple rate of ``au
-0000ab20: 6469 6f60 602e 0d0a 2020 2020 2020 2020  dio``...        
-0000ab30: 7661 645f 6f6e 6e78 203a 2062 6f6f 6c2c  vad_onnx : bool,
-0000ab40: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-0000ab50: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-0000ab60: 6865 7220 746f 2075 7365 204f 4e4e 5820  her to use ONNX 
-0000ab70: 666f 7220 5369 6c65 726f 2056 4144 2e0d  for Silero VAD..
-0000ab80: 0a20 2020 2020 2020 2076 6164 5f74 6872  .        vad_thr
-0000ab90: 6573 686f 6c64 203a 2066 6c6f 6174 2c20  eshold : float, 
-0000aba0: 6465 6661 756c 7420 302e 3335 0d0a 2020  default 0.35..  
-0000abb0: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
-0000abc0: 6f6c 6420 666f 7220 6465 7465 6374 696e  old for detectin
-0000abd0: 6720 7370 6565 6368 2077 6974 6820 5369  g speech with Si
-0000abe0: 6c65 726f 2056 4144 2e20 4c6f 7720 7468  lero VAD. Low th
-0000abf0: 7265 7368 6f6c 6420 7265 6475 6365 7320  reshold reduces 
-0000ac00: 6661 6c73 6520 706f 7369 7469 7665 7320  false positives 
-0000ac10: 666f 7220 7369 6c65 6e63 6520 6465 7465  for silence dete
-0000ac20: 6374 696f 6e2e 0d0a 2020 2020 2020 2020  ction...        
-0000ac30: 715f 6c65 7665 6c73 203a 2069 6e74 2c20  q_levels : int, 
-0000ac40: 6465 6661 756c 7420 3230 0d0a 2020 2020  default 20..    
-0000ac50: 2020 2020 2020 2020 5175 616e 7469 7a61          Quantiza
-0000ac60: 7469 6f6e 206c 6576 656c 7320 666f 7220  tion levels for 
-0000ac70: 6765 6e65 7261 7469 6e67 2074 696d 6573  generating times
-0000ac80: 7461 6d70 2073 7570 7072 6573 7369 6f6e  tamp suppression
-0000ac90: 206d 6173 6b3b 2069 676e 6f72 6564 2069   mask; ignored i
-0000aca0: 6620 6060 7661 6420 3d20 7472 7565 6060  f ``vad = true``
-0000acb0: 2e0d 0a20 2020 2020 2020 2020 2020 2041  ...            A
-0000acc0: 6374 7320 6173 2061 2074 6872 6573 686f  cts as a thresho
-0000acd0: 6c64 2074 6f20 6d61 726b 696e 6720 736f  ld to marking so
-0000ace0: 756e 6420 6173 2073 696c 656e 742e 0d0a  und as silent...
-0000acf0: 2020 2020 2020 2020 2020 2020 4665 7765              Fewe
-0000ad00: 7220 6c65 7665 6c73 2077 696c 6c20 696e  r levels will in
-0000ad10: 6372 6561 7365 2074 6865 2074 6872 6573  crease the thres
-0000ad20: 686f 6c64 206f 6620 766f 6c75 6d65 2061  hold of volume a
-0000ad30: 7420 7768 6963 6820 746f 206d 6172 6b20  t which to mark 
-0000ad40: 6120 736f 756e 6420 6173 2073 696c 656e  a sound as silen
-0000ad50: 742e 0d0a 2020 2020 2020 2020 6b5f 7369  t...        k_si
-0000ad60: 7a65 203a 2069 6e74 2c20 6465 6661 756c  ze : int, defaul
-0000ad70: 7420 350d 0a20 2020 2020 2020 2020 2020  t 5..           
-0000ad80: 204b 6572 6e65 6c20 7369 7a65 2066 6f72   Kernel size for
-0000ad90: 2061 7667 2d70 6f6f 6c69 6e67 2077 6176   avg-pooling wav
-0000ada0: 6566 6f72 6d20 746f 2067 656e 6572 6174  eform to generat
-0000adb0: 6520 7469 6d65 7374 616d 7020 7375 7070  e timestamp supp
-0000adc0: 7265 7373 696f 6e20 6d61 736b 3b20 6967  ression mask; ig
-0000add0: 6e6f 7265 6420 6966 2060 6076 6164 203d  nored if ``vad =
-0000ade0: 2074 7275 6560 602e 0d0a 2020 2020 2020   true``...      
-0000adf0: 2020 2020 2020 5265 636f 6d6d 656e 6420        Recommend 
-0000ae00: 3520 6f72 2033 3b20 6869 6768 6572 2073  5 or 3; higher s
-0000ae10: 697a 6573 2077 696c 6c20 7265 6475 6365  izes will reduce
-0000ae20: 2064 6574 6563 7469 6f6e 206f 6620 7369   detection of si
-0000ae30: 6c65 6e63 652e 0d0a 2020 2020 2020 2020  lence...        
-0000ae40: 6d69 6e5f 776f 7264 5f64 7572 203a 2066  min_word_dur : f
-0000ae50: 6c6f 6174 206f 7220 4e6f 6e65 2c20 6465  loat or None, de
-0000ae60: 6661 756c 7420 4e6f 6e65 206d 6561 6e69  fault None meani
-0000ae70: 6e67 2075 7365 2060 6073 7461 626c 655f  ng use ``stable_
-0000ae80: 7768 6973 7065 722e 6465 6661 756c 742e  whisper.default.
-0000ae90: 4445 4641 554c 545f 5641 4c55 4553 6060  DEFAULT_VALUES``
-0000aea0: 0d0a 2020 2020 2020 2020 2020 2020 5368  ..            Sh
-0000aeb0: 6f72 7465 7374 2064 7572 6174 696f 6e20  ortest duration 
-0000aec0: 6561 6368 2077 6f72 6420 6973 2061 6c6c  each word is all
-0000aed0: 6f77 6564 2074 6f20 7265 6163 6820 6672  owed to reach fr
-0000aee0: 6f6d 2061 646a 7573 746d 656e 7473 2e0d  om adjustments..
-0000aef0: 0a20 2020 2020 2020 206d 696e 5f73 696c  .        min_sil
-0000af00: 656e 6365 5f64 7572 203a 2066 6c6f 6174  ence_dur : float
-0000af10: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-0000af20: 2020 2020 2020 2020 5368 6f72 7465 7374          Shortest
-0000af30: 2064 7572 6174 696f 6e20 6f66 2073 696c   duration of sil
-0000af40: 656e 6365 2061 6c6c 6f77 6564 2066 6f72  ence allowed for
-0000af50: 2073 696c 656e 6365 2073 7570 7072 6573   silence suppres
-0000af60: 7369 6f6e 2e0d 0a20 2020 2020 2020 2077  sion...        w
-0000af70: 6f72 645f 6c65 7665 6c20 3a20 626f 6f6c  ord_level : bool
-0000af80: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-0000af90: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-0000afa0: 6865 7220 746f 2073 6574 7469 6e67 7320  her to settings 
-0000afb0: 746f 2077 6f72 6420 6c65 7665 6c20 7469  to word level ti
-0000afc0: 6d65 7374 616d 7073 2e0d 0a20 2020 2020  mestamps...     
-0000afd0: 2020 206e 6f6e 7370 6565 6368 5f65 7272     nonspeech_err
-0000afe0: 6f72 203a 2066 6c6f 6174 2c20 6465 6661  or : float, defa
-0000aff0: 756c 7420 302e 330d 0a20 2020 2020 2020  ult 0.3..       
-0000b000: 2020 2020 2052 656c 6174 6976 6520 6572       Relative er
-0000b010: 726f 7220 6f66 206e 6f6e 2d73 7065 6563  ror of non-speec
-0000b020: 6820 7365 6374 696f 6e73 2074 6861 7420  h sections that 
-0000b030: 6170 7065 6172 2069 6e20 6265 7477 6565  appear in betwee
-0000b040: 6e20 6120 776f 7264 2066 6f72 2061 646a  n a word for adj
-0000b050: 7573 746d 656e 7473 2e0d 0a20 2020 2020  ustments...     
-0000b060: 2020 2075 7365 5f77 6f72 645f 706f 7369     use_word_posi
-0000b070: 7469 6f6e 203a 2062 6f6f 6c2c 2064 6566  tion : bool, def
-0000b080: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-0000b090: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-0000b0a0: 6f20 7573 6520 706f 7369 7469 6f6e 206f  o use position o
-0000b0b0: 6620 7468 6520 776f 7264 2069 6e20 6974  f the word in it
-0000b0c0: 7320 7365 676d 656e 7420 746f 2064 6574  s segment to det
-0000b0d0: 6572 6d69 6e65 2077 6865 7468 6572 2074  ermine whether t
-0000b0e0: 6f20 6b65 6570 2065 6e64 206f 7220 7374  o keep end or st
-0000b0f0: 6172 7420 7469 6d65 7374 616d 7073 2069  art timestamps i
-0000b100: 660d 0a20 2020 2020 2020 2020 2020 2061  f..            a
-0000b110: 646a 7573 746d 656e 7473 2061 7265 2072  djustments are r
-0000b120: 6571 7569 7265 642e 2049 6620 6974 2069  equired. If it i
-0000b130: 7320 7468 6520 6669 7273 7420 776f 7264  s the first word
-0000b140: 2c20 6b65 6570 2065 6e64 2e20 456c 7365  , keep end. Else
-0000b150: 2069 6620 6974 2069 7320 7468 6520 6c61   if it is the la
-0000b160: 7374 2077 6f72 642c 206b 6565 7020 7468  st word, keep th
-0000b170: 6520 7374 6172 742e 0d0a 0d0a 2020 2020  e start.....    
-0000b180: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-0000b190: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-0000b1a0: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
-0000b1b0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
-0000b1c0: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
-0000b1d0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
-0000b1e0: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
-0000b1f0: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
-0000b200: 0d0a 2020 2020 2020 2020 4e6f 7465 730d  ..        Notes.
-0000b210: 0a20 2020 2020 2020 202d 2d2d 2d2d 0d0a  .        -----..
-0000b220: 2020 2020 2020 2020 5468 6973 206f 7065          This ope
-0000b230: 7261 7469 6f6e 2069 7320 616c 7265 6164  ration is alread
-0000b240: 7920 7065 7266 6f72 6d65 6420 6279 203a  y performed by :
-0000b250: 6675 6e63 3a60 7374 6162 6c65 5f77 6869  func:`stable_whi
-0000b260: 7370 6572 2e77 6869 7370 6572 5f77 6f72  sper.whisper_wor
-0000b270: 645f 6c65 7665 6c2e 7472 616e 7363 7269  d_level.transcri
-0000b280: 6265 5f73 7461 626c 6560 202f 0d0a 2020  be_stable` /..  
-0000b290: 2020 2020 2020 3a66 756e 633a 6073 7461        :func:`sta
-0000b2a0: 626c 655f 7768 6973 7065 722e 7768 6973  ble_whisper.whis
-0000b2b0: 7065 725f 776f 7264 5f6c 6576 656c 2e74  per_word_level.t
-0000b2c0: 7261 6e73 6372 6962 655f 6d69 6e69 6d61  ranscribe_minima
-0000b2d0: 6c60 2f0d 0a20 2020 2020 2020 203a 6675  l`/..        :fu
-0000b2e0: 6e63 3a60 7374 6162 6c65 5f77 6869 7370  nc:`stable_whisp
-0000b2f0: 6572 2e6e 6f6e 5f77 6869 7370 6572 2e74  er.non_whisper.t
-0000b300: 7261 6e73 6372 6962 655f 616e 7960 202f  ranscribe_any` /
-0000b310: 203a 6675 6e63 3a60 7374 6162 6c65 5f77   :func:`stable_w
-0000b320: 6869 7370 6572 2e61 6c69 676e 6d65 6e74  hisper.alignment
-0000b330: 2e61 6c69 676e 600d 0a20 2020 2020 2020  .align`..       
-0000b340: 2069 6620 6060 7375 7070 7265 7373 5f73   if ``suppress_s
-0000b350: 696c 656e 6365 203d 2054 7275 6560 602e  ilence = True``.
-0000b360: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000b370: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
-0000b380: 6475 7220 3d20 6765 745f 6d69 6e5f 776f  dur = get_min_wo
-0000b390: 7264 5f64 7572 286d 696e 5f77 6f72 645f  rd_dur(min_word_
-0000b3a0: 6475 7229 0d0a 2020 2020 2020 2020 6966  dur)..        if
-0000b3b0: 2076 6164 3a0d 0a20 2020 2020 2020 2020   vad:..         
-0000b3c0: 2020 2061 7564 696f 203d 2061 7564 696f     audio = audio
-0000b3d0: 5f74 6f5f 7465 6e73 6f72 5f72 6573 616d  _to_tensor_resam
-0000b3e0: 706c 6528 6175 6469 6f2c 2073 616d 706c  ple(audio, sampl
-0000b3f0: 655f 7261 7465 2c20 5641 445f 5341 4d50  e_rate, VAD_SAMP
-0000b400: 4c45 5f52 4154 4553 5b30 5d29 0d0a 2020  LE_RATES[0])..  
-0000b410: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-0000b420: 5f72 6174 6520 3d20 5641 445f 5341 4d50  _rate = VAD_SAMP
-0000b430: 4c45 5f52 4154 4553 5b30 5d0d 0a20 2020  LE_RATES[0]..   
-0000b440: 2020 2020 2020 2020 2073 696c 656e 745f           silent_
-0000b450: 7469 6d69 6e67 7320 3d20 6765 745f 7661  timings = get_va
-0000b460: 645f 7369 6c65 6e63 655f 6675 6e63 280d  d_silence_func(.
-0000b470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b480: 206f 6e6e 783d 7661 645f 6f6e 6e78 2c0d   onnx=vad_onnx,.
-0000b490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b4a0: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-0000b4b0: 0d0a 2020 2020 2020 2020 2020 2020 2928  ..            )(
-0000b4c0: 6175 6469 6f2c 2073 7065 6563 685f 7468  audio, speech_th
-0000b4d0: 7265 7368 6f6c 643d 7661 645f 7468 7265  reshold=vad_thre
-0000b4e0: 7368 6f6c 642c 2073 723d 7361 6d70 6c65  shold, sr=sample
-0000b4f0: 5f72 6174 6529 0d0a 2020 2020 2020 2020  _rate)..        
-0000b500: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000b510: 2020 2073 696c 656e 745f 7469 6d69 6e67     silent_timing
-0000b520: 7320 3d20 6175 6469 6f32 7469 6d69 6e67  s = audio2timing
-0000b530: 7328 6175 6469 6f2c 2071 5f6c 6576 656c  s(audio, q_level
-0000b540: 733d 715f 6c65 7665 6c73 2c20 6b5f 7369  s=q_levels, k_si
-0000b550: 7a65 3d6b 5f73 697a 652c 2073 723d 7361  ze=k_size, sr=sa
-0000b560: 6d70 6c65 5f72 6174 6529 0d0a 2020 2020  mple_rate)..    
-0000b570: 2020 2020 6966 2073 696c 656e 745f 7469      if silent_ti
-0000b580: 6d69 6e67 7320 6973 204e 6f6e 653a 0d0a  mings is None:..
-0000b590: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b5a0: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
-0000b5b0: 2069 6620 6d69 6e5f 7369 6c65 6e63 655f   if min_silence_
-0000b5c0: 6475 723a 0d0a 2020 2020 2020 2020 2020  dur:..          
-0000b5d0: 2020 7369 6c65 6e74 5f74 696d 696e 6773    silent_timings
-0000b5e0: 203d 2066 696c 7465 725f 7469 6d69 6e67   = filter_timing
-0000b5f0: 7328 7369 6c65 6e74 5f74 696d 696e 6773  s(silent_timings
-0000b600: 2c20 6d69 6e5f 7369 6c65 6e63 655f 6475  , min_silence_du
-0000b610: 7229 0d0a 2020 2020 2020 2020 7365 6c66  r)..        self
-0000b620: 2e73 7570 7072 6573 735f 7369 6c65 6e63  .suppress_silenc
-0000b630: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-0000b640: 2a73 696c 656e 745f 7469 6d69 6e67 732c  *silent_timings,
-0000b650: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0000b660: 6e5f 776f 7264 5f64 7572 3d6d 696e 5f77  n_word_dur=min_w
-0000b670: 6f72 645f 6475 722c 0d0a 2020 2020 2020  ord_dur,..      
-0000b680: 2020 2020 2020 776f 7264 5f6c 6576 656c        word_level
-0000b690: 3d77 6f72 645f 6c65 7665 6c2c 0d0a 2020  =word_level,..  
-0000b6a0: 2020 2020 2020 2020 2020 6e6f 6e73 7065            nonspe
-0000b6b0: 6563 685f 6572 726f 723d 6e6f 6e73 7065  ech_error=nonspe
-0000b6c0: 6563 685f 6572 726f 722c 0d0a 2020 2020  ech_error,..    
-0000b6d0: 2020 2020 2020 2020 7573 655f 776f 7264          use_word
-0000b6e0: 5f70 6f73 6974 696f 6e3d 7573 655f 776f  _position=use_wo
-0000b6f0: 7264 5f70 6f73 6974 696f 6e2c 0d0a 2020  rd_position,..  
-0000b700: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-0000b710: 653d 7665 7262 6f73 650d 0a20 2020 2020  e=verbose..     
-0000b720: 2020 2029 0d0a 2020 2020 2020 2020 7365     )..        se
-0000b730: 6c66 2e75 7064 6174 655f 6e6f 6e73 7065  lf.update_nonspe
-0000b740: 6563 685f 7365 6374 696f 6e73 282a 7369  ech_sections(*si
-0000b750: 6c65 6e74 5f74 696d 696e 6773 290d 0a20  lent_timings).. 
-0000b760: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000b770: 6c66 0d0a 0d0a 2020 2020 6465 6620 6164  lf....    def ad
-0000b780: 6a75 7374 5f62 795f 7265 7375 6c74 280d  just_by_result(.
-0000b790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b7a0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-0000b7b0: 6f74 6865 725f 7265 7375 6c74 3a20 2257  other_result: "W
-0000b7c0: 6869 7370 6572 5265 7375 6c74 222c 0d0a  hisperResult",..
-0000b7d0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-0000b7e0: 776f 7264 5f64 7572 3a20 4f70 7469 6f6e  word_dur: Option
-0000b7f0: 616c 5b66 6c6f 6174 5d20 3d20 4e6f 6e65  al[float] = None
-0000b800: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-0000b810: 6572 626f 7365 3a20 626f 6f6c 203d 2046  erbose: bool = F
-0000b820: 616c 7365 0d0a 2020 2020 293a 0d0a 2020  alse..    ):..  
-0000b830: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000b840: 2020 204d 696e 696d 697a 6520 7468 6520     Minimize the 
-0000b850: 6475 7261 7469 6f6e 206f 6620 776f 7264  duration of word
-0000b860: 7320 7573 696e 6720 7469 6d65 7374 616d  s using timestam
-0000b870: 7073 206f 6620 616e 6f74 6865 7220 7265  ps of another re
-0000b880: 7375 6c74 2e0d 0a0d 0a20 2020 2020 2020  sult.....       
-0000b890: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-0000b8a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-0000b8b0: 0a20 2020 2020 2020 206f 7468 6572 5f72  .        other_r
-0000b8c0: 6573 756c 7420 3a20 2257 6869 7370 6572  esult : "Whisper
-0000b8d0: 5265 7375 6c74 220d 0a20 2020 2020 2020  Result"..       
-0000b8e0: 2020 2020 2054 696d 696e 6720 6461 7461       Timing data
-0000b8f0: 206f 6620 7468 6520 7361 6d65 2077 6f72   of the same wor
-0000b900: 6473 2069 6e20 6120 5768 6973 7065 7252  ds in a WhisperR
-0000b910: 6573 756c 7420 696e 7374 616e 6365 2e0d  esult instance..
-0000b920: 0a20 2020 2020 2020 206d 696e 5f77 6f72  .        min_wor
-0000b930: 645f 6475 7220 3a20 666c 6f61 7420 6f72  d_dur : float or
-0000b940: 204e 6f6e 652c 2064 6566 6175 6c74 204e   None, default N
-0000b950: 6f6e 6520 6d65 616e 696e 6720 7573 6520  one meaning use 
-0000b960: 6060 7374 6162 6c65 5f77 6869 7370 6572  ``stable_whisper
-0000b970: 2e64 6566 6175 6c74 2e44 4546 4155 4c54  .default.DEFAULT
-0000b980: 5f56 414c 5545 5360 600d 0a20 2020 2020  _VALUES``..     
-0000b990: 2020 2020 2020 2050 7265 7665 6e74 2063         Prevent c
-0000b9a0: 6861 6e67 6573 2074 6f20 7469 6d65 7374  hanges to timest
-0000b9b0: 616d 7073 2069 6620 7468 6520 7265 7375  amps if the resu
-0000b9c0: 6c74 616e 7420 776f 7264 2064 7572 6174  ltant word durat
-0000b9d0: 696f 6e20 6973 206c 6573 7320 7468 616e  ion is less than
-0000b9e0: 2060 606d 696e 5f77 6f72 645f 6475 7260   ``min_word_dur`
-0000b9f0: 602e 0d0a 2020 2020 2020 2020 7665 7262  `...        verb
-0000ba00: 6f73 6520 3a20 626f 6f6c 2c20 6465 6661  ose : bool, defa
-0000ba10: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
-0000ba20: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-0000ba30: 6f20 7072 696e 7420 6f75 7420 7468 6520  o print out the 
-0000ba40: 7469 6d65 7374 616d 7020 6368 616e 6765  timestamp change
-0000ba50: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
-0000ba60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000ba70: 2873 656c 662e 6861 735f 776f 7264 7320  (self.has_words 
-0000ba80: 616e 6420 6f74 6865 725f 7265 7375 6c74  and other_result
-0000ba90: 2e68 6173 5f77 6f72 6473 293a 0d0a 2020  .has_words):..  
-0000baa0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000bab0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-0000bac0: 726f 7228 2754 6869 7320 6f70 6572 6174  ror('This operat
-0000bad0: 696f 6e20 6361 6e20 6f6e 6c79 2062 6520  ion can only be 
-0000bae0: 7065 7266 6f72 6d65 6420 6f6e 2072 6573  performed on res
-0000baf0: 756c 7473 2077 6974 6820 776f 7264 2074  ults with word t
-0000bb00: 696d 6573 7461 6d70 7327 290d 0a20 2020  imestamps')..   
-0000bb10: 2020 2020 2061 7373 6572 7420 5b77 2e77       assert [w.w
-0000bb20: 6f72 6420 666f 7220 7720 696e 2073 656c  ord for w in sel
-0000bb30: 662e 616c 6c5f 776f 7264 7328 295d 203d  f.all_words()] =
-0000bb40: 3d20 5b77 2e77 6f72 6420 666f 7220 7720  = [w.word for w 
-0000bb50: 696e 206f 7468 6572 5f72 6573 756c 742e  in other_result.
-0000bb60: 616c 6c5f 776f 7264 7328 295d 2c20 5c0d  all_words()], \.
-0000bb70: 0a20 2020 2020 2020 2020 2020 2027 5468  .            'Th
-0000bb80: 6520 776f 7264 7320 696e 205b 6f74 6865  e words in [othe
-0000bb90: 725f 7265 7375 6c74 5d20 646f 206e 6f74  r_result] do not
-0000bba0: 206d 6174 6368 2074 6865 2063 7572 7265   match the curre
-0000bbb0: 6e74 2077 6f72 6473 2e27 0d0a 2020 2020  nt words.'..    
-0000bbc0: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
-0000bbd0: 203d 2067 6574 5f6d 696e 5f77 6f72 645f   = get_min_word_
-0000bbe0: 6475 7228 6d69 6e5f 776f 7264 5f64 7572  dur(min_word_dur
-0000bbf0: 290d 0a20 2020 2020 2020 2066 6f72 2077  )..        for w
-0000bc00: 6f72 642c 206f 7468 6572 5f77 6f72 6420  ord, other_word 
-0000bc10: 696e 207a 6970 2873 656c 662e 616c 6c5f  in zip(self.all_
-0000bc20: 776f 7264 7328 292c 206f 7468 6572 5f72  words(), other_r
-0000bc30: 6573 756c 742e 616c 6c5f 776f 7264 7328  esult.all_words(
-0000bc40: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-0000bc50: 2069 6620 776f 7264 2e65 6e64 203e 206f   if word.end > o
-0000bc60: 7468 6572 5f77 6f72 642e 7374 6172 743a  ther_word.start:
-0000bc70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bc80: 2020 6e65 775f 7374 6172 7420 3d20 6d61    new_start = ma
-0000bc90: 7828 776f 7264 2e73 7461 7274 2c20 6f74  x(word.start, ot
-0000bca0: 6865 725f 776f 7264 2e73 7461 7274 290d  her_word.start).
-0000bcb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bcc0: 206e 6577 5f65 6e64 203d 206d 696e 2877   new_end = min(w
-0000bcd0: 6f72 642e 656e 642c 206f 7468 6572 5f77  ord.end, other_w
-0000bce0: 6f72 642e 656e 6429 0d0a 2020 2020 2020  ord.end)..      
-0000bcf0: 2020 2020 2020 2020 2020 6966 206e 6577            if new
-0000bd00: 5f65 6e64 202d 206e 6577 5f73 7461 7274  _end - new_start
-0000bd10: 203e 3d20 6d69 6e5f 776f 7264 5f64 7572   >= min_word_dur
-0000bd20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bd30: 2020 2020 2020 206c 696e 6520 3d20 2727         line = ''
-0000bd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bd50: 2020 2020 2020 6966 2077 6f72 642e 7374        if word.st
-0000bd60: 6172 7420 213d 206e 6577 5f73 7461 7274  art != new_start
-0000bd70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bd80: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
-0000bd90: 7262 6f73 653a 0d0a 2020 2020 2020 2020  rbose:..        
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 6c69 6e65 202b 3d20 6627 5b53      line += f'[S
-0000bdc0: 7461 7274 3a7b 776f 7264 2e73 7461 7274  tart:{word.start
-0000bdd0: 3a2e 3366 7d2d 3e7b 6e65 775f 7374 6172  :.3f}->{new_star
-0000bde0: 743a 2e33 667d 5d20 270d 0a20 2020 2020  t:.3f}] '..     
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2077 6f72 642e 7374 6172 7420 3d20     word.start = 
-0000be10: 6e65 775f 7374 6172 740d 0a20 2020 2020  new_start..     
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000be30: 6620 776f 7264 2e65 6e64 2021 3d20 6e65  f word.end != ne
-0000be40: 775f 656e 643a 0d0a 2020 2020 2020 2020  w_end:..        
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 6966 2076 6572 626f 7365 3a0d 0a20 2020  if verbose:..   
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2020 2020 2020 2020 206c 696e 6520 2b3d           line +=
-0000be90: 2066 275b 456e 643a 7b77 6f72 642e 656e   f'[End:{word.en
-0000bea0: 643a 2e33 667d 2d3e 7b6e 6577 5f65 6e64  d:.3f}->{new_end
-0000beb0: 3a2e 3366 7d5d 2020 270d 0a20 2020 2020  :.3f}]  '..     
-0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 2020 2077 6f72 642e 656e 6420 3d20 6e65     word.end = ne
-0000bee0: 775f 656e 640d 0a20 2020 2020 2020 2020  w_end..         
-0000bef0: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-0000bf00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000bf10: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000bf20: 6e74 2866 277b 6c69 6e65 7d22 7b77 6f72  nt(f'{line}"{wor
-0000bf30: 642e 776f 7264 7d22 2729 0d0a 0d0a 2020  d.word}"')....  
-0000bf40: 2020 6465 6620 7265 6173 7369 676e 5f69    def reassign_i
-0000bf50: 6473 2873 656c 662c 206f 6e6c 795f 7365  ds(self, only_se
-0000bf60: 676d 656e 7473 3a20 626f 6f6c 203d 2046  gments: bool = F
-0000bf70: 616c 7365 2c20 7374 6172 743a 204f 7074  alse, start: Opt
-0000bf80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0000bf90: 6529 3a0d 0a20 2020 2020 2020 2066 6f72  e):..        for
-0000bfa0: 2069 2c20 7320 696e 2065 6e75 6d65 7261   i, s in enumera
-0000bfb0: 7465 2873 656c 662e 7365 676d 656e 7473  te(self.segments
-0000bfc0: 5b73 7461 7274 3a5d 2c20 7374 6172 7420  [start:], start 
-0000bfd0: 6f72 2030 293a 0d0a 2020 2020 2020 2020  or 0):..        
-0000bfe0: 2020 2020 732e 6964 203d 2069 0d0a 2020      s.id = i..  
-0000bff0: 2020 2020 2020 2020 2020 732e 7265 7375            s.resu
-0000c000: 6c74 203d 2073 656c 660d 0a20 2020 2020  lt = self..     
-0000c010: 2020 2020 2020 2069 6620 6e6f 7420 6f6e         if not on
-0000c020: 6c79 5f73 6567 6d65 6e74 733a 0d0a 2020  ly_segments:..  
-0000c030: 2020 2020 2020 2020 2020 2020 2020 732e                s.
-0000c040: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
-0000c050: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
-0000c060: 5f6e 6f5f 776f 7264 5f73 6567 6d65 6e74  _no_word_segment
-0000c070: 7328 7365 6c66 2c20 6967 6e6f 7265 5f6f  s(self, ignore_o
-0000c080: 7269 3d46 616c 7365 2c20 7265 6173 7369  ri=False, reassi
-0000c090: 676e 5f69 6473 3a20 626f 6f6c 203d 2054  gn_ids: bool = T
-0000c0a0: 7275 6529 3a0d 0a20 2020 2020 2020 2066  rue):..        f
-0000c0b0: 6f72 2069 2069 6e20 7265 7665 7273 6564  or i in reversed
-0000c0c0: 2872 616e 6765 286c 656e 2873 656c 662e  (range(len(self.
-0000c0d0: 7365 676d 656e 7473 2929 293a 0d0a 2020  segments))):..  
-0000c0e0: 2020 2020 2020 2020 2020 6966 2028 6967            if (ig
-0000c0f0: 6e6f 7265 5f6f 7269 206f 7220 7365 6c66  nore_ori or self
-0000c100: 2e73 6567 6d65 6e74 735b 695d 2e6f 7269  .segments[i].ori
-0000c110: 5f68 6173 5f77 6f72 6473 2920 616e 6420  _has_words) and 
-0000c120: 6e6f 7420 7365 6c66 2e73 6567 6d65 6e74  not self.segment
-0000c130: 735b 695d 2e68 6173 5f77 6f72 6473 3a0d  s[i].has_words:.
-0000c140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c150: 2064 656c 2073 656c 662e 7365 676d 656e   del self.segmen
-0000c160: 7473 5b69 5d0d 0a20 2020 2020 2020 2069  ts[i]..        i
-0000c170: 6620 7265 6173 7369 676e 5f69 6473 3a0d  f reassign_ids:.
-0000c180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c190: 662e 7265 6173 7369 676e 5f69 6473 2829  f.reassign_ids()
-0000c1a0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-0000c1b0: 6c6f 636b 6564 5f69 6e64 6963 6573 2873  locked_indices(s
-0000c1c0: 656c 6629 3a0d 0a20 2020 2020 2020 206c  elf):..        l
-0000c1d0: 6f63 6b65 645f 696e 6469 6365 7320 3d20  ocked_indices = 
-0000c1e0: 5b69 0d0a 2020 2020 2020 2020 2020 2020  [i..            
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000c200: 7220 692c 2028 6c65 6674 2c20 7269 6768  r i, (left, righ
-0000c210: 7429 2069 6e20 656e 756d 6572 6174 6528  t) in enumerate(
-0000c220: 7a69 7028 7365 6c66 2e73 6567 6d65 6e74  zip(self.segment
-0000c230: 735b 313a 5d2c 2073 656c 662e 7365 676d  s[1:], self.segm
-0000c240: 656e 7473 5b3a 2d31 5d29 290d 0a20 2020  ents[:-1]))..   
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 2020 2020 2020 2069 6620 6c65 6674 2e6c         if left.l
-0000c270: 6566 745f 6c6f 636b 6564 206f 7220 7269  eft_locked or ri
-0000c280: 6768 742e 7269 6768 745f 6c6f 636b 6564  ght.right_locked
-0000c290: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-0000c2a0: 6e20 6c6f 636b 6564 5f69 6e64 6963 6573  n locked_indices
-0000c2b0: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-0000c2c0: 6761 7073 2873 656c 662c 2061 735f 6e64  gaps(self, as_nd
-0000c2d0: 6172 7261 793d 4661 6c73 6529 3a0d 0a20  array=False):.. 
-0000c2e0: 2020 2020 2020 2073 5f74 7320 3d20 6e70         s_ts = np
-0000c2f0: 2e61 7272 6179 285b 732e 7374 6172 7420  .array([s.start 
-0000c300: 666f 7220 7320 696e 2073 656c 662e 7365  for s in self.se
-0000c310: 676d 656e 7473 5d29 0d0a 2020 2020 2020  gments])..      
-0000c320: 2020 655f 7473 203d 206e 702e 6172 7261    e_ts = np.arra
-0000c330: 7928 5b73 2e65 6e64 2066 6f72 2073 2069  y([s.end for s i
-0000c340: 6e20 7365 6c66 2e73 6567 6d65 6e74 735d  n self.segments]
-0000c350: 290d 0a20 2020 2020 2020 2067 6170 203d  )..        gap =
-0000c360: 2073 5f74 735b 313a 5d20 2d20 655f 7473   s_ts[1:] - e_ts
-0000c370: 5b3a 2d31 5d0d 0a20 2020 2020 2020 2072  [:-1]..        r
-0000c380: 6574 7572 6e20 6761 7020 6966 2061 735f  eturn gap if as_
-0000c390: 6e64 6172 7261 7920 656c 7365 2067 6170  ndarray else gap
-0000c3a0: 2e74 6f6c 6973 7428 290d 0a0d 0a20 2020  .tolist()....   
-0000c3b0: 2064 6566 2067 6574 5f67 6170 5f69 6e64   def get_gap_ind
-0000c3c0: 6963 6573 2873 656c 662c 206d 696e 5f67  ices(self, min_g
-0000c3d0: 6170 3a20 666c 6f61 7420 3d20 302e 3129  ap: float = 0.1)
-0000c3e0: 3a20 2023 2066 6f72 206d 6572 6769 6e67  :  # for merging
-0000c3f0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0000c400: 2873 656c 662e 7365 676d 656e 7473 2920  (self.segments) 
-0000c410: 3c20 323a 0d0a 2020 2020 2020 2020 2020  < 2:..          
-0000c420: 2020 7265 7475 726e 205b 5d0d 0a20 2020    return []..   
-0000c430: 2020 2020 2069 6620 6d69 6e5f 6761 7020       if min_gap 
-0000c440: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-0000c450: 2020 2020 2020 6d69 6e5f 6761 7020 3d20        min_gap = 
-0000c460: 300d 0a20 2020 2020 2020 2069 6e64 6963  0..        indic
-0000c470: 6573 203d 2028 7365 6c66 2e67 6574 5f67  es = (self.get_g
-0000c480: 6170 7328 5472 7565 2920 3c3d 206d 696e  aps(True) <= min
-0000c490: 5f67 6170 292e 6e6f 6e7a 6572 6f28 295b  _gap).nonzero()[
-0000c4a0: 305d 2e74 6f6c 6973 7428 290d 0a20 2020  0].tolist()..   
-0000c4b0: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
-0000c4c0: 6564 2873 6574 2869 6e64 6963 6573 2920  ed(set(indices) 
-0000c4d0: 2d20 7365 7428 7365 6c66 2e67 6574 5f6c  - set(self.get_l
-0000c4e0: 6f63 6b65 645f 696e 6469 6365 7328 2929  ocked_indices())
-0000c4f0: 290d 0a0d 0a20 2020 2064 6566 2067 6574  )....    def get
-0000c500: 5f70 756e 6374 7561 7469 6f6e 5f69 6e64  _punctuation_ind
-0000c510: 6963 6573 2873 656c 662c 2070 756e 6374  ices(self, punct
-0000c520: 7561 7469 6f6e 3a20 556e 696f 6e5b 4c69  uation: Union[Li
-0000c530: 7374 5b73 7472 5d2c 204c 6973 745b 5475  st[str], List[Tu
-0000c540: 706c 655b 7374 722c 2073 7472 5d5d 2c20  ple[str, str]], 
-0000c550: 7374 725d 293a 2020 2320 666f 7220 6d65  str]):  # for me
-0000c560: 7267 696e 670d 0a20 2020 2020 2020 2069  rging..        i
-0000c570: 6620 6c65 6e28 7365 6c66 2e73 6567 6d65  f len(self.segme
-0000c580: 6e74 7329 203c 2032 3a0d 0a20 2020 2020  nts) < 2:..     
-0000c590: 2020 2020 2020 2072 6574 7572 6e20 5b5d         return []
-0000c5a0: 0d0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-0000c5b0: 6e73 7461 6e63 6528 7075 6e63 7475 6174  nstance(punctuat
-0000c5c0: 696f 6e2c 2073 7472 293a 0d0a 2020 2020  ion, str):..    
-0000c5d0: 2020 2020 2020 2020 7075 6e63 7475 6174          punctuat
-0000c5e0: 696f 6e20 3d20 5b70 756e 6374 7561 7469  ion = [punctuati
-0000c5f0: 6f6e 5d0d 0a20 2020 2020 2020 2069 6e64  on]..        ind
-0000c600: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
-0000c610: 2020 2066 6f72 2070 2069 6e20 7075 6e63     for p in punc
-0000c620: 7475 6174 696f 6e3a 0d0a 2020 2020 2020  tuation:..      
-0000c630: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000c640: 6e63 6528 702c 2073 7472 293a 0d0a 2020  nce(p, str):..  
-0000c650: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000c660: 7220 692c 2073 2069 6e20 656e 756d 6572  r i, s in enumer
-0000c670: 6174 6528 7365 6c66 2e73 6567 6d65 6e74  ate(self.segment
-0000c680: 735b 3a2d 315d 293a 0d0a 2020 2020 2020  s[:-1]):..      
-0000c690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c6a0: 2073 2e74 6578 742e 656e 6473 7769 7468   s.text.endswith
-0000c6b0: 2870 293a 0d0a 2020 2020 2020 2020 2020  (p):..          
-0000c6c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000c6d0: 6469 6365 732e 6170 7065 6e64 2869 290d  dices.append(i).
-0000c6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c6f0: 2020 2020 2065 6c69 6620 6920 213d 2030       elif i != 0
-0000c700: 2061 6e64 2073 2e74 6578 742e 7374 6172   and s.text.star
-0000c710: 7473 7769 7468 2870 293a 0d0a 2020 2020  tswith(p):..    
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2020 2020 696e 6469 6365 732e 6170 7065      indices.appe
-0000c740: 6e64 2869 2d31 290d 0a20 2020 2020 2020  nd(i-1)..       
-0000c750: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000c760: 2020 2020 2020 2020 2020 2020 656e 6469              endi
-0000c770: 6e67 2c20 6265 6769 6e6e 696e 6720 3d20  ng, beginning = 
-0000c780: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-0000c790: 2020 2069 6e64 6963 6573 2e65 7874 656e     indices.exten
-0000c7a0: 6428 5b69 2066 6f72 2069 2c20 2873 302c  d([i for i, (s0,
-0000c7b0: 2073 3129 2069 6e20 656e 756d 6572 6174   s1) in enumerat
-0000c7c0: 6528 7a69 7028 7365 6c66 2e73 6567 6d65  e(zip(self.segme
-0000c7d0: 6e74 735b 3a2d 315d 2c20 7365 6c66 2e73  nts[:-1], self.s
-0000c7e0: 6567 6d65 6e74 735b 313a 5d29 290d 0a20  egments[1:])).. 
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000c810: 6620 7330 2e74 6578 742e 656e 6473 7769  f s0.text.endswi
-0000c820: 7468 2865 6e64 696e 6729 2061 6e64 2073  th(ending) and s
-0000c830: 312e 7465 7874 2e73 7461 7274 7377 6974  1.text.startswit
-0000c840: 6828 6265 6769 6e6e 696e 6729 5d29 0d0a  h(beginning)])..
-0000c850: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000c860: 2073 6f72 7465 6428 7365 7428 696e 6469   sorted(set(indi
-0000c870: 6365 7329 202d 2073 6574 2873 656c 662e  ces) - set(self.
-0000c880: 6765 745f 6c6f 636b 6564 5f69 6e64 6963  get_locked_indic
-0000c890: 6573 2829 2929 0d0a 0d0a 2020 2020 6465  es()))....    de
-0000c8a0: 6620 616c 6c5f 776f 7264 7328 7365 6c66  f all_words(self
-0000c8b0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-0000c8c0: 726e 206c 6973 7428 6368 6169 6e2e 6672  rn list(chain.fr
-0000c8d0: 6f6d 5f69 7465 7261 626c 6528 732e 776f  om_iterable(s.wo
-0000c8e0: 7264 7320 666f 7220 7320 696e 2073 656c  rds for s in sel
-0000c8f0: 662e 7365 676d 656e 7473 2929 0d0a 0d0a  f.segments))....
-0000c900: 2020 2020 6465 6620 616c 6c5f 776f 7264      def all_word
-0000c910: 735f 6f72 5f73 6567 6d65 6e74 7328 7365  s_or_segments(se
-0000c920: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-0000c930: 7475 726e 2073 656c 662e 616c 6c5f 776f  turn self.all_wo
-0000c940: 7264 7328 2920 6966 2073 656c 662e 6861  rds() if self.ha
-0000c950: 735f 776f 7264 7320 656c 7365 2073 656c  s_words else sel
-0000c960: 662e 7365 676d 656e 7473 0d0a 0d0a 2020  f.segments....  
-0000c970: 2020 6465 6620 616c 6c5f 776f 7264 735f    def all_words_
-0000c980: 6279 5f6c 6f63 6b28 7365 6c66 2c20 6f6e  by_lock(self, on
-0000c990: 6c79 5f74 6578 743a 2062 6f6f 6c20 3d20  ly_text: bool = 
-0000c9a0: 5472 7565 2c20 6279 5f73 6567 6d65 6e74  True, by_segment
-0000c9b0: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-0000c9c0: 696e 636c 7564 655f 7369 6e67 6c65 3a20  include_single: 
-0000c9d0: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
-0000c9e0: 2020 2020 2020 2020 6966 2062 795f 7365          if by_se
-0000c9f0: 676d 656e 743a 0d0a 2020 2020 2020 2020  gment:..        
-0000ca00: 2020 2020 7265 7475 726e 205b 0d0a 2020      return [..  
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ca20: 676d 656e 742e 776f 7264 735f 6279 5f6c  gment.words_by_l
-0000ca30: 6f63 6b28 6f6e 6c79 5f74 6578 743d 6f6e  ock(only_text=on
-0000ca40: 6c79 5f74 6578 742c 2069 6e63 6c75 6465  ly_text, include
-0000ca50: 5f73 696e 676c 653d 696e 636c 7564 655f  _single=include_
-0000ca60: 7369 6e67 6c65 290d 0a20 2020 2020 2020  single)..       
-0000ca70: 2020 2020 2020 2020 2066 6f72 2073 6567           for seg
-0000ca80: 6d65 6e74 2069 6e20 7365 6c66 2e73 6567  ment in self.seg
-0000ca90: 6d65 6e74 730d 0a20 2020 2020 2020 2020  ments..         
-0000caa0: 2020 205d 0d0a 2020 2020 2020 2020 7265     ]..        re
-0000cab0: 7475 726e 205f 776f 7264 735f 6279 5f6c  turn _words_by_l
-0000cac0: 6f63 6b28 7365 6c66 2e61 6c6c 5f77 6f72  ock(self.all_wor
-0000cad0: 6473 2829 2c20 6f6e 6c79 5f74 6578 743d  ds(), only_text=
-0000cae0: 6f6e 6c79 5f74 6578 742c 2069 6e63 6c75  only_text, inclu
-0000caf0: 6465 5f73 696e 676c 653d 696e 636c 7564  de_single=includ
-0000cb00: 655f 7369 6e67 6c65 290d 0a0d 0a20 2020  e_single)....   
-0000cb10: 2064 6566 2061 6c6c 5f74 6f6b 656e 7328   def all_tokens(
-0000cb20: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-0000cb30: 7265 7475 726e 206c 6973 7428 6368 6169  return list(chai
-0000cb40: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
-0000cb50: 732e 746f 6b65 6e73 2066 6f72 2073 2069  s.tokens for s i
-0000cb60: 6e20 7365 6c66 2e61 6c6c 5f77 6f72 6473  n self.all_words
-0000cb70: 2829 2929 0d0a 0d0a 2020 2020 6465 6620  ()))....    def 
-0000cb80: 746f 5f64 6963 7428 7365 6c66 2c20 6b65  to_dict(self, ke
-0000cb90: 6570 5f6f 7269 673a 2062 6f6f 6c20 3d20  ep_orig: bool = 
-0000cba0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-0000cbb0: 6f72 695f 6469 6374 203d 2073 656c 662e  ori_dict = self.
-0000cbc0: 6f72 695f 6469 6374 2069 6620 6b65 6570  ori_dict if keep
-0000cbd0: 5f6f 7269 6720 656c 7365 207b 7d0d 0a20  _orig else {}.. 
-0000cbe0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0000cbf0: 6374 2874 6578 743d 7365 6c66 2e74 6578  ct(text=self.tex
-0000cc00: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-0000cc10: 2020 2020 2020 2020 7365 676d 656e 7473          segments
-0000cc20: 3d73 656c 662e 7365 676d 656e 7473 5f74  =self.segments_t
-0000cc30: 6f5f 6469 6374 7328 292c 0d0a 2020 2020  o_dicts(),..    
-0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc50: 6c61 6e67 7561 6765 3d73 656c 662e 6c61  language=self.la
-0000cc60: 6e67 7561 6765 2c0d 0a20 2020 2020 2020  nguage,..       
-0000cc70: 2020 2020 2020 2020 2020 2020 206f 7269               ori
-0000cc80: 5f64 6963 743d 6f72 695f 6469 6374 2c0d  _dict=ori_dict,.
-0000cc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cca0: 2020 2020 2072 6567 726f 7570 5f68 6973       regroup_his
-0000ccb0: 746f 7279 3d73 656c 662e 5f72 6567 726f  tory=self._regro
-0000ccc0: 7570 5f68 6973 746f 7279 2c0d 0a20 2020  up_history,..   
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cce0: 206e 6f6e 7370 6565 6368 5f73 6563 7469   nonspeech_secti
-0000ccf0: 6f6e 733d 7365 6c66 2e5f 6e6f 6e73 7065  ons=self._nonspe
-0000cd00: 6563 685f 7365 6374 696f 6e73 290d 0a0d  ech_sections)...
-0000cd10: 0a20 2020 2064 6566 2073 6567 6d65 6e74  .    def segment
-0000cd20: 735f 746f 5f64 6963 7473 2873 656c 662c  s_to_dicts(self,
-0000cd30: 2072 6576 6572 7365 5f74 6578 743a 2055   reverse_text: U
-0000cd40: 6e69 6f6e 5b62 6f6f 6c2c 2074 7570 6c65  nion[bool, tuple
-0000cd50: 5d20 3d20 4661 6c73 6529 3a0d 0a20 2020  ] = False):..   
-0000cd60: 2020 2020 2072 6574 7572 6e20 5b73 2e74       return [s.t
-0000cd70: 6f5f 6469 6374 2872 6576 6572 7365 5f74  o_dict(reverse_t
-0000cd80: 6578 743d 7265 7665 7273 655f 7465 7874  ext=reverse_text
-0000cd90: 2920 666f 7220 7320 696e 2073 656c 662e  ) for s in self.
-0000cda0: 7365 676d 656e 7473 5d0d 0a0d 0a20 2020  segments]....   
-0000cdb0: 2064 6566 205f 7370 6c69 745f 7365 676d   def _split_segm
-0000cdc0: 656e 7473 2873 656c 662c 2067 6574 5f69  ents(self, get_i
-0000cdd0: 6e64 6963 6573 2c20 6172 6773 3a20 6c69  ndices, args: li
-0000cde0: 7374 203d 204e 6f6e 652c 202a 2c20 6c6f  st = None, *, lo
-0000cdf0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-0000ce00: 2c20 6e65 776c 696e 653a 2062 6f6f 6c20  , newline: bool 
-0000ce10: 3d20 4661 6c73 6529 3a0d 0a20 2020 2020  = False):..     
-0000ce20: 2020 2069 6620 6172 6773 2069 7320 4e6f     if args is No
-0000ce30: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000ce40: 2061 7267 7320 3d20 5b5d 0d0a 2020 2020   args = []..    
-0000ce50: 2020 2020 6e6f 5f77 6f72 6473 203d 2046      no_words = F
-0000ce60: 616c 7365 0d0a 2020 2020 2020 2020 666f  alse..        fo
-0000ce70: 7220 6920 696e 2072 6576 6572 7365 6428  r i in reversed(
-0000ce80: 7261 6e67 6528 302c 206c 656e 2873 656c  range(0, len(sel
-0000ce90: 662e 7365 676d 656e 7473 2929 293a 0d0a  f.segments))):..
-0000cea0: 2020 2020 2020 2020 2020 2020 6e6f 5f77              no_w
-0000ceb0: 6f72 6473 203d 206e 6f5f 776f 7264 7320  ords = no_words 
-0000cec0: 6f72 206e 6f74 2073 656c 662e 7365 676d  or not self.segm
-0000ced0: 656e 7473 5b69 5d2e 6861 735f 776f 7264  ents[i].has_word
-0000cee0: 730d 0a20 2020 2020 2020 2020 2020 2069  s..            i
-0000cef0: 6e64 6963 6573 203d 2073 6f72 7465 6428  ndices = sorted(
-0000cf00: 7365 7428 6765 745f 696e 6469 6365 7328  set(get_indices(
-0000cf10: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
-0000cf20: 2c20 2a61 7267 7329 2929 0d0a 2020 2020  , *args)))..    
-0000cf30: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0000cf40: 6e64 6963 6573 3a0d 0a20 2020 2020 2020  ndices:..       
-0000cf50: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000cf60: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
-0000cf70: 6620 6e65 776c 696e 653a 0d0a 2020 2020  f newline:..    
-0000cf80: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000cf90: 6e64 6963 6573 5b2d 315d 203d 3d20 6c65  ndices[-1] == le
-0000cfa0: 6e28 7365 6c66 2e73 6567 6d65 6e74 735b  n(self.segments[
-0000cfb0: 695d 2e77 6f72 6473 2920 2d20 313a 0d0a  i].words) - 1:..
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 6465 6c20 696e 6469 6365 735b      del indices[
-0000cfe0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
-0000cff0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000d000: 696e 6469 6365 733a 0d0a 2020 2020 2020  indices:..      
-0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d020: 2020 636f 6e74 696e 7565 0d0a 0d0a 2020    continue....  
-0000d030: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000d040: 7220 776f 7264 5f69 6478 2069 6e20 696e  r word_idx in in
-0000d050: 6469 6365 733a 0d0a 2020 2020 2020 2020  dices:..        
-0000d060: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000d070: 656c 662e 7365 676d 656e 7473 5b69 5d2e  elf.segments[i].
-0000d080: 776f 7264 735b 776f 7264 5f69 6478 5d2e  words[word_idx].
-0000d090: 776f 7264 2e65 6e64 7377 6974 6828 275c  word.endswith('\
-0000d0a0: 6e27 293a 0d0a 2020 2020 2020 2020 2020  n'):..          
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000d0c0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-0000d0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d0e0: 2e73 6567 6d65 6e74 735b 695d 2e77 6f72  .segments[i].wor
-0000d0f0: 6473 5b77 6f72 645f 6964 785d 2e77 6f72  ds[word_idx].wor
-0000d100: 6420 2b3d 2027 5c6e 270d 0a20 2020 2020  d += '\n'..     
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d120: 6620 6c6f 636b 3a0d 0a20 2020 2020 2020  f lock:..       
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2073 656c 662e 7365 676d 656e 7473 5b69   self.segments[i
-0000d150: 5d2e 776f 7264 735b 776f 7264 5f69 6478  ].words[word_idx
-0000d160: 5d2e 6c6f 636b 5f72 6967 6874 2829 0d0a  ].lock_right()..
-0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 2020 2020 2020 2020 6966 2077 6f72 645f          if word_
-0000d190: 6964 7820 2b20 3120 3c20 6c65 6e28 7365  idx + 1 < len(se
-0000d1a0: 6c66 2e73 6567 6d65 6e74 735b 695d 2e77  lf.segments[i].w
-0000d1b0: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1d0: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-0000d1e0: 735b 695d 2e77 6f72 6473 5b77 6f72 645f  s[i].words[word_
-0000d1f0: 6964 782b 315d 2e6c 6f63 6b5f 6c65 6674  idx+1].lock_left
-0000d200: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000d210: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000d220: 2020 2020 2020 206e 6577 5f73 6567 6d65         new_segme
-0000d230: 6e74 7320 3d20 7365 6c66 2e73 6567 6d65  nts = self.segme
-0000d240: 6e74 735b 695d 2e73 706c 6974 2869 6e64  nts[i].split(ind
-0000d250: 6963 6573 290d 0a20 2020 2020 2020 2020  ices)..         
-0000d260: 2020 2020 2020 2069 6620 6c6f 636b 3a0d         if lock:.
-0000d270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d280: 2020 2020 2066 6f72 2073 2069 6e20 6e65       for s in ne
-0000d290: 775f 7365 676d 656e 7473 3a0d 0a20 2020  w_segments:..   
-0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2b0: 2020 2020 2069 6620 7320 3d3d 206e 6577       if s == new
-0000d2c0: 5f73 6567 6d65 6e74 735b 305d 3a0d 0a20  _segments[0]:.. 
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2020 2020 2020 2073 2e6c 6f63             s.loc
-0000d2f0: 6b5f 7269 6768 7428 290d 0a20 2020 2020  k_right()..     
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2020 2065 6c69 6620 7320 3d3d 206e 6577     elif s == new
-0000d320: 5f73 6567 6d65 6e74 735b 2d31 5d3a 0d0a  _segments[-1]:..
-0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d340: 2020 2020 2020 2020 2020 2020 732e 6c6f              s.lo
-0000d350: 636b 5f6c 6566 7428 290d 0a20 2020 2020  ck_left()..     
-0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d370: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 732e 6c6f 636b 5f62 6f74        s.lock_bot
-0000d3a0: 6828 290d 0a20 2020 2020 2020 2020 2020  h()..           
-0000d3b0: 2020 2020 2064 656c 2073 656c 662e 7365       del self.se
-0000d3c0: 676d 656e 7473 5b69 5d0d 0a20 2020 2020  gments[i]..     
-0000d3d0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-0000d3e0: 2069 6e20 7265 7665 7273 6564 286e 6577   in reversed(new
-0000d3f0: 5f73 6567 6d65 6e74 7329 3a0d 0a20 2020  _segments):..   
-0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d410: 2073 656c 662e 7365 676d 656e 7473 2e69   self.segments.i
-0000d420: 6e73 6572 7428 692c 2073 290d 0a20 2020  nsert(i, s)..   
-0000d430: 2020 2020 2069 6620 6e6f 5f77 6f72 6473       if no_words
-0000d440: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
-0000d450: 6172 6e69 6e67 732e 7761 726e 2827 466f  arnings.warn('Fo
-0000d460: 756e 6420 7365 676d 656e 7428 7329 2077  und segment(s) w
-0000d470: 6974 686f 7574 2077 6f72 6420 7469 6d69  ithout word timi
-0000d480: 6e67 732e 2054 6865 7365 2073 6567 6d65  ngs. These segme
-0000d490: 6e74 2873 2920 6361 6e6e 6f74 2062 6520  nt(s) cannot be 
-0000d4a0: 7370 6c69 742e 2729 0d0a 2020 2020 2020  split.')..      
-0000d4b0: 2020 7365 6c66 2e72 656d 6f76 655f 6e6f    self.remove_no
-0000d4c0: 5f77 6f72 645f 7365 676d 656e 7473 2829  _word_segments()
-0000d4d0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6572  ....    def _mer
-0000d4e0: 6765 5f73 6567 6d65 6e74 7328 7365 6c66  ge_segments(self
-0000d4f0: 2c20 696e 6469 6365 733a 204c 6973 745b  , indices: List[
-0000d500: 696e 745d 2c0d 0a20 2020 2020 2020 2020  int],..         
-0000d510: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000d520: 2c20 6d61 785f 776f 7264 733a 2069 6e74  , max_words: int
-0000d530: 203d 204e 6f6e 652c 206d 6178 5f63 6861   = None, max_cha
-0000d540: 7273 3a20 696e 7420 3d20 4e6f 6e65 2c20  rs: int = None, 
-0000d550: 6973 5f73 756d 5f6d 6178 3a20 626f 6f6c  is_sum_max: bool
-0000d560: 203d 2046 616c 7365 2c20 6c6f 636b 3a20   = False, lock: 
-0000d570: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
-0000d580: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
-0000d590: 6e64 6963 6573 2920 3d3d 2030 3a0d 0a20  ndices) == 0:.. 
-0000d5a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000d5b0: 6e0d 0a20 2020 2020 2020 2066 6f72 2069  n..        for i
-0000d5c0: 2069 6e20 7265 7665 7273 6564 2869 6e64   in reversed(ind
-0000d5d0: 6963 6573 293a 0d0a 2020 2020 2020 2020  ices):..        
-0000d5e0: 2020 2020 7365 6720 3d20 7365 6c66 2e73      seg = self.s
-0000d5f0: 6567 6d65 6e74 735b 695d 0d0a 2020 2020  egments[i]..    
-0000d600: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
+00009210: 2020 2020 2070 7269 6e74 2870 6172 745f       print(part_
+00009220: 696e 666f 2c20 656e 643d 275c 6e5c 6e27  info, end='\n\n'
+00009230: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00009240: 2064 6174 6120 3d20 7365 6c66 2e74 6f5f   data = self.to_
+00009250: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
+00009260: 2020 2020 6966 2063 6865 636b 5f73 6f72      if check_sor
+00009270: 7465 6420 6973 2054 7275 653a 0d0a 2020  ted is True:..  
+00009280: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00009290: 6973 6520 556e 736f 7274 6564 4578 6365  ise UnsortedExce
+000092a0: 7074 696f 6e28 6461 7461 3d64 6174 6129  ption(data=data)
+000092b0: 0d0a 2020 2020 2020 2020 2020 2020 7761  ..            wa
+000092c0: 726e 696e 6773 2e77 6172 6e28 2754 696d  rnings.warn('Tim
+000092d0: 6573 7461 6d70 7320 6172 6520 6e6f 7420  estamps are not 
+000092e0: 696e 2061 7363 656e 6469 6e67 206f 7264  in ascending ord
+000092f0: 6572 2e20 270d 0a20 2020 2020 2020 2020  er. '..         
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2027 4966 2064 6174 6120 6973 2070 726f   'If data is pro
+00009320: 6475 6365 6420 6279 2053 7461 626c 652d  duced by Stable-
+00009330: 7473 2c20 706c 6561 7365 2073 7562 6d69  ts, please submi
+00009340: 7420 616e 2069 7373 7565 2077 6974 6820  t an issue with 
+00009350: 7468 6520 7361 7665 6420 6461 7461 2e27  the saved data.'
+00009360: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00009370: 6176 655f 6173 5f6a 736f 6e28 6461 7461  ave_as_json(data
+00009380: 2c20 6368 6563 6b5f 736f 7274 6564 290d  , check_sorted).
+00009390: 0a0d 0a20 2020 2064 6566 2075 7064 6174  ...    def updat
+000093a0: 655f 616c 6c5f 7365 6773 5f77 6974 685f  e_all_segs_with_
+000093b0: 776f 7264 7328 7365 6c66 293a 0d0a 2020  words(self):..  
+000093c0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+000093d0: 6172 6e28 2741 7474 7269 6275 7465 7320  arn('Attributes 
+000093e0: 7468 6174 2072 6571 7569 7265 6420 7570  that required up
+000093f0: 6461 7469 6e67 2061 7265 206e 6f77 2070  dating are now p
+00009400: 726f 7065 7274 6965 7320 6261 7365 6420  roperties based 
+00009410: 6f6e 2074 6865 2060 6077 6f72 6473 6060  on the ``words``
+00009420: 2065 7863 6570 7420 666f 7220 6060 6964   except for ``id
+00009430: 6060 2e20 270d 0a20 2020 2020 2020 2020  ``. '..         
+00009440: 2020 2020 2020 2020 2020 2020 2027 6060               '``
+00009450: 7570 6461 7465 5f61 6c6c 5f73 6567 735f  update_all_segs_
+00009460: 7769 7468 5f77 6f72 6473 2829 6060 2069  with_words()`` i
+00009470: 7320 6465 7072 6563 6174 6564 2061 6e64  s deprecated and
+00009480: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
+00009490: 2069 6e20 6675 7475 7265 2076 6572 7369   in future versi
+000094a0: 6f6e 732e 2027 0d0a 2020 2020 2020 2020  ons. '..        
+000094b0: 2020 2020 2020 2020 2020 2020 2020 2755                'U
+000094c0: 7365 2060 602e 7265 6173 7369 676e 5f69  se ``.reassign_i
+000094d0: 6473 2829 6060 2074 6f20 6d61 6e75 616c  ds()`` to manual
+000094e0: 6c79 2075 7064 6174 6520 6964 7327 2c0d  ly update ids',.
+000094f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009500: 2020 2020 2020 2073 7461 636b 6c65 7665         stackleve
+00009510: 6c3d 3229 0d0a 2020 2020 2020 2020 7365  l=2)..        se
+00009520: 6c66 2e72 6561 7373 6967 6e5f 6964 7328  lf.reassign_ids(
+00009530: 290d 0a0d 0a20 2020 2064 6566 2075 7064  )....    def upd
+00009540: 6174 655f 6e6f 6e73 7065 6563 685f 7365  ate_nonspeech_se
+00009550: 6374 696f 6e73 2873 656c 662c 2073 696c  ctions(self, sil
+00009560: 656e 745f 7374 6172 7473 2c20 7369 6c65  ent_starts, sile
+00009570: 6e74 5f65 6e64 7329 3a0d 0a20 2020 2020  nt_ends):..     
+00009580: 2020 2073 656c 662e 5f6e 6f6e 7370 6565     self._nonspee
+00009590: 6368 5f73 6563 7469 6f6e 7320 3d20 5b0d  ch_sections = [.
+000095a0: 0a20 2020 2020 2020 2020 2020 2064 6963  .            dic
+000095b0: 7428 7374 6172 743d 726f 756e 6428 732c  t(start=round(s,
+000095c0: 2033 292c 2065 6e64 3d72 6f75 6e64 2865   3), end=round(e
+000095d0: 2c20 3329 2920 666f 7220 732c 2065 2069  , 3)) for s, e i
+000095e0: 6e20 7a69 7028 7369 6c65 6e74 5f73 7461  n zip(silent_sta
+000095f0: 7274 732c 2073 696c 656e 745f 656e 6473  rts, silent_ends
+00009600: 290d 0a20 2020 2020 2020 205d 0d0a 0d0a  )..        ]....
+00009610: 2020 2020 6465 6620 6164 645f 7365 676d      def add_segm
+00009620: 656e 7473 2873 656c 662c 2069 6e64 6578  ents(self, index
+00009630: 303a 2069 6e74 2c20 696e 6465 7831 3a20  0: int, index1: 
+00009640: 696e 742c 2069 6e70 6c61 6365 3a20 626f  int, inplace: bo
+00009650: 6f6c 203d 2046 616c 7365 2c20 6c6f 636b  ol = False, lock
+00009660: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
+00009670: 6e65 776c 696e 653a 2062 6f6f 6c20 3d20  newline: bool = 
+00009680: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00009690: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
+000096a0: 7365 676d 656e 7473 5b69 6e64 6578 305d  segments[index0]
+000096b0: 2e61 6464 2873 656c 662e 7365 676d 656e  .add(self.segmen
+000096c0: 7473 5b69 6e64 6578 315d 2c20 636f 7079  ts[index1], copy
+000096d0: 5f77 6f72 6473 3d46 616c 7365 2c20 6e65  _words=False, ne
+000096e0: 776c 696e 653d 6e65 776c 696e 6529 0d0a  wline=newline)..
+000096f0: 2020 2020 2020 2020 6966 206c 6f63 6b20          if lock 
+00009700: 616e 6420 7365 6c66 2e73 6567 6d65 6e74  and self.segment
+00009710: 735b 696e 6465 7830 5d2e 6861 735f 776f  s[index0].has_wo
+00009720: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
+00009730: 2020 6c6f 636b 5f69 6478 203d 206c 656e    lock_idx = len
+00009740: 2873 656c 662e 7365 676d 656e 7473 5b69  (self.segments[i
+00009750: 6e64 6578 305d 2e77 6f72 6473 290d 0a20  ndex0].words).. 
+00009760: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+00009770: 6567 2e77 6f72 6473 5b6c 6f63 6b5f 6964  eg.words[lock_id
+00009780: 7820 2d20 315d 2e6c 6f63 6b5f 7269 6768  x - 1].lock_righ
+00009790: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+000097a0: 2069 6620 6c6f 636b 5f69 6478 203c 206c   if lock_idx < l
+000097b0: 656e 286e 6577 5f73 6567 2e77 6f72 6473  en(new_seg.words
+000097c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000097d0: 2020 2020 6e65 775f 7365 672e 776f 7264      new_seg.word
+000097e0: 735b 6c6f 636b 5f69 6478 5d2e 6c6f 636b  s[lock_idx].lock
+000097f0: 5f6c 6566 7428 290d 0a20 2020 2020 2020  _left()..       
+00009800: 2069 6620 696e 706c 6163 653a 0d0a 2020   if inplace:..  
+00009810: 2020 2020 2020 2020 2020 6930 2c20 6931            i0, i1
+00009820: 203d 2073 6f72 7465 6428 5b69 6e64 6578   = sorted([index
+00009830: 302c 2069 6e64 6578 315d 290d 0a20 2020  0, index1])..   
+00009840: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00009850: 676d 656e 7473 5b69 305d 203d 206e 6577  gments[i0] = new
+00009860: 5f73 6567 0d0a 2020 2020 2020 2020 2020  _seg..          
+00009870: 2020 6465 6c20 7365 6c66 2e73 6567 6d65    del self.segme
+00009880: 6e74 735b 6931 5d0d 0a20 2020 2020 2020  nts[i1]..       
+00009890: 2072 6574 7572 6e20 6e65 775f 7365 670d   return new_seg.
+000098a0: 0a0d 0a20 2020 2064 6566 2072 6573 6361  ...    def resca
+000098b0: 6c65 5f74 696d 6528 7365 6c66 2c20 7363  le_time(self, sc
+000098c0: 616c 655f 6661 6374 6f72 3a20 666c 6f61  ale_factor: floa
+000098d0: 7429 3a0d 0a20 2020 2020 2020 2066 6f72  t):..        for
+000098e0: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
+000098f0: 6e74 733a 0d0a 2020 2020 2020 2020 2020  nts:..          
+00009900: 2020 732e 7265 7363 616c 655f 7469 6d65    s.rescale_time
+00009910: 2873 6361 6c65 5f66 6163 746f 7229 0d0a  (scale_factor)..
+00009920: 0d0a 2020 2020 6465 6620 6170 706c 795f  ..    def apply_
+00009930: 6d69 6e5f 6475 7228 7365 6c66 2c20 6d69  min_dur(self, mi
+00009940: 6e5f 6475 723a 2066 6c6f 6174 2c20 696e  n_dur: float, in
+00009950: 706c 6163 653a 2062 6f6f 6c20 3d20 4661  place: bool = Fa
+00009960: 6c73 6529 3a0d 0a20 2020 2020 2020 2022  lse):..        "
+00009970: 2222 0d0a 2020 2020 2020 2020 4d65 7267  ""..        Merg
+00009980: 6520 616e 7920 776f 7264 2f73 6567 6d65  e any word/segme
+00009990: 6e74 2077 6974 6820 6164 6a61 6365 6e74  nt with adjacent
+000099a0: 2077 6f72 642f 7365 676d 656e 7420 6966   word/segment if
+000099b0: 2069 7473 2064 7572 6174 696f 6e20 6973   its duration is
+000099c0: 206c 6573 7320 7468 616e 2060 606d 696e   less than ``min
+000099d0: 5f64 7572 6060 2e0d 0a20 2020 2020 2020  _dur``...       
+000099e0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+000099f0: 7375 6c74 203d 2073 656c 6620 6966 2069  sult = self if i
+00009a00: 6e70 6c61 6365 2065 6c73 6520 6465 6570  nplace else deep
+00009a10: 636f 7079 2873 656c 6629 0d0a 2020 2020  copy(self)..    
+00009a20: 2020 2020 6d61 785f 6920 3d20 6c65 6e28      max_i = len(
+00009a30: 7265 7375 6c74 2e73 6567 6d65 6e74 7329  result.segments)
+00009a40: 202d 2031 0d0a 2020 2020 2020 2020 6966   - 1..        if
+00009a50: 206d 6178 5f69 203d 3d20 303a 0d0a 2020   max_i == 0:..  
+00009a60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009a70: 2072 6573 756c 740d 0a20 2020 2020 2020   result..       
+00009a80: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
+00009a90: 6564 2872 616e 6765 286c 656e 2872 6573  ed(range(len(res
+00009aa0: 756c 742e 7365 676d 656e 7473 2929 293a  ult.segments))):
+00009ab0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009ac0: 206d 6178 5f69 203d 3d20 303a 0d0a 2020   max_i == 0:..  
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00009ae0: 6561 6b0d 0a20 2020 2020 2020 2020 2020  eak..           
+00009af0: 2069 6620 7265 7375 6c74 2e73 6567 6d65   if result.segme
+00009b00: 6e74 735b 695d 2e64 7572 6174 696f 6e20  nts[i].duration 
+00009b10: 3c20 6d69 6e5f 6475 723a 0d0a 2020 2020  < min_dur:..    
+00009b20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00009b30: 203d 3d20 6d61 785f 693a 0d0a 2020 2020   == max_i:..    
+00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 7265 7375 6c74 2e61 6464 5f73 6567 6d65  result.add_segme
+00009b60: 6e74 7328 692d 312c 2069 2c20 696e 706c  nts(i-1, i, inpl
+00009b70: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
+00009b80: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00009b90: 6920 3d3d 2030 3a0d 0a20 2020 2020 2020  i == 0:..       
+00009ba0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00009bb0: 756c 742e 6164 645f 7365 676d 656e 7473  ult.add_segments
+00009bc0: 2869 2c20 692b 312c 2069 6e70 6c61 6365  (i, i+1, inplace
+00009bd0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00009be0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2069 6620 7265 7375 6c74 2e73 6567     if result.seg
+00009c10: 6d65 6e74 735b 692b 315d 2e64 7572 6174  ments[i+1].durat
+00009c20: 696f 6e20 3c20 7265 7375 6c74 2e73 6567  ion < result.seg
+00009c30: 6d65 6e74 735b 692d 315d 2e64 7572 6174  ments[i-1].durat
+00009c40: 696f 6e3a 0d0a 2020 2020 2020 2020 2020  ion:..          
+00009c50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009c60: 7375 6c74 2e61 6464 5f73 6567 6d65 6e74  sult.add_segment
+00009c70: 7328 692d 312c 2069 2c20 696e 706c 6163  s(i-1, i, inplac
+00009c80: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00009c90: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00009ca0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00009cb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00009cc0: 6c74 2e61 6464 5f73 6567 6d65 6e74 7328  lt.add_segments(
+00009cd0: 692c 2069 2b31 2c20 696e 706c 6163 653d  i, i+1, inplace=
+00009ce0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00009cf0: 2020 2020 2020 206d 6178 5f69 202d 3d20         max_i -= 
+00009d00: 310d 0a20 2020 2020 2020 2072 6573 756c  1..        resul
+00009d10: 742e 7265 6173 7369 676e 5f69 6473 2829  t.reassign_ids()
+00009d20: 0d0a 2020 2020 2020 2020 666f 7220 7320  ..        for s 
+00009d30: 696e 2072 6573 756c 742e 7365 676d 656e  in result.segmen
+00009d40: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00009d50: 2073 2e61 7070 6c79 5f6d 696e 5f64 7572   s.apply_min_dur
+00009d60: 286d 696e 5f64 7572 2c20 696e 706c 6163  (min_dur, inplac
+00009d70: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00009d80: 2072 6574 7572 6e20 7265 7375 6c74 0d0a   return result..
+00009d90: 0d0a 2020 2020 6465 6620 6f66 6673 6574  ..    def offset
+00009da0: 5f74 696d 6528 7365 6c66 2c20 6f66 6673  _time(self, offs
+00009db0: 6574 5f73 6563 6f6e 6473 3a20 666c 6f61  et_seconds: floa
+00009dc0: 7429 3a0d 0a20 2020 2020 2020 2066 6f72  t):..        for
+00009dd0: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
+00009de0: 6e74 733a 0d0a 2020 2020 2020 2020 2020  nts:..          
+00009df0: 2020 732e 6f66 6673 6574 5f74 696d 6528    s.offset_time(
+00009e00: 6f66 6673 6574 5f73 6563 6f6e 6473 290d  offset_seconds).
+00009e10: 0a0d 0a20 2020 2064 6566 2073 7570 7072  ...    def suppr
+00009e20: 6573 735f 7369 6c65 6e63 6528 0d0a 2020  ess_silence(..  
+00009e30: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+00009e40: 0a20 2020 2020 2020 2020 2020 2073 696c  .            sil
+00009e50: 656e 745f 7374 6172 7473 3a20 6e70 2e6e  ent_starts: np.n
+00009e60: 6461 7272 6179 2c0d 0a20 2020 2020 2020  darray,..       
+00009e70: 2020 2020 2073 696c 656e 745f 656e 6473       silent_ends
+00009e80: 3a20 6e70 2e6e 6461 7272 6179 2c0d 0a20  : np.ndarray,.. 
+00009e90: 2020 2020 2020 2020 2020 206d 696e 5f77             min_w
+00009ea0: 6f72 645f 6475 723a 204f 7074 696f 6e61  ord_dur: Optiona
+00009eb0: 6c5b 666c 6f61 745d 203d 204e 6f6e 652c  l[float] = None,
+00009ec0: 0d0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+00009ed0: 7264 5f6c 6576 656c 3a20 626f 6f6c 203d  rd_level: bool =
+00009ee0: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+00009ef0: 2020 2020 6e6f 6e73 7065 6563 685f 6572      nonspeech_er
+00009f00: 726f 723a 2066 6c6f 6174 203d 2030 2e33  ror: float = 0.3
+00009f10: 2c0d 0a20 2020 2020 2020 2020 2020 2075  ,..            u
+00009f20: 7365 5f77 6f72 645f 706f 7369 7469 6f6e  se_word_position
+00009f30: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+00009f40: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+00009f50: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
+00009f60: 2c0d 0a20 2020 2029 202d 3e20 2257 6869  ,..    ) -> "Whi
+00009f70: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
+00009f80: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00009f90: 2020 204d 6f76 6520 616e 7920 7374 6172     Move any star
+00009fa0: 742f 656e 6420 7469 6d65 7374 616d 7073  t/end timestamps
+00009fb0: 2069 6e20 7369 6c65 6e63 6520 7061 7274   in silence part
+00009fc0: 7320 6f66 2061 7564 696f 2074 6f20 7468  s of audio to th
+00009fd0: 6520 626f 756e 6461 7269 6573 206f 6620  e boundaries of 
+00009fe0: 7468 6520 7369 6c65 6e63 652e 0d0a 0d0a  the silence.....
+00009ff0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000a000: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0000a010: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000a020: 7369 6c65 6e74 5f73 7461 7274 7320 3a20  silent_starts : 
+0000a030: 6e75 6d70 792e 6e64 6172 7261 790d 0a20  numpy.ndarray.. 
+0000a040: 2020 2020 2020 2020 2020 2041 6e20 6172             An ar
+0000a050: 7261 7920 7374 6172 7469 6e67 2074 696d  ray starting tim
+0000a060: 6573 7461 6d70 7320 6f66 2073 696c 656e  estamps of silen
+0000a070: 7420 7365 6374 696f 6e73 206f 6620 6175  t sections of au
+0000a080: 6469 6f2e 0d0a 2020 2020 2020 2020 7369  dio...        si
+0000a090: 6c65 6e74 5f65 6e64 7320 3a20 6e75 6d70  lent_ends : nump
+0000a0a0: 792e 6e64 6172 7261 790d 0a20 2020 2020  y.ndarray..     
+0000a0b0: 2020 2020 2020 2041 6e20 6172 7261 7920         An array 
+0000a0c0: 656e 6469 6e67 2074 696d 6573 7461 6d70  ending timestamp
+0000a0d0: 7320 6f66 2073 696c 656e 7420 7365 6374  s of silent sect
+0000a0e0: 696f 6e73 206f 6620 6175 6469 6f2e 0d0a  ions of audio...
+0000a0f0: 2020 2020 2020 2020 6d69 6e5f 776f 7264          min_word
+0000a100: 5f64 7572 203a 2066 6c6f 6174 206f 7220  _dur : float or 
+0000a110: 4e6f 6e65 2c20 6465 6661 756c 7420 4e6f  None, default No
+0000a120: 6e65 206d 6561 6e69 6e67 2075 7365 2060  ne meaning use `
+0000a130: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
+0000a140: 6465 6661 756c 742e 4445 4641 554c 545f  default.DEFAULT_
+0000a150: 5641 4c55 4553 6060 0d0a 2020 2020 2020  VALUES``..      
+0000a160: 2020 2020 2020 5368 6f72 7465 7374 2064        Shortest d
+0000a170: 7572 6174 696f 6e20 6561 6368 2077 6f72  uration each wor
+0000a180: 6420 6973 2061 6c6c 6f77 6564 2074 6f20  d is allowed to 
+0000a190: 7265 6163 6820 666f 7220 6164 6a75 7374  reach for adjust
+0000a1a0: 6d65 6e74 732e 0d0a 2020 2020 2020 2020  ments...        
+0000a1b0: 776f 7264 5f6c 6576 656c 203a 2062 6f6f  word_level : boo
+0000a1c0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+0000a1d0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+0000a1e0: 6574 6865 7220 746f 2073 6574 7469 6e67  ether to setting
+0000a1f0: 7320 746f 2077 6f72 6420 6c65 7665 6c20  s to word level 
+0000a200: 7469 6d65 7374 616d 7073 2e0d 0a20 2020  timestamps...   
+0000a210: 2020 2020 206e 6f6e 7370 6565 6368 5f65       nonspeech_e
+0000a220: 7272 6f72 203a 2066 6c6f 6174 2c20 6465  rror : float, de
+0000a230: 6661 756c 7420 302e 330d 0a20 2020 2020  fault 0.3..     
+0000a240: 2020 2020 2020 2052 656c 6174 6976 6520         Relative 
+0000a250: 6572 726f 7220 6f66 206e 6f6e 2d73 7065  error of non-spe
+0000a260: 6563 6820 7365 6374 696f 6e73 2074 6861  ech sections tha
+0000a270: 7420 6170 7065 6172 2069 6e20 6265 7477  t appear in betw
+0000a280: 6565 6e20 6120 776f 7264 2066 6f72 2061  een a word for a
+0000a290: 646a 7573 746d 656e 7473 2e0d 0a20 2020  djustments...   
+0000a2a0: 2020 2020 2075 7365 5f77 6f72 645f 706f       use_word_po
+0000a2b0: 7369 7469 6f6e 203a 2062 6f6f 6c2c 2064  sition : bool, d
+0000a2c0: 6566 6175 6c74 2054 7275 650d 0a20 2020  efault True..   
+0000a2d0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+0000a2e0: 2074 6f20 7573 6520 706f 7369 7469 6f6e   to use position
+0000a2f0: 206f 6620 7468 6520 776f 7264 2069 6e20   of the word in 
+0000a300: 6974 7320 7365 676d 656e 7420 746f 2064  its segment to d
+0000a310: 6574 6572 6d69 6e65 2077 6865 7468 6572  etermine whether
+0000a320: 2074 6f20 6b65 6570 2065 6e64 206f 7220   to keep end or 
+0000a330: 7374 6172 7420 7469 6d65 7374 616d 7073  start timestamps
+0000a340: 2069 660d 0a20 2020 2020 2020 2020 2020   if..           
+0000a350: 2061 646a 7573 746d 656e 7473 2061 7265   adjustments are
+0000a360: 2072 6571 7569 7265 642e 2049 6620 6974   required. If it
+0000a370: 2069 7320 7468 6520 6669 7273 7420 776f   is the first wo
+0000a380: 7264 2c20 6b65 6570 2065 6e64 2e20 456c  rd, keep end. El
+0000a390: 7365 2069 6620 6974 2069 7320 7468 6520  se if it is the 
+0000a3a0: 6c61 7374 2077 6f72 642c 206b 6565 7020  last word, keep 
+0000a3b0: 7468 6520 7374 6172 742e 0d0a 2020 2020  the start...    
+0000a3c0: 2020 2020 7665 7262 6f73 6520 3a20 626f      verbose : bo
+0000a3d0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+0000a3e0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+0000a3f0: 6574 6865 7220 746f 2075 7365 2070 726f  ether to use pro
+0000a400: 6772 6573 7362 6172 2074 6f20 7368 6f77  gressbar to show
+0000a410: 2070 726f 6772 6573 732e 0d0a 0d0a 2020   progress.....  
+0000a420: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+0000a430: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+0000a440: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+0000a450: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+0000a460: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
+0000a470: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
+0000a480: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
+0000a490: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
+0000a4a0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000a4b0: 2020 2020 2020 206d 696e 5f77 6f72 645f         min_word_
+0000a4c0: 6475 7220 3d20 6765 745f 6d69 6e5f 776f  dur = get_min_wo
+0000a4d0: 7264 5f64 7572 286d 696e 5f77 6f72 645f  rd_dur(min_word_
+0000a4e0: 6475 7229 0d0a 2020 2020 2020 2020 6d61  dur)..        ma
+0000a4f0: 785f 7473 203d 2073 656c 662e 7365 676d  x_ts = self.segm
+0000a500: 656e 7473 5b2d 315d 2e65 6e64 2069 6620  ents[-1].end if 
+0000a510: 7365 6c66 2e73 6567 6d65 6e74 7320 656c  self.segments el
+0000a520: 7365 2030 0d0a 2020 2020 2020 2020 7769  se 0..        wi
+0000a530: 7468 2074 7164 6d28 746f 7461 6c3d 6d61  th tqdm(total=ma
+0000a540: 785f 7473 2c20 756e 6974 3d27 7365 6327  x_ts, unit='sec'
+0000a550: 2c20 6469 7361 626c 653d 6e6f 7420 7665  , disable=not ve
+0000a560: 7262 6f73 652c 2064 6573 633d 2741 646a  rbose, desc='Adj
+0000a570: 7573 746d 656e 7427 2920 6173 2074 7164  ustment') as tqd
+0000a580: 6d5f 7062 6172 3a0d 0a20 2020 2020 2020  m_pbar:..       
+0000a590: 2020 2020 2066 6f72 2073 2069 6e20 7365       for s in se
+0000a5a0: 6c66 2e73 6567 6d65 6e74 733a 0d0a 2020  lf.segments:..  
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 732e                s.
+0000a5c0: 7375 7070 7265 7373 5f73 696c 656e 6365  suppress_silence
+0000a5d0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000a5e0: 2020 2020 2020 2073 696c 656e 745f 7374         silent_st
+0000a5f0: 6172 7473 2c0d 0a20 2020 2020 2020 2020  arts,..         
+0000a600: 2020 2020 2020 2020 2020 2073 696c 656e             silen
+0000a610: 745f 656e 6473 2c0d 0a20 2020 2020 2020  t_ends,..       
+0000a620: 2020 2020 2020 2020 2020 2020 206d 696e               min
+0000a630: 5f77 6f72 645f 6475 722c 0d0a 2020 2020  _word_dur,..    
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a650: 776f 7264 5f6c 6576 656c 3d77 6f72 645f  word_level=word_
+0000a660: 6c65 7665 6c2c 0d0a 2020 2020 2020 2020  level,..        
+0000a670: 2020 2020 2020 2020 2020 2020 6e6f 6e73              nons
+0000a680: 7065 6563 685f 6572 726f 723d 6e6f 6e73  peech_error=nons
+0000a690: 7065 6563 685f 6572 726f 722c 0d0a 2020  peech_error,..  
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6b0: 2020 7573 655f 776f 7264 5f70 6f73 6974    use_word_posit
+0000a6c0: 696f 6e3d 7573 655f 776f 7264 5f70 6f73  ion=use_word_pos
+0000a6d0: 6974 696f 6e0d 0a20 2020 2020 2020 2020  ition..         
+0000a6e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000a6f0: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+0000a700: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+0000a710: 2020 2020 2020 2020 2020 2074 7164 6d5f             tqdm_
+0000a720: 7062 6172 2e75 7064 6174 6528 732e 656e  pbar.update(s.en
+0000a730: 6420 2d20 7471 646d 5f70 6261 722e 6e29  d - tqdm_pbar.n)
+0000a740: 0d0a 2020 2020 2020 2020 2020 2020 7471  ..            tq
+0000a750: 646d 5f70 6261 722e 7570 6461 7465 2874  dm_pbar.update(t
+0000a760: 7164 6d5f 7062 6172 2e74 6f74 616c 202d  qdm_pbar.total -
+0000a770: 2074 7164 6d5f 7062 6172 2e6e 290d 0a0d   tqdm_pbar.n)...
+0000a780: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a790: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
+0000a7a0: 6164 6a75 7374 5f62 795f 7369 6c65 6e63  adjust_by_silenc
+0000a7b0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+0000a7c0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+0000a7d0: 2020 2061 7564 696f 3a20 556e 696f 6e5b     audio: Union[
+0000a7e0: 746f 7263 682e 5465 6e73 6f72 2c20 6e70  torch.Tensor, np
+0000a7f0: 2e6e 6461 7272 6179 2c20 7374 722c 2062  .ndarray, str, b
+0000a800: 7974 6573 5d2c 0d0a 2020 2020 2020 2020  ytes],..        
+0000a810: 2020 2020 7661 643a 2062 6f6f 6c20 3d20      vad: bool = 
+0000a820: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+0000a830: 2020 2020 2a2c 0d0a 2020 2020 2020 2020      *,..        
+0000a840: 2020 2020 7665 7262 6f73 653a 2028 626f      verbose: (bo
+0000a850: 6f6c 2c20 4e6f 6e65 2920 3d20 4661 6c73  ol, None) = Fals
+0000a860: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+0000a870: 7361 6d70 6c65 5f72 6174 653a 2069 6e74  sample_rate: int
+0000a880: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0000a890: 2020 2020 2020 7661 645f 6f6e 6e78 3a20        vad_onnx: 
+0000a8a0: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+0000a8b0: 2020 2020 2020 2020 2020 2076 6164 5f74             vad_t
+0000a8c0: 6872 6573 686f 6c64 3a20 666c 6f61 7420  hreshold: float 
+0000a8d0: 3d20 302e 3335 2c0d 0a20 2020 2020 2020  = 0.35,..       
+0000a8e0: 2020 2020 2071 5f6c 6576 656c 733a 2069       q_levels: i
+0000a8f0: 6e74 203d 2032 302c 0d0a 2020 2020 2020  nt = 20,..      
+0000a900: 2020 2020 2020 6b5f 7369 7a65 3a20 696e        k_size: in
+0000a910: 7420 3d20 352c 0d0a 2020 2020 2020 2020  t = 5,..        
+0000a920: 2020 2020 6d69 6e5f 776f 7264 5f64 7572      min_word_dur
+0000a930: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+0000a940: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+0000a950: 2020 2020 2020 206d 696e 5f73 696c 656e         min_silen
+0000a960: 6365 5f64 7572 3a20 4f70 7469 6f6e 616c  ce_dur: Optional
+0000a970: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2c0d  [float] = None,.
+0000a980: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+0000a990: 645f 6c65 7665 6c3a 2062 6f6f 6c20 3d20  d_level: bool = 
+0000a9a0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+0000a9b0: 2020 206e 6f6e 7370 6565 6368 5f65 7272     nonspeech_err
+0000a9c0: 6f72 3a20 666c 6f61 7420 3d20 302e 332c  or: float = 0.3,
+0000a9d0: 0d0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+0000a9e0: 655f 776f 7264 5f70 6f73 6974 696f 6e3a  e_word_position:
+0000a9f0: 2062 6f6f 6c20 3d20 5472 7565 0d0a 0d0a   bool = True....
+0000aa00: 2020 2020 2920 2d3e 2022 5768 6973 7065      ) -> "Whispe
+0000aa10: 7252 6573 756c 7422 3a0d 0a20 2020 2020  rResult":..     
+0000aa20: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000aa30: 4164 6a75 7374 2074 696d 6573 7461 6d70  Adjust timestamp
+0000aa40: 7320 6261 7365 206f 6e20 6465 7465 6374  s base on detect
+0000aa50: 6564 2073 7065 6563 6820 6761 7073 2e0d  ed speech gaps..
+0000aa60: 0a0d 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+0000aa70: 6973 206d 6574 686f 6420 636f 6d62 696e  is method combin
+0000aa80: 6573 203a 6d65 7468 3a60 7374 6162 6c65  es :meth:`stable
+0000aa90: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+0000aaa0: 5768 6973 7065 7252 6573 756c 742e 7375  WhisperResult.su
+0000aab0: 7070 7265 7373 5f73 696c 656e 6365 6020  ppress_silence` 
+0000aac0: 7769 7468 2073 696c 656e 6365 2064 6574  with silence det
+0000aad0: 6563 7469 6f6e 2e0d 0a0d 0a20 2020 2020  ection.....     
+0000aae0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+0000aaf0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000ab00: 2d0d 0a20 2020 2020 2020 2061 7564 696f  -..        audio
+0000ab10: 203a 2073 7472 206f 7220 6e75 6d70 792e   : str or numpy.
+0000ab20: 6e64 6172 7261 7920 6f72 2074 6f72 6368  ndarray or torch
+0000ab30: 2e54 656e 736f 7220 6f72 2062 7974 6573  .Tensor or bytes
+0000ab40: 0d0a 2020 2020 2020 2020 2020 2020 5061  ..            Pa
+0000ab50: 7468 2f55 524c 2074 6f20 7468 6520 6175  th/URL to the au
+0000ab60: 6469 6f20 6669 6c65 2c20 7468 6520 6175  dio file, the au
+0000ab70: 6469 6f20 7761 7665 666f 726d 2c20 6f72  dio waveform, or
+0000ab80: 2062 7974 6573 206f 6620 6175 6469 6f20   bytes of audio 
+0000ab90: 6669 6c65 2e0d 0a20 2020 2020 2020 2076  file...        v
+0000aba0: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+0000abb0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+0000abc0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+0000abd0: 2075 7365 2053 696c 6572 6f20 5641 4420   use Silero VAD 
+0000abe0: 746f 2067 656e 6572 6174 6520 7469 6d65  to generate time
+0000abf0: 7374 616d 7020 7375 7070 7265 7373 696f  stamp suppressio
+0000ac00: 6e20 6d61 736b 2e0d 0a20 2020 2020 2020  n mask...       
+0000ac10: 2020 2020 2053 696c 6572 6f20 5641 4420       Silero VAD 
+0000ac20: 7265 7175 6972 6573 2050 7954 6f72 6368  requires PyTorch
+0000ac30: 2031 2e31 322e 302b 2e20 4f66 6669 6369   1.12.0+. Offici
+0000ac40: 616c 2072 6570 6f2c 2068 7474 7073 3a2f  al repo, https:/
+0000ac50: 2f67 6974 6875 622e 636f 6d2f 736e 616b  /github.com/snak
+0000ac60: 6572 7334 2f73 696c 6572 6f2d 7661 642e  ers4/silero-vad.
+0000ac70: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
+0000ac80: 6520 3a20 626f 6f6c 206f 7220 4e6f 6e65  e : bool or None
+0000ac90: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
+0000aca0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
+0000acb0: 706c 6179 7320 616c 6c20 696e 666f 2069  plays all info i
+0000acc0: 6620 6060 5472 7565 6060 2e20 4469 7370  f ``True``. Disp
+0000acd0: 6c61 7973 2070 726f 6772 6573 7362 6172  lays progressbar
+0000ace0: 2069 6620 6060 4661 6c73 6560 602e 2044   if ``False``. D
+0000acf0: 6973 706c 6179 206e 6f74 6869 6e67 2069  isplay nothing i
+0000ad00: 6620 6060 4e6f 6e65 6060 2e0d 0a20 2020  f ``None``...   
+0000ad10: 2020 2020 2020 2020 2049 6620 6060 7661           If ``va
+0000ad20: 6420 3d20 5472 7565 6060 2061 6e64 2060  d = True`` and `
+0000ad30: 6046 616c 7365 6060 2c20 6d75 7465 206d  `False``, mute m
+0000ad40: 6573 7361 6765 7320 6162 6f75 7420 6869  essages about hi
+0000ad50: 7474 696e 6720 6c6f 6361 6c20 6361 6368  tting local cach
+0000ad60: 6573 2e0d 0a20 2020 2020 2020 2020 2020  es...           
+0000ad70: 204e 6f74 6520 7468 6174 2074 6865 206d   Note that the m
+0000ad80: 6573 7361 6765 2061 626f 7574 2066 6972  essage about fir
+0000ad90: 7374 2064 6f77 6e6c 6f61 6420 6361 6e6e  st download cann
+0000ada0: 6f74 2062 6520 6d75 7465 642e 0d0a 2020  ot be muted...  
+0000adb0: 2020 2020 2020 7361 6d70 6c65 5f72 6174        sample_rat
+0000adc0: 6520 3a20 696e 742c 2064 6566 6175 6c74  e : int, default
+0000add0: 204e 6f6e 652c 206d 6561 6e69 6e67 2060   None, meaning `
+0000ade0: 6077 6869 7370 6572 2e61 7564 696f 2e53  `whisper.audio.S
+0000adf0: 414d 504c 455f 5241 5445 6060 2c20 3136  AMPLE_RATE``, 16
+0000ae00: 6b48 5a0d 0a20 2020 2020 2020 2020 2020  kHZ..           
+0000ae10: 2054 6865 2073 616d 706c 6520 7261 7465   The sample rate
+0000ae20: 206f 6620 6060 6175 6469 6f60 602e 0d0a   of ``audio``...
+0000ae30: 2020 2020 2020 2020 7661 645f 6f6e 6e78          vad_onnx
+0000ae40: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0000ae50: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000ae60: 2020 2020 5768 6574 6865 7220 746f 2075      Whether to u
+0000ae70: 7365 204f 4e4e 5820 666f 7220 5369 6c65  se ONNX for Sile
+0000ae80: 726f 2056 4144 2e0d 0a20 2020 2020 2020  ro VAD...       
+0000ae90: 2076 6164 5f74 6872 6573 686f 6c64 203a   vad_threshold :
+0000aea0: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+0000aeb0: 302e 3335 0d0a 2020 2020 2020 2020 2020  0.35..          
+0000aec0: 2020 5468 7265 7368 6f6c 6420 666f 7220    Threshold for 
+0000aed0: 6465 7465 6374 696e 6720 7370 6565 6368  detecting speech
+0000aee0: 2077 6974 6820 5369 6c65 726f 2056 4144   with Silero VAD
+0000aef0: 2e20 4c6f 7720 7468 7265 7368 6f6c 6420  . Low threshold 
+0000af00: 7265 6475 6365 7320 6661 6c73 6520 706f  reduces false po
+0000af10: 7369 7469 7665 7320 666f 7220 7369 6c65  sitives for sile
+0000af20: 6e63 6520 6465 7465 6374 696f 6e2e 0d0a  nce detection...
+0000af30: 2020 2020 2020 2020 715f 6c65 7665 6c73          q_levels
+0000af40: 203a 2069 6e74 2c20 6465 6661 756c 7420   : int, default 
+0000af50: 3230 0d0a 2020 2020 2020 2020 2020 2020  20..            
+0000af60: 5175 616e 7469 7a61 7469 6f6e 206c 6576  Quantization lev
+0000af70: 656c 7320 666f 7220 6765 6e65 7261 7469  els for generati
+0000af80: 6e67 2074 696d 6573 7461 6d70 2073 7570  ng timestamp sup
+0000af90: 7072 6573 7369 6f6e 206d 6173 6b3b 2069  pression mask; i
+0000afa0: 676e 6f72 6564 2069 6620 6060 7661 6420  gnored if ``vad 
+0000afb0: 3d20 7472 7565 6060 2e0d 0a20 2020 2020  = true``...     
+0000afc0: 2020 2020 2020 2041 6374 7320 6173 2061         Acts as a
+0000afd0: 2074 6872 6573 686f 6c64 2074 6f20 6d61   threshold to ma
+0000afe0: 726b 696e 6720 736f 756e 6420 6173 2073  rking sound as s
+0000aff0: 696c 656e 742e 0d0a 2020 2020 2020 2020  ilent...        
+0000b000: 2020 2020 4665 7765 7220 6c65 7665 6c73      Fewer levels
+0000b010: 2077 696c 6c20 696e 6372 6561 7365 2074   will increase t
+0000b020: 6865 2074 6872 6573 686f 6c64 206f 6620  he threshold of 
+0000b030: 766f 6c75 6d65 2061 7420 7768 6963 6820  volume at which 
+0000b040: 746f 206d 6172 6b20 6120 736f 756e 6420  to mark a sound 
+0000b050: 6173 2073 696c 656e 742e 0d0a 2020 2020  as silent...    
+0000b060: 2020 2020 6b5f 7369 7a65 203a 2069 6e74      k_size : int
+0000b070: 2c20 6465 6661 756c 7420 350d 0a20 2020  , default 5..   
+0000b080: 2020 2020 2020 2020 204b 6572 6e65 6c20           Kernel 
+0000b090: 7369 7a65 2066 6f72 2061 7667 2d70 6f6f  size for avg-poo
+0000b0a0: 6c69 6e67 2077 6176 6566 6f72 6d20 746f  ling waveform to
+0000b0b0: 2067 656e 6572 6174 6520 7469 6d65 7374   generate timest
+0000b0c0: 616d 7020 7375 7070 7265 7373 696f 6e20  amp suppression 
+0000b0d0: 6d61 736b 3b20 6967 6e6f 7265 6420 6966  mask; ignored if
+0000b0e0: 2060 6076 6164 203d 2074 7275 6560 602e   ``vad = true``.
+0000b0f0: 0d0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+0000b100: 636f 6d6d 656e 6420 3520 6f72 2033 3b20  commend 5 or 3; 
+0000b110: 6869 6768 6572 2073 697a 6573 2077 696c  higher sizes wil
+0000b120: 6c20 7265 6475 6365 2064 6574 6563 7469  l reduce detecti
+0000b130: 6f6e 206f 6620 7369 6c65 6e63 652e 0d0a  on of silence...
+0000b140: 2020 2020 2020 2020 6d69 6e5f 776f 7264          min_word
+0000b150: 5f64 7572 203a 2066 6c6f 6174 206f 7220  _dur : float or 
+0000b160: 4e6f 6e65 2c20 6465 6661 756c 7420 4e6f  None, default No
+0000b170: 6e65 206d 6561 6e69 6e67 2075 7365 2060  ne meaning use `
+0000b180: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
+0000b190: 6465 6661 756c 742e 4445 4641 554c 545f  default.DEFAULT_
+0000b1a0: 5641 4c55 4553 6060 0d0a 2020 2020 2020  VALUES``..      
+0000b1b0: 2020 2020 2020 5368 6f72 7465 7374 2064        Shortest d
+0000b1c0: 7572 6174 696f 6e20 6561 6368 2077 6f72  uration each wor
+0000b1d0: 6420 6973 2061 6c6c 6f77 6564 2074 6f20  d is allowed to 
+0000b1e0: 7265 6163 6820 6672 6f6d 2061 646a 7573  reach from adjus
+0000b1f0: 746d 656e 7473 2e0d 0a20 2020 2020 2020  tments...       
+0000b200: 206d 696e 5f73 696c 656e 6365 5f64 7572   min_silence_dur
+0000b210: 203a 2066 6c6f 6174 2c20 6f70 7469 6f6e   : float, option
+0000b220: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
+0000b230: 5368 6f72 7465 7374 2064 7572 6174 696f  Shortest duratio
+0000b240: 6e20 6f66 2073 696c 656e 6365 2061 6c6c  n of silence all
+0000b250: 6f77 6564 2066 6f72 2073 696c 656e 6365  owed for silence
+0000b260: 2073 7570 7072 6573 7369 6f6e 2e0d 0a20   suppression... 
+0000b270: 2020 2020 2020 2077 6f72 645f 6c65 7665         word_leve
+0000b280: 6c20 3a20 626f 6f6c 2c20 6465 6661 756c  l : bool, defaul
+0000b290: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+0000b2a0: 2020 2020 5768 6574 6865 7220 746f 2073      Whether to s
+0000b2b0: 6574 7469 6e67 7320 746f 2077 6f72 6420  ettings to word 
+0000b2c0: 6c65 7665 6c20 7469 6d65 7374 616d 7073  level timestamps
+0000b2d0: 2e0d 0a20 2020 2020 2020 206e 6f6e 7370  ...        nonsp
+0000b2e0: 6565 6368 5f65 7272 6f72 203a 2066 6c6f  eech_error : flo
+0000b2f0: 6174 2c20 6465 6661 756c 7420 302e 330d  at, default 0.3.
+0000b300: 0a20 2020 2020 2020 2020 2020 2052 656c  .            Rel
+0000b310: 6174 6976 6520 6572 726f 7220 6f66 206e  ative error of n
+0000b320: 6f6e 2d73 7065 6563 6820 7365 6374 696f  on-speech sectio
+0000b330: 6e73 2074 6861 7420 6170 7065 6172 2069  ns that appear i
+0000b340: 6e20 6265 7477 6565 6e20 6120 776f 7264  n between a word
+0000b350: 2066 6f72 2061 646a 7573 746d 656e 7473   for adjustments
+0000b360: 2e0d 0a20 2020 2020 2020 2075 7365 5f77  ...        use_w
+0000b370: 6f72 645f 706f 7369 7469 6f6e 203a 2062  ord_position : b
+0000b380: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+0000b390: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+0000b3a0: 6865 7468 6572 2074 6f20 7573 6520 706f  hether to use po
+0000b3b0: 7369 7469 6f6e 206f 6620 7468 6520 776f  sition of the wo
+0000b3c0: 7264 2069 6e20 6974 7320 7365 676d 656e  rd in its segmen
+0000b3d0: 7420 746f 2064 6574 6572 6d69 6e65 2077  t to determine w
+0000b3e0: 6865 7468 6572 2074 6f20 6b65 6570 2065  hether to keep e
+0000b3f0: 6e64 206f 7220 7374 6172 7420 7469 6d65  nd or start time
+0000b400: 7374 616d 7073 2069 660d 0a20 2020 2020  stamps if..     
+0000b410: 2020 2020 2020 2061 646a 7573 746d 656e         adjustmen
+0000b420: 7473 2061 7265 2072 6571 7569 7265 642e  ts are required.
+0000b430: 2049 6620 6974 2069 7320 7468 6520 6669   If it is the fi
+0000b440: 7273 7420 776f 7264 2c20 6b65 6570 2065  rst word, keep e
+0000b450: 6e64 2e20 456c 7365 2069 6620 6974 2069  nd. Else if it i
+0000b460: 7320 7468 6520 6c61 7374 2077 6f72 642c  s the last word,
+0000b470: 206b 6565 7020 7468 6520 7374 6172 742e   keep the start.
+0000b480: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+0000b490: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+0000b4a0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
+0000b4b0: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+0000b4c0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+0000b4d0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
+0000b4e0: 6865 2063 7572 7265 6e74 2069 6e73 7461  he current insta
+0000b4f0: 6e63 6520 6166 7465 7220 7468 6520 6368  nce after the ch
+0000b500: 616e 6765 732e 0d0a 0d0a 2020 2020 2020  anges.....      
+0000b510: 2020 4e6f 7465 730d 0a20 2020 2020 2020    Notes..       
+0000b520: 202d 2d2d 2d2d 0d0a 2020 2020 2020 2020   -----..        
+0000b530: 5468 6973 206f 7065 7261 7469 6f6e 2069  This operation i
+0000b540: 7320 616c 7265 6164 7920 7065 7266 6f72  s already perfor
+0000b550: 6d65 6420 6279 203a 6675 6e63 3a60 7374  med by :func:`st
+0000b560: 6162 6c65 5f77 6869 7370 6572 2e77 6869  able_whisper.whi
+0000b570: 7370 6572 5f77 6f72 645f 6c65 7665 6c2e  sper_word_level.
+0000b580: 7472 616e 7363 7269 6265 5f73 7461 626c  transcribe_stabl
+0000b590: 6560 202f 0d0a 2020 2020 2020 2020 3a66  e` /..        :f
+0000b5a0: 756e 633a 6073 7461 626c 655f 7768 6973  unc:`stable_whis
+0000b5b0: 7065 722e 7768 6973 7065 725f 776f 7264  per.whisper_word
+0000b5c0: 5f6c 6576 656c 2e74 7261 6e73 6372 6962  _level.transcrib
+0000b5d0: 655f 6d69 6e69 6d61 6c60 2f0d 0a20 2020  e_minimal`/..   
+0000b5e0: 2020 2020 203a 6675 6e63 3a60 7374 6162       :func:`stab
+0000b5f0: 6c65 5f77 6869 7370 6572 2e6e 6f6e 5f77  le_whisper.non_w
+0000b600: 6869 7370 6572 2e74 7261 6e73 6372 6962  hisper.transcrib
+0000b610: 655f 616e 7960 202f 203a 6675 6e63 3a60  e_any` / :func:`
+0000b620: 7374 6162 6c65 5f77 6869 7370 6572 2e61  stable_whisper.a
+0000b630: 6c69 676e 6d65 6e74 2e61 6c69 676e 600d  lignment.align`.
+0000b640: 0a20 2020 2020 2020 2069 6620 6060 7375  .        if ``su
+0000b650: 7070 7265 7373 5f73 696c 656e 6365 203d  ppress_silence =
+0000b660: 2054 7275 6560 602e 0d0a 2020 2020 2020   True``...      
+0000b670: 2020 2222 220d 0a20 2020 2020 2020 206d    """..        m
+0000b680: 696e 5f77 6f72 645f 6475 7220 3d20 6765  in_word_dur = ge
+0000b690: 745f 6d69 6e5f 776f 7264 5f64 7572 286d  t_min_word_dur(m
+0000b6a0: 696e 5f77 6f72 645f 6475 7229 0d0a 2020  in_word_dur)..  
+0000b6b0: 2020 2020 2020 6966 2076 6164 3a0d 0a20        if vad:.. 
+0000b6c0: 2020 2020 2020 2020 2020 2061 7564 696f             audio
+0000b6d0: 203d 2061 7564 696f 5f74 6f5f 7465 6e73   = audio_to_tens
+0000b6e0: 6f72 5f72 6573 616d 706c 6528 6175 6469  or_resample(audi
+0000b6f0: 6f2c 2073 616d 706c 655f 7261 7465 2c20  o, sample_rate, 
+0000b700: 5641 445f 5341 4d50 4c45 5f52 4154 4553  VAD_SAMPLE_RATES
+0000b710: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
+0000b720: 2020 7361 6d70 6c65 5f72 6174 6520 3d20    sample_rate = 
+0000b730: 5641 445f 5341 4d50 4c45 5f52 4154 4553  VAD_SAMPLE_RATES
+0000b740: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+0000b750: 2073 696c 656e 745f 7469 6d69 6e67 7320   silent_timings 
+0000b760: 3d20 6765 745f 7661 645f 7369 6c65 6e63  = get_vad_silenc
+0000b770: 655f 6675 6e63 280d 0a20 2020 2020 2020  e_func(..       
+0000b780: 2020 2020 2020 2020 206f 6e6e 783d 7661           onnx=va
+0000b790: 645f 6f6e 6e78 2c0d 0a20 2020 2020 2020  d_onnx,..       
+0000b7a0: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+0000b7b0: 3d76 6572 626f 7365 0d0a 2020 2020 2020  =verbose..      
+0000b7c0: 2020 2020 2020 2928 6175 6469 6f2c 2073        )(audio, s
+0000b7d0: 7065 6563 685f 7468 7265 7368 6f6c 643d  peech_threshold=
+0000b7e0: 7661 645f 7468 7265 7368 6f6c 642c 2073  vad_threshold, s
+0000b7f0: 723d 7361 6d70 6c65 5f72 6174 6529 0d0a  r=sample_rate)..
+0000b800: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000b810: 2020 2020 2020 2020 2020 2073 696c 656e             silen
+0000b820: 745f 7469 6d69 6e67 7320 3d20 6175 6469  t_timings = audi
+0000b830: 6f32 7469 6d69 6e67 7328 6175 6469 6f2c  o2timings(audio,
+0000b840: 2071 5f6c 6576 656c 733d 715f 6c65 7665   q_levels=q_leve
+0000b850: 6c73 2c20 6b5f 7369 7a65 3d6b 5f73 697a  ls, k_size=k_siz
+0000b860: 652c 2073 723d 7361 6d70 6c65 5f72 6174  e, sr=sample_rat
+0000b870: 6529 0d0a 2020 2020 2020 2020 6966 2073  e)..        if s
+0000b880: 696c 656e 745f 7469 6d69 6e67 7320 6973  ilent_timings is
+0000b890: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000b8a0: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+0000b8b0: 0a20 2020 2020 2020 2069 6620 6d69 6e5f  .        if min_
+0000b8c0: 7369 6c65 6e63 655f 6475 723a 0d0a 2020  silence_dur:..  
+0000b8d0: 2020 2020 2020 2020 2020 7369 6c65 6e74            silent
+0000b8e0: 5f74 696d 696e 6773 203d 2066 696c 7465  _timings = filte
+0000b8f0: 725f 7469 6d69 6e67 7328 7369 6c65 6e74  r_timings(silent
+0000b900: 5f74 696d 696e 6773 2c20 6d69 6e5f 7369  _timings, min_si
+0000b910: 6c65 6e63 655f 6475 7229 0d0a 2020 2020  lence_dur)..    
+0000b920: 2020 2020 7365 6c66 2e73 7570 7072 6573      self.suppres
+0000b930: 735f 7369 6c65 6e63 6528 0d0a 2020 2020  s_silence(..    
+0000b940: 2020 2020 2020 2020 2a73 696c 656e 745f          *silent_
+0000b950: 7469 6d69 6e67 732c 0d0a 2020 2020 2020  timings,..      
+0000b960: 2020 2020 2020 6d69 6e5f 776f 7264 5f64        min_word_d
+0000b970: 7572 3d6d 696e 5f77 6f72 645f 6475 722c  ur=min_word_dur,
+0000b980: 0d0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+0000b990: 7264 5f6c 6576 656c 3d77 6f72 645f 6c65  rd_level=word_le
+0000b9a0: 7665 6c2c 0d0a 2020 2020 2020 2020 2020  vel,..          
+0000b9b0: 2020 6e6f 6e73 7065 6563 685f 6572 726f    nonspeech_erro
+0000b9c0: 723d 6e6f 6e73 7065 6563 685f 6572 726f  r=nonspeech_erro
+0000b9d0: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+0000b9e0: 7573 655f 776f 7264 5f70 6f73 6974 696f  use_word_positio
+0000b9f0: 6e3d 7573 655f 776f 7264 5f70 6f73 6974  n=use_word_posit
+0000ba00: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
+0000ba10: 2020 7665 7262 6f73 653d 7665 7262 6f73    verbose=verbos
+0000ba20: 6520 6973 206e 6f74 204e 6f6e 650d 0a20  e is not None.. 
+0000ba30: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000ba40: 2020 7365 6c66 2e75 7064 6174 655f 6e6f    self.update_no
+0000ba50: 6e73 7065 6563 685f 7365 6374 696f 6e73  nspeech_sections
+0000ba60: 282a 7369 6c65 6e74 5f74 696d 696e 6773  (*silent_timings
+0000ba70: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000ba80: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+0000ba90: 6620 6164 6a75 7374 5f62 795f 7265 7375  f adjust_by_resu
+0000baa0: 6c74 280d 0a20 2020 2020 2020 2020 2020  lt(..           
+0000bab0: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+0000bac0: 2020 2020 6f74 6865 725f 7265 7375 6c74      other_result
+0000bad0: 3a20 2257 6869 7370 6572 5265 7375 6c74  : "WhisperResult
+0000bae0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000baf0: 6d69 6e5f 776f 7264 5f64 7572 3a20 4f70  min_word_dur: Op
+0000bb00: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+0000bb10: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+0000bb20: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+0000bb30: 203d 2046 616c 7365 0d0a 2020 2020 293a   = False..    ):
+0000bb40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000bb50: 2020 2020 2020 204d 696e 696d 697a 6520         Minimize 
+0000bb60: 7468 6520 6475 7261 7469 6f6e 206f 6620  the duration of 
+0000bb70: 776f 7264 7320 7573 696e 6720 7469 6d65  words using time
+0000bb80: 7374 616d 7073 206f 6620 616e 6f74 6865  stamps of anothe
+0000bb90: 7220 7265 7375 6c74 2e0d 0a0d 0a20 2020  r result.....   
+0000bba0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+0000bbb0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000bbc0: 2d2d 2d0d 0a20 2020 2020 2020 206f 7468  ---..        oth
+0000bbd0: 6572 5f72 6573 756c 7420 3a20 2257 6869  er_result : "Whi
+0000bbe0: 7370 6572 5265 7375 6c74 220d 0a20 2020  sperResult"..   
+0000bbf0: 2020 2020 2020 2020 2054 696d 696e 6720           Timing 
+0000bc00: 6461 7461 206f 6620 7468 6520 7361 6d65  data of the same
+0000bc10: 2077 6f72 6473 2069 6e20 6120 5768 6973   words in a Whis
+0000bc20: 7065 7252 6573 756c 7420 696e 7374 616e  perResult instan
+0000bc30: 6365 2e0d 0a20 2020 2020 2020 206d 696e  ce...        min
+0000bc40: 5f77 6f72 645f 6475 7220 3a20 666c 6f61  _word_dur : floa
+0000bc50: 7420 6f72 204e 6f6e 652c 2064 6566 6175  t or None, defau
+0000bc60: 6c74 204e 6f6e 6520 6d65 616e 696e 6720  lt None meaning 
+0000bc70: 7573 6520 6060 7374 6162 6c65 5f77 6869  use ``stable_whi
+0000bc80: 7370 6572 2e64 6566 6175 6c74 2e44 4546  sper.default.DEF
+0000bc90: 4155 4c54 5f56 414c 5545 5360 600d 0a20  AULT_VALUES``.. 
+0000bca0: 2020 2020 2020 2020 2020 2050 7265 7665             Preve
+0000bcb0: 6e74 2063 6861 6e67 6573 2074 6f20 7469  nt changes to ti
+0000bcc0: 6d65 7374 616d 7073 2069 6620 7468 6520  mestamps if the 
+0000bcd0: 7265 7375 6c74 616e 7420 776f 7264 2064  resultant word d
+0000bce0: 7572 6174 696f 6e20 6973 206c 6573 7320  uration is less 
+0000bcf0: 7468 616e 2060 606d 696e 5f77 6f72 645f  than ``min_word_
+0000bd00: 6475 7260 602e 0d0a 2020 2020 2020 2020  dur``...        
+0000bd10: 7665 7262 6f73 6520 3a20 626f 6f6c 2c20  verbose : bool, 
+0000bd20: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+0000bd30: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+0000bd40: 6572 2074 6f20 7072 696e 7420 6f75 7420  er to print out 
+0000bd50: 7468 6520 7469 6d65 7374 616d 7020 6368  the timestamp ch
+0000bd60: 616e 6765 732e 0d0a 2020 2020 2020 2020  anges...        
+0000bd70: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+0000bd80: 6e6f 7420 2873 656c 662e 6861 735f 776f  not (self.has_wo
+0000bd90: 7264 7320 616e 6420 6f74 6865 725f 7265  rds and other_re
+0000bda0: 7375 6c74 2e68 6173 5f77 6f72 6473 293a  sult.has_words):
+0000bdb0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+0000bdc0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+0000bdd0: 6564 4572 726f 7228 2754 6869 7320 6f70  edError('This op
+0000bde0: 6572 6174 696f 6e20 6361 6e20 6f6e 6c79  eration can only
+0000bdf0: 2062 6520 7065 7266 6f72 6d65 6420 6f6e   be performed on
+0000be00: 2072 6573 756c 7473 2077 6974 6820 776f   results with wo
+0000be10: 7264 2074 696d 6573 7461 6d70 7327 290d  rd timestamps').
+0000be20: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000be30: 5b77 2e77 6f72 6420 666f 7220 7720 696e  [w.word for w in
+0000be40: 2073 656c 662e 616c 6c5f 776f 7264 7328   self.all_words(
+0000be50: 295d 203d 3d20 5b77 2e77 6f72 6420 666f  )] == [w.word fo
+0000be60: 7220 7720 696e 206f 7468 6572 5f72 6573  r w in other_res
+0000be70: 756c 742e 616c 6c5f 776f 7264 7328 295d  ult.all_words()]
+0000be80: 2c20 5c0d 0a20 2020 2020 2020 2020 2020  , \..           
+0000be90: 2027 5468 6520 776f 7264 7320 696e 205b   'The words in [
+0000bea0: 6f74 6865 725f 7265 7375 6c74 5d20 646f  other_result] do
+0000beb0: 206e 6f74 206d 6174 6368 2074 6865 2063   not match the c
+0000bec0: 7572 7265 6e74 2077 6f72 6473 2e27 0d0a  urrent words.'..
+0000bed0: 2020 2020 2020 2020 6d69 6e5f 776f 7264          min_word
+0000bee0: 5f64 7572 203d 2067 6574 5f6d 696e 5f77  _dur = get_min_w
+0000bef0: 6f72 645f 6475 7228 6d69 6e5f 776f 7264  ord_dur(min_word
+0000bf00: 5f64 7572 290d 0a20 2020 2020 2020 2066  _dur)..        f
+0000bf10: 6f72 2077 6f72 642c 206f 7468 6572 5f77  or word, other_w
+0000bf20: 6f72 6420 696e 207a 6970 2873 656c 662e  ord in zip(self.
+0000bf30: 616c 6c5f 776f 7264 7328 292c 206f 7468  all_words(), oth
+0000bf40: 6572 5f72 6573 756c 742e 616c 6c5f 776f  er_result.all_wo
+0000bf50: 7264 7328 2929 3a0d 0a20 2020 2020 2020  rds()):..       
+0000bf60: 2020 2020 2069 6620 776f 7264 2e65 6e64       if word.end
+0000bf70: 203e 206f 7468 6572 5f77 6f72 642e 7374   > other_word.st
+0000bf80: 6172 743a 0d0a 2020 2020 2020 2020 2020  art:..          
+0000bf90: 2020 2020 2020 6e65 775f 7374 6172 7420        new_start 
+0000bfa0: 3d20 6d61 7828 776f 7264 2e73 7461 7274  = max(word.start
+0000bfb0: 2c20 6f74 6865 725f 776f 7264 2e73 7461  , other_word.sta
+0000bfc0: 7274 290d 0a20 2020 2020 2020 2020 2020  rt)..           
+0000bfd0: 2020 2020 206e 6577 5f65 6e64 203d 206d       new_end = m
+0000bfe0: 696e 2877 6f72 642e 656e 642c 206f 7468  in(word.end, oth
+0000bff0: 6572 5f77 6f72 642e 656e 6429 0d0a 2020  er_word.end)..  
+0000c000: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c010: 206e 6577 5f65 6e64 202d 206e 6577 5f73   new_end - new_s
+0000c020: 7461 7274 203e 3d20 6d69 6e5f 776f 7264  tart >= min_word
+0000c030: 5f64 7572 3a0d 0a20 2020 2020 2020 2020  _dur:..         
+0000c040: 2020 2020 2020 2020 2020 206c 696e 6520             line 
+0000c050: 3d20 2727 0d0a 2020 2020 2020 2020 2020  = ''..          
+0000c060: 2020 2020 2020 2020 2020 6966 2077 6f72            if wor
+0000c070: 642e 7374 6172 7420 213d 206e 6577 5f73  d.start != new_s
+0000c080: 7461 7274 3a0d 0a20 2020 2020 2020 2020  tart:..         
+0000c090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c0a0: 6620 7665 7262 6f73 653a 0d0a 2020 2020  f verbose:..    
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0c0: 2020 2020 2020 2020 6c69 6e65 202b 3d20          line += 
+0000c0d0: 6627 5b53 7461 7274 3a7b 776f 7264 2e73  f'[Start:{word.s
+0000c0e0: 7461 7274 3a2e 3366 7d2d 3e7b 6e65 775f  tart:.3f}->{new_
+0000c0f0: 7374 6172 743a 2e33 667d 5d20 270d 0a20  start:.3f}] '.. 
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2020 2020 2020 2077 6f72 642e 7374 6172         word.star
+0000c120: 7420 3d20 6e65 775f 7374 6172 740d 0a20  t = new_start.. 
+0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c140: 2020 2069 6620 776f 7264 2e65 6e64 2021     if word.end !
+0000c150: 3d20 6e65 775f 656e 643a 0d0a 2020 2020  = new_end:..    
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
+0000c180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c190: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000c1a0: 6520 2b3d 2066 275b 456e 643a 7b77 6f72  e += f'[End:{wor
+0000c1b0: 642e 656e 643a 2e33 667d 2d3e 7b6e 6577  d.end:.3f}->{new
+0000c1c0: 5f65 6e64 3a2e 3366 7d5d 2020 270d 0a20  _end:.3f}]  '.. 
+0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1e0: 2020 2020 2020 2077 6f72 642e 656e 6420         word.end 
+0000c1f0: 3d20 6e65 775f 656e 640d 0a20 2020 2020  = new_end..     
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c210: 6620 6c69 6e65 3a0d 0a20 2020 2020 2020  f line:..       
+0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c230: 2070 7269 6e74 2866 277b 6c69 6e65 7d22   print(f'{line}"
+0000c240: 7b77 6f72 642e 776f 7264 7d22 2729 0d0a  {word.word}"')..
+0000c250: 0d0a 2020 2020 6465 6620 7265 6173 7369  ..    def reassi
+0000c260: 676e 5f69 6473 2873 656c 662c 206f 6e6c  gn_ids(self, onl
+0000c270: 795f 7365 676d 656e 7473 3a20 626f 6f6c  y_segments: bool
+0000c280: 203d 2046 616c 7365 2c20 7374 6172 743a   = False, start:
+0000c290: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0000c2a0: 204e 6f6e 6529 3a0d 0a20 2020 2020 2020   None):..       
+0000c2b0: 2066 6f72 2069 2c20 7320 696e 2065 6e75   for i, s in enu
+0000c2c0: 6d65 7261 7465 2873 656c 662e 7365 676d  merate(self.segm
+0000c2d0: 656e 7473 5b73 7461 7274 3a5d 2c20 7374  ents[start:], st
+0000c2e0: 6172 7420 6f72 2030 293a 0d0a 2020 2020  art or 0):..    
+0000c2f0: 2020 2020 2020 2020 732e 6964 203d 2069          s.id = i
+0000c300: 0d0a 2020 2020 2020 2020 2020 2020 732e  ..            s.
+0000c310: 7265 7375 6c74 203d 2073 656c 660d 0a20  result = self.. 
+0000c320: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000c330: 7420 6f6e 6c79 5f73 6567 6d65 6e74 733a  t only_segments:
+0000c340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c350: 2020 732e 7265 6173 7369 676e 5f69 6473    s.reassign_ids
+0000c360: 2829 0d0a 0d0a 2020 2020 6465 6620 7265  ()....    def re
+0000c370: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
+0000c380: 6d65 6e74 7328 7365 6c66 2c20 6967 6e6f  ments(self, igno
+0000c390: 7265 5f6f 7269 3d46 616c 7365 2c20 7265  re_ori=False, re
+0000c3a0: 6173 7369 676e 5f69 6473 3a20 626f 6f6c  assign_ids: bool
+0000c3b0: 203d 2054 7275 6529 3a0d 0a20 2020 2020   = True):..     
+0000c3c0: 2020 2066 6f72 2069 2069 6e20 7265 7665     for i in reve
+0000c3d0: 7273 6564 2872 616e 6765 286c 656e 2873  rsed(range(len(s
+0000c3e0: 656c 662e 7365 676d 656e 7473 2929 293a  elf.segments))):
+0000c3f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000c400: 2028 6967 6e6f 7265 5f6f 7269 206f 7220   (ignore_ori or 
+0000c410: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
+0000c420: 2e6f 7269 5f68 6173 5f77 6f72 6473 2920  .ori_has_words) 
+0000c430: 616e 6420 6e6f 7420 7365 6c66 2e73 6567  and not self.seg
+0000c440: 6d65 6e74 735b 695d 2e68 6173 5f77 6f72  ments[i].has_wor
+0000c450: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+0000c460: 2020 2020 2064 656c 2073 656c 662e 7365       del self.se
+0000c470: 676d 656e 7473 5b69 5d0d 0a20 2020 2020  gments[i]..     
+0000c480: 2020 2069 6620 7265 6173 7369 676e 5f69     if reassign_i
+0000c490: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+0000c4a0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
+0000c4b0: 6473 2829 0d0a 0d0a 2020 2020 6465 6620  ds()....    def 
+0000c4c0: 6765 745f 6c6f 636b 6564 5f69 6e64 6963  get_locked_indic
+0000c4d0: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+0000c4e0: 2020 206c 6f63 6b65 645f 696e 6469 6365     locked_indice
+0000c4f0: 7320 3d20 5b69 0d0a 2020 2020 2020 2020  s = [i..        
+0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c510: 2020 666f 7220 692c 2028 6c65 6674 2c20    for i, (left, 
+0000c520: 7269 6768 7429 2069 6e20 656e 756d 6572  right) in enumer
+0000c530: 6174 6528 7a69 7028 7365 6c66 2e73 6567  ate(zip(self.seg
+0000c540: 6d65 6e74 735b 313a 5d2c 2073 656c 662e  ments[1:], self.
+0000c550: 7365 676d 656e 7473 5b3a 2d31 5d29 290d  segments[:-1])).
+0000c560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c570: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000c580: 6674 2e6c 6566 745f 6c6f 636b 6564 206f  ft.left_locked o
+0000c590: 7220 7269 6768 742e 7269 6768 745f 6c6f  r right.right_lo
+0000c5a0: 636b 6564 5d0d 0a20 2020 2020 2020 2072  cked]..        r
+0000c5b0: 6574 7572 6e20 6c6f 636b 6564 5f69 6e64  eturn locked_ind
+0000c5c0: 6963 6573 0d0a 0d0a 2020 2020 6465 6620  ices....    def 
+0000c5d0: 6765 745f 6761 7073 2873 656c 662c 2061  get_gaps(self, a
+0000c5e0: 735f 6e64 6172 7261 793d 4661 6c73 6529  s_ndarray=False)
+0000c5f0: 3a0d 0a20 2020 2020 2020 2073 5f74 7320  :..        s_ts 
+0000c600: 3d20 6e70 2e61 7272 6179 285b 732e 7374  = np.array([s.st
+0000c610: 6172 7420 666f 7220 7320 696e 2073 656c  art for s in sel
+0000c620: 662e 7365 676d 656e 7473 5d29 0d0a 2020  f.segments])..  
+0000c630: 2020 2020 2020 655f 7473 203d 206e 702e        e_ts = np.
+0000c640: 6172 7261 7928 5b73 2e65 6e64 2066 6f72  array([s.end for
+0000c650: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
+0000c660: 6e74 735d 290d 0a20 2020 2020 2020 2067  nts])..        g
+0000c670: 6170 203d 2073 5f74 735b 313a 5d20 2d20  ap = s_ts[1:] - 
+0000c680: 655f 7473 5b3a 2d31 5d0d 0a20 2020 2020  e_ts[:-1]..     
+0000c690: 2020 2072 6574 7572 6e20 6761 7020 6966     return gap if
+0000c6a0: 2061 735f 6e64 6172 7261 7920 656c 7365   as_ndarray else
+0000c6b0: 2067 6170 2e74 6f6c 6973 7428 290d 0a0d   gap.tolist()...
+0000c6c0: 0a20 2020 2064 6566 2067 6574 5f67 6170  .    def get_gap
+0000c6d0: 5f69 6e64 6963 6573 2873 656c 662c 206d  _indices(self, m
+0000c6e0: 696e 5f67 6170 3a20 666c 6f61 7420 3d20  in_gap: float = 
+0000c6f0: 302e 3129 3a20 2023 2066 6f72 206d 6572  0.1):  # for mer
+0000c700: 6769 6e67 0d0a 2020 2020 2020 2020 6966  ging..        if
+0000c710: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
+0000c720: 7473 2920 3c20 323a 0d0a 2020 2020 2020  ts) < 2:..      
+0000c730: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
+0000c740: 0a20 2020 2020 2020 2069 6620 6d69 6e5f  .        if min_
+0000c750: 6761 7020 6973 204e 6f6e 653a 0d0a 2020  gap is None:..  
+0000c760: 2020 2020 2020 2020 2020 6d69 6e5f 6761            min_ga
+0000c770: 7020 3d20 300d 0a20 2020 2020 2020 2069  p = 0..        i
+0000c780: 6e64 6963 6573 203d 2028 7365 6c66 2e67  ndices = (self.g
+0000c790: 6574 5f67 6170 7328 5472 7565 2920 3c3d  et_gaps(True) <=
+0000c7a0: 206d 696e 5f67 6170 292e 6e6f 6e7a 6572   min_gap).nonzer
+0000c7b0: 6f28 295b 305d 2e74 6f6c 6973 7428 290d  o()[0].tolist().
+0000c7c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c7d0: 736f 7274 6564 2873 6574 2869 6e64 6963  sorted(set(indic
+0000c7e0: 6573 2920 2d20 7365 7428 7365 6c66 2e67  es) - set(self.g
+0000c7f0: 6574 5f6c 6f63 6b65 645f 696e 6469 6365  et_locked_indice
+0000c800: 7328 2929 290d 0a0d 0a20 2020 2064 6566  s()))....    def
+0000c810: 2067 6574 5f70 756e 6374 7561 7469 6f6e   get_punctuation
+0000c820: 5f69 6e64 6963 6573 2873 656c 662c 2070  _indices(self, p
+0000c830: 756e 6374 7561 7469 6f6e 3a20 556e 696f  unctuation: Unio
+0000c840: 6e5b 4c69 7374 5b73 7472 5d2c 204c 6973  n[List[str], Lis
+0000c850: 745b 5475 706c 655b 7374 722c 2073 7472  t[Tuple[str, str
+0000c860: 5d5d 2c20 7374 725d 293a 2020 2320 666f  ]], str]):  # fo
+0000c870: 7220 6d65 7267 696e 670d 0a20 2020 2020  r merging..     
+0000c880: 2020 2069 6620 6c65 6e28 7365 6c66 2e73     if len(self.s
+0000c890: 6567 6d65 6e74 7329 203c 2032 3a0d 0a20  egments) < 2:.. 
+0000c8a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c8b0: 6e20 5b5d 0d0a 2020 2020 2020 2020 6966  n []..        if
+0000c8c0: 2069 7369 6e73 7461 6e63 6528 7075 6e63   isinstance(punc
+0000c8d0: 7475 6174 696f 6e2c 2073 7472 293a 0d0a  tuation, str):..
+0000c8e0: 2020 2020 2020 2020 2020 2020 7075 6e63              punc
+0000c8f0: 7475 6174 696f 6e20 3d20 5b70 756e 6374  tuation = [punct
+0000c900: 7561 7469 6f6e 5d0d 0a20 2020 2020 2020  uation]..       
+0000c910: 2069 6e64 6963 6573 203d 205b 5d0d 0a20   indices = [].. 
+0000c920: 2020 2020 2020 2066 6f72 2070 2069 6e20         for p in 
+0000c930: 7075 6e63 7475 6174 696f 6e3a 0d0a 2020  punctuation:..  
+0000c940: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000c950: 6e73 7461 6e63 6528 702c 2073 7472 293a  nstance(p, str):
+0000c960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c970: 2020 666f 7220 692c 2073 2069 6e20 656e    for i, s in en
+0000c980: 756d 6572 6174 6528 7365 6c66 2e73 6567  umerate(self.seg
+0000c990: 6d65 6e74 735b 3a2d 315d 293a 0d0a 2020  ments[:-1]):..  
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 6966 2073 2e74 6578 742e 656e 6473    if s.text.ends
+0000c9c0: 7769 7468 2870 293a 0d0a 2020 2020 2020  with(p):..      
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9e0: 2020 696e 6469 6365 732e 6170 7065 6e64    indices.append
+0000c9f0: 2869 290d 0a20 2020 2020 2020 2020 2020  (i)..           
+0000ca00: 2020 2020 2020 2020 2065 6c69 6620 6920           elif i 
+0000ca10: 213d 2030 2061 6e64 2073 2e74 6578 742e  != 0 and s.text.
+0000ca20: 7374 6172 7473 7769 7468 2870 293a 0d0a  startswith(p):..
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 2020 2020 696e 6469 6365 732e          indices.
+0000ca50: 6170 7065 6e64 2869 2d31 290d 0a20 2020  append(i-1)..   
+0000ca60: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 656e 6469 6e67 2c20 6265 6769 6e6e 696e  ending, beginnin
+0000ca90: 6720 3d20 700d 0a20 2020 2020 2020 2020  g = p..         
+0000caa0: 2020 2020 2020 2069 6e64 6963 6573 2e65         indices.e
+0000cab0: 7874 656e 6428 5b69 2066 6f72 2069 2c20  xtend([i for i, 
+0000cac0: 2873 302c 2073 3129 2069 6e20 656e 756d  (s0, s1) in enum
+0000cad0: 6572 6174 6528 7a69 7028 7365 6c66 2e73  erate(zip(self.s
+0000cae0: 6567 6d65 6e74 735b 3a2d 315d 2c20 7365  egments[:-1], se
+0000caf0: 6c66 2e73 6567 6d65 6e74 735b 313a 5d29  lf.segments[1:])
+0000cb00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb20: 2020 2069 6620 7330 2e74 6578 742e 656e     if s0.text.en
+0000cb30: 6473 7769 7468 2865 6e64 696e 6729 2061  dswith(ending) a
+0000cb40: 6e64 2073 312e 7465 7874 2e73 7461 7274  nd s1.text.start
+0000cb50: 7377 6974 6828 6265 6769 6e6e 696e 6729  swith(beginning)
+0000cb60: 5d29 0d0a 0d0a 2020 2020 2020 2020 7265  ])....        re
+0000cb70: 7475 726e 2073 6f72 7465 6428 7365 7428  turn sorted(set(
+0000cb80: 696e 6469 6365 7329 202d 2073 6574 2873  indices) - set(s
+0000cb90: 656c 662e 6765 745f 6c6f 636b 6564 5f69  elf.get_locked_i
+0000cba0: 6e64 6963 6573 2829 2929 0d0a 0d0a 2020  ndices()))....  
+0000cbb0: 2020 6465 6620 616c 6c5f 776f 7264 7328    def all_words(
+0000cbc0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0000cbd0: 7265 7475 726e 206c 6973 7428 6368 6169  return list(chai
+0000cbe0: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
+0000cbf0: 732e 776f 7264 7320 666f 7220 7320 696e  s.words for s in
+0000cc00: 2073 656c 662e 7365 676d 656e 7473 2929   self.segments))
+0000cc10: 0d0a 0d0a 2020 2020 6465 6620 616c 6c5f  ....    def all_
+0000cc20: 776f 7264 735f 6f72 5f73 6567 6d65 6e74  words_or_segment
+0000cc30: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+0000cc40: 2020 7265 7475 726e 2073 656c 662e 616c    return self.al
+0000cc50: 6c5f 776f 7264 7328 2920 6966 2073 656c  l_words() if sel
+0000cc60: 662e 6861 735f 776f 7264 7320 656c 7365  f.has_words else
+0000cc70: 2073 656c 662e 7365 676d 656e 7473 0d0a   self.segments..
+0000cc80: 0d0a 2020 2020 6465 6620 616c 6c5f 776f  ..    def all_wo
+0000cc90: 7264 735f 6279 5f6c 6f63 6b28 7365 6c66  rds_by_lock(self
+0000cca0: 2c20 6f6e 6c79 5f74 6578 743a 2062 6f6f  , only_text: boo
+0000ccb0: 6c20 3d20 5472 7565 2c20 6279 5f73 6567  l = True, by_seg
+0000ccc0: 6d65 6e74 3a20 626f 6f6c 203d 2046 616c  ment: bool = Fal
+0000ccd0: 7365 2c20 696e 636c 7564 655f 7369 6e67  se, include_sing
+0000cce0: 6c65 3a20 626f 6f6c 203d 2046 616c 7365  le: bool = False
+0000ccf0: 293a 0d0a 2020 2020 2020 2020 6966 2062  ):..        if b
+0000cd00: 795f 7365 676d 656e 743a 0d0a 2020 2020  y_segment:..    
+0000cd10: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+0000cd20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cd30: 2020 7365 676d 656e 742e 776f 7264 735f    segment.words_
+0000cd40: 6279 5f6c 6f63 6b28 6f6e 6c79 5f74 6578  by_lock(only_tex
+0000cd50: 743d 6f6e 6c79 5f74 6578 742c 2069 6e63  t=only_text, inc
+0000cd60: 6c75 6465 5f73 696e 676c 653d 696e 636c  lude_single=incl
+0000cd70: 7564 655f 7369 6e67 6c65 290d 0a20 2020  ude_single)..   
+0000cd80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000cd90: 2073 6567 6d65 6e74 2069 6e20 7365 6c66   segment in self
+0000cda0: 2e73 6567 6d65 6e74 730d 0a20 2020 2020  .segments..     
+0000cdb0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+0000cdc0: 2020 7265 7475 726e 205f 776f 7264 735f    return _words_
+0000cdd0: 6279 5f6c 6f63 6b28 7365 6c66 2e61 6c6c  by_lock(self.all
+0000cde0: 5f77 6f72 6473 2829 2c20 6f6e 6c79 5f74  _words(), only_t
+0000cdf0: 6578 743d 6f6e 6c79 5f74 6578 742c 2069  ext=only_text, i
+0000ce00: 6e63 6c75 6465 5f73 696e 676c 653d 696e  nclude_single=in
+0000ce10: 636c 7564 655f 7369 6e67 6c65 290d 0a0d  clude_single)...
+0000ce20: 0a20 2020 2064 6566 2061 6c6c 5f74 6f6b  .    def all_tok
+0000ce30: 656e 7328 7365 6c66 293a 0d0a 2020 2020  ens(self):..    
+0000ce40: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
+0000ce50: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
+0000ce60: 626c 6528 732e 746f 6b65 6e73 2066 6f72  ble(s.tokens for
+0000ce70: 2073 2069 6e20 7365 6c66 2e61 6c6c 5f77   s in self.all_w
+0000ce80: 6f72 6473 2829 2929 0d0a 0d0a 2020 2020  ords()))....    
+0000ce90: 6465 6620 746f 5f64 6963 7428 7365 6c66  def to_dict(self
+0000cea0: 2c20 6b65 6570 5f6f 7269 673a 2062 6f6f  , keep_orig: boo
+0000ceb0: 6c20 3d20 5472 7565 293a 0d0a 2020 2020  l = True):..    
+0000cec0: 2020 2020 6f72 695f 6469 6374 203d 2073      ori_dict = s
+0000ced0: 656c 662e 6f72 695f 6469 6374 2069 6620  elf.ori_dict if 
+0000cee0: 6b65 6570 5f6f 7269 6720 656c 7365 207b  keep_orig else {
+0000cef0: 7d0d 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+0000cf00: 6e20 6469 6374 2874 6578 743d 7365 6c66  n dict(text=self
+0000cf10: 2e74 6578 742c 0d0a 2020 2020 2020 2020  .text,..        
+0000cf20: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+0000cf30: 656e 7473 3d73 656c 662e 7365 676d 656e  ents=self.segmen
+0000cf40: 7473 5f74 6f5f 6469 6374 7328 292c 0d0a  ts_to_dicts(),..
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf60: 2020 2020 6c61 6e67 7561 6765 3d73 656c      language=sel
+0000cf70: 662e 6c61 6e67 7561 6765 2c0d 0a20 2020  f.language,..   
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 206f 7269 5f64 6963 743d 6f72 695f 6469   ori_dict=ori_di
+0000cfa0: 6374 2c0d 0a20 2020 2020 2020 2020 2020  ct,..           
+0000cfb0: 2020 2020 2020 2020 2072 6567 726f 7570           regroup
+0000cfc0: 5f68 6973 746f 7279 3d73 656c 662e 5f72  _history=self._r
+0000cfd0: 6567 726f 7570 5f68 6973 746f 7279 2c0d  egroup_history,.
+0000cfe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cff0: 2020 2020 206e 6f6e 7370 6565 6368 5f73       nonspeech_s
+0000d000: 6563 7469 6f6e 733d 7365 6c66 2e5f 6e6f  ections=self._no
+0000d010: 6e73 7065 6563 685f 7365 6374 696f 6e73  nspeech_sections
+0000d020: 290d 0a0d 0a20 2020 2064 6566 2073 6567  )....    def seg
+0000d030: 6d65 6e74 735f 746f 5f64 6963 7473 2873  ments_to_dicts(s
+0000d040: 656c 662c 2072 6576 6572 7365 5f74 6578  elf, reverse_tex
+0000d050: 743a 2055 6e69 6f6e 5b62 6f6f 6c2c 2074  t: Union[bool, t
+0000d060: 7570 6c65 5d20 3d20 4661 6c73 6529 3a0d  uple] = False):.
+0000d070: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000d080: 5b73 2e74 6f5f 6469 6374 2872 6576 6572  [s.to_dict(rever
+0000d090: 7365 5f74 6578 743d 7265 7665 7273 655f  se_text=reverse_
+0000d0a0: 7465 7874 2920 666f 7220 7320 696e 2073  text) for s in s
+0000d0b0: 656c 662e 7365 676d 656e 7473 5d0d 0a0d  elf.segments]...
+0000d0c0: 0a20 2020 2064 6566 205f 7370 6c69 745f  .    def _split_
+0000d0d0: 7365 676d 656e 7473 2873 656c 662c 2067  segments(self, g
+0000d0e0: 6574 5f69 6e64 6963 6573 2c20 6172 6773  et_indices, args
+0000d0f0: 3a20 6c69 7374 203d 204e 6f6e 652c 202a  : list = None, *
+0000d100: 2c20 6c6f 636b 3a20 626f 6f6c 203d 2046  , lock: bool = F
+0000d110: 616c 7365 2c20 6e65 776c 696e 653a 2062  alse, newline: b
+0000d120: 6f6f 6c20 3d20 4661 6c73 6529 3a0d 0a20  ool = False):.. 
+0000d130: 2020 2020 2020 2069 6620 6172 6773 2069         if args i
+0000d140: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+0000d150: 2020 2020 2061 7267 7320 3d20 5b5d 0d0a       args = []..
+0000d160: 2020 2020 2020 2020 6e6f 5f77 6f72 6473          no_words
+0000d170: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+0000d180: 2020 666f 7220 6920 696e 2072 6576 6572    for i in rever
+0000d190: 7365 6428 7261 6e67 6528 302c 206c 656e  sed(range(0, len
+0000d1a0: 2873 656c 662e 7365 676d 656e 7473 2929  (self.segments))
+0000d1b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000d1c0: 6e6f 5f77 6f72 6473 203d 206e 6f5f 776f  no_words = no_wo
+0000d1d0: 7264 7320 6f72 206e 6f74 2073 656c 662e  rds or not self.
+0000d1e0: 7365 676d 656e 7473 5b69 5d2e 6861 735f  segments[i].has_
+0000d1f0: 776f 7264 730d 0a20 2020 2020 2020 2020  words..         
+0000d200: 2020 2069 6e64 6963 6573 203d 2073 6f72     indices = sor
+0000d210: 7465 6428 7365 7428 6765 745f 696e 6469  ted(set(get_indi
+0000d220: 6365 7328 7365 6c66 2e73 6567 6d65 6e74  ces(self.segment
+0000d230: 735b 695d 2c20 2a61 7267 7329 2929 0d0a  s[i], *args)))..
+0000d240: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000d250: 6f74 2069 6e64 6963 6573 3a0d 0a20 2020  ot indices:..   
+0000d260: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000d270: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
+0000d280: 2020 2069 6620 6e65 776c 696e 653a 0d0a     if newline:..
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 6966 2069 6e64 6963 6573 5b2d 315d 203d  if indices[-1] =
+0000d2b0: 3d20 6c65 6e28 7365 6c66 2e73 6567 6d65  = len(self.segme
+0000d2c0: 6e74 735b 695d 2e77 6f72 6473 2920 2d20  nts[i].words) - 
+0000d2d0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0000d2e0: 2020 2020 2020 2020 6465 6c20 696e 6469          del indi
+0000d2f0: 6365 735b 2d31 5d0d 0a20 2020 2020 2020  ces[-1]..       
+0000d300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d310: 6e6f 7420 696e 6469 6365 733a 0d0a 2020  not indices:..  
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+0000d340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d350: 2020 666f 7220 776f 7264 5f69 6478 2069    for word_idx i
+0000d360: 6e20 696e 6469 6365 733a 0d0a 2020 2020  n indices:..    
+0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d380: 6966 2073 656c 662e 7365 676d 656e 7473  if self.segments
+0000d390: 5b69 5d2e 776f 7264 735b 776f 7264 5f69  [i].words[word_i
+0000d3a0: 6478 5d2e 776f 7264 2e65 6e64 7377 6974  dx].word.endswit
+0000d3b0: 6828 275c 6e27 293a 0d0a 2020 2020 2020  h('\n'):..      
+0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3d0: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
+0000d400: 2e77 6f72 6473 5b77 6f72 645f 6964 785d  .words[word_idx]
+0000d410: 2e77 6f72 6420 2b3d 2027 5c6e 270d 0a20  .word += '\n'.. 
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 2020 2069 6620 6c6f 636b 3a0d 0a20 2020     if lock:..   
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
+0000d460: 7473 5b69 5d2e 776f 7264 735b 776f 7264  ts[i].words[word
+0000d470: 5f69 6478 5d2e 6c6f 636b 5f72 6967 6874  _idx].lock_right
+0000d480: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000d490: 2020 2020 2020 2020 2020 2020 6966 2077              if w
+0000d4a0: 6f72 645f 6964 7820 2b20 3120 3c20 6c65  ord_idx + 1 < le
+0000d4b0: 6e28 7365 6c66 2e73 6567 6d65 6e74 735b  n(self.segments[
+0000d4c0: 695d 2e77 6f72 6473 293a 0d0a 2020 2020  i].words):..    
+0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4e0: 2020 2020 2020 2020 7365 6c66 2e73 6567          self.seg
+0000d4f0: 6d65 6e74 735b 695d 2e77 6f72 6473 5b77  ments[i].words[w
+0000d500: 6f72 645f 6964 782b 315d 2e6c 6f63 6b5f  ord_idx+1].lock_
+0000d510: 6c65 6674 2829 0d0a 2020 2020 2020 2020  left()..        
+0000d520: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000d530: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+0000d540: 6567 6d65 6e74 7320 3d20 7365 6c66 2e73  egments = self.s
+0000d550: 6567 6d65 6e74 735b 695d 2e73 706c 6974  egments[i].split
+0000d560: 2869 6e64 6963 6573 290d 0a20 2020 2020  (indices)..     
+0000d570: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+0000d580: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000d590: 2020 2020 2020 2020 2066 6f72 2073 2069           for s i
+0000d5a0: 6e20 6e65 775f 7365 676d 656e 7473 3a0d  n new_segments:.
+0000d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d5c0: 2020 2020 2020 2020 2069 6620 7320 3d3d           if s ==
+0000d5d0: 206e 6577 5f73 6567 6d65 6e74 735b 305d   new_segments[0]
+0000d5e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d600: 2e6c 6f63 6b5f 7269 6768 7428 290d 0a20  .lock_right().. 
 0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 206d 6178 5f77 6f72 6473 2061 6e64 0d0a   max_words and..
+0000d620: 2020 2020 2020 2065 6c69 6620 7320 3d3d         elif s ==
+0000d630: 206e 6577 5f73 6567 6d65 6e74 735b 2d31   new_segments[-1
+0000d640: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
 0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2020 2020 2020 2020 2020 2020 7365 672e              seg.
-0000d670: 6861 735f 776f 7264 7320 616e 640d 0a20  has_words and.. 
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
-0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2873 6567 2e77 6f72 645f 636f 756e    (seg.word_coun
-0000d6d0: 7428 2920 2b20 7365 6c66 2e73 6567 6d65  t() + self.segme
-0000d6e0: 6e74 735b 6920 2b20 315d 2e77 6f72 645f  nts[i + 1].word_
-0000d6f0: 636f 756e 7428 2920 3e20 6d61 785f 776f  count() > max_wo
-0000d700: 7264 7329 0d0a 2020 2020 2020 2020 2020  rds)..          
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
-0000d730: 7375 6d5f 6d61 7820 656c 7365 0d0a 2020  sum_max else..  
-0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2873 6567 2e77 6f72 645f 636f 756e    (seg.word_coun
-0000d770: 7428 2920 3e20 6d61 785f 776f 7264 7320  t() > max_words 
-0000d780: 616e 6420 7365 6c66 2e73 6567 6d65 6e74  and self.segment
-0000d790: 735b 6920 2b20 315d 2e77 6f72 645f 636f  s[i + 1].word_co
-0000d7a0: 756e 7428 2920 3e20 6d61 785f 776f 7264  unt() > max_word
-0000d7b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d7e0: 2020 2020 2020 2029 206f 720d 0a20 2020         ) or..   
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d800: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 6d61 785f 6368 6172 7320 616e 640d 0a20  max_chars and.. 
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d840: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
-0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 2873 6567 2e63 6861 725f 636f 756e    (seg.char_coun
-0000d880: 7428 2920 2b20 7365 6c66 2e73 6567 6d65  t() + self.segme
-0000d890: 6e74 735b 6920 2b20 315d 2e63 6861 725f  nts[i + 1].char_
-0000d8a0: 636f 756e 7428 2920 3e20 6d61 785f 6368  count() > max_ch
-0000d8b0: 6172 7329 0d0a 2020 2020 2020 2020 2020  ars)..          
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8d0: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
-0000d8e0: 7375 6d5f 6d61 7820 656c 7365 0d0a 2020  sum_max else..  
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d910: 2020 2873 6567 2e63 6861 725f 636f 756e    (seg.char_coun
-0000d920: 7428 2920 3e20 6d61 785f 6368 6172 7320  t() > max_chars 
-0000d930: 616e 6420 7365 6c66 2e73 6567 6d65 6e74  and self.segment
-0000d940: 735b 6920 2b20 315d 2e63 6861 725f 636f  s[i + 1].char_co
-0000d950: 756e 7428 2920 3e20 6d61 785f 6368 6172  unt() > max_char
-0000d960: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d990: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000d9a0: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
-0000d9b0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000d9c0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-0000d9d0: 7365 6c66 2e61 6464 5f73 6567 6d65 6e74  self.add_segment
-0000d9e0: 7328 692c 2069 202b 2031 2c20 696e 706c  s(i, i + 1, inpl
-0000d9f0: 6163 653d 5472 7565 2c20 6c6f 636b 3d6c  ace=True, lock=l
-0000da00: 6f63 6b29 0d0a 2020 2020 2020 2020 7365  ock)..        se
-0000da10: 6c66 2e72 656d 6f76 655f 6e6f 5f77 6f72  lf.remove_no_wor
-0000da20: 645f 7365 676d 656e 7473 2829 0d0a 0d0a  d_segments()....
-0000da30: 2020 2020 6465 6620 6765 745f 636f 6e74      def get_cont
-0000da40: 656e 745f 6279 5f74 696d 6528 0d0a 2020  ent_by_time(..  
-0000da50: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-0000da60: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-0000da70: 653a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  e: Union[float, 
-0000da80: 5475 706c 655b 666c 6f61 742c 2066 6c6f  Tuple[float, flo
-0000da90: 6174 5d2c 2064 6963 745d 2c0d 0a20 2020  at], dict],..   
-0000daa0: 2020 2020 2020 2020 2077 6974 6869 6e3a           within:
-0000dab0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-0000dac0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
-0000dad0: 656e 745f 6c65 7665 6c3a 2062 6f6f 6c20  ent_level: bool 
-0000dae0: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
-0000daf0: 3e20 556e 696f 6e5b 4c69 7374 5b57 6f72  > Union[List[Wor
-0000db00: 6454 696d 696e 675d 2c20 4c69 7374 5b53  dTiming], List[S
-0000db10: 6567 6d65 6e74 5d5d 3a0d 0a20 2020 2020  egment]]:..     
-0000db20: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000db30: 5265 7475 726e 2063 6f6e 7465 6e74 2069  Return content i
-0000db40: 6e20 7468 6520 6060 7469 6d65 6060 2072  n the ``time`` r
-0000db50: 616e 6765 2e0d 0a0d 0a20 2020 2020 2020  ange.....       
-0000db60: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-0000db70: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-0000db80: 0a20 2020 2020 2020 2074 696d 6520 3a20  .        time : 
-0000db90: 666c 6f61 7420 6f72 2074 7570 6c65 206f  float or tuple o
-0000dba0: 6620 2866 6c6f 6174 2c20 666c 6f61 7429  f (float, float)
-0000dbb0: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
-0000dbc0: 2020 2020 2020 5261 6e67 6520 6f66 2074        Range of t
-0000dbd0: 696d 6520 746f 2066 696e 6420 636f 6e74  ime to find cont
-0000dbe0: 656e 742e 2046 6f72 2074 7570 6c65 206f  ent. For tuple o
-0000dbf0: 6620 7477 6f20 666c 6f61 7473 2c20 6669  f two floats, fi
-0000dc00: 7273 7420 7661 6c75 6520 6973 2074 6865  rst value is the
-0000dc10: 2073 7461 7274 2074 696d 6520 616e 6420   start time and 
-0000dc20: 7365 636f 6e64 2076 616c 7565 2069 730d  second value is.
-0000dc30: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-0000dc40: 2065 6e64 2074 696d 652e 2046 6f72 2061   end time. For a
-0000dc50: 2073 696e 676c 6520 666c 6f61 7420 7661   single float va
-0000dc60: 6c75 652c 2069 7420 6973 2074 7265 6174  lue, it is treat
-0000dc70: 6564 2061 7320 626f 7468 2074 6865 2073  ed as both the s
-0000dc80: 7461 7274 2061 6e64 2065 6e64 2074 696d  tart and end tim
-0000dc90: 652e 0d0a 2020 2020 2020 2020 7769 7468  e...        with
-0000dca0: 696e 203a 2062 6f6f 6c2c 2064 6566 6175  in : bool, defau
-0000dcb0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-0000dcc0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-0000dcd0: 206f 6e6c 7920 6669 6e64 2063 6f6e 7465   only find conte
-0000dce0: 6e74 2066 756c 6c79 206f 7665 726c 6170  nt fully overlap
-0000dcf0: 7320 7769 7468 2060 6074 696d 6560 6020  s with ``time`` 
-0000dd00: 7261 6e67 652e 0d0a 2020 2020 2020 2020  range...        
-0000dd10: 7365 676d 656e 745f 6c65 7665 6c20 3a20  segment_level : 
-0000dd20: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0000dd30: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-0000dd40: 2057 6865 7468 6572 2074 6f20 6c6f 6f6b   Whether to look
-0000dd50: 206f 6e6c 7920 6f6e 2074 6865 2073 6567   only on the seg
-0000dd60: 6d65 6e74 206c 6576 656c 2061 6e64 2072  ment level and r
-0000dd70: 6574 7572 6e20 696e 7374 616e 6365 7320  eturn instances 
-0000dd80: 6f66 203a 636c 6173 733a 6073 7461 626c  of :class:`stabl
-0000dd90: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
-0000dda0: 2e53 6567 6d65 6e74 600d 0a20 2020 2020  .Segment`..     
-0000ddb0: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
-0000ddc0: 6620 3a63 6c61 7373 3a60 7374 6162 6c65  f :class:`stable
-0000ddd0: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-0000dde0: 576f 7264 5469 6d69 6e67 602e 0d0a 0d0a  WordTiming`.....
-0000ddf0: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
-0000de00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000de10: 0d0a 2020 2020 2020 2020 6c69 7374 206f  ..        list o
-0000de20: 6620 7374 6162 6c65 5f77 6869 7370 6572  f stable_whisper
-0000de30: 2e72 6573 756c 742e 576f 7264 5469 6d69  .result.WordTimi
-0000de40: 6e67 206f 7220 6c69 7374 206f 6620 7374  ng or list of st
-0000de50: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
-0000de60: 756c 742e 5365 676d 656e 740d 0a20 2020  ult.Segment..   
-0000de70: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
-0000de80: 2063 6f6e 7465 6e74 7320 696e 2074 6865   contents in the
-0000de90: 2060 6074 696d 6560 6020 7261 6e67 652e   ``time`` range.
-0000dea0: 2054 6865 2063 6f6e 7465 6e74 7320 6172   The contents ar
-0000deb0: 6520 696e 7374 616e 6365 7320 6f66 0d0a  e instances of..
-0000dec0: 2020 2020 2020 2020 2020 2020 3a63 6c61              :cla
-0000ded0: 7373 3a60 7374 6162 6c65 5f77 6869 7370  ss:`stable_whisp
-0000dee0: 6572 2e72 6573 756c 742e 5365 676d 656e  er.result.Segmen
-0000def0: 7460 2069 6620 6060 7365 676d 656e 745f  t` if ``segment_
-0000df00: 6c65 7665 6c20 3d20 5472 7565 6060 2065  level = True`` e
-0000df10: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-0000df20: 203a 636c 6173 733a 6073 7461 626c 655f   :class:`stable_
-0000df30: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-0000df40: 6f72 6454 696d 696e 6760 2e0d 0a20 2020  ordTiming`...   
-0000df50: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000df60: 2020 6966 206e 6f74 2073 6567 6d65 6e74    if not segment
-0000df70: 5f6c 6576 656c 2061 6e64 206e 6f74 2073  _level and not s
-0000df80: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
-0000df90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000dfa0: 6520 5661 6c75 6545 7272 6f72 2827 4d69  e ValueError('Mi
-0000dfb0: 7373 696e 6720 776f 7264 2074 696d 6573  ssing word times
-0000dfc0: 7461 6d70 7320 696e 2072 6573 756c 742e  tamps in result.
-0000dfd0: 2055 7365 2060 6073 6567 6d65 6e74 5f6c   Use ``segment_l
-0000dfe0: 6576 656c 3d54 7275 6560 6020 696e 7374  evel=True`` inst
-0000dff0: 6561 642e 2729 0d0a 2020 2020 2020 2020  ead.')..        
-0000e000: 636f 6e74 656e 7473 203d 2073 656c 662e  contents = self.
-0000e010: 7365 676d 656e 7473 2069 6620 7365 676d  segments if segm
-0000e020: 656e 745f 6c65 7665 6c20 656c 7365 2073  ent_level else s
-0000e030: 656c 662e 616c 6c5f 776f 7264 7328 290d  elf.all_words().
-0000e040: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000e050: 7374 616e 6365 2874 696d 652c 2028 666c  stance(time, (fl
-0000e060: 6f61 742c 2069 6e74 2929 3a0d 0a20 2020  oat, int)):..   
-0000e070: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
-0000e080: 5b74 696d 652c 2074 696d 655d 0d0a 2020  [time, time]..  
-0000e090: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0000e0a0: 7461 6e63 6528 7469 6d65 2c20 6469 6374  tance(time, dict
-0000e0b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000e0c0: 7469 6d65 203d 205b 7469 6d65 5b27 7374  time = [time['st
-0000e0d0: 6172 7427 5d2c 2074 696d 655b 2765 6e64  art'], time['end
-0000e0e0: 275d 5d0d 0a20 2020 2020 2020 2073 7461  ']]..        sta
-0000e0f0: 7274 2c20 656e 6420 3d20 7469 6d65 0d0a  rt, end = time..
-0000e100: 0d0a 2020 2020 2020 2020 6966 2077 6974  ..        if wit
-0000e110: 6869 6e3a 0d0a 2020 2020 2020 2020 2020  hin:..          
-0000e120: 2020 6465 6620 6973 5f69 6e5f 7261 6e67    def is_in_rang
-0000e130: 6528 6329 3a0d 0a20 2020 2020 2020 2020  e(c):..         
-0000e140: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-0000e150: 6172 7420 3c3d 2063 2e73 7461 7274 2061  art <= c.start a
-0000e160: 6e64 2065 6e64 203e 3d20 632e 656e 640d  nd end >= c.end.
-0000e170: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0000e180: 2020 2020 2020 2020 2020 2020 6465 6620              def 
-0000e190: 6973 5f69 6e5f 7261 6e67 6528 6329 3a0d  is_in_range(c):.
-0000e1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e1b0: 2072 6574 7572 6e20 7374 6172 7420 3c3d   return start <=
-0000e1c0: 2063 2e65 6e64 2061 6e64 2065 6e64 203e   c.end and end >
-0000e1d0: 3d20 632e 7374 6172 740d 0a0d 0a20 2020  = c.start....   
-0000e1e0: 2020 2020 2072 6574 7572 6e20 5b63 2066       return [c f
-0000e1f0: 6f72 2063 2069 6e20 636f 6e74 656e 7473  or c in contents
-0000e200: 2069 6620 6973 5f69 6e5f 7261 6e67 6528   if is_in_range(
-0000e210: 6329 5d0d 0a0d 0a20 2020 2064 6566 2073  c)]....    def s
-0000e220: 706c 6974 5f62 795f 6761 7028 0d0a 2020  plit_by_gap(..  
-0000e230: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-0000e240: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000e250: 5f67 6170 3a20 666c 6f61 7420 3d20 302e  _gap: float = 0.
-0000e260: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
-0000e270: 6c6f 636b 3a20 626f 6f6c 203d 2046 616c  lock: bool = Fal
-0000e280: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000e290: 206e 6577 6c69 6e65 3a20 626f 6f6c 203d   newline: bool =
-0000e2a0: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
-0000e2b0: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
-0000e2c0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000e2d0: 2020 2020 2020 2020 5370 6c69 7420 2869          Split (i
-0000e2e0: 6e2d 706c 6163 6529 2061 6e79 2073 6567  n-place) any seg
-0000e2f0: 6d65 6e74 2077 6865 7265 2074 6865 2067  ment where the g
-0000e300: 6170 2062 6574 7765 656e 2074 776f 206f  ap between two o
-0000e310: 6620 6974 7320 776f 7264 7320 6973 2067  f its words is g
-0000e320: 7265 6174 6572 2074 6861 6e20 6060 6d61  reater than ``ma
-0000e330: 785f 6761 7060 602e 0d0a 0d0a 2020 2020  x_gap``.....    
-0000e340: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-0000e350: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000e360: 2d2d 0d0a 2020 2020 2020 2020 6d61 785f  --..        max_
-0000e370: 6761 7020 3a20 666c 6f61 742c 2064 6566  gap : float, def
-0000e380: 6175 6c74 2030 2e31 0d0a 2020 2020 2020  ault 0.1..      
-0000e390: 2020 2020 2020 4d61 7869 6d75 6d20 7365        Maximum se
-0000e3a0: 636f 6e64 2873 2920 616c 6c6f 7765 6420  cond(s) allowed 
-0000e3b0: 6265 7477 6565 6e20 7477 6f20 776f 7264  between two word
-0000e3c0: 7320 6966 2074 6865 2073 616d 6520 7365  s if the same se
-0000e3d0: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
-0000e3e0: 6c6f 636b 203a 2062 6f6f 6c2c 2064 6566  lock : bool, def
-0000e3f0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-0000e400: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-0000e410: 746f 2070 7265 7665 6e74 2066 7574 7572  to prevent futur
-0000e420: 6520 7370 6c69 7473 2f6d 6572 6765 7320  e splits/merges 
-0000e430: 6672 6f6d 2061 6c74 6572 696e 6720 6368  from altering ch
-0000e440: 616e 6765 7320 6d61 6465 2062 7920 7468  anges made by th
-0000e450: 6973 206d 6574 686f 642e 0d0a 2020 2020  is method...    
-0000e460: 2020 2020 6e65 776c 696e 653a 2062 6f6f      newline: boo
-0000e470: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-0000e480: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-0000e490: 6574 6865 7220 746f 2069 6e73 6572 7420  ether to insert 
-0000e4a0: 6c69 6e65 2062 7265 616b 2061 7420 7468  line break at th
-0000e4b0: 6520 7370 6c69 7420 706f 696e 7473 2069  e split points i
-0000e4c0: 6e73 7465 6164 206f 6620 7370 6c69 7474  nstead of splitt
-0000e4d0: 696e 6720 696e 746f 2073 6570 6172 6174  ing into separat
-0000e4e0: 6520 7365 676d 656e 7473 2e0d 0a0d 0a20  e segments..... 
-0000e4f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-0000e500: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-0000e510: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-0000e520: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-0000e530: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-0000e540: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-0000e550: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-0000e560: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-0000e570: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-0000e580: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-0000e590: 6c69 745f 7365 676d 656e 7473 286c 616d  lit_segments(lam
-0000e5a0: 6264 6120 783a 2078 2e67 6574 5f67 6170  bda x: x.get_gap
-0000e5b0: 5f69 6e64 6963 6573 286d 6178 5f67 6170  _indices(max_gap
-0000e5c0: 292c 206c 6f63 6b3d 6c6f 636b 2c20 6e65  ), lock=lock, ne
-0000e5d0: 776c 696e 653d 6e65 776c 696e 6529 0d0a  wline=newline)..
-0000e5e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e5f0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-0000e600: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0000e610: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
-0000e620: 746f 7279 202b 3d20 275f 270d 0a20 2020  tory += '_'..   
-0000e630: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-0000e640: 7570 5f68 6973 746f 7279 202b 3d20 6627  up_history += f'
-0000e650: 7367 3d7b 6d61 785f 6761 707d 2b7b 696e  sg={max_gap}+{in
-0000e660: 7428 6c6f 636b 297d 2b7b 696e 7428 6e65  t(lock)}+{int(ne
-0000e670: 776c 696e 6529 7d27 0d0a 2020 2020 2020  wline)}'..      
-0000e680: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-0000e690: 0a20 2020 2064 6566 206d 6572 6765 5f62  .    def merge_b
-0000e6a0: 795f 6761 7028 0d0a 2020 2020 2020 2020  y_gap(..        
-0000e6b0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-0000e6c0: 2020 2020 2020 206d 696e 5f67 6170 3a20         min_gap: 
-0000e6d0: 666c 6f61 7420 3d20 302e 312c 0d0a 2020  float = 0.1,..  
-0000e6e0: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
-0000e6f0: 7264 733a 2069 6e74 203d 204e 6f6e 652c  rds: int = None,
-0000e700: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-0000e710: 785f 6368 6172 733a 2069 6e74 203d 204e  x_chars: int = N
-0000e720: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-0000e730: 2020 6973 5f73 756d 5f6d 6178 3a20 626f    is_sum_max: bo
-0000e740: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-0000e750: 2020 2020 2020 2020 206c 6f63 6b3a 2062           lock: b
-0000e760: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
-0000e770: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
-0000e780: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
-0000e790: 2222 220d 0a20 2020 2020 2020 204d 6572  """..        Mer
-0000e7a0: 6765 2028 696e 2d70 6c61 6365 2920 616e  ge (in-place) an
-0000e7b0: 7920 7061 6972 206f 6620 6164 6a61 6365  y pair of adjace
-0000e7c0: 6e74 2073 6567 6d65 6e74 7320 6966 2074  nt segments if t
-0000e7d0: 6865 2067 6170 2062 6574 7765 656e 2074  he gap between t
-0000e7e0: 6865 6d20 3c3d 2060 606d 696e 5f67 6170  hem <= ``min_gap
-0000e7f0: 6060 2e0d 0a0d 0a20 2020 2020 2020 2050  ``.....        P
-0000e800: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0000e810: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-0000e820: 2020 2020 2020 206d 696e 5f67 6170 203a         min_gap :
-0000e830: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-0000e840: 302e 310d 0a20 2020 2020 2020 2020 2020  0.1..           
-0000e850: 204d 696e 696d 756d 2073 6563 6f6e 6428   Minimum second(
-0000e860: 7329 2061 6c6c 6f77 2062 6574 7765 656e  s) allow between
-0000e870: 2074 776f 2073 6567 6d65 6e74 2e0d 0a20   two segment... 
-0000e880: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
-0000e890: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-0000e8a0: 0d0a 2020 2020 2020 2020 2020 2020 4d61  ..            Ma
-0000e8b0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-0000e8c0: 776f 7264 7320 616c 6c6f 7765 6420 696e  words allowed in
-0000e8d0: 2065 6163 6820 7365 676d 656e 742e 0d0a   each segment...
-0000e8e0: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
-0000e8f0: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
-0000e900: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
-0000e910: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-0000e920: 2063 6861 7261 6374 6572 7320 616c 6c6f   characters allo
-0000e930: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
-0000e940: 656e 742e 0d0a 2020 2020 2020 2020 6973  ent...        is
-0000e950: 5f73 756d 5f6d 6178 203a 2062 6f6f 6c2c  _sum_max : bool,
-0000e960: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-0000e970: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-0000e980: 6865 7220 6060 6d61 785f 776f 7264 7360  her ``max_words`
-0000e990: 6020 616e 6420 6060 6d61 785f 6368 6172  ` and ``max_char
-0000e9a0: 7360 6020 6973 2061 7070 6c69 6564 2074  s`` is applied t
-0000e9b0: 6f20 7468 6520 6d65 7267 6564 2073 6567  o the merged seg
-0000e9c0: 6d65 6e74 2069 6e73 7465 6164 206f 6620  ment instead of 
-0000e9d0: 7468 6520 696e 6469 7669 6475 616c 2073  the individual s
-0000e9e0: 6567 6d65 6e74 730d 0a20 2020 2020 2020  egments..       
-0000e9f0: 2020 2020 2074 6f20 6265 206d 6572 6765       to be merge
-0000ea00: 642e 0d0a 2020 2020 2020 2020 6c6f 636b  d...        lock
-0000ea10: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0000ea20: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0000ea30: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-0000ea40: 7265 7665 6e74 2066 7574 7572 6520 7370  revent future sp
-0000ea50: 6c69 7473 2f6d 6572 6765 7320 6672 6f6d  lits/merges from
-0000ea60: 2061 6c74 6572 696e 6720 6368 616e 6765   altering change
-0000ea70: 7320 6d61 6465 2062 7920 7468 6973 206d  s made by this m
-0000ea80: 6574 686f 642e 0d0a 0d0a 2020 2020 2020  ethod.....      
-0000ea90: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
-0000eaa0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-0000eab0: 2020 2020 7374 6162 6c65 5f77 6869 7370      stable_whisp
-0000eac0: 6572 2e72 6573 756c 742e 5768 6973 7065  er.result.Whispe
-0000ead0: 7252 6573 756c 740d 0a20 2020 2020 2020  rResult..       
-0000eae0: 2020 2020 2054 6865 2063 7572 7265 6e74       The current
-0000eaf0: 2069 6e73 7461 6e63 6520 6166 7465 7220   instance after 
-0000eb00: 7468 6520 6368 616e 6765 732e 0d0a 2020  the changes...  
-0000eb10: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000eb20: 2020 2069 6e64 6963 6573 203d 2073 656c     indices = sel
-0000eb30: 662e 6765 745f 6761 705f 696e 6469 6365  f.get_gap_indice
-0000eb40: 7328 6d69 6e5f 6761 7029 0d0a 2020 2020  s(min_gap)..    
-0000eb50: 2020 2020 7365 6c66 2e5f 6d65 7267 655f      self._merge_
-0000eb60: 7365 676d 656e 7473 2869 6e64 6963 6573  segments(indices
-0000eb70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb90: 6d61 785f 776f 7264 733d 6d61 785f 776f  max_words=max_wo
-0000eba0: 7264 732c 206d 6178 5f63 6861 7273 3d6d  rds, max_chars=m
-0000ebb0: 6178 5f63 6861 7273 2c20 6973 5f73 756d  ax_chars, is_sum
-0000ebc0: 5f6d 6178 3d69 735f 7375 6d5f 6d61 782c  _max=is_sum_max,
-0000ebd0: 206c 6f63 6b3d 6c6f 636b 290d 0a20 2020   lock=lock)..   
-0000ebe0: 2020 2020 2069 6620 7365 6c66 2e5f 7265       if self._re
-0000ebf0: 6772 6f75 705f 6869 7374 6f72 793a 0d0a  group_history:..
-0000ec00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ec10: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
-0000ec20: 7920 2b3d 2027 5f27 0d0a 2020 2020 2020  y += '_'..      
-0000ec30: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-0000ec40: 6869 7374 6f72 7920 2b3d 2066 276d 673d  history += f'mg=
-0000ec50: 7b6d 696e 5f67 6170 7d2b 7b6d 6178 5f77  {min_gap}+{max_w
-0000ec60: 6f72 6473 206f 7220 2222 7d2b 7b6d 6178  ords or ""}+{max
-0000ec70: 5f63 6861 7273 206f 7220 2222 7d2b 7b69  _chars or ""}+{i
-0000ec80: 6e74 2869 735f 7375 6d5f 6d61 7829 7d2b  nt(is_sum_max)}+
-0000ec90: 7b69 6e74 286c 6f63 6b29 7d27 0d0a 2020  {int(lock)}'..  
-0000eca0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000ecb0: 660d 0a0d 0a20 2020 2064 6566 2073 706c  f....    def spl
-0000ecc0: 6974 5f62 795f 7075 6e63 7475 6174 696f  it_by_punctuatio
-0000ecd0: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
-0000ece0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-0000ecf0: 2020 2070 756e 6374 7561 7469 6f6e 3a20     punctuation: 
-0000ed00: 556e 696f 6e5b 4c69 7374 5b73 7472 5d2c  Union[List[str],
-0000ed10: 204c 6973 745b 5475 706c 655b 7374 722c   List[Tuple[str,
-0000ed20: 2073 7472 5d5d 2c20 7374 725d 2c0d 0a20   str]], str],.. 
-0000ed30: 2020 2020 2020 2020 2020 206c 6f63 6b3a             lock:
-0000ed40: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-0000ed50: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
-0000ed60: 696e 653a 2062 6f6f 6c20 3d20 4661 6c73  ine: bool = Fals
-0000ed70: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ed80: 6d69 6e5f 776f 7264 733a 204f 7074 696f  min_words: Optio
-0000ed90: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0000eda0: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0000edb0: 6e5f 6368 6172 733a 204f 7074 696f 6e61  n_chars: Optiona
-0000edc0: 6c5b 696e 745d 203d 204e 6f6e 652c 0d0a  l[int] = None,..
-0000edd0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-0000ede0: 6475 723a 204f 7074 696f 6e61 6c5b 696e  dur: Optional[in
-0000edf0: 745d 203d 204e 6f6e 650d 0a20 2020 2029  t] = None..    )
-0000ee00: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
-0000ee10: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
-0000ee20: 220d 0a20 2020 2020 2020 2053 706c 6974  "..        Split
-0000ee30: 2028 696e 2d70 6c61 6365 2920 7365 676d   (in-place) segm
-0000ee40: 656e 7473 2061 7420 776f 7264 7320 7468  ents at words th
-0000ee50: 6174 2073 7461 7274 2f65 6e64 2077 6974  at start/end wit
-0000ee60: 6820 6060 7075 6e63 7475 6174 696f 6e60  h ``punctuation`
-0000ee70: 602e 0d0a 0d0a 2020 2020 2020 2020 5061  `.....        Pa
-0000ee80: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-0000ee90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-0000eea0: 2020 2020 2020 7075 6e63 7475 6174 696f        punctuatio
-0000eeb0: 6e20 3a20 6c69 7374 206f 6620 7374 7220  n : list of str 
-0000eec0: 6f66 206c 6973 7420 6f66 2074 7570 6c65  of list of tuple
-0000eed0: 206f 6620 2873 7472 2c20 7374 7229 206f   of (str, str) o
-0000eee0: 7220 7374 720d 0a20 2020 2020 2020 2020  r str..         
-0000eef0: 2020 2050 756e 6374 7561 7469 6f6e 2873     Punctuation(s
-0000ef00: 2920 746f 2073 706c 6974 2073 6567 6d65  ) to split segme
-0000ef10: 6e74 7320 6279 2e0d 0a20 2020 2020 2020  nts by...       
-0000ef20: 206c 6f63 6b20 3a20 626f 6f6c 2c20 6465   lock : bool, de
-0000ef30: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-0000ef40: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000ef50: 2074 6f20 7072 6576 656e 7420 6675 7475   to prevent futu
-0000ef60: 7265 2073 706c 6974 732f 6d65 7267 6573  re splits/merges
-0000ef70: 2066 726f 6d20 616c 7465 7269 6e67 2063   from altering c
-0000ef80: 6861 6e67 6573 206d 6164 6520 6279 2074  hanges made by t
-0000ef90: 6869 7320 6d65 7468 6f64 2e0d 0a20 2020  his method...   
-0000efa0: 2020 2020 206e 6577 6c69 6e65 203a 2062       newline : b
-0000efb0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-0000efc0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000efd0: 5768 6574 6865 7220 746f 2069 6e73 6572  Whether to inser
-0000efe0: 7420 6c69 6e65 2062 7265 616b 2061 7420  t line break at 
-0000eff0: 7468 6520 7370 6c69 7420 706f 696e 7473  the split points
-0000f000: 2069 6e73 7465 6164 206f 6620 7370 6c69   instead of spli
-0000f010: 7474 696e 6720 696e 746f 2073 6570 6172  tting into separ
-0000f020: 6174 6520 7365 676d 656e 7473 2e0d 0a20  ate segments... 
-0000f030: 2020 2020 2020 206d 696e 5f77 6f72 6473         min_words
-0000f040: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-0000f050: 0d0a 2020 2020 2020 2020 2020 2020 5370  ..            Sp
-0000f060: 6c69 7420 7365 676d 656e 7473 2077 6974  lit segments wit
-0000f070: 6820 776f 7264 7320 3e3d 2060 606d 696e  h words >= ``min
-0000f080: 5f77 6f72 6473 6060 2e0d 0a20 2020 2020  _words``...     
-0000f090: 2020 206d 696e 5f63 6861 7273 203a 2069     min_chars : i
-0000f0a0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
-0000f0b0: 2020 2020 2020 2020 2020 5370 6c69 7420            Split 
-0000f0c0: 7365 676d 656e 7473 2077 6974 6820 6368  segments with ch
-0000f0d0: 6172 6163 7465 7273 203e 3d20 6060 6d69  aracters >= ``mi
-0000f0e0: 6e5f 6368 6172 7360 602e 0d0a 2020 2020  n_chars``...    
-0000f0f0: 2020 2020 6d69 6e5f 6475 7220 3a20 696e      min_dur : in
-0000f100: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-0000f110: 2020 2020 2020 2020 2073 706c 6974 2073           split s
-0000f120: 6567 6d65 6e74 7320 7769 7468 2064 7572  egments with dur
-0000f130: 6174 696f 6e20 2869 6e20 7365 636f 6e64  ation (in second
-0000f140: 7329 203e 3d20 6060 6d69 6e5f 6475 7260  s) >= ``min_dur`
-0000f150: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
-0000f160: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
-0000f170: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-0000f180: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
-0000f190: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
-0000f1a0: 756c 740d 0a20 2020 2020 2020 2020 2020  ult..           
-0000f1b0: 2054 6865 2063 7572 7265 6e74 2069 6e73   The current ins
-0000f1c0: 7461 6e63 6520 6166 7465 7220 7468 6520  tance after the 
-0000f1d0: 6368 616e 6765 732e 0d0a 2020 2020 2020  changes...      
-0000f1e0: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
-0000f1f0: 6566 205f 6f76 6572 5f6d 6178 2878 3a20  ef _over_max(x: 
-0000f200: 5365 676d 656e 7429 3a0d 0a20 2020 2020  Segment):..     
-0000f210: 2020 2020 2020 2072 6574 7572 6e20 280d         return (.
-0000f220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f230: 2020 2020 2028 6d69 6e5f 776f 7264 7320       (min_words 
-0000f240: 616e 6420 6c65 6e28 782e 776f 7264 7329  and len(x.words)
-0000f250: 203e 3d20 6d69 6e5f 776f 7264 7329 206f   >= min_words) o
-0000f260: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
-0000f270: 2020 2020 2020 2028 6d69 6e5f 6368 6172         (min_char
-0000f280: 7320 616e 6420 782e 6368 6172 5f63 6f75  s and x.char_cou
-0000f290: 6e74 2829 203e 3d20 6d69 6e5f 6368 6172  nt() >= min_char
-0000f2a0: 7329 206f 720d 0a20 2020 2020 2020 2020  s) or..         
-0000f2b0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
-0000f2c0: 6475 7220 616e 6420 782e 6475 7261 7469  dur and x.durati
-0000f2d0: 6f6e 203e 3d20 6d69 6e5f 6475 7229 0d0a  on >= min_dur)..
-0000f2e0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-0000f2f0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
-0000f300: 203d 2073 6574 2873 2e69 6420 666f 7220   = set(s.id for 
-0000f310: 7320 696e 2073 656c 662e 7365 676d 656e  s in self.segmen
-0000f320: 7473 2069 6620 5f6f 7665 725f 6d61 7828  ts if _over_max(
-0000f330: 7329 2920 6966 2061 6e79 2828 6d69 6e5f  s)) if any((min_
-0000f340: 776f 7264 732c 206d 696e 5f63 6861 7273  words, min_chars
-0000f350: 2c20 6d69 6e5f 6475 7229 2920 656c 7365  , min_dur)) else
-0000f360: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
-0000f370: 2064 6566 205f 6765 745f 696e 6469 6365   def _get_indice
-0000f380: 7328 783a 2053 6567 6d65 6e74 293a 0d0a  s(x: Segment):..
-0000f390: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f3a0: 726e 2078 2e67 6574 5f70 756e 6374 7561  rn x.get_punctua
-0000f3b0: 7469 6f6e 5f69 6e64 6963 6573 2870 756e  tion_indices(pun
-0000f3c0: 6374 7561 7469 6f6e 2920 6966 2069 6e64  ctuation) if ind
-0000f3d0: 6963 6573 2069 7320 4e6f 6e65 206f 7220  ices is None or 
-0000f3e0: 782e 6964 2069 6e20 696e 6469 6365 7320  x.id in indices 
-0000f3f0: 656c 7365 205b 5d0d 0a0d 0a20 2020 2020  else []....     
-0000f400: 2020 2073 656c 662e 5f73 706c 6974 5f73     self._split_s
-0000f410: 6567 6d65 6e74 7328 5f67 6574 5f69 6e64  egments(_get_ind
-0000f420: 6963 6573 2c20 6c6f 636b 3d6c 6f63 6b2c  ices, lock=lock,
-0000f430: 206e 6577 6c69 6e65 3d6e 6577 6c69 6e65   newline=newline
-0000f440: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-0000f450: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
-0000f460: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
-0000f470: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-0000f480: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
-0000f490: 2020 2020 2020 2020 7075 6e63 745f 7374          punct_st
-0000f4a0: 7220 3d20 272f 272e 6a6f 696e 2870 2069  r = '/'.join(p i
-0000f4b0: 6620 6973 696e 7374 616e 6365 2870 2c20  f isinstance(p, 
-0000f4c0: 7374 7229 2065 6c73 6520 272a 272e 6a6f  str) else '*'.jo
-0000f4d0: 696e 2870 2920 666f 7220 7020 696e 2070  in(p) for p in p
-0000f4e0: 756e 6374 7561 7469 6f6e 290d 0a20 2020  unctuation)..   
-0000f4f0: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-0000f500: 7570 5f68 6973 746f 7279 202b 3d20 6627  up_history += f'
-0000f510: 7370 3d7b 7075 6e63 745f 7374 727d 2b7b  sp={punct_str}+{
-0000f520: 696e 7428 6c6f 636b 297d 2b7b 696e 7428  int(lock)}+{int(
-0000f530: 6e65 776c 696e 6529 7d27 0d0a 2020 2020  newline)}'..    
-0000f540: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
-0000f550: 705f 6869 7374 6f72 7920 2b3d 2066 272b  p_history += f'+
-0000f560: 7b6d 696e 5f77 6f72 6473 206f 7220 2222  {min_words or ""
-0000f570: 7d2b 7b6d 696e 5f63 6861 7273 206f 7220  }+{min_chars or 
-0000f580: 2222 7d2b 7b6d 696e 5f64 7572 206f 7220  ""}+{min_dur or 
-0000f590: 2222 7d27 2e72 7374 7269 7028 272b 2729  ""}'.rstrip('+')
-0000f5a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000f5b0: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
-0000f5c0: 206d 6572 6765 5f62 795f 7075 6e63 7475   merge_by_punctu
-0000f5d0: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
-0000f5e0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-0000f5f0: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
-0000f600: 6f6e 3a20 556e 696f 6e5b 4c69 7374 5b73  on: Union[List[s
-0000f610: 7472 5d2c 204c 6973 745b 5475 706c 655b  tr], List[Tuple[
-0000f620: 7374 722c 2073 7472 5d5d 2c20 7374 725d  str, str]], str]
-0000f630: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000f640: 6178 5f77 6f72 6473 3a20 696e 7420 3d20  ax_words: int = 
-0000f650: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-0000f660: 2020 206d 6178 5f63 6861 7273 3a20 696e     max_chars: in
-0000f670: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
-0000f680: 2020 2020 2020 2069 735f 7375 6d5f 6d61         is_sum_ma
-0000f690: 783a 2062 6f6f 6c20 3d20 4661 6c73 652c  x: bool = False,
-0000f6a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-0000f6b0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-0000f6c0: 0d0a 2020 2020 2920 2d3e 2022 5768 6973  ..    ) -> "Whis
-0000f6d0: 7065 7252 6573 756c 7422 3a0d 0a20 2020  perResult":..   
-0000f6e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000f6f0: 2020 4d65 7267 6520 2869 6e2d 706c 6163    Merge (in-plac
-0000f700: 6529 2061 6e79 2074 776f 2073 6567 6d65  e) any two segme
-0000f710: 6e74 7320 7468 6174 2068 6173 2073 7065  nts that has spe
-0000f720: 6369 6669 6320 7075 6e63 7475 6174 696f  cific punctuatio
-0000f730: 6e73 2069 6e62 6574 7765 656e 2e0d 0a0d  ns inbetween....
-0000f740: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000f750: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-0000f760: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-0000f770: 2070 756e 6374 7561 7469 6f6e 203a 206c   punctuation : l
-0000f780: 6973 7420 6f66 2073 7472 206f 6620 6c69  ist of str of li
-0000f790: 7374 206f 6620 7475 706c 6520 6f66 2028  st of tuple of (
-0000f7a0: 7374 722c 2073 7472 2920 6f72 2073 7472  str, str) or str
-0000f7b0: 0d0a 2020 2020 2020 2020 2020 2020 5075  ..            Pu
-0000f7c0: 6e63 7475 6174 696f 6e28 7329 2074 6f20  nctuation(s) to 
-0000f7d0: 6d65 7267 6520 7365 676d 656e 7473 2062  merge segments b
-0000f7e0: 792e 0d0a 2020 2020 2020 2020 6d61 785f  y...        max_
-0000f7f0: 776f 7264 7320 3a20 696e 742c 206f 7074  words : int, opt
-0000f800: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-0000f810: 2020 204d 6178 696d 756d 206e 756d 6265     Maximum numbe
-0000f820: 7220 6f66 2077 6f72 6473 2061 6c6c 6f77  r of words allow
-0000f830: 6564 2069 6e20 6561 6368 2073 6567 6d65  ed in each segme
-0000f840: 6e74 2e0d 0a20 2020 2020 2020 206d 6178  nt...        max
-0000f850: 5f63 6861 7273 203a 2069 6e74 2c20 6f70  _chars : int, op
-0000f860: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-0000f870: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
-0000f880: 6572 206f 6620 6368 6172 6163 7465 7273  er of characters
-0000f890: 2061 6c6c 6f77 6564 2069 6e20 6561 6368   allowed in each
-0000f8a0: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
-0000f8b0: 2020 2069 735f 7375 6d5f 6d61 7820 3a20     is_sum_max : 
-0000f8c0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-0000f8d0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-0000f8e0: 2057 6865 7468 6572 2060 606d 6178 5f77   Whether ``max_w
-0000f8f0: 6f72 6473 6060 2061 6e64 2060 606d 6178  ords`` and ``max
-0000f900: 5f63 6861 7273 6060 2069 7320 6170 706c  _chars`` is appl
-0000f910: 6965 6420 746f 2074 6865 206d 6572 6765  ied to the merge
-0000f920: 6420 7365 676d 656e 7420 696e 7374 6561  d segment instea
-0000f930: 6420 6f66 2074 6865 2069 6e64 6976 6964  d of the individ
-0000f940: 7561 6c20 7365 676d 656e 7473 0d0a 2020  ual segments..  
-0000f950: 2020 2020 2020 2020 2020 746f 2062 6520            to be 
-0000f960: 6d65 7267 6564 2e0d 0a20 2020 2020 2020  merged...       
-0000f970: 206c 6f63 6b20 3a20 626f 6f6c 2c20 6465   lock : bool, de
-0000f980: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-0000f990: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000f9a0: 2074 6f20 7072 6576 656e 7420 6675 7475   to prevent futu
-0000f9b0: 7265 2073 706c 6974 732f 6d65 7267 6573  re splits/merges
-0000f9c0: 2066 726f 6d20 616c 7465 7269 6e67 2063   from altering c
-0000f9d0: 6861 6e67 6573 206d 6164 6520 6279 2074  hanges made by t
-0000f9e0: 6869 7320 6d65 7468 6f64 2e0d 0a0d 0a20  his method..... 
-0000f9f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-0000fa00: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-0000fa10: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-0000fa20: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-0000fa30: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-0000fa40: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-0000fa50: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-0000fa60: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-0000fa70: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-0000fa80: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-0000fa90: 3d20 7365 6c66 2e67 6574 5f70 756e 6374  = self.get_punct
-0000faa0: 7561 7469 6f6e 5f69 6e64 6963 6573 2870  uation_indices(p
-0000fab0: 756e 6374 7561 7469 6f6e 290d 0a20 2020  unctuation)..   
-0000fac0: 2020 2020 2073 656c 662e 5f6d 6572 6765       self._merge
-0000fad0: 5f73 6567 6d65 6e74 7328 696e 6469 6365  _segments(indice
-0000fae0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb00: 206d 6178 5f77 6f72 6473 3d6d 6178 5f77   max_words=max_w
-0000fb10: 6f72 6473 2c20 6d61 785f 6368 6172 733d  ords, max_chars=
-0000fb20: 6d61 785f 6368 6172 732c 2069 735f 7375  max_chars, is_su
-0000fb30: 6d5f 6d61 783d 6973 5f73 756d 5f6d 6178  m_max=is_sum_max
-0000fb40: 2c20 6c6f 636b 3d6c 6f63 6b29 0d0a 2020  , lock=lock)..  
-0000fb50: 2020 2020 2020 6966 2073 656c 662e 5f72        if self._r
-0000fb60: 6567 726f 7570 5f68 6973 746f 7279 3a0d  egroup_history:.
-0000fb70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fb80: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-0000fb90: 7279 202b 3d20 275f 270d 0a20 2020 2020  ry += '_'..     
-0000fba0: 2020 2070 756e 6374 5f73 7472 203d 2027     punct_str = '
-0000fbb0: 2f27 2e6a 6f69 6e28 7020 6966 2069 7369  /'.join(p if isi
-0000fbc0: 6e73 7461 6e63 6528 702c 2073 7472 2920  nstance(p, str) 
-0000fbd0: 656c 7365 2027 2a27 2e6a 6f69 6e28 7029  else '*'.join(p)
-0000fbe0: 2066 6f72 2070 2069 6e20 7075 6e63 7475   for p in punctu
-0000fbf0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
-0000fc00: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
-0000fc10: 7374 6f72 7920 2b3d 2066 276d 703d 7b70  story += f'mp={p
-0000fc20: 756e 6374 5f73 7472 7d2b 7b6d 6178 5f77  unct_str}+{max_w
-0000fc30: 6f72 6473 206f 7220 2222 7d2b 7b6d 6178  ords or ""}+{max
-0000fc40: 5f63 6861 7273 206f 7220 2222 7d2b 7b69  _chars or ""}+{i
-0000fc50: 6e74 2869 735f 7375 6d5f 6d61 7829 7d2b  nt(is_sum_max)}+
-0000fc60: 7b69 6e74 286c 6f63 6b29 7d27 0d0a 2020  {int(lock)}'..  
-0000fc70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000fc80: 660d 0a0d 0a20 2020 2064 6566 206d 6572  f....    def mer
-0000fc90: 6765 5f61 6c6c 5f73 6567 6d65 6e74 7328  ge_all_segments(
-0000fca0: 7365 6c66 2920 2d3e 2022 5768 6973 7065  self) -> "Whispe
-0000fcb0: 7252 6573 756c 7422 3a0d 0a20 2020 2020  rResult":..     
-0000fcc0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000fcd0: 4d65 7267 6520 616c 6c20 7365 676d 656e  Merge all segmen
-0000fce0: 7473 2069 6e74 6f20 6f6e 6520 7365 676d  ts into one segm
-0000fcf0: 656e 742e 0d0a 0d0a 2020 2020 2020 2020  ent.....        
-0000fd00: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-0000fd10: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-0000fd20: 2020 7374 6162 6c65 5f77 6869 7370 6572    stable_whisper
-0000fd30: 2e72 6573 756c 742e 5768 6973 7065 7252  .result.WhisperR
-0000fd40: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
-0000fd50: 2020 2054 6865 2063 7572 7265 6e74 2069     The current i
-0000fd60: 6e73 7461 6e63 6520 6166 7465 7220 7468  nstance after th
-0000fd70: 6520 6368 616e 6765 732e 0d0a 2020 2020  e changes...    
-0000fd80: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0000fd90: 2069 6620 6e6f 7420 7365 6c66 2e73 6567   if not self.seg
-0000fda0: 6d65 6e74 733a 0d0a 2020 2020 2020 2020  ments:..        
-0000fdb0: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
-0000fdc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000fdd0: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
-0000fde0: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
-0000fdf0: 203d 2073 656c 662e 7365 676d 656e 7473   = self.segments
-0000fe00: 5b30 5d2e 636f 7079 2873 656c 662e 616c  [0].copy(self.al
-0000fe10: 6c5f 776f 7264 7328 292c 206b 6565 705f  l_words(), keep_
-0000fe20: 7265 7375 6c74 3d54 7275 652c 2063 6f70  result=True, cop
-0000fe30: 795f 776f 7264 733d 4661 6c73 6529 0d0a  y_words=False)..
-0000fe40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000fe50: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
-0000fe60: 6567 203d 2073 656c 662e 7365 676d 656e  eg = self.segmen
-0000fe70: 7473 5b30 5d0d 0a20 2020 2020 2020 2020  ts[0]..         
-0000fe80: 2020 206e 6577 5f73 6567 2e5f 6465 6661     new_seg._defa
-0000fe90: 756c 745f 7465 7874 202b 3d20 2727 2e6a  ult_text += ''.j
-0000fea0: 6f69 6e28 732e 7465 7874 2066 6f72 2073  oin(s.text for s
-0000feb0: 2069 6e20 7365 6c66 2e73 6567 6d65 6e74   in self.segment
-0000fec0: 735b 313a 5d29 0d0a 2020 2020 2020 2020  s[1:])..        
-0000fed0: 2020 2020 6966 2061 6c6c 2873 2e74 6f6b      if all(s.tok
-0000fee0: 656e 7320 6973 206e 6f74 204e 6f6e 6520  ens is not None 
-0000fef0: 666f 7220 7320 696e 2073 656c 662e 7365  for s in self.se
-0000ff00: 676d 656e 7473 293a 0d0a 2020 2020 2020  gments):..      
-0000ff10: 2020 2020 2020 2020 2020 6e65 775f 7365            new_se
-0000ff20: 672e 5f64 6566 6175 6c74 5f74 6f6b 656e  g._default_token
-0000ff30: 7320 2b3d 206c 6973 7428 6368 6169 6e2e  s += list(chain.
-0000ff40: 6672 6f6d 5f69 7465 7261 626c 6528 732e  from_iterable(s.
-0000ff50: 746f 6b65 6e73 2066 6f72 2073 2069 6e20  tokens for s in 
-0000ff60: 7365 6c66 2e73 6567 6d65 6e74 735b 313a  self.segments[1:
-0000ff70: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-0000ff80: 206e 6577 5f73 6567 2e65 6e64 203d 2073   new_seg.end = s
-0000ff90: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
-0000ffa0: 2e65 6e64 0d0a 2020 2020 2020 2020 7365  .end..        se
-0000ffb0: 6c66 2e73 6567 6d65 6e74 7320 3d20 5b6e  lf.segments = [n
-0000ffc0: 6577 5f73 6567 5d0d 0a20 2020 2020 2020  ew_seg]..       
-0000ffd0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
-0000ffe0: 6473 2829 0d0a 2020 2020 2020 2020 6966  ds()..        if
-0000fff0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-00010000: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
-00010010: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-00010020: 7570 5f68 6973 746f 7279 202b 3d20 275f  up_history += '_
-00010030: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00010040: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-00010050: 202b 3d20 276d 7327 0d0a 2020 2020 2020   += 'ms'..      
-00010060: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
-00010070: 0a20 2020 2064 6566 2073 706c 6974 5f62  .    def split_b
-00010080: 795f 6c65 6e67 7468 280d 0a20 2020 2020  y_length(..     
-00010090: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-000100a0: 2020 2020 2020 2020 2020 6d61 785f 6368            max_ch
-000100b0: 6172 733a 2069 6e74 203d 204e 6f6e 652c  ars: int = None,
-000100c0: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-000100d0: 785f 776f 7264 733a 2069 6e74 203d 204e  x_words: int = N
-000100e0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-000100f0: 2020 6576 656e 5f73 706c 6974 3a20 626f    even_split: bo
-00010100: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
-00010110: 2020 2020 2020 2020 666f 7263 655f 6c65          force_le
-00010120: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
-00010130: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00010140: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-00010150: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-00010160: 6e63 6c75 6465 5f6c 6f63 6b3a 2062 6f6f  nclude_lock: boo
-00010170: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00010180: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
-00010190: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
-000101a0: 2020 2029 202d 3e20 2257 6869 7370 6572     ) -> "Whisper
-000101b0: 5265 7375 6c74 223a 0d0a 2020 2020 2020  Result":..      
-000101c0: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
-000101d0: 706c 6974 2028 696e 2d70 6c61 6365 2920  plit (in-place) 
-000101e0: 616e 7920 7365 676d 656e 7420 7468 6174  any segment that
-000101f0: 2065 7863 6565 6473 2060 606d 6178 5f63   exceeds ``max_c
-00010200: 6861 7273 6060 206f 7220 6060 6d61 785f  hars`` or ``max_
-00010210: 776f 7264 7360 6020 696e 746f 2073 6d61  words`` into sma
-00010220: 6c6c 6572 2073 6567 6d65 6e74 732e 0d0a  ller segments...
-00010230: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00010240: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00010250: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00010260: 2020 6d61 785f 6368 6172 7320 3a20 696e    max_chars : in
-00010270: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00010280: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
-00010290: 206e 756d 6265 7220 6f66 2063 6861 7261   number of chara
-000102a0: 6374 6572 7320 616c 6c6f 7765 6420 696e  cters allowed in
-000102b0: 2065 6163 6820 7365 676d 656e 742e 0d0a   each segment...
-000102c0: 2020 2020 2020 2020 6d61 785f 776f 7264          max_word
-000102d0: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
-000102e0: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
-000102f0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-00010300: 2077 6f72 6473 2061 6c6c 6f77 6564 2069   words allowed i
-00010310: 6e20 6561 6368 2073 6567 6d65 6e74 2e0d  n each segment..
-00010320: 0a20 2020 2020 2020 2065 7665 6e5f 7370  .        even_sp
-00010330: 6c69 7420 3a20 626f 6f6c 2c20 6465 6661  lit : bool, defa
-00010340: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-00010350: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00010360: 2065 7665 6e6c 7920 7370 6c69 7420 6120   evenly split a 
-00010370: 7365 676d 656e 7420 696e 206c 656e 6774  segment in lengt
-00010380: 6820 6966 2069 7420 6578 6365 6564 7320  h if it exceeds 
-00010390: 6060 6d61 785f 6368 6172 7360 6020 6f72  ``max_chars`` or
-000103a0: 2060 606d 6178 5f77 6f72 6473 6060 2e0d   ``max_words``..
-000103b0: 0a20 2020 2020 2020 2066 6f72 6365 5f6c  .        force_l
-000103c0: 656e 203a 2062 6f6f 6c2c 2064 6566 6175  en : bool, defau
-000103d0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-000103e0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-000103f0: 2066 6f72 6365 2061 2063 6f6e 7374 616e   force a constan
-00010400: 7420 6c65 6e67 7468 2066 6f72 2065 6163  t length for eac
-00010410: 6820 7365 676d 656e 7420 6578 6365 7074  h segment except
-00010420: 2074 6865 206c 6173 7420 7365 676d 656e   the last segmen
-00010430: 742e 0d0a 2020 2020 2020 2020 2020 2020  t...            
-00010440: 5468 6973 2077 696c 6c20 6967 6e6f 7265  This will ignore
-00010450: 2061 6c6c 2070 7265 7669 6f75 7320 6e6f   all previous no
-00010460: 6e2d 6c6f 636b 6564 2073 6567 6d65 6e74  n-locked segment
-00010470: 2062 6f75 6e64 6172 6965 732e 0d0a 2020   boundaries...  
-00010480: 2020 2020 2020 6c6f 636b 203a 2062 6f6f        lock : boo
-00010490: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-000104a0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-000104b0: 6574 6865 7220 746f 2070 7265 7665 6e74  ether to prevent
-000104c0: 2066 7574 7572 6520 7370 6c69 7473 2f6d   future splits/m
-000104d0: 6572 6765 7320 6672 6f6d 2061 6c74 6572  erges from alter
-000104e0: 696e 6720 6368 616e 6765 7320 6d61 6465  ing changes made
-000104f0: 2062 7920 7468 6973 206d 6574 686f 642e   by this method.
-00010500: 0d0a 2020 2020 2020 2020 696e 636c 7564  ..        includ
-00010510: 655f 6c6f 636b 3a20 626f 6f6c 2c20 6465  e_lock: bool, de
-00010520: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
-00010530: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-00010540: 2074 6f20 696e 636c 7564 6520 7072 6576   to include prev
-00010550: 696f 7573 206c 6f63 6b20 6265 666f 7265  ious lock before
-00010560: 2073 706c 6974 7469 6e67 2062 6173 6564   splitting based
-00010570: 206f 6e20 6d61 785f 776f 7264 732c 2069   on max_words, i
-00010580: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
-00010590: 2046 616c 7365 6060 2e0d 0a20 2020 2020   False``...     
-000105a0: 2020 2020 2020 2053 706c 6974 7469 6e67         Splitting
-000105b0: 2077 696c 6c20 6265 2064 6f6e 6520 6166   will be done af
-000105c0: 7465 7220 7468 6520 6669 7273 7420 6e6f  ter the first no
-000105d0: 6e2d 6c6f 636b 6564 2077 6f72 6420 3e20  n-locked word > 
-000105e0: 6060 6d61 785f 6368 6172 7360 6020 2f20  ``max_chars`` / 
-000105f0: 6060 6d61 785f 776f 7264 7360 602e 0d0a  ``max_words``...
-00010600: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
-00010610: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00010620: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-00010630: 2020 5768 6574 6865 7220 746f 2069 6e73    Whether to ins
-00010640: 6572 7420 6c69 6e65 2062 7265 616b 2061  ert line break a
-00010650: 7420 7468 6520 7370 6c69 7420 706f 696e  t the split poin
-00010660: 7473 2069 6e73 7465 6164 206f 6620 7370  ts instead of sp
-00010670: 6c69 7474 696e 6720 696e 746f 2073 6570  litting into sep
-00010680: 6172 6174 6520 7365 676d 656e 7473 2e0d  arate segments..
-00010690: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000106a0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-000106b0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
-000106c0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
-000106d0: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
-000106e0: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-000106f0: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
-00010700: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
-00010710: 6e67 6573 2e0d 0a0d 0a20 2020 2020 2020  nges.....       
-00010720: 204e 6f74 6573 0d0a 2020 2020 2020 2020   Notes..        
-00010730: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
-00010740: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
-00010750: 2054 7275 6560 602c 2073 6567 6d65 6e74   True``, segment
-00010760: 7320 6361 6e20 7374 696c 6c20 6578 6365  s can still exce
-00010770: 6564 2060 606d 6178 5f63 6861 7273 6060  ed ``max_chars``
-00010780: 2061 6e64 206c 6f63 6b65 6420 776f 7264   and locked word
-00010790: 7320 7769 6c6c 2062 6520 6967 6e6f 7265  s will be ignore
-000107a0: 6420 746f 2061 766f 6964 0d0a 2020 2020  d to avoid..    
-000107b0: 2020 2020 756e 6576 656e 2073 706c 6974      uneven split
-000107c0: 7469 6e67 2e0d 0a20 2020 2020 2020 2022  ting...        "
-000107d0: 2222 0d0a 2020 2020 2020 2020 6966 2066  ""..        if f
-000107e0: 6f72 6365 5f6c 656e 3a0d 0a20 2020 2020  orce_len:..     
-000107f0: 2020 2020 2020 2073 656c 662e 6d65 7267         self.merg
-00010800: 655f 616c 6c5f 7365 676d 656e 7473 2829  e_all_segments()
-00010810: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00010820: 7370 6c69 745f 7365 676d 656e 7473 280d  split_segments(.
-00010830: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-00010840: 6264 6120 783a 2078 2e67 6574 5f6c 656e  bda x: x.get_len
-00010850: 6774 685f 696e 6469 6365 7328 0d0a 2020  gth_indices(..  
-00010860: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00010870: 785f 6368 6172 733d 6d61 785f 6368 6172  x_chars=max_char
-00010880: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00010890: 2020 2020 6d61 785f 776f 7264 733d 6d61      max_words=ma
-000108a0: 785f 776f 7264 732c 0d0a 2020 2020 2020  x_words,..      
-000108b0: 2020 2020 2020 2020 2020 6576 656e 5f73            even_s
-000108c0: 706c 6974 3d65 7665 6e5f 7370 6c69 742c  plit=even_split,
-000108d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000108e0: 2020 696e 636c 7564 655f 6c6f 636b 3d69    include_lock=i
-000108f0: 6e63 6c75 6465 5f6c 6f63 6b0d 0a20 2020  nclude_lock..   
-00010900: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
-00010910: 2020 2020 2020 2020 206c 6f63 6b3d 6c6f           lock=lo
-00010920: 636b 2c0d 0a20 2020 2020 2020 2020 2020  ck,..           
-00010930: 206e 6577 6c69 6e65 3d6e 6577 6c69 6e65   newline=newline
-00010940: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-00010950: 2020 2020 2069 6620 7365 6c66 2e5f 7265       if self._re
-00010960: 6772 6f75 705f 6869 7374 6f72 793a 0d0a  group_history:..
-00010970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010980: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
-00010990: 7920 2b3d 2027 5f27 0d0a 2020 2020 2020  y += '_'..      
-000109a0: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-000109b0: 6869 7374 6f72 7920 2b3d 2028 6627 736c  history += (f'sl
-000109c0: 3d7b 6d61 785f 6368 6172 7320 6f72 2022  ={max_chars or "
-000109d0: 227d 2b7b 6d61 785f 776f 7264 7320 6f72  "}+{max_words or
-000109e0: 2022 227d 2b7b 696e 7428 6576 656e 5f73   ""}+{int(even_s
-000109f0: 706c 6974 297d 2b7b 696e 7428 666f 7263  plit)}+{int(forc
-00010a00: 655f 6c65 6e29 7d27 0d0a 2020 2020 2020  e_len)}'..      
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2020 2020 2020 2020 6627 2b7b              f'+{
-00010a30: 696e 7428 6c6f 636b 297d 2b7b 696e 7428  int(lock)}+{int(
-00010a40: 696e 636c 7564 655f 6c6f 636b 297d 2b7b  include_lock)}+{
-00010a50: 696e 7428 6e65 776c 696e 6529 7d27 290d  int(newline)}').
-00010a60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010a70: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00010a80: 7370 6c69 745f 6279 5f64 7572 6174 696f  split_by_duratio
-00010a90: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
-00010aa0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00010ab0: 2020 206d 6178 5f64 7572 3a20 666c 6f61     max_dur: floa
-00010ac0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-00010ad0: 6576 656e 5f73 706c 6974 3a20 626f 6f6c  even_split: bool
-00010ae0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-00010af0: 2020 2020 2020 666f 7263 655f 6c65 6e3a        force_len:
-00010b00: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00010b10: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
-00010b20: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
-00010b30: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
-00010b40: 6c75 6465 5f6c 6f63 6b3a 2062 6f6f 6c20  lude_lock: bool 
-00010b50: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-00010b60: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
-00010b70: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
-00010b80: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
-00010b90: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
-00010ba0: 2222 220d 0a20 2020 2020 2020 2053 706c  """..        Spl
-00010bb0: 6974 2028 696e 2d70 6c61 6365 2920 616e  it (in-place) an
-00010bc0: 7920 7365 676d 656e 7420 7468 6174 2065  y segment that e
-00010bd0: 7863 6565 6473 2060 606d 6178 5f64 7572  xceeds ``max_dur
-00010be0: 6060 2069 6e74 6f20 736d 616c 6c65 7220  `` into smaller 
-00010bf0: 7365 676d 656e 7473 2e0d 0a0d 0a20 2020  segments.....   
-00010c00: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-00010c10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00010c20: 2d2d 2d0d 0a20 2020 2020 2020 206d 6178  ---..        max
-00010c30: 5f64 7572 203a 2066 6c6f 6174 0d0a 2020  _dur : float..  
-00010c40: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
-00010c50: 6d20 6475 7261 7469 6f6e 2028 696e 2073  m duration (in s
-00010c60: 6563 6f6e 6473 2920 7065 7220 7365 676d  econds) per segm
-00010c70: 656e 742e 0d0a 2020 2020 2020 2020 6576  ent...        ev
-00010c80: 656e 5f73 706c 6974 203a 2062 6f6f 6c2c  en_split : bool,
-00010c90: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
-00010ca0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-00010cb0: 6572 2074 6f20 6576 656e 6c79 2073 706c  er to evenly spl
-00010cc0: 6974 2061 2073 6567 6d65 6e74 2069 6e20  it a segment in 
-00010cd0: 6c65 6e67 7468 2069 6620 6974 2065 7863  length if it exc
-00010ce0: 6565 6473 2060 606d 6178 5f64 7572 6060  eeds ``max_dur``
-00010cf0: 2e0d 0a20 2020 2020 2020 2066 6f72 6365  ...        force
-00010d00: 5f6c 656e 203a 2062 6f6f 6c2c 2064 6566  _len : bool, def
-00010d10: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-00010d20: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00010d30: 746f 2066 6f72 6365 2061 2063 6f6e 7374  to force a const
-00010d40: 616e 7420 6c65 6e67 7468 2066 6f72 2065  ant length for e
-00010d50: 6163 6820 7365 676d 656e 7420 6578 6365  ach segment exce
-00010d60: 7074 2074 6865 206c 6173 7420 7365 676d  pt the last segm
-00010d70: 656e 742e 0d0a 2020 2020 2020 2020 2020  ent...          
-00010d80: 2020 5468 6973 2077 696c 6c20 6967 6e6f    This will igno
-00010d90: 7265 2061 6c6c 2070 7265 7669 6f75 7320  re all previous 
-00010da0: 6e6f 6e2d 6c6f 636b 6564 2073 6567 6d65  non-locked segme
-00010db0: 6e74 2062 6f75 6e64 6172 6965 732e 0d0a  nt boundaries...
-00010dc0: 2020 2020 2020 2020 6c6f 636b 203a 2062          lock : b
-00010dd0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
-00010de0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00010df0: 5768 6574 6865 7220 746f 2070 7265 7665  Whether to preve
-00010e00: 6e74 2066 7574 7572 6520 7370 6c69 7473  nt future splits
-00010e10: 2f6d 6572 6765 7320 6672 6f6d 2061 6c74  /merges from alt
-00010e20: 6572 696e 6720 6368 616e 6765 7320 6d61  ering changes ma
-00010e30: 6465 2062 7920 7468 6973 206d 6574 686f  de by this metho
-00010e40: 642e 0d0a 2020 2020 2020 2020 696e 636c  d...        incl
-00010e50: 7564 655f 6c6f 636b 3a20 626f 6f6c 2c20  ude_lock: bool, 
-00010e60: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
-00010e70: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-00010e80: 6572 2074 6f20 696e 636c 7564 6520 7072  er to include pr
-00010e90: 6576 696f 7573 206c 6f63 6b20 6265 666f  evious lock befo
-00010ea0: 7265 2073 706c 6974 7469 6e67 2062 6173  re splitting bas
-00010eb0: 6564 206f 6e20 6d61 785f 776f 7264 732c  ed on max_words,
-00010ec0: 2069 6620 6060 6576 656e 5f73 706c 6974   if ``even_split
-00010ed0: 203d 2046 616c 7365 6060 2e0d 0a20 2020   = False``...   
-00010ee0: 2020 2020 2020 2020 2053 706c 6974 7469           Splitti
-00010ef0: 6e67 2077 696c 6c20 6265 2064 6f6e 6520  ng will be done 
-00010f00: 6166 7465 7220 7468 6520 6669 7273 7420  after the first 
-00010f10: 6e6f 6e2d 6c6f 636b 6564 2077 6f72 6420  non-locked word 
-00010f20: 3e20 6060 6d61 785f 6475 7260 602e 0d0a  > ``max_dur``...
-00010f30: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
-00010f40: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00010f50: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-00010f60: 2020 5768 6574 6865 7220 746f 2069 6e73    Whether to ins
-00010f70: 6572 7420 6c69 6e65 2062 7265 616b 2061  ert line break a
-00010f80: 7420 7468 6520 7370 6c69 7420 706f 696e  t the split poin
-00010f90: 7473 2069 6e73 7465 6164 206f 6620 7370  ts instead of sp
-00010fa0: 6c69 7474 696e 6720 696e 746f 2073 6570  litting into sep
-00010fb0: 6172 6174 6520 7365 676d 656e 7473 2e0d  arate segments..
-00010fc0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00010fd0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00010fe0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
-00010ff0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
-00011000: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
-00011010: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00011020: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
-00011030: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
-00011040: 6e67 6573 2e0d 0a0d 0a20 2020 2020 2020  nges.....       
-00011050: 204e 6f74 6573 0d0a 2020 2020 2020 2020   Notes..        
-00011060: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
-00011070: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
-00011080: 2054 7275 6560 602c 2073 6567 6d65 6e74   True``, segment
-00011090: 7320 6361 6e20 7374 696c 6c20 6578 6365  s can still exce
-000110a0: 6564 2060 606d 6178 5f64 7572 6060 2061  ed ``max_dur`` a
-000110b0: 6e64 206c 6f63 6b65 6420 776f 7264 7320  nd locked words 
-000110c0: 7769 6c6c 2062 6520 6967 6e6f 7265 6420  will be ignored 
-000110d0: 746f 2061 766f 6964 0d0a 2020 2020 2020  to avoid..      
-000110e0: 2020 756e 6576 656e 2073 706c 6974 7469    uneven splitti
-000110f0: 6e67 2e0d 0a20 2020 2020 2020 2022 2222  ng...        """
-00011100: 0d0a 2020 2020 2020 2020 6966 2066 6f72  ..        if for
-00011110: 6365 5f6c 656e 3a0d 0a20 2020 2020 2020  ce_len:..       
-00011120: 2020 2020 2073 656c 662e 6d65 7267 655f       self.merge_
-00011130: 616c 6c5f 7365 676d 656e 7473 2829 0d0a  all_segments()..
-00011140: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
-00011150: 6c69 745f 7365 676d 656e 7473 280d 0a20  lit_segments(.. 
-00011160: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
-00011170: 6120 783a 2078 2e67 6574 5f64 7572 6174  a x: x.get_durat
-00011180: 696f 6e5f 696e 6469 6365 7328 0d0a 2020  ion_indices(..  
-00011190: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000111a0: 785f 6475 723d 6d61 785f 6475 722c 0d0a  x_dur=max_dur,..
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 6576 656e 5f73 706c 6974 3d65 7665 6e5f  even_split=even_
-000111d0: 7370 6c69 742c 0d0a 2020 2020 2020 2020  split,..        
-000111e0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-000111f0: 6c6f 636b 3d69 6e63 6c75 6465 5f6c 6f63  lock=include_loc
-00011200: 6b0d 0a20 2020 2020 2020 2020 2020 2029  k..            )
-00011210: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-00011220: 6f63 6b3d 6c6f 636b 2c0d 0a20 2020 2020  ock=lock,..     
-00011230: 2020 2020 2020 206e 6577 6c69 6e65 3d6e         newline=n
-00011240: 6577 6c69 6e65 0d0a 2020 2020 2020 2020  ewline..        
-00011250: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00011260: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
-00011270: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
-00011280: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-00011290: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
-000112a0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-000112b0: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-000112c0: 2028 6627 7364 3d7b 6d61 785f 6475 727d   (f'sd={max_dur}
-000112d0: 2b7b 696e 7428 6576 656e 5f73 706c 6974  +{int(even_split
-000112e0: 297d 2b7b 696e 7428 666f 7263 655f 6c65  )}+{int(force_le
-000112f0: 6e29 7d27 0d0a 2020 2020 2020 2020 2020  n)}'..          
-00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011310: 2020 2020 2020 2020 6627 2b7b 696e 7428          f'+{int(
-00011320: 6c6f 636b 297d 2b7b 696e 7428 696e 636c  lock)}+{int(incl
-00011330: 7564 655f 6c6f 636b 297d 2b7b 696e 7428  ude_lock)}+{int(
-00011340: 6e65 776c 696e 6529 7d27 290d 0a20 2020  newline)}')..   
-00011350: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00011360: 0d0a 0d0a 2020 2020 6465 6620 636c 616d  ....    def clam
-00011370: 705f 6d61 7828 0d0a 2020 2020 2020 2020  p_max(..        
-00011380: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-00011390: 2020 2020 2020 206d 6564 6975 6d5f 6661         medium_fa
-000113a0: 6374 6f72 3a20 666c 6f61 7420 3d20 322e  ctor: float = 2.
-000113b0: 352c 0d0a 2020 2020 2020 2020 2020 2020  5,..            
-000113c0: 6d61 785f 6475 723a 2066 6c6f 6174 203d  max_dur: float =
-000113d0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-000113e0: 2020 2020 636c 6970 5f73 7461 7274 3a20      clip_start: 
-000113f0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00011400: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00011410: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00011420: 6c20 3d20 4661 6c73 650d 0a20 2020 2029  l = False..    )
-00011430: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
-00011440: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
-00011450: 220d 0a20 2020 2020 2020 2043 6c61 6d70  "..        Clamp
-00011460: 2061 6c6c 2077 6f72 6420 6475 7261 7469   all word durati
-00011470: 6f6e 7320 6162 6f76 6520 6365 7274 6169  ons above certai
-00011480: 6e20 7661 6c75 652e 0d0a 0d0a 2020 2020  n value.....    
-00011490: 2020 2020 5468 6973 2069 7320 6d6f 7374      This is most
-000114a0: 2065 6666 6563 7469 7665 2077 6865 6e20   effective when 
-000114b0: 6170 706c 6965 6420 6265 666f 7265 2061  applied before a
-000114c0: 6e64 2061 6674 6572 206f 7468 6572 2072  nd after other r
-000114d0: 6567 726f 7570 206f 7065 7261 7469 6f6e  egroup operation
-000114e0: 732e 0d0a 0d0a 2020 2020 2020 2020 5061  s.....        Pa
-000114f0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00011500: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-00011510: 2020 2020 2020 6d65 6469 756d 5f66 6163        medium_fac
-00011520: 746f 7220 3a20 666c 6f61 742c 2064 6566  tor : float, def
-00011530: 6175 6c74 2032 2e35 0d0a 2020 2020 2020  ault 2.5..      
-00011540: 2020 2020 2020 436c 616d 7020 6475 7261        Clamp dura
-00011550: 7469 6f6e 7320 6162 6f76 6520 2860 606d  tions above (``m
-00011560: 6564 6975 6d5f 6661 6374 6f72 6060 202a  edium_factor`` *
-00011570: 206d 6564 6975 6d20 6475 7261 7469 6f6e   medium duration
-00011580: 2920 7065 7220 7365 676d 656e 742e 0d0a  ) per segment...
-00011590: 2020 2020 2020 2020 2020 2020 4966 2060              If `
-000115a0: 606d 6564 6975 6d5f 6661 6374 6f72 203d  `medium_factor =
-000115b0: 204e 6f6e 652f 3060 6020 6f72 2073 6567   None/0`` or seg
-000115c0: 6d65 6e74 2068 6173 206c 6573 7320 7468  ment has less th
-000115d0: 616e 2033 2077 6f72 6473 2c20 6974 2077  an 3 words, it w
-000115e0: 696c 6c20 6265 2069 676e 6f72 6564 2061  ill be ignored a
-000115f0: 6e64 2075 7365 206f 6e6c 7920 6060 6d61  nd use only ``ma
-00011600: 785f 6475 7260 602e 0d0a 2020 2020 2020  x_dur``...      
-00011610: 2020 6d61 785f 6475 7220 3a20 666c 6f61    max_dur : floa
-00011620: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00011630: 2020 2020 2020 2020 2043 6c61 6d70 2064           Clamp d
-00011640: 7572 6174 696f 6e73 2061 626f 7665 2060  urations above `
-00011650: 606d 6178 5f64 7572 6060 2e0d 0a20 2020  `max_dur``...   
-00011660: 2020 2020 2063 6c69 705f 7374 6172 7420       clip_start 
-00011670: 3a20 626f 6f6c 206f 7220 4e6f 6e65 2c20  : bool or None, 
-00011680: 6465 6661 756c 7420 4e6f 6e65 0d0a 2020  default None..  
-00011690: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-000116a0: 7220 746f 2063 6c61 6d70 2074 6865 2073  r to clamp the s
-000116b0: 7461 7274 206f 6620 6120 776f 7264 2e20  tart of a word. 
-000116c0: 4966 2060 604e 6f6e 6560 602c 2063 6c61  If ``None``, cla
-000116d0: 6d70 2074 6865 2073 7461 7274 206f 6620  mp the start of 
-000116e0: 6669 7273 7420 776f 7264 2061 6e64 2065  first word and e
-000116f0: 6e64 206f 6620 6c61 7374 2077 6f72 6420  nd of last word 
-00011700: 7065 720d 0a20 2020 2020 2020 2020 2020  per..           
-00011710: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
-00011720: 2020 2076 6572 626f 7365 203a 2062 6f6f     verbose : boo
-00011730: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00011740: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00011750: 6574 6865 7220 746f 2070 7269 6e74 206f  ether to print o
-00011760: 7574 2074 6865 2074 696d 6573 7461 6d70  ut the timestamp
-00011770: 2063 6861 6e67 6573 2e0d 0a0d 0a20 2020   changes.....   
-00011780: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-00011790: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-000117a0: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
-000117b0: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
-000117c0: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
-000117d0: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
-000117e0: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
-000117f0: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
-00011800: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00011810: 2020 2020 2020 6966 206e 6f74 2028 6d65        if not (me
-00011820: 6469 756d 5f66 6163 746f 7220 6f72 206d  dium_factor or m
-00011830: 6178 5f64 7572 293a 0d0a 2020 2020 2020  ax_dur):..      
-00011840: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00011850: 6545 7272 6f72 2827 4174 206c 6561 7374  eError('At least
-00011860: 206f 6e65 206f 6620 666f 6c6c 6f77 696e   one of followin
-00011870: 6720 6172 6775 6d65 6e74 7320 7265 7175  g arguments requ
-00011880: 6972 6573 206e 6f6e 2d7a 6572 6f20 7661  ires non-zero va
-00011890: 6c75 653a 206d 6564 6975 6d5f 6661 6374  lue: medium_fact
-000118a0: 6f72 3b20 6d61 785f 6475 7227 290d 0a0d  or; max_dur')...
-000118b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000118c0: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
-000118d0: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
-000118e0: 6e69 6e67 732e 7761 726e 2827 4361 6e6e  nings.warn('Cann
-000118f0: 6f74 2063 6c61 6d70 2064 7565 2074 6f20  ot clamp due to 
-00011900: 6d69 7373 696e 672f 6e6f 2077 6f72 642d  missing/no word-
-00011910: 7469 6d65 7374 616d 7073 2729 0d0a 2020  timestamps')..  
-00011920: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011930: 2073 656c 660d 0a0d 0a20 2020 2020 2020   self....       
-00011940: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
-00011950: 2e73 6567 6d65 6e74 733a 0d0a 2020 2020  .segments:..    
-00011960: 2020 2020 2020 2020 6375 7272 5f6d 6178          curr_max
-00011970: 5f64 7572 203d 204e 6f6e 650d 0a20 2020  _dur = None..   
-00011980: 2020 2020 2020 2020 2069 6620 6d65 6469           if medi
-00011990: 756d 5f66 6163 746f 7220 616e 6420 6c65  um_factor and le
-000119a0: 6e28 7365 672e 776f 7264 7329 203e 2032  n(seg.words) > 2
-000119b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000119c0: 2020 2064 7572 6174 696f 6e73 203d 206e     durations = n
-000119d0: 702e 6172 7261 7928 5b77 6f72 642e 6475  p.array([word.du
-000119e0: 7261 7469 6f6e 2066 6f72 2077 6f72 6420  ration for word 
-000119f0: 696e 2073 6567 2e77 6f72 6473 5d29 0d0a  in seg.words])..
-00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a10: 6475 7261 7469 6f6e 732e 736f 7274 2829  durations.sort()
+0000d660: 732e 6c6f 636b 5f6c 6566 7428 290d 0a20  s.lock_left().. 
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6a0: 2020 2020 2020 2020 2020 732e 6c6f 636b            s.lock
+0000d6b0: 5f62 6f74 6828 290d 0a20 2020 2020 2020  _both()..       
+0000d6c0: 2020 2020 2020 2020 2064 656c 2073 656c           del sel
+0000d6d0: 662e 7365 676d 656e 7473 5b69 5d0d 0a20  f.segments[i].. 
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d6f0: 6f72 2073 2069 6e20 7265 7665 7273 6564  or s in reversed
+0000d700: 286e 6577 5f73 6567 6d65 6e74 7329 3a0d  (new_segments):.
+0000d710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d720: 2020 2020 2073 656c 662e 7365 676d 656e       self.segmen
+0000d730: 7473 2e69 6e73 6572 7428 692c 2073 290d  ts.insert(i, s).
+0000d740: 0a20 2020 2020 2020 2069 6620 6e6f 5f77  .        if no_w
+0000d750: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
+0000d760: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
+0000d770: 2827 466f 756e 6420 7365 676d 656e 7428  ('Found segment(
+0000d780: 7329 2077 6974 686f 7574 2077 6f72 6420  s) without word 
+0000d790: 7469 6d69 6e67 732e 2054 6865 7365 2073  timings. These s
+0000d7a0: 6567 6d65 6e74 2873 2920 6361 6e6e 6f74  egment(s) cannot
+0000d7b0: 2062 6520 7370 6c69 742e 2729 0d0a 2020   be split.')..  
+0000d7c0: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
+0000d7d0: 655f 6e6f 5f77 6f72 645f 7365 676d 656e  e_no_word_segmen
+0000d7e0: 7473 2829 0d0a 0d0a 2020 2020 6465 6620  ts()....    def 
+0000d7f0: 5f6d 6572 6765 5f73 6567 6d65 6e74 7328  _merge_segments(
+0000d800: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d810: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+0000d820: 2069 6e64 6963 6573 3a20 4c69 7374 5b69   indices: List[i
+0000d830: 6e74 5d2c 0d0a 2020 2020 2020 2020 2020  nt],..          
+0000d840: 2020 2a2c 0d0a 2020 2020 2020 2020 2020    *,..          
+0000d850: 2020 6d61 785f 776f 7264 733a 2069 6e74    max_words: int
+0000d860: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0000d870: 2020 2020 2020 6d61 785f 6368 6172 733a        max_chars:
+0000d880: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
+0000d890: 2020 2020 2020 2020 2020 6973 5f73 756d            is_sum
+0000d8a0: 5f6d 6178 3a20 626f 6f6c 203d 2046 616c  _max: bool = Fal
+0000d8b0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+0000d8c0: 206c 6f63 6b3a 2062 6f6f 6c20 3d20 4661   lock: bool = Fa
+0000d8d0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+0000d8e0: 2020 6e65 776c 696e 653a 2062 6f6f 6c20    newline: bool 
+0000d8f0: 3d20 4661 6c73 650d 0a20 2020 2029 3a0d  = False..    ):.
+0000d900: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0000d910: 696e 6469 6365 7329 203d 3d20 303a 0d0a  indices) == 0:..
+0000d920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d930: 726e 0d0a 2020 2020 2020 2020 666f 7220  rn..        for 
+0000d940: 6920 696e 2072 6576 6572 7365 6428 696e  i in reversed(in
+0000d950: 6469 6365 7329 3a0d 0a20 2020 2020 2020  dices):..       
+0000d960: 2020 2020 2073 6567 203d 2073 656c 662e       seg = self.
+0000d970: 7365 676d 656e 7473 5b69 5d0d 0a20 2020  segments[i]..   
+0000d980: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
+0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9a0: 2020 2028 0d0a 2020 2020 2020 2020 2020     (..          
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9c0: 2020 6d61 785f 776f 7264 7320 616e 640d    max_words and.
+0000d9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d9e0: 2020 2020 2020 2020 2020 2020 2073 6567               seg
+0000d9f0: 2e68 6173 5f77 6f72 6473 2061 6e64 0d0a  .has_words and..
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 2020 2020 2020 2020 2020 2020 280d 0a20              (.. 
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da40: 2020 2028 7365 672e 776f 7264 5f63 6f75     (seg.word_cou
+0000da50: 6e74 2829 202b 2073 656c 662e 7365 676d  nt() + self.segm
+0000da60: 656e 7473 5b69 202b 2031 5d2e 776f 7264  ents[i + 1].word
+0000da70: 5f63 6f75 6e74 2829 203e 206d 6178 5f77  _count() > max_w
+0000da80: 6f72 6473 290d 0a20 2020 2020 2020 2020  ords)..         
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000dab0: 5f73 756d 5f6d 6178 2065 6c73 650d 0a20  _sum_max else.. 
+0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 2020 2028 7365 672e 776f 7264 5f63 6f75     (seg.word_cou
+0000daf0: 6e74 2829 203e 206d 6178 5f77 6f72 6473  nt() > max_words
+0000db00: 2061 6e64 2073 656c 662e 7365 676d 656e   and self.segmen
+0000db10: 7473 5b69 202b 2031 5d2e 776f 7264 5f63  ts[i + 1].word_c
+0000db20: 6f75 6e74 2829 203e 206d 6178 5f77 6f72  ount() > max_wor
+0000db30: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000db60: 2020 2020 2020 2020 2920 6f72 0d0a 2020          ) or..  
+0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 206d 6178 5f63 6861 7273 2061 6e64 0d0a   max_chars and..
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 2020 2020 2020 2020 2020 2020 280d 0a20              (.. 
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2020 2028 7365 672e 6368 6172 5f63 6f75     (seg.char_cou
+0000dc00: 6e74 2829 202b 2073 656c 662e 7365 676d  nt() + self.segm
+0000dc10: 656e 7473 5b69 202b 2031 5d2e 6368 6172  ents[i + 1].char
+0000dc20: 5f63 6f75 6e74 2829 203e 206d 6178 5f63  _count() > max_c
+0000dc30: 6861 7273 290d 0a20 2020 2020 2020 2020  hars)..         
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000dc60: 5f73 756d 5f6d 6178 2065 6c73 650d 0a20  _sum_max else.. 
+0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc90: 2020 2028 7365 672e 6368 6172 5f63 6f75     (seg.char_cou
+0000dca0: 6e74 2829 203e 206d 6178 5f63 6861 7273  nt() > max_chars
+0000dcb0: 2061 6e64 2073 656c 662e 7365 676d 656e   and self.segmen
+0000dcc0: 7473 5b69 202b 2031 5d2e 6368 6172 5f63  ts[i + 1].char_c
+0000dcd0: 6f75 6e74 2829 203e 206d 6178 5f63 6861  ount() > max_cha
+0000dce0: 7273 290d 0a20 2020 2020 2020 2020 2020  rs)..           
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000dd10: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000dd20: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+0000dd30: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000dd40: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
+0000dd50: 2073 656c 662e 6164 645f 7365 676d 656e   self.add_segmen
+0000dd60: 7473 2869 2c20 6920 2b20 312c 2069 6e70  ts(i, i + 1, inp
+0000dd70: 6c61 6365 3d54 7275 652c 206c 6f63 6b3d  lace=True, lock=
+0000dd80: 6c6f 636b 2c20 6e65 776c 696e 653d 6e65  lock, newline=ne
+0000dd90: 776c 696e 6529 0d0a 2020 2020 2020 2020  wline)..        
+0000dda0: 7365 6c66 2e72 656d 6f76 655f 6e6f 5f77  self.remove_no_w
+0000ddb0: 6f72 645f 7365 676d 656e 7473 2829 0d0a  ord_segments()..
+0000ddc0: 0d0a 2020 2020 6465 6620 6765 745f 636f  ..    def get_co
+0000ddd0: 6e74 656e 745f 6279 5f74 696d 6528 0d0a  ntent_by_time(..
+0000dde0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ddf0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+0000de00: 696d 653a 2055 6e69 6f6e 5b66 6c6f 6174  ime: Union[float
+0000de10: 2c20 5475 706c 655b 666c 6f61 742c 2066  , Tuple[float, f
+0000de20: 6c6f 6174 5d2c 2064 6963 745d 2c0d 0a20  loat], dict],.. 
+0000de30: 2020 2020 2020 2020 2020 2077 6974 6869             withi
+0000de40: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
+0000de50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000de60: 676d 656e 745f 6c65 7665 6c3a 2062 6f6f  gment_level: boo
+0000de70: 6c20 3d20 4661 6c73 650d 0a20 2020 2029  l = False..    )
+0000de80: 202d 3e20 556e 696f 6e5b 4c69 7374 5b57   -> Union[List[W
+0000de90: 6f72 6454 696d 696e 675d 2c20 4c69 7374  ordTiming], List
+0000dea0: 5b53 6567 6d65 6e74 5d5d 3a0d 0a20 2020  [Segment]]:..   
+0000deb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000dec0: 2020 5265 7475 726e 2063 6f6e 7465 6e74    Return content
+0000ded0: 2069 6e20 7468 6520 6060 7469 6d65 6060   in the ``time``
+0000dee0: 2072 616e 6765 2e0d 0a0d 0a20 2020 2020   range.....     
+0000def0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+0000df00: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000df10: 2d0d 0a20 2020 2020 2020 2074 696d 6520  -..        time 
+0000df20: 3a20 666c 6f61 7420 6f72 2074 7570 6c65  : float or tuple
+0000df30: 206f 6620 2866 6c6f 6174 2c20 666c 6f61   of (float, floa
+0000df40: 7429 206f 7220 6469 6374 0d0a 2020 2020  t) or dict..    
+0000df50: 2020 2020 2020 2020 5261 6e67 6520 6f66          Range of
+0000df60: 2074 696d 6520 746f 2066 696e 6420 636f   time to find co
+0000df70: 6e74 656e 742e 2046 6f72 2074 7570 6c65  ntent. For tuple
+0000df80: 206f 6620 7477 6f20 666c 6f61 7473 2c20   of two floats, 
+0000df90: 6669 7273 7420 7661 6c75 6520 6973 2074  first value is t
+0000dfa0: 6865 2073 7461 7274 2074 696d 6520 616e  he start time an
+0000dfb0: 6420 7365 636f 6e64 2076 616c 7565 2069  d second value i
+0000dfc0: 730d 0a20 2020 2020 2020 2020 2020 2074  s..            t
+0000dfd0: 6865 2065 6e64 2074 696d 652e 2046 6f72  he end time. For
+0000dfe0: 2061 2073 696e 676c 6520 666c 6f61 7420   a single float 
+0000dff0: 7661 6c75 652c 2069 7420 6973 2074 7265  value, it is tre
+0000e000: 6174 6564 2061 7320 626f 7468 2074 6865  ated as both the
+0000e010: 2073 7461 7274 2061 6e64 2065 6e64 2074   start and end t
+0000e020: 696d 652e 0d0a 2020 2020 2020 2020 7769  ime...        wi
+0000e030: 7468 696e 203a 2062 6f6f 6c2c 2064 6566  thin : bool, def
+0000e040: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+0000e050: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+0000e060: 746f 206f 6e6c 7920 6669 6e64 2063 6f6e  to only find con
+0000e070: 7465 6e74 2066 756c 6c79 206f 7665 726c  tent fully overl
+0000e080: 6170 7320 7769 7468 2060 6074 696d 6560  aps with ``time`
+0000e090: 6020 7261 6e67 652e 0d0a 2020 2020 2020  ` range...      
+0000e0a0: 2020 7365 676d 656e 745f 6c65 7665 6c20    segment_level 
+0000e0b0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+0000e0c0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+0000e0d0: 2020 2057 6865 7468 6572 2074 6f20 6c6f     Whether to lo
+0000e0e0: 6f6b 206f 6e6c 7920 6f6e 2074 6865 2073  ok only on the s
+0000e0f0: 6567 6d65 6e74 206c 6576 656c 2061 6e64  egment level and
+0000e100: 2072 6574 7572 6e20 696e 7374 616e 6365   return instance
+0000e110: 7320 6f66 203a 636c 6173 733a 6073 7461  s of :class:`sta
+0000e120: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+0000e130: 6c74 2e53 6567 6d65 6e74 600d 0a20 2020  lt.Segment`..   
+0000e140: 2020 2020 2020 2020 2069 6e73 7465 6164           instead
+0000e150: 206f 6620 3a63 6c61 7373 3a60 7374 6162   of :class:`stab
+0000e160: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
+0000e170: 742e 576f 7264 5469 6d69 6e67 602e 0d0a  t.WordTiming`...
+0000e180: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000e190: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+0000e1a0: 2d2d 0d0a 2020 2020 2020 2020 6c69 7374  --..        list
+0000e1b0: 206f 6620 7374 6162 6c65 5f77 6869 7370   of stable_whisp
+0000e1c0: 6572 2e72 6573 756c 742e 576f 7264 5469  er.result.WordTi
+0000e1d0: 6d69 6e67 206f 7220 6c69 7374 206f 6620  ming or list of 
+0000e1e0: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
+0000e1f0: 6573 756c 742e 5365 676d 656e 740d 0a20  esult.Segment.. 
+0000e200: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+0000e210: 6f66 2063 6f6e 7465 6e74 7320 696e 2074  of contents in t
+0000e220: 6865 2060 6074 696d 6560 6020 7261 6e67  he ``time`` rang
+0000e230: 652e 2054 6865 2063 6f6e 7465 6e74 7320  e. The contents 
+0000e240: 6172 6520 696e 7374 616e 6365 7320 6f66  are instances of
+0000e250: 0d0a 2020 2020 2020 2020 2020 2020 3a63  ..            :c
+0000e260: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
+0000e270: 7370 6572 2e72 6573 756c 742e 5365 676d  sper.result.Segm
+0000e280: 656e 7460 2069 6620 6060 7365 676d 656e  ent` if ``segmen
+0000e290: 745f 6c65 7665 6c20 3d20 5472 7565 6060  t_level = True``
+0000e2a0: 2065 6c73 650d 0a20 2020 2020 2020 2020   else..         
+0000e2b0: 2020 203a 636c 6173 733a 6073 7461 626c     :class:`stabl
+0000e2c0: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+0000e2d0: 2e57 6f72 6454 696d 696e 6760 2e0d 0a20  .WordTiming`... 
+0000e2e0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000e2f0: 2020 2020 6966 206e 6f74 2073 6567 6d65      if not segme
+0000e300: 6e74 5f6c 6576 656c 2061 6e64 206e 6f74  nt_level and not
+0000e310: 2073 656c 662e 6861 735f 776f 7264 733a   self.has_words:
+0000e320: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+0000e330: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000e340: 4d69 7373 696e 6720 776f 7264 2074 696d  Missing word tim
+0000e350: 6573 7461 6d70 7320 696e 2072 6573 756c  estamps in resul
+0000e360: 742e 2055 7365 2060 6073 6567 6d65 6e74  t. Use ``segment
+0000e370: 5f6c 6576 656c 3d54 7275 6560 6020 696e  _level=True`` in
+0000e380: 7374 6561 642e 2729 0d0a 2020 2020 2020  stead.')..      
+0000e390: 2020 636f 6e74 656e 7473 203d 2073 656c    contents = sel
+0000e3a0: 662e 7365 676d 656e 7473 2069 6620 7365  f.segments if se
+0000e3b0: 676d 656e 745f 6c65 7665 6c20 656c 7365  gment_level else
+0000e3c0: 2073 656c 662e 616c 6c5f 776f 7264 7328   self.all_words(
+0000e3d0: 290d 0a20 2020 2020 2020 2069 6620 6973  )..        if is
+0000e3e0: 696e 7374 616e 6365 2874 696d 652c 2028  instance(time, (
+0000e3f0: 666c 6f61 742c 2069 6e74 2929 3a0d 0a20  float, int)):.. 
+0000e400: 2020 2020 2020 2020 2020 2074 696d 6520             time 
+0000e410: 3d20 5b74 696d 652c 2074 696d 655d 0d0a  = [time, time]..
+0000e420: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+0000e430: 6e73 7461 6e63 6528 7469 6d65 2c20 6469  nstance(time, di
+0000e440: 6374 293a 0d0a 2020 2020 2020 2020 2020  ct):..          
+0000e450: 2020 7469 6d65 203d 205b 7469 6d65 5b27    time = [time['
+0000e460: 7374 6172 7427 5d2c 2074 696d 655b 2765  start'], time['e
+0000e470: 6e64 275d 5d0d 0a20 2020 2020 2020 2073  nd']]..        s
+0000e480: 7461 7274 2c20 656e 6420 3d20 7469 6d65  tart, end = time
+0000e490: 0d0a 0d0a 2020 2020 2020 2020 6966 2077  ....        if w
+0000e4a0: 6974 6869 6e3a 0d0a 2020 2020 2020 2020  ithin:..        
+0000e4b0: 2020 2020 6465 6620 6973 5f69 6e5f 7261      def is_in_ra
+0000e4c0: 6e67 6528 6329 3a0d 0a20 2020 2020 2020  nge(c):..       
+0000e4d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e4e0: 7374 6172 7420 3c3d 2063 2e73 7461 7274  start <= c.start
+0000e4f0: 2061 6e64 2065 6e64 203e 3d20 632e 656e   and end >= c.en
+0000e500: 640d 0a20 2020 2020 2020 2065 6c73 653a  d..        else:
+0000e510: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+0000e520: 6620 6973 5f69 6e5f 7261 6e67 6528 6329  f is_in_range(c)
+0000e530: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e540: 2020 2072 6574 7572 6e20 7374 6172 7420     return start 
+0000e550: 3c3d 2063 2e65 6e64 2061 6e64 2065 6e64  <= c.end and end
+0000e560: 203e 3d20 632e 7374 6172 740d 0a0d 0a20   >= c.start.... 
+0000e570: 2020 2020 2020 2072 6574 7572 6e20 5b63         return [c
+0000e580: 2066 6f72 2063 2069 6e20 636f 6e74 656e   for c in conten
+0000e590: 7473 2069 6620 6973 5f69 6e5f 7261 6e67  ts if is_in_rang
+0000e5a0: 6528 6329 5d0d 0a0d 0a20 2020 2064 6566  e(c)]....    def
+0000e5b0: 2073 706c 6974 5f62 795f 6761 7028 0d0a   split_by_gap(..
+0000e5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e5d0: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+0000e5e0: 6178 5f67 6170 3a20 666c 6f61 7420 3d20  ax_gap: float = 
+0000e5f0: 302e 312c 0d0a 2020 2020 2020 2020 2020  0.1,..          
+0000e600: 2020 6c6f 636b 3a20 626f 6f6c 203d 2046    lock: bool = F
+0000e610: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+0000e620: 2020 206e 6577 6c69 6e65 3a20 626f 6f6c     newline: bool
+0000e630: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
+0000e640: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
+0000e650: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
+0000e660: 0d0a 2020 2020 2020 2020 5370 6c69 7420  ..        Split 
+0000e670: 2869 6e2d 706c 6163 6529 2061 6e79 2073  (in-place) any s
+0000e680: 6567 6d65 6e74 2077 6865 7265 2074 6865  egment where the
+0000e690: 2067 6170 2062 6574 7765 656e 2074 776f   gap between two
+0000e6a0: 206f 6620 6974 7320 776f 7264 7320 6973   of its words is
+0000e6b0: 2067 7265 6174 6572 2074 6861 6e20 6060   greater than ``
+0000e6c0: 6d61 785f 6761 7060 602e 0d0a 0d0a 2020  max_gap``.....  
+0000e6d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0000e6e0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0000e6f0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6d61  ----..        ma
+0000e700: 785f 6761 7020 3a20 666c 6f61 742c 2064  x_gap : float, d
+0000e710: 6566 6175 6c74 2030 2e31 0d0a 2020 2020  efault 0.1..    
+0000e720: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
+0000e730: 7365 636f 6e64 2873 2920 616c 6c6f 7765  second(s) allowe
+0000e740: 6420 6265 7477 6565 6e20 7477 6f20 776f  d between two wo
+0000e750: 7264 7320 6966 2074 6865 2073 616d 6520  rds if the same 
+0000e760: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
+0000e770: 2020 6c6f 636b 203a 2062 6f6f 6c2c 2064    lock : bool, d
+0000e780: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
+0000e790: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+0000e7a0: 7220 746f 2070 7265 7665 6e74 2066 7574  r to prevent fut
+0000e7b0: 7572 6520 7370 6c69 7473 2f6d 6572 6765  ure splits/merge
+0000e7c0: 7320 6672 6f6d 2061 6c74 6572 696e 6720  s from altering 
+0000e7d0: 6368 616e 6765 7320 6d61 6465 2062 7920  changes made by 
+0000e7e0: 7468 6973 206d 6574 686f 642e 0d0a 2020  this method...  
+0000e7f0: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
+0000e800: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+0000e810: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000e820: 5768 6574 6865 7220 746f 2069 6e73 6572  Whether to inser
+0000e830: 7420 6c69 6e65 2062 7265 616b 2061 7420  t line break at 
+0000e840: 7468 6520 7370 6c69 7420 706f 696e 7473  the split points
+0000e850: 2069 6e73 7465 6164 206f 6620 7370 6c69   instead of spli
+0000e860: 7474 696e 6720 696e 746f 2073 6570 6172  tting into separ
+0000e870: 6174 6520 7365 676d 656e 7473 2e0d 0a0d  ate segments....
+0000e880: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000e890: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0000e8a0: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
+0000e8b0: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+0000e8c0: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
+0000e8d0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000e8e0: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
+0000e8f0: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
+0000e900: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
+0000e910: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000e920: 7370 6c69 745f 7365 676d 656e 7473 286c  split_segments(l
+0000e930: 616d 6264 6120 783a 2078 2e67 6574 5f67  ambda x: x.get_g
+0000e940: 6170 5f69 6e64 6963 6573 286d 6178 5f67  ap_indices(max_g
+0000e950: 6170 292c 206c 6f63 6b3d 6c6f 636b 2c20  ap), lock=lock, 
+0000e960: 6e65 776c 696e 653d 6e65 776c 696e 6529  newline=newline)
+0000e970: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000e980: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
+0000e990: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+0000e9a0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+0000e9b0: 6973 746f 7279 202b 3d20 275f 270d 0a20  istory += '_'.. 
+0000e9c0: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
+0000e9d0: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
+0000e9e0: 6627 7367 3d7b 6d61 785f 6761 707d 2b7b  f'sg={max_gap}+{
+0000e9f0: 696e 7428 6c6f 636b 297d 2b7b 696e 7428  int(lock)}+{int(
+0000ea00: 6e65 776c 696e 6529 7d27 0d0a 2020 2020  newline)}'..    
+0000ea10: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+0000ea20: 0a0d 0a20 2020 2064 6566 206d 6572 6765  ...    def merge
+0000ea30: 5f62 795f 6761 7028 0d0a 2020 2020 2020  _by_gap(..      
+0000ea40: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+0000ea50: 2020 2020 2020 2020 206d 696e 5f67 6170           min_gap
+0000ea60: 3a20 666c 6f61 7420 3d20 302e 312c 0d0a  : float = 0.1,..
+0000ea70: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000ea80: 776f 7264 733a 2069 6e74 203d 204e 6f6e  words: int = Non
+0000ea90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+0000eaa0: 6d61 785f 6368 6172 733a 2069 6e74 203d  max_chars: int =
+0000eab0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+0000eac0: 2020 2020 6973 5f73 756d 5f6d 6178 3a20      is_sum_max: 
+0000ead0: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+0000eae0: 2020 2020 2020 2020 2020 206c 6f63 6b3a             lock:
+0000eaf0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+0000eb00: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
+0000eb10: 696e 653a 2062 6f6f 6c20 3d20 4661 6c73  ine: bool = Fals
+0000eb20: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
+0000eb30: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
+0000eb40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000eb50: 2020 204d 6572 6765 2028 696e 2d70 6c61     Merge (in-pla
+0000eb60: 6365 2920 616e 7920 7061 6972 206f 6620  ce) any pair of 
+0000eb70: 6164 6a61 6365 6e74 2073 6567 6d65 6e74  adjacent segment
+0000eb80: 7320 6966 2074 6865 2067 6170 2062 6574  s if the gap bet
+0000eb90: 7765 656e 2074 6865 6d20 3c3d 2060 606d  ween them <= ``m
+0000eba0: 696e 5f67 6170 6060 2e0d 0a0d 0a20 2020  in_gap``.....   
+0000ebb0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+0000ebc0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000ebd0: 2d2d 2d0d 0a20 2020 2020 2020 206d 696e  ---..        min
+0000ebe0: 5f67 6170 203a 2066 6c6f 6174 2c20 6465  _gap : float, de
+0000ebf0: 6661 756c 7420 302e 310d 0a20 2020 2020  fault 0.1..     
+0000ec00: 2020 2020 2020 204d 696e 696d 756d 2073         Minimum s
+0000ec10: 6563 6f6e 6428 7329 2061 6c6c 6f77 2062  econd(s) allow b
+0000ec20: 6574 7765 656e 2074 776f 2073 6567 6d65  etween two segme
+0000ec30: 6e74 2e0d 0a20 2020 2020 2020 206d 6178  nt...        max
+0000ec40: 5f77 6f72 6473 203a 2069 6e74 2c20 6f70  _words : int, op
+0000ec50: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000ec60: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
+0000ec70: 6572 206f 6620 776f 7264 7320 616c 6c6f  er of words allo
+0000ec80: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
+0000ec90: 656e 742e 0d0a 2020 2020 2020 2020 6d61  ent...        ma
+0000eca0: 785f 6368 6172 7320 3a20 696e 742c 206f  x_chars : int, o
+0000ecb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000ecc0: 2020 2020 204d 6178 696d 756d 206e 756d       Maximum num
+0000ecd0: 6265 7220 6f66 2063 6861 7261 6374 6572  ber of character
+0000ece0: 7320 616c 6c6f 7765 6420 696e 2065 6163  s allowed in eac
+0000ecf0: 6820 7365 676d 656e 742e 0d0a 2020 2020  h segment...    
+0000ed00: 2020 2020 6973 5f73 756d 5f6d 6178 203a      is_sum_max :
+0000ed10: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+0000ed20: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+0000ed30: 2020 5768 6574 6865 7220 6060 6d61 785f    Whether ``max_
+0000ed40: 776f 7264 7360 6020 616e 6420 6060 6d61  words`` and ``ma
+0000ed50: 785f 6368 6172 7360 6020 6973 2061 7070  x_chars`` is app
+0000ed60: 6c69 6564 2074 6f20 7468 6520 6d65 7267  lied to the merg
+0000ed70: 6564 2073 6567 6d65 6e74 2069 6e73 7465  ed segment inste
+0000ed80: 6164 206f 6620 7468 6520 696e 6469 7669  ad of the indivi
+0000ed90: 6475 616c 2073 6567 6d65 6e74 730d 0a20  dual segments.. 
+0000eda0: 2020 2020 2020 2020 2020 2074 6f20 6265             to be
+0000edb0: 206d 6572 6765 642e 0d0a 2020 2020 2020   merged...      
+0000edc0: 2020 6c6f 636b 203a 2062 6f6f 6c2c 2064    lock : bool, d
+0000edd0: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
+0000ede0: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+0000edf0: 7220 746f 2070 7265 7665 6e74 2066 7574  r to prevent fut
+0000ee00: 7572 6520 7370 6c69 7473 2f6d 6572 6765  ure splits/merge
+0000ee10: 7320 6672 6f6d 2061 6c74 6572 696e 6720  s from altering 
+0000ee20: 6368 616e 6765 7320 6d61 6465 2062 7920  changes made by 
+0000ee30: 7468 6973 206d 6574 686f 642e 0d0a 2020  this method...  
+0000ee40: 2020 2020 2020 6e65 776c 696e 6520 3a20        newline : 
+0000ee50: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+0000ee60: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+0000ee70: 2057 6865 7468 6572 2074 6f20 696e 7365   Whether to inse
+0000ee80: 7274 2061 206c 696e 6520 6272 6561 6b20  rt a line break 
+0000ee90: 6265 7477 6565 6e20 7468 6520 6d65 7267  between the merg
+0000eea0: 6564 2073 6567 6d65 6e74 732e 0d0a 0d0a  ed segments.....
+0000eeb0: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+0000eec0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000eed0: 0d0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
+0000eee0: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+0000eef0: 5768 6973 7065 7252 6573 756c 740d 0a20  WhisperResult.. 
+0000ef00: 2020 2020 2020 2020 2020 2054 6865 2063             The c
+0000ef10: 7572 7265 6e74 2069 6e73 7461 6e63 6520  urrent instance 
+0000ef20: 6166 7465 7220 7468 6520 6368 616e 6765  after the change
+0000ef30: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
+0000ef40: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+0000ef50: 203d 2073 656c 662e 6765 745f 6761 705f   = self.get_gap_
+0000ef60: 696e 6469 6365 7328 6d69 6e5f 6761 7029  indices(min_gap)
+0000ef70: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000ef80: 6d65 7267 655f 7365 676d 656e 7473 280d  merge_segments(.
+0000ef90: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+0000efa0: 6963 6573 2c0d 0a20 2020 2020 2020 2020  ices,..         
+0000efb0: 2020 206d 6178 5f77 6f72 6473 3d6d 6178     max_words=max
+0000efc0: 5f77 6f72 6473 2c0d 0a20 2020 2020 2020  _words,..       
+0000efd0: 2020 2020 206d 6178 5f63 6861 7273 3d6d       max_chars=m
+0000efe0: 6178 5f63 6861 7273 2c0d 0a20 2020 2020  ax_chars,..     
+0000eff0: 2020 2020 2020 2069 735f 7375 6d5f 6d61         is_sum_ma
+0000f000: 783d 6973 5f73 756d 5f6d 6178 2c0d 0a20  x=is_sum_max,.. 
+0000f010: 2020 2020 2020 2020 2020 206c 6f63 6b3d             lock=
+0000f020: 6c6f 636b 2c0d 0a20 2020 2020 2020 2020  lock,..         
+0000f030: 2020 206e 6577 6c69 6e65 3d6e 6577 6c69     newline=newli
+0000f040: 6e65 0d0a 2020 2020 2020 2020 290d 0a20  ne..        ).. 
+0000f050: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000f060: 7265 6772 6f75 705f 6869 7374 6f72 793a  regroup_history:
+0000f070: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000f080: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
+0000f090: 6f72 7920 2b3d 2027 5f27 0d0a 2020 2020  ory += '_'..    
+0000f0a0: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
+0000f0b0: 705f 6869 7374 6f72 7920 2b3d 2028 0d0a  p_history += (..
+0000f0c0: 2020 2020 2020 2020 2020 2020 6627 6d67              f'mg
+0000f0d0: 3d7b 6d69 6e5f 6761 707d 2b7b 6d61 785f  ={min_gap}+{max_
+0000f0e0: 776f 7264 7320 6f72 2022 227d 2b7b 6d61  words or ""}+{ma
+0000f0f0: 785f 6368 6172 7320 6f72 2022 227d 2b7b  x_chars or ""}+{
+0000f100: 696e 7428 6973 5f73 756d 5f6d 6178 297d  int(is_sum_max)}
+0000f110: 2b7b 696e 7428 6c6f 636b 297d 2b7b 696e  +{int(lock)}+{in
+0000f120: 7428 6e65 776c 696e 6529 7d27 0d0a 2020  t(newline)}'..  
+0000f130: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000f140: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+0000f150: 2020 2020 6465 6620 7370 6c69 745f 6279      def split_by
+0000f160: 5f70 756e 6374 7561 7469 6f6e 280d 0a20  _punctuation(.. 
+0000f170: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+0000f180: 0d0a 2020 2020 2020 2020 2020 2020 7075  ..            pu
+0000f190: 6e63 7475 6174 696f 6e3a 2055 6e69 6f6e  nctuation: Union
+0000f1a0: 5b4c 6973 745b 7374 725d 2c20 4c69 7374  [List[str], List
+0000f1b0: 5b54 7570 6c65 5b73 7472 2c20 7374 725d  [Tuple[str, str]
+0000f1c0: 5d2c 2073 7472 5d2c 0d0a 2020 2020 2020  ], str],..      
+0000f1d0: 2020 2020 2020 6c6f 636b 3a20 626f 6f6c        lock: bool
+0000f1e0: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+0000f1f0: 2020 2020 2020 206e 6577 6c69 6e65 3a20         newline: 
+0000f200: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+0000f210: 2020 2020 2020 2020 2020 206d 696e 5f77             min_w
+0000f220: 6f72 6473 3a20 4f70 7469 6f6e 616c 5b69  ords: Optional[i
+0000f230: 6e74 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  nt] = None,..   
+0000f240: 2020 2020 2020 2020 206d 696e 5f63 6861           min_cha
+0000f250: 7273 3a20 4f70 7469 6f6e 616c 5b69 6e74  rs: Optional[int
+0000f260: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+0000f270: 2020 2020 2020 206d 696e 5f64 7572 3a20         min_dur: 
+0000f280: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0000f290: 4e6f 6e65 0d0a 2020 2020 2920 2d3e 2022  None..    ) -> "
+0000f2a0: 5768 6973 7065 7252 6573 756c 7422 3a0d  WhisperResult":.
+0000f2b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000f2c0: 2020 2020 2020 5370 6c69 7420 2869 6e2d        Split (in-
+0000f2d0: 706c 6163 6529 2073 6567 6d65 6e74 7320  place) segments 
+0000f2e0: 6174 2077 6f72 6473 2074 6861 7420 7374  at words that st
+0000f2f0: 6172 742f 656e 6420 7769 7468 2060 6070  art/end with ``p
+0000f300: 756e 6374 7561 7469 6f6e 6060 2e0d 0a0d  unctuation``....
+0000f310: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000f320: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+0000f330: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+0000f340: 2070 756e 6374 7561 7469 6f6e 203a 206c   punctuation : l
+0000f350: 6973 7420 6f66 2073 7472 206f 6620 6c69  ist of str of li
+0000f360: 7374 206f 6620 7475 706c 6520 6f66 2028  st of tuple of (
+0000f370: 7374 722c 2073 7472 2920 6f72 2073 7472  str, str) or str
+0000f380: 0d0a 2020 2020 2020 2020 2020 2020 5075  ..            Pu
+0000f390: 6e63 7475 6174 696f 6e28 7329 2074 6f20  nctuation(s) to 
+0000f3a0: 7370 6c69 7420 7365 676d 656e 7473 2062  split segments b
+0000f3b0: 792e 0d0a 2020 2020 2020 2020 6c6f 636b  y...        lock
+0000f3c0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0000f3d0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000f3e0: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+0000f3f0: 7265 7665 6e74 2066 7574 7572 6520 7370  revent future sp
+0000f400: 6c69 7473 2f6d 6572 6765 7320 6672 6f6d  lits/merges from
+0000f410: 2061 6c74 6572 696e 6720 6368 616e 6765   altering change
+0000f420: 7320 6d61 6465 2062 7920 7468 6973 206d  s made by this m
+0000f430: 6574 686f 642e 0d0a 2020 2020 2020 2020  ethod...        
+0000f440: 6e65 776c 696e 6520 3a20 626f 6f6c 2c20  newline : bool, 
+0000f450: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+0000f460: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+0000f470: 6572 2074 6f20 696e 7365 7274 206c 696e  er to insert lin
+0000f480: 6520 6272 6561 6b20 6174 2074 6865 2073  e break at the s
+0000f490: 706c 6974 2070 6f69 6e74 7320 696e 7374  plit points inst
+0000f4a0: 6561 6420 6f66 2073 706c 6974 7469 6e67  ead of splitting
+0000f4b0: 2069 6e74 6f20 7365 7061 7261 7465 2073   into separate s
+0000f4c0: 6567 6d65 6e74 732e 0d0a 2020 2020 2020  egments...      
+0000f4d0: 2020 6d69 6e5f 776f 7264 7320 3a20 696e    min_words : in
+0000f4e0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+0000f4f0: 2020 2020 2020 2020 2053 706c 6974 2073           Split s
+0000f500: 6567 6d65 6e74 7320 7769 7468 2077 6f72  egments with wor
+0000f510: 6473 203e 3d20 6060 6d69 6e5f 776f 7264  ds >= ``min_word
+0000f520: 7360 602e 0d0a 2020 2020 2020 2020 6d69  s``...        mi
+0000f530: 6e5f 6368 6172 7320 3a20 696e 742c 206f  n_chars : int, o
+0000f540: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000f550: 2020 2020 2053 706c 6974 2073 6567 6d65       Split segme
+0000f560: 6e74 7320 7769 7468 2063 6861 7261 6374  nts with charact
+0000f570: 6572 7320 3e3d 2060 606d 696e 5f63 6861  ers >= ``min_cha
+0000f580: 7273 6060 2e0d 0a20 2020 2020 2020 206d  rs``...        m
+0000f590: 696e 5f64 7572 203a 2069 6e74 2c20 6f70  in_dur : int, op
+0000f5a0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000f5b0: 2020 2020 7370 6c69 7420 7365 676d 656e      split segmen
+0000f5c0: 7473 2077 6974 6820 6475 7261 7469 6f6e  ts with duration
+0000f5d0: 2028 696e 2073 6563 6f6e 6473 2920 3e3d   (in seconds) >=
+0000f5e0: 2060 606d 696e 5f64 7572 6060 2e0d 0a0d   ``min_dur``....
+0000f5f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000f600: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+0000f610: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
+0000f620: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+0000f630: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
+0000f640: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000f650: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
+0000f660: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
+0000f670: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
+0000f680: 0d0a 2020 2020 2020 2020 6465 6620 5f6f  ..        def _o
+0000f690: 7665 725f 6d61 7828 783a 2053 6567 6d65  ver_max(x: Segme
+0000f6a0: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
+0000f6b0: 2020 7265 7475 726e 2028 0d0a 2020 2020    return (..    
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6d0: 286d 696e 5f77 6f72 6473 2061 6e64 206c  (min_words and l
+0000f6e0: 656e 2878 2e77 6f72 6473 2920 3e3d 206d  en(x.words) >= m
+0000f6f0: 696e 5f77 6f72 6473 2920 6f72 0d0a 2020  in_words) or..  
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 2020 286d 696e 5f63 6861 7273 2061 6e64    (min_chars and
+0000f720: 2078 2e63 6861 725f 636f 756e 7428 2920   x.char_count() 
+0000f730: 3e3d 206d 696e 5f63 6861 7273 2920 6f72  >= min_chars) or
+0000f740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f750: 2020 2020 2020 286d 696e 5f64 7572 2061        (min_dur a
+0000f760: 6e64 2078 2e64 7572 6174 696f 6e20 3e3d  nd x.duration >=
+0000f770: 206d 696e 5f64 7572 290d 0a20 2020 2020   min_dur)..     
+0000f780: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+0000f790: 2020 2020 696e 6469 6365 7320 3d20 7365      indices = se
+0000f7a0: 7428 732e 6964 2066 6f72 2073 2069 6e20  t(s.id for s in 
+0000f7b0: 7365 6c66 2e73 6567 6d65 6e74 7320 6966  self.segments if
+0000f7c0: 205f 6f76 6572 5f6d 6178 2873 2929 2069   _over_max(s)) i
+0000f7d0: 6620 616e 7928 286d 696e 5f77 6f72 6473  f any((min_words
+0000f7e0: 2c20 6d69 6e5f 6368 6172 732c 206d 696e  , min_chars, min
+0000f7f0: 5f64 7572 2929 2065 6c73 6520 4e6f 6e65  _dur)) else None
+0000f800: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
+0000f810: 5f67 6574 5f69 6e64 6963 6573 2878 3a20  _get_indices(x: 
+0000f820: 5365 676d 656e 7429 3a0d 0a20 2020 2020  Segment):..     
+0000f830: 2020 2020 2020 2072 6574 7572 6e20 782e         return x.
+0000f840: 6765 745f 7075 6e63 7475 6174 696f 6e5f  get_punctuation_
+0000f850: 696e 6469 6365 7328 7075 6e63 7475 6174  indices(punctuat
+0000f860: 696f 6e29 2069 6620 696e 6469 6365 7320  ion) if indices 
+0000f870: 6973 204e 6f6e 6520 6f72 2078 2e69 6420  is None or x.id 
+0000f880: 696e 2069 6e64 6963 6573 2065 6c73 6520  in indices else 
+0000f890: 5b5d 0d0a 0d0a 2020 2020 2020 2020 7365  []....        se
+0000f8a0: 6c66 2e5f 7370 6c69 745f 7365 676d 656e  lf._split_segmen
+0000f8b0: 7473 285f 6765 745f 696e 6469 6365 732c  ts(_get_indices,
+0000f8c0: 206c 6f63 6b3d 6c6f 636b 2c20 6e65 776c   lock=lock, newl
+0000f8d0: 696e 653d 6e65 776c 696e 6529 0d0a 2020  ine=newline)..  
+0000f8e0: 2020 2020 2020 6966 2073 656c 662e 5f72        if self._r
+0000f8f0: 6567 726f 7570 5f68 6973 746f 7279 3a0d  egroup_history:.
+0000f900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f910: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
+0000f920: 7279 202b 3d20 275f 270d 0a20 2020 2020  ry += '_'..     
+0000f930: 2020 2070 756e 6374 5f73 7472 203d 2027     punct_str = '
+0000f940: 2f27 2e6a 6f69 6e28 7020 6966 2069 7369  /'.join(p if isi
+0000f950: 6e73 7461 6e63 6528 702c 2073 7472 2920  nstance(p, str) 
+0000f960: 656c 7365 2027 2a27 2e6a 6f69 6e28 7029  else '*'.join(p)
+0000f970: 2066 6f72 2070 2069 6e20 7075 6e63 7475   for p in punctu
+0000f980: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+0000f990: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
+0000f9a0: 7374 6f72 7920 2b3d 2066 2773 703d 7b70  story += f'sp={p
+0000f9b0: 756e 6374 5f73 7472 7d2b 7b69 6e74 286c  unct_str}+{int(l
+0000f9c0: 6f63 6b29 7d2b 7b69 6e74 286e 6577 6c69  ock)}+{int(newli
+0000f9d0: 6e65 297d 270d 0a20 2020 2020 2020 2073  ne)}'..        s
+0000f9e0: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+0000f9f0: 746f 7279 202b 3d20 6627 2b7b 6d69 6e5f  tory += f'+{min_
+0000fa00: 776f 7264 7320 6f72 2022 227d 2b7b 6d69  words or ""}+{mi
+0000fa10: 6e5f 6368 6172 7320 6f72 2022 227d 2b7b  n_chars or ""}+{
+0000fa20: 6d69 6e5f 6475 7220 6f72 2022 227d 272e  min_dur or ""}'.
+0000fa30: 7273 7472 6970 2827 2b27 290d 0a20 2020  rstrip('+')..   
+0000fa40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000fa50: 0d0a 0d0a 2020 2020 6465 6620 6d65 7267  ....    def merg
+0000fa60: 655f 6279 5f70 756e 6374 7561 7469 6f6e  e_by_punctuation
+0000fa70: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+0000fa80: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+0000fa90: 2020 7075 6e63 7475 6174 696f 6e3a 2055    punctuation: U
+0000faa0: 6e69 6f6e 5b4c 6973 745b 7374 725d 2c20  nion[List[str], 
+0000fab0: 4c69 7374 5b54 7570 6c65 5b73 7472 2c20  List[Tuple[str, 
+0000fac0: 7374 725d 5d2c 2073 7472 5d2c 0d0a 2020  str]], str],..  
+0000fad0: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
+0000fae0: 7264 733a 2069 6e74 203d 204e 6f6e 652c  rds: int = None,
+0000faf0: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+0000fb00: 785f 6368 6172 733a 2069 6e74 203d 204e  x_chars: int = N
+0000fb10: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+0000fb20: 2020 6973 5f73 756d 5f6d 6178 3a20 626f    is_sum_max: bo
+0000fb30: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
+0000fb40: 2020 2020 2020 2020 206c 6f63 6b3a 2062           lock: b
+0000fb50: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+0000fb60: 2020 2020 2020 2020 2020 6e65 776c 696e            newlin
+0000fb70: 653a 2062 6f6f 6c20 3d20 4661 6c73 650d  e: bool = False.
+0000fb80: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
+0000fb90: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
+0000fba0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000fbb0: 204d 6572 6765 2028 696e 2d70 6c61 6365   Merge (in-place
+0000fbc0: 2920 616e 7920 7477 6f20 7365 676d 656e  ) any two segmen
+0000fbd0: 7473 2074 6861 7420 6861 7320 7370 6563  ts that has spec
+0000fbe0: 6966 6963 2070 756e 6374 7561 7469 6f6e  ific punctuation
+0000fbf0: 7320 696e 6265 7477 6565 6e2e 0d0a 0d0a  s inbetween.....
+0000fc00: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000fc10: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+0000fc20: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000fc30: 7075 6e63 7475 6174 696f 6e20 3a20 6c69  punctuation : li
+0000fc40: 7374 206f 6620 7374 7220 6f66 206c 6973  st of str of lis
+0000fc50: 7420 6f66 2074 7570 6c65 206f 6620 2873  t of tuple of (s
+0000fc60: 7472 2c20 7374 7229 206f 7220 7374 720d  tr, str) or str.
+0000fc70: 0a20 2020 2020 2020 2020 2020 2050 756e  .            Pun
+0000fc80: 6374 7561 7469 6f6e 2873 2920 746f 206d  ctuation(s) to m
+0000fc90: 6572 6765 2073 6567 6d65 6e74 7320 6279  erge segments by
+0000fca0: 2e0d 0a20 2020 2020 2020 206d 6178 5f77  ...        max_w
+0000fcb0: 6f72 6473 203a 2069 6e74 2c20 6f70 7469  ords : int, opti
+0000fcc0: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+0000fcd0: 2020 4d61 7869 6d75 6d20 6e75 6d62 6572    Maximum number
+0000fce0: 206f 6620 776f 7264 7320 616c 6c6f 7765   of words allowe
+0000fcf0: 6420 696e 2065 6163 6820 7365 676d 656e  d in each segmen
+0000fd00: 742e 0d0a 2020 2020 2020 2020 6d61 785f  t...        max_
+0000fd10: 6368 6172 7320 3a20 696e 742c 206f 7074  chars : int, opt
+0000fd20: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
+0000fd30: 2020 204d 6178 696d 756d 206e 756d 6265     Maximum numbe
+0000fd40: 7220 6f66 2063 6861 7261 6374 6572 7320  r of characters 
+0000fd50: 616c 6c6f 7765 6420 696e 2065 6163 6820  allowed in each 
+0000fd60: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
+0000fd70: 2020 6973 5f73 756d 5f6d 6178 203a 2062    is_sum_max : b
+0000fd80: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+0000fd90: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000fda0: 5768 6574 6865 7220 6060 6d61 785f 776f  Whether ``max_wo
+0000fdb0: 7264 7360 6020 616e 6420 6060 6d61 785f  rds`` and ``max_
+0000fdc0: 6368 6172 7360 6020 6973 2061 7070 6c69  chars`` is appli
+0000fdd0: 6564 2074 6f20 7468 6520 6d65 7267 6564  ed to the merged
+0000fde0: 2073 6567 6d65 6e74 2069 6e73 7465 6164   segment instead
+0000fdf0: 206f 6620 7468 6520 696e 6469 7669 6475   of the individu
+0000fe00: 616c 2073 6567 6d65 6e74 730d 0a20 2020  al segments..   
+0000fe10: 2020 2020 2020 2020 2074 6f20 6265 206d           to be m
+0000fe20: 6572 6765 642e 0d0a 2020 2020 2020 2020  erged...        
+0000fe30: 6c6f 636b 203a 2062 6f6f 6c2c 2064 6566  lock : bool, def
+0000fe40: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+0000fe50: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+0000fe60: 746f 2070 7265 7665 6e74 2066 7574 7572  to prevent futur
+0000fe70: 6520 7370 6c69 7473 2f6d 6572 6765 7320  e splits/merges 
+0000fe80: 6672 6f6d 2061 6c74 6572 696e 6720 6368  from altering ch
+0000fe90: 616e 6765 7320 6d61 6465 2062 7920 7468  anges made by th
+0000fea0: 6973 206d 6574 686f 642e 0d0a 2020 2020  is method...    
+0000feb0: 2020 2020 6e65 776c 696e 6520 3a20 626f      newline : bo
+0000fec0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+0000fed0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+0000fee0: 6865 7468 6572 2074 6f20 696e 7365 7274  hether to insert
+0000fef0: 2061 206c 696e 6520 6272 6561 6b20 6265   a line break be
+0000ff00: 7477 6565 6e20 7468 6520 6d65 7267 6564  tween the merged
+0000ff10: 2073 6567 6d65 6e74 732e 0d0a 0d0a 2020   segments.....  
+0000ff20: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+0000ff30: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+0000ff40: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+0000ff50: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+0000ff60: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
+0000ff70: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
+0000ff80: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
+0000ff90: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
+0000ffa0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000ffb0: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+0000ffc0: 2073 656c 662e 6765 745f 7075 6e63 7475   self.get_punctu
+0000ffd0: 6174 696f 6e5f 696e 6469 6365 7328 7075  ation_indices(pu
+0000ffe0: 6e63 7475 6174 696f 6e29 0d0a 2020 2020  nctuation)..    
+0000fff0: 2020 2020 7365 6c66 2e5f 6d65 7267 655f      self._merge_
+00010000: 7365 676d 656e 7473 280d 0a20 2020 2020  segments(..     
+00010010: 2020 2020 2020 2069 6e64 6963 6573 2c0d         indices,.
+00010020: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00010030: 5f77 6f72 6473 3d6d 6178 5f77 6f72 6473  _words=max_words
+00010040: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+00010050: 6178 5f63 6861 7273 3d6d 6178 5f63 6861  ax_chars=max_cha
+00010060: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+00010070: 2069 735f 7375 6d5f 6d61 783d 6973 5f73   is_sum_max=is_s
+00010080: 756d 5f6d 6178 2c0d 0a20 2020 2020 2020  um_max,..       
+00010090: 2020 2020 206c 6f63 6b3d 6c6f 636b 2c0d       lock=lock,.
+000100a0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+000100b0: 6c69 6e65 3d6e 6577 6c69 6e65 0d0a 2020  line=newline..  
+000100c0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000100d0: 2069 6620 7365 6c66 2e5f 7265 6772 6f75   if self._regrou
+000100e0: 705f 6869 7374 6f72 793a 0d0a 2020 2020  p_history:..    
+000100f0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00010100: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+00010110: 2027 5f27 0d0a 2020 2020 2020 2020 7075   '_'..        pu
+00010120: 6e63 745f 7374 7220 3d20 272f 272e 6a6f  nct_str = '/'.jo
+00010130: 696e 2870 2069 6620 6973 696e 7374 616e  in(p if isinstan
+00010140: 6365 2870 2c20 7374 7229 2065 6c73 6520  ce(p, str) else 
+00010150: 272a 272e 6a6f 696e 2870 2920 666f 7220  '*'.join(p) for 
+00010160: 7020 696e 2070 756e 6374 7561 7469 6f6e  p in punctuation
+00010170: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00010180: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+00010190: 202b 3d20 280d 0a20 2020 2020 2020 2020   += (..         
+000101a0: 2020 2066 276d 703d 7b70 756e 6374 5f73     f'mp={punct_s
+000101b0: 7472 7d2b 7b6d 6178 5f77 6f72 6473 206f  tr}+{max_words o
+000101c0: 7220 2222 7d2b 7b6d 6178 5f63 6861 7273  r ""}+{max_chars
+000101d0: 206f 7220 2222 7d2b 7b69 6e74 2869 735f   or ""}+{int(is_
+000101e0: 7375 6d5f 6d61 7829 7d2b 7b69 6e74 286c  sum_max)}+{int(l
+000101f0: 6f63 6b29 7d2b 7b69 6e74 286e 6577 6c69  ock)}+{int(newli
+00010200: 6e65 297d 270d 0a20 2020 2020 2020 2029  ne)}'..        )
+00010210: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00010220: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
+00010230: 2070 6164 280d 0a20 2020 2020 2020 2020   pad(..         
+00010240: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+00010250: 2020 2020 2020 7374 6172 745f 7061 643a        start_pad:
+00010260: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00010270: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+00010280: 2020 2020 2020 656e 645f 7061 643a 204f        end_pad: O
+00010290: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
+000102a0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000102b0: 2020 2020 6d61 785f 6475 723a 204f 7074      max_dur: Opt
+000102c0: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
+000102d0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+000102e0: 2020 6d61 785f 656e 643a 204f 7074 696f    max_end: Optio
+000102f0: 6e61 6c5b 666c 6f61 745d 203d 204e 6f6e  nal[float] = Non
+00010300: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00010310: 776f 7264 5f6c 6576 656c 3a20 626f 6f6c  word_level: bool
+00010320: 203d 2046 616c 7365 0d0a 2020 2020 2920   = False..    ) 
+00010330: 2d3e 2022 5768 6973 7065 7252 6573 756c  -> "WhisperResul
+00010340: 7422 3a0d 0a20 2020 2020 2020 2022 2222  t":..        """
+00010350: 0d0a 2020 2020 2020 2020 5061 6420 2869  ..        Pad (i
+00010360: 6e2d 706c 6163 6529 2074 696d 6573 7461  n-place) timesta
+00010370: 6d70 7320 696e 2063 6872 6f6e 6f6c 6f67  mps in chronolog
+00010380: 6963 616c 206f 7264 6572 2e0d 0a0d 0a20  ical order..... 
+00010390: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000103a0: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+000103b0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
+000103c0: 7461 7274 5f70 6164 203a 2066 6c6f 6174  tart_pad : float
+000103d0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000103e0: 2020 2020 2020 2020 5365 636f 6e64 7320          Seconds 
+000103f0: 746f 2070 6164 2073 7461 7274 2074 696d  to pad start tim
+00010400: 6573 7461 6d70 732e 0d0a 2020 2020 2020  estamps...      
+00010410: 2020 2020 2020 4561 6368 2073 7461 7274        Each start
+00010420: 2074 696d 6573 7461 6d70 2077 696c 6c20   timestamp will 
+00010430: 6265 2065 7874 656e 6465 6420 6e6f 2065  be extended no e
+00010440: 6172 6c69 6572 2074 6861 6e20 7468 6520  arlier than the 
+00010450: 656e 6420 7469 6d65 7374 616d 7020 6f66  end timestamp of
+00010460: 2074 6865 2070 7265 7669 6f75 7320 776f   the previous wo
+00010470: 7264 2e0d 0a20 2020 2020 2020 2065 6e64  rd...        end
+00010480: 5f70 6164 203a 2066 6c6f 6174 2c20 6f70  _pad : float, op
+00010490: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+000104a0: 2020 2020 5365 636f 6e64 7320 746f 2070      Seconds to p
+000104b0: 6164 2065 6e64 2074 696d 6573 7461 6d70  ad end timestamp
+000104c0: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
+000104d0: 4561 6368 2065 6e64 2074 696d 6573 7461  Each end timesta
+000104e0: 6d70 2077 696c 6c20 6265 2065 7874 656e  mp will be exten
+000104f0: 6465 6420 6e6f 206c 6174 6572 2074 6861  ded no later tha
+00010500: 6e20 7468 6520 7374 6172 7420 7469 6d65  n the start time
+00010510: 7374 616d 7020 6f66 2074 6865 206e 6578  stamp of the nex
+00010520: 7420 776f 7264 206f 7220 6060 6d61 785f  t word or ``max_
+00010530: 656e 6460 602e 0d0a 2020 2020 2020 2020  end``...        
+00010540: 6d61 785f 6475 7220 3a20 666c 6f61 742c  max_dur : float,
+00010550: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00010560: 2020 2020 2020 204f 6e6c 7920 7061 6420         Only pad 
+00010570: 7365 676d 656e 7473 206f 7220 776f 7264  segments or word
+00010580: 7320 2860 6077 6f72 645f 6c65 7665 6c3d  s (``word_level=
+00010590: 5472 7565 6060 2920 7769 7468 2064 7572  True``) with dur
+000105a0: 6174 696f 6e20 2869 6e20 7365 636f 6e64  ation (in second
+000105b0: 7329 2075 6e64 6572 206f 7220 6571 7561  s) under or equa
+000105c0: 6c20 746f 2060 606d 6178 5f64 7572 6060  l to ``max_dur``
+000105d0: 2e0d 0a20 2020 2020 2020 206d 6178 5f65  ...        max_e
+000105e0: 6e64 203a 2066 6c6f 6174 2c20 6f70 7469  nd : float, opti
+000105f0: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+00010600: 2020 5469 6d65 7374 616d 7020 2869 6e20    Timestamp (in 
+00010610: 7365 636f 6e64 7329 2074 6861 7420 7061  seconds) that pa
+00010620: 6464 6564 2074 696d 6573 7461 6d70 7320  dded timestamps 
+00010630: 6361 6e6e 6f74 2065 7863 6565 642e 0d0a  cannot exceed...
+00010640: 2020 2020 2020 2020 2020 2020 4765 6e65              Gene
+00010650: 7261 6c6c 7920 7573 6564 2074 6f20 7072  rally used to pr
+00010660: 6576 656e 7420 7468 6520 6c61 7374 2070  event the last p
+00010670: 6164 6465 6420 656e 6420 7469 6d65 7374  added end timest
+00010680: 616d 7020 6672 6f6d 2065 7863 6565 6469  amp from exceedi
+00010690: 6e67 2074 6865 2074 6f74 616c 2064 7572  ng the total dur
+000106a0: 6174 696f 6e20 6f66 2074 6865 2061 7564  ation of the aud
+000106b0: 696f 2e0d 0a20 2020 2020 2020 2077 6f72  io...        wor
+000106c0: 645f 6c65 7665 6c20 3a20 626f 6f6c 2c20  d_level : bool, 
+000106d0: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+000106e0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000106f0: 6572 2074 6f20 7061 6420 7365 676d 656e  er to pad segmen
+00010700: 7420 7469 6d65 7374 616d 7073 206f 7220  t timestamps or 
+00010710: 776f 7264 2074 696d 6573 7461 6d70 732e  word timestamps.
+00010720: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00010730: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00010740: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
+00010750: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+00010760: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+00010770: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
+00010780: 6865 2063 7572 7265 6e74 2069 6e73 7461  he current insta
+00010790: 6e63 6520 6166 7465 7220 7468 6520 6368  nce after the ch
+000107a0: 616e 6765 732e 0d0a 2020 2020 2020 2020  anges...        
+000107b0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+000107c0: 6e6f 7420 2873 7461 7274 5f70 6164 206f  not (start_pad o
+000107d0: 7220 656e 645f 7061 6429 3a0d 0a20 2020  r end_pad):..   
+000107e0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+000107f0: 732e 7761 726e 2866 274e 6f20 6060 7374  s.warn(f'No ``st
+00010800: 6172 745f 7061 6460 6020 6f72 2060 6065  art_pad`` or ``e
+00010810: 6e64 5f70 6164 6060 2067 6976 656e 2e27  nd_pad`` given.'
+00010820: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00010830: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00010840: 636b 6c65 7665 6c3d 3229 0d0a 2020 2020  cklevel=2)..    
+00010850: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00010860: 656c 660d 0a20 2020 2020 2020 2069 6620  elf..        if 
+00010870: 776f 7264 5f6c 6576 656c 2061 6e64 206e  word_level and n
+00010880: 6f74 2073 656c 662e 6861 735f 776f 7264  ot self.has_word
+00010890: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000108a0: 776f 7264 5f6c 6576 656c 203d 2046 616c  word_level = Fal
+000108b0: 7365 0d0a 2020 2020 2020 2020 7061 7274  se..        part
+000108c0: 7320 3d20 7365 6c66 2e61 6c6c 5f77 6f72  s = self.all_wor
+000108d0: 6473 2829 2069 6620 776f 7264 5f6c 6576  ds() if word_lev
+000108e0: 656c 2065 6c73 6520 7365 6c66 2e73 6567  el else self.seg
+000108f0: 6d65 6e74 730d 0a20 2020 2020 2020 2061  ments..        a
+00010900: 7373 6572 7420 6e6f 7420 7374 6172 745f  ssert not start_
+00010910: 7061 6420 6f72 2073 7461 7274 5f70 6164  pad or start_pad
+00010920: 203e 2030 2c20 2760 6073 7461 7274 5f70   > 0, '``start_p
+00010930: 6164 6060 206d 7573 7420 6265 2070 6f73  ad`` must be pos
+00010940: 6974 6976 6527 0d0a 2020 2020 2020 2020  itive'..        
+00010950: 6173 7365 7274 206e 6f74 2065 6e64 5f70  assert not end_p
+00010960: 6164 206f 7220 656e 645f 7061 6420 3e20  ad or end_pad > 
+00010970: 302c 2027 6060 656e 645f 7061 6460 6020  0, '``end_pad`` 
+00010980: 6d75 7374 2062 6520 706f 7369 7469 7665  must be positive
+00010990: 270d 0a20 2020 2020 2020 2061 7373 6572  '..        asser
+000109a0: 7420 6d61 785f 6475 7220 6973 204e 6f6e  t max_dur is Non
+000109b0: 6520 6f72 206d 6178 5f64 7572 203e 2030  e or max_dur > 0
+000109c0: 2c20 2760 606d 6178 5f64 7572 6060 206d  , '``max_dur`` m
+000109d0: 7573 7420 6265 2067 7265 6174 6572 2074  ust be greater t
+000109e0: 6861 6e20 3027 0d0a 2020 2020 2020 2020  han 0'..        
+000109f0: 6173 7365 7274 206d 6178 5f65 6e64 2069  assert max_end i
+00010a00: 7320 4e6f 6e65 206f 7220 6d61 785f 656e  s None or max_en
+00010a10: 6420 3e20 302c 2027 6060 6d61 785f 656e  d > 0, '``max_en
+00010a20: 6460 6020 6d75 7374 2062 6520 6772 6561  d`` must be grea
+00010a30: 7465 7220 7468 616e 2030 270d 0a20 2020  ter than 0'..   
+00010a40: 2020 2020 2066 6f72 2069 2c20 7061 7274       for i, part
+00010a50: 2069 6e20 656e 756d 6572 6174 6528 7061   in enumerate(pa
+00010a60: 7274 732c 2031 293a 0d0a 2020 2020 2020  rts, 1):..      
+00010a70: 2020 2020 2020 6966 206d 6178 5f64 7572        if max_dur
+00010a80: 2061 6e64 2070 6172 742e 656e 6420 2d20   and part.end - 
+00010a90: 7061 7274 2e73 7461 7274 203e 206d 6178  part.start > max
+00010aa0: 5f64 7572 3a0d 0a20 2020 2020 2020 2020  _dur:..         
+00010ab0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00010ac0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00010ad0: 7374 6172 745f 7061 643a 0d0a 2020 2020  start_pad:..    
+00010ae0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00010af0: 7374 6172 7420 3d20 7061 7274 2e73 7461  start = part.sta
+00010b00: 7274 202d 2073 7461 7274 5f70 6164 0d0a  rt - start_pad..
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b20: 6e65 775f 7374 6172 7420 3d20 6d61 7828  new_start = max(
+00010b30: 3020 6966 2069 203d 3d20 3120 656c 7365  0 if i == 1 else
+00010b40: 2070 6172 7473 5b69 2d32 5d2e 656e 642c   parts[i-2].end,
+00010b50: 206e 6577 5f73 7461 7274 290d 0a20 2020   new_start)..   
+00010b60: 2020 2020 2020 2020 2020 2020 2070 6172               par
+00010b70: 742e 7374 6172 7420 3d20 6e65 775f 7374  t.start = new_st
+00010b80: 6172 740d 0a20 2020 2020 2020 2020 2020  art..           
+00010b90: 2069 6620 656e 645f 7061 643a 0d0a 2020   if end_pad:..  
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00010bb0: 775f 656e 6420 3d20 7061 7274 2e65 6e64  w_end = part.end
+00010bc0: 202b 2065 6e64 5f70 6164 0d0a 2020 2020   + end_pad..    
+00010bd0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00010be0: 5f6d 6178 5f65 6e64 203d 206d 6178 5f65  _max_end = max_e
+00010bf0: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
+00010c00: 2020 2020 6966 2069 2021 3d20 6c65 6e28      if i != len(
+00010c10: 7061 7274 7329 3a0d 0a20 2020 2020 2020  parts):..       
+00010c20: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+00010c30: 705f 6d61 785f 656e 6420 3d20 6d69 6e28  p_max_end = min(
+00010c40: 6d61 785f 656e 642c 2070 6172 7473 5b69  max_end, parts[i
+00010c50: 5d2e 7374 6172 7429 2069 6620 6d61 785f  ].start) if max_
+00010c60: 656e 6420 656c 7365 2070 6172 7473 5b69  end else parts[i
+00010c70: 5d2e 7374 6172 740d 0a20 2020 2020 2020  ].start..       
+00010c80: 2020 2020 2020 2020 2069 6620 7465 6d70           if temp
+00010c90: 5f6d 6178 5f65 6e64 2061 6e64 2074 656d  _max_end and tem
+00010ca0: 705f 6d61 785f 656e 6420 3c20 6e65 775f  p_max_end < new_
+00010cb0: 656e 643a 0d0a 2020 2020 2020 2020 2020  end:..          
+00010cc0: 2020 2020 2020 2020 2020 6e65 775f 656e            new_en
+00010cd0: 6420 3d20 7465 6d70 5f6d 6178 5f65 6e64  d = temp_max_end
+00010ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010cf0: 2020 6966 206e 6577 5f65 6e64 203e 2070    if new_end > p
+00010d00: 6172 742e 656e 643a 0d0a 2020 2020 2020  art.end:..      
+00010d10: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00010d20: 7274 2e65 6e64 203d 206e 6577 5f65 6e64  rt.end = new_end
+00010d30: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+00010d40: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+00010d50: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
+00010d60: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
+00010d70: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
+00010d80: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00010d90: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
+00010da0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00010db0: 2066 2770 3d7b 7374 6172 745f 7061 6420   f'p={start_pad 
+00010dc0: 6f72 2022 227d 2b7b 656e 645f 7061 6420  or ""}+{end_pad 
+00010dd0: 6f72 2022 227d 2b7b 6d61 785f 6475 7220  or ""}+{max_dur 
+00010de0: 6f72 2022 227d 2b7b 6d61 785f 656e 6420  or ""}+{max_end 
+00010df0: 6f72 2022 227d 2b7b 696e 7428 776f 7264  or ""}+{int(word
+00010e00: 5f6c 6576 656c 297d 270d 0a20 2020 2020  _level)}'..     
+00010e10: 2020 2029 0d0a 2020 2020 2020 2020 7265     )..        re
+00010e20: 7475 726e 2073 656c 660d 0a0d 0a20 2020  turn self....   
+00010e30: 2064 6566 206d 6572 6765 5f61 6c6c 5f73   def merge_all_s
+00010e40: 6567 6d65 6e74 7328 7365 6c66 2920 2d3e  egments(self) ->
+00010e50: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
+00010e60: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00010e70: 2020 2020 2020 2020 4d65 7267 6520 616c          Merge al
+00010e80: 6c20 7365 676d 656e 7473 2069 6e74 6f20  l segments into 
+00010e90: 6f6e 6520 7365 676d 656e 742e 0d0a 0d0a  one segment.....
+00010ea0: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+00010eb0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00010ec0: 0d0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
+00010ed0: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+00010ee0: 5768 6973 7065 7252 6573 756c 740d 0a20  WhisperResult.. 
+00010ef0: 2020 2020 2020 2020 2020 2054 6865 2063             The c
+00010f00: 7572 7265 6e74 2069 6e73 7461 6e63 6520  urrent instance 
+00010f10: 6166 7465 7220 7468 6520 6368 616e 6765  after the change
+00010f20: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
+00010f30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00010f40: 7365 6c66 2e73 6567 6d65 6e74 733a 0d0a  self.segments:..
+00010f50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010f60: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
+00010f70: 2069 6620 7365 6c66 2e68 6173 5f77 6f72   if self.has_wor
+00010f80: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00010f90: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
+00010fa0: 7365 676d 656e 7473 5b30 5d2e 636f 7079  segments[0].copy
+00010fb0: 2873 656c 662e 616c 6c5f 776f 7264 7328  (self.all_words(
+00010fc0: 292c 206b 6565 705f 7265 7375 6c74 3d54  ), keep_result=T
+00010fd0: 7275 652c 2063 6f70 795f 776f 7264 733d  rue, copy_words=
+00010fe0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00010ff0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00011000: 2020 206e 6577 5f73 6567 203d 2073 656c     new_seg = sel
+00011010: 662e 7365 676d 656e 7473 5b30 5d0d 0a20  f.segments[0].. 
+00011020: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+00011030: 6567 2e5f 6465 6661 756c 745f 7465 7874  eg._default_text
+00011040: 203d 2027 272e 6a6f 696e 2873 2e74 6578   = ''.join(s.tex
+00011050: 7420 666f 7220 7320 696e 2073 656c 662e  t for s in self.
+00011060: 7365 676d 656e 7473 290d 0a20 2020 2020  segments)..     
+00011070: 2020 2020 2020 2069 6620 616c 6c28 732e         if all(s.
+00011080: 746f 6b65 6e73 2069 7320 6e6f 7420 4e6f  tokens is not No
+00011090: 6e65 2066 6f72 2073 2069 6e20 7365 6c66  ne for s in self
+000110a0: 2e73 6567 6d65 6e74 7329 3a0d 0a20 2020  .segments):..   
+000110b0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+000110c0: 5f73 6567 2e5f 6465 6661 756c 745f 746f  _seg._default_to
+000110d0: 6b65 6e73 203d 206c 6973 7428 6368 6169  kens = list(chai
+000110e0: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
+000110f0: 732e 746f 6b65 6e73 2066 6f72 2073 2069  s.tokens for s i
+00011100: 6e20 7365 6c66 2e73 6567 6d65 6e74 7329  n self.segments)
+00011110: 290d 0a20 2020 2020 2020 2020 2020 206e  )..            n
+00011120: 6577 5f73 6567 2e65 6e64 203d 2073 656c  ew_seg.end = sel
+00011130: 662e 7365 676d 656e 7473 5b2d 315d 2e65  f.segments[-1].e
+00011140: 6e64 0d0a 2020 2020 2020 2020 7365 6c66  nd..        self
+00011150: 2e73 6567 6d65 6e74 7320 3d20 5b6e 6577  .segments = [new
+00011160: 5f73 6567 5d0d 0a20 2020 2020 2020 2073  _seg]..        s
+00011170: 656c 662e 7265 6173 7369 676e 5f69 6473  elf.reassign_ids
+00011180: 2829 0d0a 2020 2020 2020 2020 6966 2073  ()..        if s
+00011190: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+000111a0: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
+000111b0: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
+000111c0: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
+000111d0: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+000111e0: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
+000111f0: 3d20 276d 7327 0d0a 2020 2020 2020 2020  = 'ms'..        
+00011200: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
+00011210: 2020 2064 6566 2073 706c 6974 5f62 795f     def split_by_
+00011220: 6c65 6e67 7468 280d 0a20 2020 2020 2020  length(..       
+00011230: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+00011240: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
+00011250: 733a 2069 6e74 203d 204e 6f6e 652c 0d0a  s: int = None,..
+00011260: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00011270: 776f 7264 733a 2069 6e74 203d 204e 6f6e  words: int = Non
+00011280: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00011290: 6576 656e 5f73 706c 6974 3a20 626f 6f6c  even_split: bool
+000112a0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+000112b0: 2020 2020 2020 666f 7263 655f 6c65 6e3a        force_len:
+000112c0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+000112d0: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
+000112e0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+000112f0: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
+00011300: 6c75 6465 5f6c 6f63 6b3a 2062 6f6f 6c20  lude_lock: bool 
+00011310: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00011320: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
+00011330: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
+00011340: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
+00011350: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
+00011360: 2222 220d 0a20 2020 2020 2020 2053 706c  """..        Spl
+00011370: 6974 2028 696e 2d70 6c61 6365 2920 616e  it (in-place) an
+00011380: 7920 7365 676d 656e 7420 7468 6174 2065  y segment that e
+00011390: 7863 6565 6473 2060 606d 6178 5f63 6861  xceeds ``max_cha
+000113a0: 7273 6060 206f 7220 6060 6d61 785f 776f  rs`` or ``max_wo
+000113b0: 7264 7360 6020 696e 746f 2073 6d61 6c6c  rds`` into small
+000113c0: 6572 2073 6567 6d65 6e74 732e 0d0a 0d0a  er segments.....
+000113d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000113e0: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+000113f0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00011400: 6d61 785f 6368 6172 7320 3a20 696e 742c  max_chars : int,
+00011410: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00011420: 2020 2020 2020 204d 6178 696d 756d 206e         Maximum n
+00011430: 756d 6265 7220 6f66 2063 6861 7261 6374  umber of charact
+00011440: 6572 7320 616c 6c6f 7765 6420 696e 2065  ers allowed in e
+00011450: 6163 6820 7365 676d 656e 742e 0d0a 2020  ach segment...  
+00011460: 2020 2020 2020 6d61 785f 776f 7264 7320        max_words 
+00011470: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+00011480: 0a20 2020 2020 2020 2020 2020 204d 6178  .            Max
+00011490: 696d 756d 206e 756d 6265 7220 6f66 2077  imum number of w
+000114a0: 6f72 6473 2061 6c6c 6f77 6564 2069 6e20  ords allowed in 
+000114b0: 6561 6368 2073 6567 6d65 6e74 2e0d 0a20  each segment... 
+000114c0: 2020 2020 2020 2065 7665 6e5f 7370 6c69         even_spli
+000114d0: 7420 3a20 626f 6f6c 2c20 6465 6661 756c  t : bool, defaul
+000114e0: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+000114f0: 2020 2020 5768 6574 6865 7220 746f 2065      Whether to e
+00011500: 7665 6e6c 7920 7370 6c69 7420 6120 7365  venly split a se
+00011510: 676d 656e 7420 696e 206c 656e 6774 6820  gment in length 
+00011520: 6966 2069 7420 6578 6365 6564 7320 6060  if it exceeds ``
+00011530: 6d61 785f 6368 6172 7360 6020 6f72 2060  max_chars`` or `
+00011540: 606d 6178 5f77 6f72 6473 6060 2e0d 0a20  `max_words``... 
+00011550: 2020 2020 2020 2066 6f72 6365 5f6c 656e         force_len
+00011560: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00011570: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00011580: 2020 2020 5768 6574 6865 7220 746f 2066      Whether to f
+00011590: 6f72 6365 2061 2063 6f6e 7374 616e 7420  orce a constant 
+000115a0: 6c65 6e67 7468 2066 6f72 2065 6163 6820  length for each 
+000115b0: 7365 676d 656e 7420 6578 6365 7074 2074  segment except t
+000115c0: 6865 206c 6173 7420 7365 676d 656e 742e  he last segment.
+000115d0: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000115e0: 6973 2077 696c 6c20 6967 6e6f 7265 2061  is will ignore a
+000115f0: 6c6c 2070 7265 7669 6f75 7320 6e6f 6e2d  ll previous non-
+00011600: 6c6f 636b 6564 2073 6567 6d65 6e74 2062  locked segment b
+00011610: 6f75 6e64 6172 6965 732e 0d0a 2020 2020  oundaries...    
+00011620: 2020 2020 6c6f 636b 203a 2062 6f6f 6c2c      lock : bool,
+00011630: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+00011640: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00011650: 6865 7220 746f 2070 7265 7665 6e74 2066  her to prevent f
+00011660: 7574 7572 6520 7370 6c69 7473 2f6d 6572  uture splits/mer
+00011670: 6765 7320 6672 6f6d 2061 6c74 6572 696e  ges from alterin
+00011680: 6720 6368 616e 6765 7320 6d61 6465 2062  g changes made b
+00011690: 7920 7468 6973 206d 6574 686f 642e 0d0a  y this method...
+000116a0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+000116b0: 6c6f 636b 3a20 626f 6f6c 2c20 6465 6661  lock: bool, defa
+000116c0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
+000116d0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+000116e0: 6f20 696e 636c 7564 6520 7072 6576 696f  o include previo
+000116f0: 7573 206c 6f63 6b20 6265 666f 7265 2073  us lock before s
+00011700: 706c 6974 7469 6e67 2062 6173 6564 206f  plitting based o
+00011710: 6e20 6d61 785f 776f 7264 732c 2069 6620  n max_words, if 
+00011720: 6060 6576 656e 5f73 706c 6974 203d 2046  ``even_split = F
+00011730: 616c 7365 6060 2e0d 0a20 2020 2020 2020  alse``...       
+00011740: 2020 2020 2053 706c 6974 7469 6e67 2077       Splitting w
+00011750: 696c 6c20 6265 2064 6f6e 6520 6166 7465  ill be done afte
+00011760: 7220 7468 6520 6669 7273 7420 6e6f 6e2d  r the first non-
+00011770: 6c6f 636b 6564 2077 6f72 6420 3e20 6060  locked word > ``
+00011780: 6d61 785f 6368 6172 7360 6020 2f20 6060  max_chars`` / ``
+00011790: 6d61 785f 776f 7264 7360 602e 0d0a 2020  max_words``...  
+000117a0: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
+000117b0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+000117c0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+000117d0: 5768 6574 6865 7220 746f 2069 6e73 6572  Whether to inser
+000117e0: 7420 6c69 6e65 2062 7265 616b 2061 7420  t line break at 
+000117f0: 7468 6520 7370 6c69 7420 706f 696e 7473  the split points
+00011800: 2069 6e73 7465 6164 206f 6620 7370 6c69   instead of spli
+00011810: 7474 696e 6720 696e 746f 2073 6570 6172  tting into separ
+00011820: 6174 6520 7365 676d 656e 7473 2e0d 0a0d  ate segments....
+00011830: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00011840: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00011850: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
+00011860: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+00011870: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
+00011880: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00011890: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
+000118a0: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
+000118b0: 6573 2e0d 0a0d 0a20 2020 2020 2020 204e  es.....        N
+000118c0: 6f74 6573 0d0a 2020 2020 2020 2020 2d2d  otes..        --
+000118d0: 2d2d 2d0d 0a20 2020 2020 2020 2049 6620  ---..        If 
+000118e0: 6060 6576 656e 5f73 706c 6974 203d 2054  ``even_split = T
+000118f0: 7275 6560 602c 2073 6567 6d65 6e74 7320  rue``, segments 
+00011900: 6361 6e20 7374 696c 6c20 6578 6365 6564  can still exceed
+00011910: 2060 606d 6178 5f63 6861 7273 6060 2061   ``max_chars`` a
+00011920: 6e64 206c 6f63 6b65 6420 776f 7264 7320  nd locked words 
+00011930: 7769 6c6c 2062 6520 6967 6e6f 7265 6420  will be ignored 
+00011940: 746f 2061 766f 6964 0d0a 2020 2020 2020  to avoid..      
+00011950: 2020 756e 6576 656e 2073 706c 6974 7469    uneven splitti
+00011960: 6e67 2e0d 0a20 2020 2020 2020 2022 2222  ng...        """
+00011970: 0d0a 2020 2020 2020 2020 6966 2066 6f72  ..        if for
+00011980: 6365 5f6c 656e 3a0d 0a20 2020 2020 2020  ce_len:..       
+00011990: 2020 2020 2073 656c 662e 6d65 7267 655f       self.merge_
+000119a0: 616c 6c5f 7365 676d 656e 7473 2829 0d0a  all_segments()..
+000119b0: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+000119c0: 6c69 745f 7365 676d 656e 7473 280d 0a20  lit_segments(.. 
+000119d0: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+000119e0: 6120 783a 2078 2e67 6574 5f6c 656e 6774  a x: x.get_lengt
+000119f0: 685f 696e 6469 6365 7328 0d0a 2020 2020  h_indices(..    
+00011a00: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00011a10: 6368 6172 733d 6d61 785f 6368 6172 732c  chars=max_chars,
 00011a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011a30: 2020 6375 7272 5f6d 6178 5f64 7572 203d    curr_max_dur =
-00011a40: 206d 6564 6975 6d5f 6661 6374 6f72 202a   medium_factor *
-00011a50: 2064 7572 6174 696f 6e73 5b6c 656e 2864   durations[len(d
-00011a60: 7572 6174 696f 6e73 292f 2f32 202b 2031  urations)//2 + 1
-00011a70: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00011a80: 2069 6620 6d61 785f 6475 7220 616e 6420   if max_dur and 
-00011a90: 286e 6f74 2063 7572 725f 6d61 785f 6475  (not curr_max_du
-00011aa0: 7220 6f72 2063 7572 725f 6d61 785f 6475  r or curr_max_du
-00011ab0: 7220 3e20 6d61 785f 6475 7229 3a0d 0a20  r > max_dur):.. 
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011ad0: 7572 725f 6d61 785f 6475 7220 3d20 6d61  urr_max_dur = ma
-00011ae0: 785f 6475 720d 0a0d 0a20 2020 2020 2020  x_dur....       
-00011af0: 2020 2020 2069 6620 6e6f 7420 6375 7272       if not curr
-00011b00: 5f6d 6178 5f64 7572 3a0d 0a20 2020 2020  _max_dur:..     
-00011b10: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00011b20: 6e75 650d 0a0d 0a20 2020 2020 2020 2020  nue....         
-00011b30: 2020 2069 6620 636c 6970 5f73 7461 7274     if clip_start
-00011b40: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00011b50: 2020 2020 2020 2020 2020 2073 6567 2e77             seg.w
-00011b60: 6f72 6473 5b30 5d2e 636c 616d 705f 6d61  ords[0].clamp_ma
-00011b70: 7828 6375 7272 5f6d 6178 5f64 7572 2c20  x(curr_max_dur, 
-00011b80: 636c 6970 5f73 7461 7274 3d54 7275 652c  clip_start=True,
-00011b90: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-00011ba0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00011bb0: 2020 2073 6567 2e77 6f72 6473 5b2d 315d     seg.words[-1]
-00011bc0: 2e63 6c61 6d70 5f6d 6178 2863 7572 725f  .clamp_max(curr_
-00011bd0: 6d61 785f 6475 722c 2063 6c69 705f 7374  max_dur, clip_st
-00011be0: 6172 743d 4661 6c73 652c 2076 6572 626f  art=False, verbo
-00011bf0: 7365 3d76 6572 626f 7365 290d 0a20 2020  se=verbose)..   
-00011c00: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 666f 7220 692c 2077 6f72 6420 696e 2065  for i, word in e
-00011c30: 6e75 6d65 7261 7465 2873 6567 2e77 6f72  numerate(seg.wor
-00011c40: 6473 293a 0d0a 2020 2020 2020 2020 2020  ds):..          
-00011c50: 2020 2020 2020 2020 2020 776f 7264 2e63            word.c
-00011c60: 6c61 6d70 5f6d 6178 2863 7572 725f 6d61  lamp_max(curr_ma
-00011c70: 785f 6475 722c 2063 6c69 705f 7374 6172  x_dur, clip_star
-00011c80: 743d 636c 6970 5f73 7461 7274 2c20 7665  t=clip_start, ve
-00011c90: 7262 6f73 653d 7665 7262 6f73 6529 0d0a  rbose=verbose)..
-00011ca0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00011cb0: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-00011cc0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00011cd0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-00011ce0: 6973 746f 7279 202b 3d20 275f 270d 0a20  istory += '_'.. 
-00011cf0: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
-00011d00: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
-00011d10: 6627 636d 3d7b 6d65 6469 756d 5f66 6163  f'cm={medium_fac
-00011d20: 746f 727d 2b7b 6d61 785f 6475 7220 6f72  tor}+{max_dur or
-00011d30: 2022 227d 2b7b 636c 6970 5f73 7461 7274   ""}+{clip_start
-00011d40: 206f 7220 2222 7d2b 7b69 6e74 2876 6572   or ""}+{int(ver
-00011d50: 626f 7365 297d 270d 0a20 2020 2020 2020  bose)}'..       
-00011d60: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00011d70: 2020 2020 6465 6620 6c6f 636b 280d 0a20      def lock(.. 
-00011d80: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00011d90: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00011da0: 6172 7473 7769 7468 3a20 556e 696f 6e5b  artswith: Union[
-00011db0: 7374 722c 204c 6973 745b 7374 725d 5d20  str, List[str]] 
-00011dc0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00011dd0: 2020 2020 2065 6e64 7377 6974 683a 2055       endswith: U
-00011de0: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
-00011df0: 7472 5d5d 203d 204e 6f6e 652c 0d0a 2020  tr]] = None,..  
-00011e00: 2020 2020 2020 2020 2020 7269 6768 743a            right:
-00011e10: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
-00011e20: 2020 2020 2020 2020 2020 206c 6566 743a             left:
-00011e30: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00011e40: 2020 2020 2020 2020 2020 2020 6361 7365              case
-00011e50: 5f73 656e 7369 7469 7665 3a20 626f 6f6c  _sensitive: bool
-00011e60: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00011e70: 2020 2020 2020 2073 7472 6970 3a20 626f         strip: bo
-00011e80: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
-00011e90: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
-00011ea0: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
-00011eb0: 220d 0a20 2020 2020 2020 204c 6f63 6b20  "..        Lock 
-00011ec0: 776f 7264 732f 7365 676d 656e 7473 2077  words/segments w
-00011ed0: 6974 6820 6d61 7463 6869 6e67 2070 7265  ith matching pre
-00011ee0: 6669 782f 7375 6666 6978 2074 6f20 7072  fix/suffix to pr
-00011ef0: 6576 656e 7420 7370 6c69 7474 696e 672f  event splitting/
-00011f00: 6d65 7267 696e 672e 0d0a 0d0a 2020 2020  merging.....    
-00011f10: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00011f20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00011f30: 2d2d 0d0a 2020 2020 2020 2020 7374 6172  --..        star
-00011f40: 7473 7769 7468 3a20 7374 7220 6f72 206c  tswith: str or l
-00011f50: 6973 7420 6f66 2073 7472 0d0a 2020 2020  ist of str..    
-00011f60: 2020 2020 2020 2020 5072 6566 6978 6573          Prefixes
-00011f70: 2074 6f20 6c6f 636b 2e0d 0a20 2020 2020   to lock...     
-00011f80: 2020 2065 6e64 7377 6974 683a 2073 7472     endswith: str
-00011f90: 206f 7220 6c69 7374 206f 6620 7374 720d   or list of str.
-00011fa0: 0a20 2020 2020 2020 2020 2020 2053 7566  .            Suf
-00011fb0: 6669 7865 7320 746f 206c 6f63 6b2e 0d0a  fixes to lock...
-00011fc0: 2020 2020 2020 2020 7269 6768 7420 3a20          right : 
-00011fd0: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00011fe0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00011ff0: 5768 6574 6865 7220 7072 6576 656e 7420  Whether prevent 
-00012000: 7370 6c69 7473 2f6d 6572 6765 7320 7769  splits/merges wi
-00012010: 7468 2074 6865 206e 6578 7420 776f 7264  th the next word
-00012020: 2f73 6567 6d65 6e74 2e0d 0a20 2020 2020  /segment...     
-00012030: 2020 206c 6566 7420 3a20 626f 6f6c 2c20     left : bool, 
-00012040: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
-00012050: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-00012060: 6572 2070 7265 7665 6e74 2073 706c 6974  er prevent split
-00012070: 732f 6d65 7267 6573 2077 6974 6820 7468  s/merges with th
-00012080: 6520 7072 6576 696f 7573 2077 6f72 642f  e previous word/
-00012090: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
-000120a0: 2020 6361 7365 5f73 656e 7369 7469 7665    case_sensitive
-000120b0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-000120c0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-000120d0: 2020 2020 5768 6574 6865 7220 746f 206d      Whether to m
-000120e0: 6174 6368 2074 6865 2063 6173 6520 6f66  atch the case of
-000120f0: 2074 6865 2070 7265 6669 7865 732f 7375   the prefixes/su
-00012100: 6666 6978 6573 2077 6974 6820 7468 6520  ffixes with the 
-00012110: 776f 7264 732f 7365 676d 656e 7473 2e0d  words/segments..
-00012120: 0a20 2020 2020 2020 2073 7472 6970 203a  .        strip :
-00012130: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
-00012140: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-00012150: 2057 6865 7468 6572 2074 6f20 6967 6e6f   Whether to igno
-00012160: 7265 2073 7061 6365 7320 6265 666f 7265  re spaces before
-00012170: 2061 6e64 2061 6674 6572 2062 6f74 6820   and after both 
-00012180: 776f 7264 732f 7365 676d 656e 7473 2061  words/segments a
-00012190: 6e64 2070 7265 6669 7865 732f 7375 6666  nd prefixes/suff
-000121a0: 6978 6573 2e0d 0a0d 0a20 2020 2020 2020  ixes.....       
-000121b0: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-000121c0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-000121d0: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
-000121e0: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-000121f0: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
-00012200: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
-00012210: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
-00012220: 6865 2063 6861 6e67 6573 2e0d 0a20 2020  he changes...   
-00012230: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00012240: 2020 6173 7365 7274 2073 7461 7274 7377    assert startsw
-00012250: 6974 6820 6f72 2065 6e64 7377 6974 682c  ith or endswith,
-00012260: 2027 4d75 7374 2073 7065 6369 6679 205b   'Must specify [
-00012270: 7374 6172 7473 7769 7468 5d20 6f72 2f61  startswith] or/a
-00012280: 6e64 205b 656e 6473 7769 7468 5d2e 270d  nd [endswith].'.
-00012290: 0a20 2020 2020 2020 2073 7461 7274 7377  .        startsw
-000122a0: 6974 6820 3d20 5b5d 2069 6620 7374 6172  ith = [] if star
-000122b0: 7473 7769 7468 2069 7320 4e6f 6e65 2065  tswith is None e
-000122c0: 6c73 6520 285b 7374 6172 7473 7769 7468  lse ([startswith
-000122d0: 5d20 6966 2069 7369 6e73 7461 6e63 6528  ] if isinstance(
-000122e0: 7374 6172 7473 7769 7468 2c20 7374 7229  startswith, str)
-000122f0: 2065 6c73 6520 7374 6172 7473 7769 7468   else startswith
-00012300: 290d 0a20 2020 2020 2020 2065 6e64 7377  )..        endsw
-00012310: 6974 6820 3d20 5b5d 2069 6620 656e 6473  ith = [] if ends
-00012320: 7769 7468 2069 7320 4e6f 6e65 2065 6c73  with is None els
-00012330: 6520 285b 656e 6473 7769 7468 5d20 6966  e ([endswith] if
-00012340: 2069 7369 6e73 7461 6e63 6528 656e 6473   isinstance(ends
-00012350: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
-00012360: 656e 6473 7769 7468 290d 0a20 2020 2020  endswith)..     
-00012370: 2020 2069 6620 6e6f 7420 6361 7365 5f73     if not case_s
-00012380: 656e 7369 7469 7665 3a0d 0a20 2020 2020  ensitive:..     
-00012390: 2020 2020 2020 2073 7461 7274 7377 6974         startswit
-000123a0: 6820 3d20 5b74 2e6c 6f77 6572 2829 2066  h = [t.lower() f
-000123b0: 6f72 2074 2069 6e20 7374 6172 7473 7769  or t in startswi
-000123c0: 7468 5d0d 0a20 2020 2020 2020 2020 2020  th]..           
-000123d0: 2065 6e64 7377 6974 6820 3d20 5b74 2e6c   endswith = [t.l
-000123e0: 6f77 6572 2829 2066 6f72 2074 2069 6e20  ower() for t in 
-000123f0: 656e 6473 7769 7468 5d0d 0a20 2020 2020  endswith]..     
-00012400: 2020 2069 6620 7374 7269 703a 0d0a 2020     if strip:..  
-00012410: 2020 2020 2020 2020 2020 7374 6172 7473            starts
-00012420: 7769 7468 203d 205b 742e 7374 7269 7028  with = [t.strip(
-00012430: 2920 666f 7220 7420 696e 2073 7461 7274  ) for t in start
-00012440: 7377 6974 685d 0d0a 2020 2020 2020 2020  swith]..        
-00012450: 2020 2020 656e 6473 7769 7468 203d 205b      endswith = [
-00012460: 742e 7374 7269 7028 2920 666f 7220 7420  t.strip() for t 
-00012470: 696e 2065 6e64 7377 6974 685d 0d0a 2020  in endswith]..  
-00012480: 2020 2020 2020 666f 7220 7061 7274 2069        for part i
-00012490: 6e20 7365 6c66 2e61 6c6c 5f77 6f72 6473  n self.all_words
-000124a0: 5f6f 725f 7365 676d 656e 7473 2829 3a0d  _or_segments():.
-000124b0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-000124c0: 7420 3d20 7061 7274 2e77 6f72 6420 6966  t = part.word if
-000124d0: 2068 6173 6174 7472 2870 6172 742c 2027   hasattr(part, '
-000124e0: 776f 7264 2729 2065 6c73 6520 7061 7274  word') else part
-000124f0: 2e74 6578 740d 0a20 2020 2020 2020 2020  .text..         
-00012500: 2020 2069 6620 6e6f 7420 6361 7365 5f73     if not case_s
-00012510: 656e 7369 7469 7665 3a0d 0a20 2020 2020  ensitive:..     
-00012520: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-00012530: 3d20 7465 7874 2e6c 6f77 6572 2829 0d0a  = text.lower()..
-00012540: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00012550: 7472 6970 3a0d 0a20 2020 2020 2020 2020  trip:..         
-00012560: 2020 2020 2020 2074 6578 7420 3d20 7465         text = te
-00012570: 7874 2e73 7472 6970 2829 0d0a 2020 2020  xt.strip()..    
-00012580: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
-00012590: 6978 2069 6e20 7374 6172 7473 7769 7468  ix in startswith
-000125a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000125b0: 2020 2069 6620 7465 7874 2e73 7461 7274     if text.start
-000125c0: 7377 6974 6828 7072 6566 6978 293a 0d0a  swith(prefix):..
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 6966 2072 6967 6874 3a0d 0a20      if right:.. 
-000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012600: 2020 2020 2020 2070 6172 742e 6c6f 636b         part.lock
-00012610: 5f72 6967 6874 2829 0d0a 2020 2020 2020  _right()..      
-00012620: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012630: 206c 6566 743a 0d0a 2020 2020 2020 2020   left:..        
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 7061 7274 2e6c 6f63 6b5f 6c65 6674 2829  part.lock_left()
-00012660: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00012670: 7220 7375 6666 6978 2069 6e20 656e 6473  r suffix in ends
-00012680: 7769 7468 3a0d 0a20 2020 2020 2020 2020  with:..         
-00012690: 2020 2020 2020 2069 6620 7465 7874 2e65         if text.e
-000126a0: 6e64 7377 6974 6828 7375 6666 6978 293a  ndswith(suffix):
-000126b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000126c0: 2020 2020 2020 6966 2072 6967 6874 3a0d        if right:.
-000126d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000126e0: 2020 2020 2020 2020 2070 6172 742e 6c6f           part.lo
-000126f0: 636b 5f72 6967 6874 2829 0d0a 2020 2020  ck_right()..    
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 6966 206c 6566 743a 0d0a 2020 2020 2020  if left:..      
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012730: 2020 7061 7274 2e6c 6f63 6b5f 6c65 6674    part.lock_left
-00012740: 2829 0d0a 2020 2020 2020 2020 6966 2073  ()..        if s
-00012750: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
-00012760: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
-00012770: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
-00012780: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
-00012790: 0a20 2020 2020 2020 2073 7461 7274 7377  .        startsw
-000127a0: 6974 685f 7374 7220 3d20 2873 7461 7274  ith_str = (start
-000127b0: 7377 6974 6820 6966 2069 7369 6e73 7461  swith if isinsta
-000127c0: 6e63 6528 7374 6172 7473 7769 7468 2c20  nce(startswith, 
-000127d0: 7374 7229 2065 6c73 6520 272f 272e 6a6f  str) else '/'.jo
-000127e0: 696e 2873 7461 7274 7377 6974 6829 2920  in(startswith)) 
-000127f0: 6966 2073 7461 7274 7377 6974 6820 656c  if startswith el
-00012800: 7365 2022 220d 0a20 2020 2020 2020 2065  se ""..        e
-00012810: 6e64 7377 6974 685f 7374 7220 3d20 2865  ndswith_str = (e
-00012820: 6e64 7377 6974 6820 6966 2069 7369 6e73  ndswith if isins
-00012830: 7461 6e63 6528 656e 6473 7769 7468 2c20  tance(endswith, 
-00012840: 7374 7229 2065 6c73 6520 272f 272e 6a6f  str) else '/'.jo
-00012850: 696e 2865 6e64 7377 6974 6829 2920 6966  in(endswith)) if
-00012860: 2065 6e64 7377 6974 6820 656c 7365 2022   endswith else "
-00012870: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00012880: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-00012890: 202b 3d20 2866 276c 3d7b 7374 6172 7473   += (f'l={starts
-000128a0: 7769 7468 5f73 7472 7d2b 7b65 6e64 7377  with_str}+{endsw
-000128b0: 6974 685f 7374 727d 270d 0a20 2020 2020  ith_str}'..     
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 2020 2020 2020 2020 2020 2020 2066 272b               f'+
-000128e0: 7b69 6e74 2872 6967 6874 297d 2b7b 696e  {int(right)}+{in
-000128f0: 7428 6c65 6674 297d 2b7b 696e 7428 6361  t(left)}+{int(ca
-00012900: 7365 5f73 656e 7369 7469 7665 297d 2b7b  se_sensitive)}+{
-00012910: 696e 7428 7374 7269 7029 7d27 290d 0a20  int(strip)}').. 
-00012920: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012930: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
-00012940: 6d6f 7665 5f77 6f72 6428 0d0a 2020 2020  move_word(..    
-00012950: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00012960: 2020 2020 2020 2020 2020 2077 6f72 643a             word:
-00012970: 2055 6e69 6f6e 5b57 6f72 6454 696d 696e   Union[WordTimin
-00012980: 672c 2054 7570 6c65 5b69 6e74 2c20 696e  g, Tuple[int, in
-00012990: 745d 5d2c 0d0a 2020 2020 2020 2020 2020  t]],..          
-000129a0: 2020 7265 6173 7369 676e 5f69 6473 3a20    reassign_ids: 
-000129b0: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
-000129c0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-000129d0: 653a 2062 6f6f 6c20 3d20 5472 7565 0d0a  e: bool = True..
-000129e0: 2020 2020 2920 2d3e 2027 5768 6973 7065      ) -> 'Whispe
-000129f0: 7252 6573 756c 7427 3a0d 0a20 2020 2020  rResult':..     
-00012a00: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00012a10: 5265 6d6f 7665 2061 2077 6f72 642e 0d0a  Remove a word...
-00012a20: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00012a30: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00012a40: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00012a50: 2020 776f 7264 203a 2057 6f72 6454 696d    word : WordTim
-00012a60: 696e 6720 6f72 2074 7570 6c65 206f 6620  ing or tuple of 
-00012a70: 2869 6e74 2c20 696e 7429 0d0a 2020 2020  (int, int)..    
-00012a80: 2020 2020 2020 2020 496e 7374 616e 6365          Instance
-00012a90: 206f 6620 3a63 6c61 7373 3a60 7374 6162   of :class:`stab
-00012aa0: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
-00012ab0: 742e 576f 7264 5469 6d69 6e67 6020 6f72  t.WordTiming` or
-00012ac0: 2074 7570 6c65 206f 6620 2873 6567 6d65   tuple of (segme
-00012ad0: 6e74 2069 6e64 6578 2c20 776f 7264 2069  nt index, word i
-00012ae0: 6e64 6578 292e 0d0a 2020 2020 2020 2020  ndex)...        
-00012af0: 7265 6173 7369 676e 5f69 6473 203a 2062  reassign_ids : b
-00012b00: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-00012b10: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-00012b20: 6865 7468 6572 2074 6f20 7265 6173 7369  hether to reassi
-00012b30: 676e 2073 6567 6d65 6e74 2061 6e64 2077  gn segment and w
-00012b40: 6f72 6420 6964 7320 2869 6e64 6963 6573  ord ids (indices
-00012b50: 2920 6166 7465 7220 7265 6d6f 7669 6e67  ) after removing
-00012b60: 2060 6077 6f72 6460 602e 0d0a 2020 2020   ``word``...    
-00012b70: 2020 2020 7665 7262 6f73 6520 3a20 626f      verbose : bo
-00012b80: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-00012b90: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00012ba0: 6574 6865 7220 746f 2070 7269 6e74 2064  ether to print d
-00012bb0: 6574 6169 6c20 6f66 2074 6865 2072 656d  etail of the rem
-00012bc0: 6f76 6564 2077 6f72 642e 0d0a 0d0a 2020  oved word.....  
-00012bd0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-00012be0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-00012bf0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
-00012c00: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-00012c10: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
-00012c20: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
-00012c30: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
-00012c40: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
-00012c50: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00012c60: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00012c70: 616e 6365 2877 6f72 642c 2057 6f72 6454  ance(word, WordT
-00012c80: 696d 696e 6729 3a0d 0a20 2020 2020 2020  iming):..       
-00012c90: 2020 2020 2069 6620 7365 6c66 5b77 6f72       if self[wor
-00012ca0: 642e 7365 676d 656e 745f 6964 5d5b 776f  d.segment_id][wo
-00012cb0: 7264 2e69 645d 2069 7320 6e6f 7420 776f  rd.id] is not wo
-00012cc0: 7264 3a0d 0a20 2020 2020 2020 2020 2020  rd:..           
-00012cd0: 2020 2020 2073 656c 662e 7265 6173 7369       self.reassi
-00012ce0: 676e 5f69 6473 2829 0d0a 2020 2020 2020  gn_ids()..      
-00012cf0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00012d00: 665b 776f 7264 2e73 6567 6d65 6e74 5f69  f[word.segment_i
-00012d10: 645d 5b77 6f72 642e 6964 5d20 6973 206e  d][word.id] is n
-00012d20: 6f74 2077 6f72 643a 0d0a 2020 2020 2020  ot word:..      
-00012d30: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00012d40: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00012d50: 776f 7264 206e 6f74 2069 6e20 7265 7375  word not in resu
-00012d60: 6c74 2729 0d0a 2020 2020 2020 2020 2020  lt')..          
-00012d70: 2020 7365 675f 6964 2c20 776f 7264 5f69    seg_id, word_i
-00012d80: 6420 3d20 776f 7264 2e73 6567 6d65 6e74  d = word.segment
-00012d90: 5f69 642c 2077 6f72 642e 6964 0d0a 2020  _id, word.id..  
-00012da0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00012db0: 2020 2020 2020 2020 2073 6567 5f69 642c           seg_id,
-00012dc0: 2077 6f72 645f 6964 203d 2077 6f72 640d   word_id = word.
-00012dd0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-00012de0: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
-00012df0: 2020 7072 696e 7428 6627 5265 6d6f 7665    print(f'Remove
-00012e00: 643a 207b 7365 6c66 5b73 6567 5f69 645d  d: {self[seg_id]
-00012e10: 5b77 6f72 645f 6964 5d2e 746f 5f64 6963  [word_id].to_dic
-00012e20: 7428 297d 2729 0d0a 2020 2020 2020 2020  t()}')..        
-00012e30: 6465 6c20 7365 6c66 2e73 6567 6d65 6e74  del self.segment
-00012e40: 735b 7365 675f 6964 5d2e 776f 7264 735b  s[seg_id].words[
-00012e50: 776f 7264 5f69 645d 0d0a 2020 2020 2020  word_id]..      
-00012e60: 2020 6966 206e 6f74 2072 6561 7373 6967    if not reassig
-00012e70: 6e5f 6964 733a 0d0a 2020 2020 2020 2020  n_ids:..        
-00012e80: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
-00012e90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00012ea0: 5b73 6567 5f69 645d 2e68 6173 5f77 6f72  [seg_id].has_wor
-00012eb0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00012ec0: 2073 656c 665b 7365 675f 6964 5d2e 7265   self[seg_id].re
-00012ed0: 6173 7369 676e 5f69 6473 2829 0d0a 2020  assign_ids()..  
-00012ee0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00012ef0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00012f00: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
-00012f10: 6d65 6e74 7328 290d 0a20 2020 2020 2020  ments()..       
-00012f20: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00012f30: 2020 2020 6465 6620 7265 6d6f 7665 5f73      def remove_s
-00012f40: 6567 6d65 6e74 280d 0a20 2020 2020 2020  egment(..       
-00012f50: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00012f60: 2020 2020 2020 2020 7365 676d 656e 743a          segment:
-00012f70: 2055 6e69 6f6e 5b53 6567 6d65 6e74 2c20   Union[Segment, 
-00012f80: 696e 745d 2c0d 0a20 2020 2020 2020 2020  int],..         
-00012f90: 2020 2072 6561 7373 6967 6e5f 6964 733a     reassign_ids:
-00012fa0: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
-00012fb0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
-00012fc0: 7365 3a20 626f 6f6c 203d 2054 7275 650d  se: bool = True.
-00012fd0: 0a20 2020 2029 202d 3e20 2757 6869 7370  .    ) -> 'Whisp
-00012fe0: 6572 5265 7375 6c74 273a 0d0a 2020 2020  erResult':..    
-00012ff0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00013000: 2052 656d 6f76 6520 6120 7365 676d 656e   Remove a segmen
-00013010: 742e 0d0a 0d0a 2020 2020 2020 2020 5061  t.....        Pa
-00013020: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00013030: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-00013040: 2020 2020 2020 7365 676d 656e 7420 3a20        segment : 
-00013050: 5365 676d 656e 7420 6f72 2069 6e74 0d0a  Segment or int..
-00013060: 2020 2020 2020 2020 2020 2020 496e 7374              Inst
-00013070: 616e 6365 203a 636c 6173 733a 6073 7461  ance :class:`sta
-00013080: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
-00013090: 6c74 2e53 6567 6d65 6e74 6020 6f72 2073  lt.Segment` or s
-000130a0: 6567 6d65 6e74 2069 6e64 6578 2e0d 0a20  egment index... 
-000130b0: 2020 2020 2020 2072 6561 7373 6967 6e5f         reassign_
-000130c0: 6964 7320 3a20 626f 6f6c 2c20 6465 6661  ids : bool, defa
-000130d0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-000130e0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-000130f0: 2072 6561 7373 6967 6e20 7365 676d 656e   reassign segmen
-00013100: 7420 4944 7320 2869 6e64 6963 6573 2920  t IDs (indices) 
-00013110: 6166 7465 7220 7265 6d6f 7669 6e67 2060  after removing `
-00013120: 6073 6567 6d65 6e74 6060 2e0d 0a20 2020  `segment``...   
-00013130: 2020 2020 2076 6572 626f 7365 203a 2062       verbose : b
-00013140: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
-00013150: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-00013160: 6865 7468 6572 2074 6f20 7072 696e 7420  hether to print 
-00013170: 6465 7461 696c 206f 6620 7468 6520 7265  detail of the re
-00013180: 6d6f 7665 6420 776f 7264 2e0d 0a0d 0a20  moved word..... 
-00013190: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-000131a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-000131b0: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-000131c0: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-000131d0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-000131e0: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-000131f0: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-00013200: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-00013210: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00013220: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00013230: 7461 6e63 6528 7365 676d 656e 742c 2053  tance(segment, S
-00013240: 6567 6d65 6e74 293a 0d0a 2020 2020 2020  egment):..      
-00013250: 2020 2020 2020 6966 2073 656c 665b 7365        if self[se
-00013260: 676d 656e 742e 6964 5d20 6973 206e 6f74  gment.id] is not
-00013270: 2073 6567 6d65 6e74 3a0d 0a20 2020 2020   segment:..     
-00013280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013290: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 6966 2073 656c 665b 7365 676d 656e 742e  if self[segment.
-000132c0: 6964 5d20 6973 206e 6f74 2073 6567 6d65  id] is not segme
-000132d0: 6e74 3a0d 0a20 2020 2020 2020 2020 2020  nt:..           
-000132e0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000132f0: 616c 7565 4572 726f 7228 2773 6567 6d65  alueError('segme
-00013300: 6e74 206e 6f74 2069 6e20 7265 7375 6c74  nt not in result
-00013310: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00013320: 7365 676d 656e 7420 3d20 7365 676d 656e  segment = segmen
-00013330: 742e 6964 0d0a 2020 2020 2020 2020 6966  t.id..        if
-00013340: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
-00013350: 2020 2020 2020 2070 7269 6e74 2866 2752         print(f'R
-00013360: 656d 6f76 6564 3a20 5b69 643a 7b73 656c  emoved: [id:{sel
-00013370: 665b 7365 676d 656e 745d 2e69 647d 5d20  f[segment].id}] 
-00013380: 7b73 656c 665b 7365 676d 656e 745d 2e74  {self[segment].t
-00013390: 6f5f 6469 7370 6c61 795f 7374 7228 5472  o_display_str(Tr
-000133a0: 7565 297d 2729 0d0a 2020 2020 2020 2020  ue)}')..        
-000133b0: 6465 6c20 7365 6c66 2e73 6567 6d65 6e74  del self.segment
-000133c0: 735b 7365 676d 656e 745d 0d0a 2020 2020  s[segment]..    
-000133d0: 2020 2020 6966 206e 6f74 2072 6561 7373      if not reass
-000133e0: 6967 6e5f 6964 733a 0d0a 2020 2020 2020  ign_ids:..      
-000133f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00013400: 660d 0a20 2020 2020 2020 2073 656c 662e  f..        self.
-00013410: 7265 6173 7369 676e 5f69 6473 2854 7275  reassign_ids(Tru
-00013420: 652c 2073 7461 7274 3d73 6567 6d65 6e74  e, start=segment
-00013430: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00013440: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
-00013450: 6620 7265 6d6f 7665 5f72 6570 6574 6974  f remove_repetit
-00013460: 696f 6e28 0d0a 2020 2020 2020 2020 2020  ion(..          
-00013470: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00013480: 2020 2020 206d 6178 5f77 6f72 6473 3a20       max_words: 
-00013490: 696e 7420 3d20 312c 0d0a 2020 2020 2020  int = 1,..      
-000134a0: 2020 2020 2020 6361 7365 5f73 656e 7369        case_sensi
-000134b0: 7469 7665 3a20 626f 6f6c 203d 2046 616c  tive: bool = Fal
-000134c0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-000134d0: 2073 7472 6970 3a20 626f 6f6c 203d 2054   strip: bool = T
-000134e0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-000134f0: 2020 6967 6e6f 7265 5f70 756e 6374 7561    ignore_punctua
-00013500: 7469 6f6e 733a 2073 7472 203d 2022 5c22  tions: str = "\"
-00013510: 272c 2e3f 2122 2c0d 0a20 2020 2020 2020  ',.?!",..       
-00013520: 2020 2020 2065 7874 656e 645f 6475 7261       extend_dura
-00013530: 7469 6f6e 3a20 626f 6f6c 203d 2054 7275  tion: bool = Tru
-00013540: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00013550: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00013560: 5472 7565 0d0a 2020 2020 2920 2d3e 2027  True..    ) -> '
-00013570: 5768 6973 7065 7252 6573 756c 7427 3a0d  WhisperResult':.
-00013580: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00013590: 2020 2020 2020 5265 6d6f 7665 2077 6f72        Remove wor
-000135a0: 6473 2074 6861 7420 7265 7065 6174 2063  ds that repeat c
-000135b0: 6f6e 7365 6375 7469 7665 6c79 2e0d 0a0d  onsecutively....
-000135c0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000135d0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-000135e0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000135f0: 206d 6178 5f77 6f72 6473 203a 2069 6e74   max_words : int
-00013600: 0d0a 2020 2020 2020 2020 2020 2020 4d61  ..            Ma
-00013610: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-00013620: 776f 7264 7320 746f 206c 6f6f 6b20 666f  words to look fo
-00013630: 7220 636f 6e73 6563 7574 6976 656c 792e  r consecutively.
-00013640: 0d0a 2020 2020 2020 2020 6361 7365 5f73  ..        case_s
-00013650: 656e 7369 7469 7665 203a 2062 6f6f 6c2c  ensitive : bool,
-00013660: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-00013670: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00013680: 6865 7220 7468 6520 6361 7365 206f 6620  her the case of 
-00013690: 776f 7264 7320 6e65 6564 2074 6f20 6d61  words need to ma
-000136a0: 7463 6820 746f 2062 6520 636f 6e73 6964  tch to be consid
-000136b0: 6572 6564 2061 7320 7265 7065 7469 7469  ered as repetiti
-000136c0: 6f6e 2e0d 0a20 2020 2020 2020 2073 7472  on...        str
-000136d0: 6970 203a 2062 6f6f 6c2c 2064 6566 6175  ip : bool, defau
-000136e0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
-000136f0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00013700: 6967 6e6f 7265 2073 7061 6365 7320 6265  ignore spaces be
-00013710: 666f 7265 2061 6e64 2061 6674 6572 2065  fore and after e
-00013720: 6163 6820 776f 7264 2e0d 0a20 2020 2020  ach word...     
-00013730: 2020 2069 676e 6f72 655f 7075 6e63 7475     ignore_punctu
-00013740: 6174 696f 6e73 203a 2062 6f6f 6c2c 2064  ations : bool, d
-00013750: 6566 6175 6c74 2027 2227 2c2e 3f21 270d  efault '"',.?!'.
-00013760: 0a20 2020 2020 2020 2020 2020 2045 6e64  .            End
-00013770: 696e 6720 7075 6e63 7475 6174 696f 6e73  ing punctuations
-00013780: 2074 6f20 6967 6e6f 7265 2e0d 0a20 2020   to ignore...   
-00013790: 2020 2020 2065 7874 656e 645f 6475 7261       extend_dura
-000137a0: 7469 6f6e 3a20 626f 6f6c 2c20 6465 6661  tion: bool, defa
-000137b0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-000137c0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-000137d0: 2065 7874 656e 6420 7468 6520 6475 7261   extend the dura
-000137e0: 7469 6f6e 206f 6620 7468 6520 7072 6576  tion of the prev
-000137f0: 696f 7573 2077 6f72 6420 746f 2063 6f76  ious word to cov
-00013800: 6572 2074 6865 2064 7572 6174 696f 6e20  er the duration 
-00013810: 6f66 2074 6865 2072 6570 6574 6974 696f  of the repetitio
-00013820: 6e2e 0d0a 2020 2020 2020 2020 7665 7262  n...        verb
-00013830: 6f73 653a 2062 6f6f 6c2c 2064 6566 6175  ose: bool, defau
-00013840: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
-00013850: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00013860: 7072 696e 7420 6465 7461 696c 206f 6620  print detail of 
-00013870: 7468 6520 7265 6d6f 7665 6420 7265 7065  the removed repe
-00013880: 7469 7469 6f6e 732e 0d0a 0d0a 2020 2020  titions.....    
-00013890: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-000138a0: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-000138b0: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
-000138c0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
-000138d0: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
-000138e0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
-000138f0: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
-00013900: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
-00013910: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00013920: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00013930: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
-00013940: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00013950: 7365 6c66 0d0a 0d0a 2020 2020 2020 2020  self....        
-00013960: 666f 7220 636f 756e 7420 696e 2072 616e  for count in ran
-00013970: 6765 2831 2c20 6d61 785f 776f 7264 7320  ge(1, max_words 
-00013980: 2b20 3129 3a0d 0a20 2020 2020 2020 2020  + 1):..         
-00013990: 2020 2061 6c6c 5f77 6f72 6473 203d 2073     all_words = s
-000139a0: 656c 662e 616c 6c5f 776f 7264 7328 290d  elf.all_words().
-000139b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000139c0: 6c65 6e28 616c 6c5f 776f 7264 7329 203c  len(all_words) <
-000139d0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-000139e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000139f0: 0d0a 2020 2020 2020 2020 2020 2020 616c  ..            al
-00013a00: 6c5f 776f 7264 735f 7374 7220 3d20 5b77  l_words_str = [w
-00013a10: 2e77 6f72 6420 666f 7220 7720 696e 2061  .word for w in a
-00013a20: 6c6c 5f77 6f72 6473 5d0d 0a20 2020 2020  ll_words]..     
-00013a30: 2020 2020 2020 2069 6620 7374 7269 703a         if strip:
-00013a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013a50: 2020 616c 6c5f 776f 7264 735f 7374 7220    all_words_str 
-00013a60: 3d20 5b77 2e73 7472 6970 2829 2066 6f72  = [w.strip() for
-00013a70: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
-00013a80: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
-00013a90: 2020 6966 2069 676e 6f72 655f 7075 6e63    if ignore_punc
-00013aa0: 7475 6174 696f 6e73 3a0d 0a20 2020 2020  tuations:..     
-00013ab0: 2020 2020 2020 2020 2020 2070 746e 203d             ptn =
-00013ac0: 2066 275b 7b69 676e 6f72 655f 7075 6e63   f'[{ignore_punc
-00013ad0: 7475 6174 696f 6e73 7d5d 2b24 270d 0a20  tuations}]+$'.. 
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00013af0: 6c6c 5f77 6f72 6473 5f73 7472 203d 205b  ll_words_str = [
-00013b00: 7265 2e73 7562 2870 746e 2c20 2727 2c20  re.sub(ptn, '', 
-00013b10: 7729 2066 6f72 2077 2069 6e20 616c 6c5f  w) for w in all_
-00013b20: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
-00013b30: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
-00013b40: 6173 655f 7365 6e73 6974 6976 653a 0d0a  ase_sensitive:..
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 616c 6c5f 776f 7264 735f 7374 7220 3d20  all_words_str = 
-00013b70: 5b77 2e6c 6f77 6572 2829 2066 6f72 2077  [w.lower() for w
-00013b80: 2069 6e20 616c 6c5f 776f 7264 735f 7374   in all_words_st
-00013b90: 725d 0d0a 2020 2020 2020 2020 2020 2020  r]..            
-00013ba0: 6e65 7874 5f69 203d 204e 6f6e 650d 0a20  next_i = None.. 
-00013bb0: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
-00013bc0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-00013bd0: 2020 2020 2066 6f72 2069 2069 6e20 7265       for i in re
-00013be0: 7665 7273 6564 2872 616e 6765 2863 6f75  versed(range(cou
-00013bf0: 6e74 2a32 2c20 6c65 6e28 616c 6c5f 776f  nt*2, len(all_wo
-00013c00: 7264 735f 7374 7229 2b31 2929 3a0d 0a20  rds_str)+1)):.. 
-00013c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013c20: 6620 6e65 7874 5f69 2069 7320 6e6f 7420  f next_i is not 
-00013c30: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00013c40: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
-00013c50: 7874 5f69 2021 3d20 693a 0d0a 2020 2020  xt_i != i:..    
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c90: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 206e 6578 745f 6920 3d20 4e6f 6e65 0d0a   next_i = None..
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 7320 3d20 6920 2d20 636f 756e 740d 0a20  s = i - count.. 
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013cf0: 6620 616c 6c5f 776f 7264 735f 7374 725b  f all_words_str[
-00013d00: 7320 2d20 636f 756e 743a 735d 2021 3d20  s - count:s] != 
-00013d10: 616c 6c5f 776f 7264 735f 7374 725b 733a  all_words_str[s:
-00013d20: 695d 3a0d 0a20 2020 2020 2020 2020 2020  i]:..           
-00013d30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00013d40: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00013d50: 2020 206e 6578 745f 6920 3d20 730d 0a20     next_i = s.. 
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013d70: 6620 6578 7465 6e64 5f64 7572 6174 696f  f extend_duratio
-00013d80: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-00013d90: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-00013da0: 735b 732d 315d 2e65 6e64 203d 2061 6c6c  s[s-1].end = all
-00013db0: 5f77 6f72 6473 5b69 2d31 5d2e 656e 640d  _words[i-1].end.
-00013dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013dd0: 2074 656d 705f 6368 616e 6765 7320 3d20   temp_changes = 
-00013de0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013df0: 2020 2020 666f 7220 6a20 696e 2072 6576      for j in rev
-00013e00: 6572 7365 6428 7261 6e67 6528 732c 2069  ersed(range(s, i
-00013e10: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00013e20: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
-00013e30: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
-00013e40: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00013e50: 6d70 5f63 6861 6e67 6573 2e61 7070 656e  mp_changes.appen
-00013e60: 6428 6627 2d20 7b61 6c6c 5f77 6f72 6473  d(f'- {all_words
-00013e70: 5b6a 5d2e 746f 5f64 6963 7428 297d 2729  [j].to_dict()}')
-00013e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013e90: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
-00013ea0: 655f 776f 7264 2861 6c6c 5f77 6f72 6473  e_word(all_words
-00013eb0: 5b6a 5d2c 2046 616c 7365 2c20 7665 7262  [j], False, verb
-00013ec0: 6f73 653d 4661 6c73 6529 0d0a 2020 2020  ose=False)..    
-00013ed0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00013ee0: 656d 705f 6368 616e 6765 733a 0d0a 2020  emp_changes:..  
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2020 6368 616e 6765 732e 6170 7065 6e64    changes.append
-00013f10: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00013f20: 2020 2020 2020 2020 2020 2066 2752 656d             f'Rem
-00013f30: 6f76 653a 205b 7b66 6f72 6d61 745f 7469  ove: [{format_ti
-00013f40: 6d65 7374 616d 7028 616c 6c5f 776f 7264  mestamp(all_word
-00013f50: 735b 735d 2e73 7461 7274 297d 202d 3e20  s[s].start)} -> 
-00013f60: 7b66 6f72 6d61 745f 7469 6d65 7374 616d  {format_timestam
-00013f70: 7028 616c 6c5f 776f 7264 735b 692d 315d  p(all_words[i-1]
-00013f80: 2e65 6e64 297d 5d20 270d 0a20 2020 2020  .end)}] '..     
-00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 202b 2027 272e 6a6f 696e 285f 772e     + ''.join(_w.
-00013fb0: 776f 7264 2066 6f72 205f 7720 696e 2061  word for _w in a
-00013fc0: 6c6c 5f77 6f72 6473 5b73 3a69 5d29 202b  ll_words[s:i]) +
-00013fd0: 2027 5c6e 270d 0a20 2020 2020 2020 2020   '\n'..         
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00013ff0: 2027 5c6e 272e 6a6f 696e 2872 6576 6572   '\n'.join(rever
-00014000: 7365 6428 7465 6d70 5f63 6861 6e67 6573  sed(temp_changes
-00014010: 2929 202b 2027 5c6e 270d 0a20 2020 2020  )) + '\n'..     
-00014020: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00014030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014040: 2020 666f 7220 6930 2c20 6931 2069 6e20    for i0, i1 in 
-00014050: 7a69 7028 7261 6e67 6528 7320 2d20 636f  zip(range(s - co
-00014060: 756e 742c 2073 292c 2072 616e 6765 2873  unt, s), range(s
-00014070: 2c20 6929 293a 0d0a 2020 2020 2020 2020  , i)):..        
-00014080: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00014090: 656e 2861 6c6c 5f77 6f72 6473 5b69 305d  en(all_words[i0]
-000140a0: 2e77 6f72 6429 203c 206c 656e 2861 6c6c  .word) < len(all
-000140b0: 5f77 6f72 6473 5b69 315d 2e77 6f72 6429  _words[i1].word)
-000140c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000140d0: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
-000140e0: 6f72 6473 5b69 315d 2e73 7461 7274 203d  ords[i1].start =
-000140f0: 2061 6c6c 5f77 6f72 6473 5b69 305d 2e73   all_words[i0].s
-00014100: 7461 7274 0d0a 2020 2020 2020 2020 2020  tart..          
-00014110: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00014120: 6c5f 776f 7264 735b 6931 5d2e 656e 6420  l_words[i1].end 
-00014130: 3d20 616c 6c5f 776f 7264 735b 6930 5d2e  = all_words[i0].
-00014140: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-00014150: 2020 2020 2020 2020 2020 2020 205f 7369               _si
-00014160: 642c 205f 7769 6420 3d20 616c 6c5f 776f  d, _wid = all_wo
-00014170: 7264 735b 6930 5d2e 7365 676d 656e 745f  rds[i0].segment_
-00014180: 6964 2c20 616c 6c5f 776f 7264 735b 6930  id, all_words[i0
-00014190: 5d2e 6964 0d0a 2020 2020 2020 2020 2020  ].id..          
-000141a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000141b0: 6c66 2e73 6567 6d65 6e74 735b 5f73 6964  lf.segments[_sid
-000141c0: 5d2e 776f 7264 735b 5f77 6964 5d20 3d20  ].words[_wid] = 
-000141d0: 616c 6c5f 776f 7264 735b 6931 5d0d 0a0d  all_words[i1]...
-000141e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000141f0: 6368 616e 6765 733a 0d0a 2020 2020 2020  changes:..      
-00014200: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00014210: 275c 6e27 2e6a 6f69 6e28 7265 7665 7273  '\n'.join(revers
-00014220: 6564 2863 6861 6e67 6573 2929 290d 0a0d  ed(changes)))...
-00014230: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014240: 662e 7265 6d6f 7665 5f6e 6f5f 776f 7264  f.remove_no_word
-00014250: 5f73 6567 6d65 6e74 7328 7265 6173 7369  _segments(reassi
-00014260: 676e 5f69 6473 3d46 616c 7365 290d 0a20  gn_ids=False).. 
-00014270: 2020 2020 2020 2073 656c 662e 7265 6173         self.reas
-00014280: 7369 676e 5f69 6473 2829 0d0a 0d0a 2020  sign_ids()....  
-00014290: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000142a0: 660d 0a0d 0a20 2020 2064 6566 2072 656d  f....    def rem
-000142b0: 6f76 655f 776f 7264 735f 6279 5f73 7472  ove_words_by_str
-000142c0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-000142d0: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-000142e0: 2020 776f 7264 733a 2055 6e69 6f6e 5b73    words: Union[s
-000142f0: 7472 2c20 4c69 7374 5b73 7472 5d2c 204e  tr, List[str], N
-00014300: 6f6e 655d 2c0d 0a20 2020 2020 2020 2020  one],..         
-00014310: 2020 2063 6173 655f 7365 6e73 6974 6976     case_sensitiv
-00014320: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
-00014330: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00014340: 7269 703a 2062 6f6f 6c20 3d20 5472 7565  rip: bool = True
-00014350: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-00014360: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
-00014370: 6e73 3a20 7374 7220 3d20 225c 2227 2c2e  ns: str = "\"',.
-00014380: 3f21 222c 0d0a 2020 2020 2020 2020 2020  ?!",..          
-00014390: 2020 6d69 6e5f 7072 6f62 3a20 666c 6f61    min_prob: floa
-000143a0: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
-000143b0: 2020 2020 2020 2066 696c 7465 7273 3a20         filters: 
-000143c0: 4361 6c6c 6162 6c65 203d 204e 6f6e 652c  Callable = None,
-000143d0: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-000143e0: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
-000143f0: 7565 0d0a 2020 2020 2920 2d3e 2027 5768  ue..    ) -> 'Wh
-00014400: 6973 7065 7252 6573 756c 7427 3a0d 0a20  isperResult':.. 
-00014410: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00014420: 2020 2020 5265 6d6f 7665 2077 6f72 6473      Remove words
-00014430: 2074 6861 7420 6d61 7463 6820 6060 776f   that match ``wo
-00014440: 7264 7360 602e 0d0a 0d0a 2020 2020 2020  rds``.....      
-00014450: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00014460: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00014470: 0d0a 2020 2020 2020 2020 776f 7264 7320  ..        words 
-00014480: 3a20 7374 7220 6f72 206c 6973 7420 6f66  : str or list of
-00014490: 2073 7472 206f 7220 4e6f 6e65 0d0a 2020   str or None..  
-000144a0: 2020 2020 2020 2020 2020 4120 776f 7264            A word
-000144b0: 206f 7220 6c69 7374 206f 6620 776f 7264   or list of word
-000144c0: 7320 746f 2072 656d 6f76 652e 6060 4e6f  s to remove.``No
-000144d0: 6e65 6060 2066 6f72 2061 6c6c 2077 6f72  ne`` for all wor
-000144e0: 6473 2074 6f20 6265 2070 6173 7365 6420  ds to be passed 
-000144f0: 696e 746f 2060 6066 696c 7465 7273 6060  into ``filters``
-00014500: 2e0d 0a20 2020 2020 2020 2063 6173 655f  ...        case_
-00014510: 7365 6e73 6974 6976 6520 3a20 626f 6f6c  sensitive : bool
-00014520: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
-00014530: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-00014540: 7468 6572 2074 6865 2063 6173 6520 6f66  ther the case of
-00014550: 2077 6f72 6473 206e 6565 6420 746f 206d   words need to m
-00014560: 6174 6368 2074 6f20 6265 2063 6f6e 7369  atch to be consi
-00014570: 6465 7265 6420 6173 2072 6570 6574 6974  dered as repetit
-00014580: 696f 6e2e 0d0a 2020 2020 2020 2020 7374  ion...        st
-00014590: 7269 7020 3a20 626f 6f6c 2c20 6465 6661  rip : bool, defa
-000145a0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-000145b0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-000145c0: 2069 676e 6f72 6520 7370 6163 6573 2062   ignore spaces b
-000145d0: 6566 6f72 6520 616e 6420 6166 7465 7220  efore and after 
-000145e0: 6561 6368 2077 6f72 642e 0d0a 2020 2020  each word...    
-000145f0: 2020 2020 6967 6e6f 7265 5f70 756e 6374      ignore_punct
-00014600: 7561 7469 6f6e 7320 3a20 626f 6f6c 2c20  uations : bool, 
-00014610: 6465 6661 756c 7420 2722 272c 2e3f 2127  default '"',.?!'
-00014620: 0d0a 2020 2020 2020 2020 2020 2020 456e  ..            En
-00014630: 6469 6e67 2070 756e 6374 7561 7469 6f6e  ding punctuation
-00014640: 7320 746f 2069 676e 6f72 652e 0d0a 2020  s to ignore...  
-00014650: 2020 2020 2020 6d69 6e5f 7072 6f62 203a        min_prob :
-00014660: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00014670: 0d0a 2020 2020 2020 2020 2020 2020 4163  ..            Ac
-00014680: 7473 2061 7320 7468 6520 6669 7273 7420  ts as the first 
-00014690: 6669 6c74 6572 2074 6865 2066 6f72 2074  filter the for t
-000146a0: 6865 2077 6f72 6473 2074 6861 7420 6d61  he words that ma
-000146b0: 7463 6820 6060 776f 7264 7360 602e 2057  tch ``words``. W
-000146c0: 6f72 6473 2077 6974 6820 7072 6f62 6162  ords with probab
-000146d0: 696c 6974 7920 3c20 6060 6d69 6e5f 7072  ility < ``min_pr
-000146e0: 6f62 6060 2077 696c 6c0d 0a20 2020 2020  ob`` will..     
-000146f0: 2020 2020 2020 2062 6520 7265 6d6f 7665         be remove
-00014700: 6420 6966 2060 6066 696c 7465 7273 6060  d if ``filters``
-00014710: 2069 7320 6060 4e6f 6e65 6060 2c20 656c   is ``None``, el
-00014720: 7365 2070 6173 7320 7468 6520 776f 7264  se pass the word
-00014730: 7320 696e 746f 2060 6066 696c 7465 7273  s into ``filters
-00014740: 6060 2e20 576f 7264 7320 7769 7468 6f75  ``. Words withou
-00014750: 7420 7072 6f62 6162 696c 6974 7920 7769  t probability wi
-00014760: 6c6c 0d0a 2020 2020 2020 2020 2020 2020  ll..            
-00014770: 6265 2074 7265 6174 6564 2061 7320 6861  be treated as ha
-00014780: 7669 6e67 2070 726f 6261 6269 6c69 7479  ving probability
-00014790: 203c 2060 606d 696e 5f70 726f 6260 602e   < ``min_prob``.
-000147a0: 0d0a 2020 2020 2020 2020 6669 6c74 6572  ..        filter
-000147b0: 7320 3a20 4361 6c6c 6162 6c65 2c20 6f70  s : Callable, op
-000147c0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-000147d0: 2020 2020 4120 6675 6e63 7469 6f6e 2074      A function t
-000147e0: 6861 7420 7461 6b65 7320 616e 2069 6e73  hat takes an ins
-000147f0: 7461 6e63 6520 6f66 203a 636c 6173 733a  tance of :class:
-00014800: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
-00014810: 7265 7375 6c74 2e57 6f72 6454 696d 696e  result.WordTimin
-00014820: 6760 2061 7320 6974 7320 6f6e 6c79 2061  g` as its only a
-00014830: 7267 756d 656e 742e 0d0a 2020 2020 2020  rgument...      
-00014840: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00014850: 696f 6e20 6973 2063 7573 746f 6d20 6669  ion is custom fi
-00014860: 6c74 6572 2066 6f72 2074 6865 2077 6f72  lter for the wor
-00014870: 6473 2074 6861 7420 6d61 7463 6820 6060  ds that match ``
-00014880: 776f 7264 7360 6020 616e 6420 7765 7265  words`` and were
-00014890: 206e 6f74 2063 6175 6768 7420 6279 2060   not caught by `
-000148a0: 606d 696e 5f70 726f 6260 602e 0d0a 2020  `min_prob``...  
-000148b0: 2020 2020 2020 7665 7262 6f73 653a 0d0a        verbose:..
-000148c0: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-000148d0: 6865 7220 746f 2070 7269 6e74 2064 6574  her to print det
-000148e0: 6169 6c20 6f66 2074 6865 2072 656d 6f76  ail of the remov
-000148f0: 6564 2077 6f72 6473 2e0d 0a0d 0a20 2020  ed words.....   
-00014900: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-00014910: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-00014920: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
-00014930: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
-00014940: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
-00014950: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
-00014960: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
-00014970: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
-00014980: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00014990: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-000149a0: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
-000149b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000149c0: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
-000149d0: 6620 6973 696e 7374 616e 6365 2877 6f72  f isinstance(wor
-000149e0: 6473 2c20 7374 7229 3a0d 0a20 2020 2020  ds, str):..     
-000149f0: 2020 2020 2020 2077 6f72 6473 203d 205b         words = [
-00014a00: 776f 7264 735d 0d0a 2020 2020 2020 2020  words]..        
-00014a10: 616c 6c5f 776f 7264 7320 3d20 7365 6c66  all_words = self
-00014a20: 2e61 6c6c 5f77 6f72 6473 2829 0d0a 2020  .all_words()..  
-00014a30: 2020 2020 2020 616c 6c5f 776f 7264 735f        all_words_
-00014a40: 7374 7220 3d20 5b77 2e77 6f72 6420 666f  str = [w.word fo
-00014a50: 7220 7720 696e 2061 6c6c 5f77 6f72 6473  r w in all_words
-00014a60: 5d0d 0a20 2020 2020 2020 2069 6620 7374  ]..        if st
-00014a70: 7269 703a 0d0a 2020 2020 2020 2020 2020  rip:..          
-00014a80: 2020 616c 6c5f 776f 7264 735f 7374 7220    all_words_str 
-00014a90: 3d20 5b77 2e73 7472 6970 2829 2066 6f72  = [w.strip() for
-00014aa0: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
-00014ab0: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
-00014ac0: 2020 776f 7264 7320 3d20 5b77 2e73 7472    words = [w.str
-00014ad0: 6970 2829 2066 6f72 2077 2069 6e20 776f  ip() for w in wo
-00014ae0: 7264 735d 0d0a 2020 2020 2020 2020 6966  rds]..        if
-00014af0: 2069 676e 6f72 655f 7075 6e63 7475 6174   ignore_punctuat
-00014b00: 696f 6e73 3a0d 0a20 2020 2020 2020 2020  ions:..         
-00014b10: 2020 2070 746e 203d 2066 275b 7b69 676e     ptn = f'[{ign
-00014b20: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
-00014b30: 7d5d 2b24 270d 0a20 2020 2020 2020 2020  }]+$'..         
-00014b40: 2020 2061 6c6c 5f77 6f72 6473 5f73 7472     all_words_str
-00014b50: 203d 205b 7265 2e73 7562 2870 746e 2c20   = [re.sub(ptn, 
-00014b60: 2727 2c20 7729 2066 6f72 2077 2069 6e20  '', w) for w in 
-00014b70: 616c 6c5f 776f 7264 735f 7374 725d 0d0a  all_words_str]..
-00014b80: 2020 2020 2020 2020 2020 2020 776f 7264              word
-00014b90: 7320 3d20 5b72 652e 7375 6228 7074 6e2c  s = [re.sub(ptn,
-00014ba0: 2027 272c 2077 2920 666f 7220 7720 696e   '', w) for w in
-00014bb0: 2077 6f72 6473 5d0d 0a20 2020 2020 2020   words]..       
-00014bc0: 2069 6620 6e6f 7420 6361 7365 5f73 656e   if not case_sen
-00014bd0: 7369 7469 7665 3a0d 0a20 2020 2020 2020  sitive:..       
-00014be0: 2020 2020 2061 6c6c 5f77 6f72 6473 5f73       all_words_s
-00014bf0: 7472 203d 205b 772e 6c6f 7765 7228 2920  tr = [w.lower() 
-00014c00: 666f 7220 7720 696e 2061 6c6c 5f77 6f72  for w in all_wor
-00014c10: 6473 5f73 7472 5d0d 0a20 2020 2020 2020  ds_str]..       
-00014c20: 2020 2020 2077 6f72 6473 203d 205b 772e       words = [w.
-00014c30: 6c6f 7765 7228 2920 666f 7220 7720 696e  lower() for w in
-00014c40: 2077 6f72 6473 5d0d 0a0d 0a20 2020 2020   words]....     
-00014c50: 2020 2063 6861 6e67 6573 203d 205b 5d0d     changes = [].
-00014c60: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00014c70: 7720 696e 2072 6576 6572 7365 6428 6c69  w in reversed(li
-00014c80: 7374 2865 6e75 6d65 7261 7465 2861 6c6c  st(enumerate(all
-00014c90: 5f77 6f72 6473 5f73 7472 2929 293a 0d0a  _words_str))):..
-00014ca0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00014cb0: 6f74 2028 776f 7264 7320 6973 204e 6f6e  ot (words is Non
-00014cc0: 6520 6f72 2061 6e79 2877 203d 3d20 5f77  e or any(w == _w
-00014cd0: 2066 6f72 205f 7720 696e 2077 6f72 6473   for _w in words
-00014ce0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00014cf0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00014d00: 2020 2020 2020 2020 2020 2069 6620 280d             if (.
-00014d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014d20: 2020 2020 2028 6d69 6e5f 7072 6f62 2069       (min_prob i
-00014d30: 7320 4e6f 6e65 206f 7220 616c 6c5f 776f  s None or all_wo
-00014d40: 7264 735b 695d 2e70 726f 6261 6269 6c69  rds[i].probabili
-00014d50: 7479 2069 7320 4e6f 6e65 206f 7220 6d69  ty is None or mi
-00014d60: 6e5f 7072 6f62 203e 2061 6c6c 5f77 6f72  n_prob > all_wor
-00014d70: 6473 5b69 5d2e 7072 6f62 6162 696c 6974  ds[i].probabilit
-00014d80: 7929 2061 6e64 0d0a 2020 2020 2020 2020  y) and..        
-00014d90: 2020 2020 2020 2020 2020 2020 2866 696c              (fil
-00014da0: 7465 7273 2069 7320 4e6f 6e65 206f 7220  ters is None or 
-00014db0: 6669 6c74 6572 7328 616c 6c5f 776f 7264  filters(all_word
-00014dc0: 735b 695d 2929 0d0a 2020 2020 2020 2020  s[i]))..        
-00014dd0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-00014de0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-00014df0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00014e00: 2020 2020 2020 2020 2063 6861 6e67 6573           changes
-00014e10: 2e61 7070 656e 6428 6627 5265 6d6f 7665  .append(f'Remove
-00014e20: 643a 207b 616c 6c5f 776f 7264 735b 695d  d: {all_words[i]
-00014e30: 2e74 6f5f 6469 6374 2829 7d27 290d 0a20  .to_dict()}').. 
-00014e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014e50: 656c 662e 7265 6d6f 7665 5f77 6f72 6428  elf.remove_word(
-00014e60: 616c 6c5f 776f 7264 735b 695d 2c20 4661  all_words[i], Fa
-00014e70: 6c73 652c 2076 6572 626f 7365 3d46 616c  lse, verbose=Fal
-00014e80: 7365 290d 0a20 2020 2020 2020 2069 6620  se)..        if 
-00014e90: 6368 616e 6765 733a 0d0a 2020 2020 2020  changes:..      
-00014ea0: 2020 2020 2020 7072 696e 7428 275c 6e27        print('\n'
-00014eb0: 2e6a 6f69 6e28 7265 7665 7273 6564 2863  .join(reversed(c
-00014ec0: 6861 6e67 6573 2929 290d 0a20 2020 2020  hanges)))..     
-00014ed0: 2020 2073 656c 662e 7265 6d6f 7665 5f6e     self.remove_n
-00014ee0: 6f5f 776f 7264 5f73 6567 6d65 6e74 7328  o_word_segments(
-00014ef0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-00014f00: 7572 6e20 7365 6c66 0d0a 0d0a 2020 2020  urn self....    
-00014f10: 6465 6620 6669 6c6c 5f69 6e5f 6761 7073  def fill_in_gaps
-00014f20: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
-00014f30: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-00014f40: 2020 6f74 6865 725f 7265 7375 6c74 3a20    other_result: 
-00014f50: 556e 696f 6e5b 2757 6869 7370 6572 5265  Union['WhisperRe
-00014f60: 7375 6c74 272c 2073 7472 5d2c 0d0a 2020  sult', str],..  
-00014f70: 2020 2020 2020 2020 2020 6d69 6e5f 6761            min_ga
-00014f80: 703a 2066 6c6f 6174 203d 2030 2e31 2c0d  p: float = 0.1,.
-00014f90: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
-00014fa0: 655f 7365 6e73 6974 6976 653a 2062 6f6f  e_sensitive: boo
-00014fb0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00014fc0: 2020 2020 2020 2020 7374 7269 703a 2062          strip: b
-00014fd0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
-00014fe0: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
-00014ff0: 7075 6e63 7475 6174 696f 6e73 3a20 7374  punctuations: st
-00015000: 7220 3d20 225c 2227 2c2e 3f21 222c 0d0a  r = "\"',.?!",..
-00015010: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00015020: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
-00015030: 0d0a 2020 2020 2920 2d3e 2027 5768 6973  ..    ) -> 'Whis
-00015040: 7065 7252 6573 756c 7427 3a0d 0a20 2020  perResult':..   
-00015050: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00015060: 2020 4669 6c6c 2069 6e20 7365 676d 656e    Fill in segmen
-00015070: 7420 6761 7073 206c 6172 6765 7220 7468  t gaps larger th
-00015080: 616e 2060 606d 696e 5f67 6170 6060 2077  an ``min_gap`` w
-00015090: 6974 6820 636f 6e74 656e 7420 6672 6f6d  ith content from
-000150a0: 2060 606f 7468 6572 5f72 6573 756c 7460   ``other_result`
-000150b0: 6020 6174 2074 6865 2074 696d 6573 206f  ` at the times o
-000150c0: 6620 6761 7073 2e0d 0a0d 0a20 2020 2020  f gaps.....     
-000150d0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-000150e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000150f0: 2d0d 0a20 2020 2020 2020 206f 7468 6572  -..        other
-00015100: 5f72 6573 756c 7420 3a20 5768 6973 7065  _result : Whispe
-00015110: 7252 6573 756c 7420 6f72 2073 7472 0d0a  rResult or str..
-00015120: 2020 2020 2020 2020 2020 2020 416e 6f74              Anot
-00015130: 6865 7220 7472 616e 7363 7269 7074 696f  her transcriptio
-00015140: 6e20 7265 7375 6c74 2061 7320 616e 2069  n result as an i
-00015150: 6e73 7461 6e63 6520 6f66 203a 636c 6173  nstance of :clas
-00015160: 733a 6073 7461 626c 655f 7768 6973 7065  s:`stable_whispe
-00015170: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-00015180: 5265 7375 6c74 6020 6f72 2070 6174 6820  Result` or path 
-00015190: 746f 2074 6865 0d0a 2020 2020 2020 2020  to the..        
-000151a0: 2020 2020 4a53 4f4e 206f 6620 7468 6520      JSON of the 
-000151b0: 7265 7375 6c74 2e0d 0a20 2020 2020 2020  result...       
-000151c0: 206d 696e 5f67 6170 203a 2066 6c6f 6174   min_gap : float
-000151d0: 2c20 6465 6661 756c 7420 302e 310d 0a20  , default 0.1.. 
-000151e0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-000151f0: 696e 696d 756d 2073 6563 6f6e 6473 206f  inimum seconds o
-00015200: 6620 6120 6761 7020 6265 7477 6565 6e20  f a gap between 
-00015210: 7365 676d 656e 7473 2074 6861 7420 6d75  segments that mu
-00015220: 7374 2062 6520 6578 6365 6564 6564 2074  st be exceeded t
-00015230: 6f20 6265 2066 696c 6c65 6420 696e 2e0d  o be filled in..
-00015240: 0a20 2020 2020 2020 2063 6173 655f 7365  .        case_se
-00015250: 6e73 6974 6976 6520 3a20 626f 6f6c 2c20  nsitive : bool, 
-00015260: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
-00015270: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-00015280: 6572 2074 6f20 636f 6e73 6964 6572 2074  er to consider t
-00015290: 6865 2063 6173 6520 6f66 2074 6865 2066  he case of the f
-000152a0: 6972 7374 2061 6e64 206c 6173 7420 776f  irst and last wo
-000152b0: 7264 206f 6620 7468 6520 6761 7020 746f  rd of the gap to
-000152c0: 2064 6574 6572 6d69 6e65 206f 7665 726c   determine overl
-000152d0: 6170 7069 6e67 2077 6f72 6473 2074 6f20  apping words to 
-000152e0: 7265 6d6f 7665 0d0a 2020 2020 2020 2020  remove..        
-000152f0: 2020 2020 6265 666f 7265 2066 696c 6c69      before filli
-00015300: 6e67 2069 6e2e 0d0a 2020 2020 2020 2020  ng in...        
-00015310: 7374 7269 7020 3a20 626f 6f6c 2c20 6465  strip : bool, de
-00015320: 6661 756c 7420 5472 7565 0d0a 2020 2020  fault True..    
-00015330: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00015340: 746f 2069 676e 6f72 6520 7370 6163 6573  to ignore spaces
-00015350: 2062 6566 6f72 6520 616e 6420 6166 7465   before and afte
-00015360: 7220 7468 6520 6669 7273 7420 616e 6420  r the first and 
-00015370: 6c61 7374 2077 6f72 6420 6f66 2074 6865  last word of the
-00015380: 2067 6170 2074 6f20 6465 7465 726d 696e   gap to determin
-00015390: 6520 6f76 6572 6c61 7070 696e 6720 776f  e overlapping wo
-000153a0: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
-000153b0: 2074 6f20 7265 6d6f 7665 2062 6566 6f72   to remove befor
-000153c0: 6520 6669 6c6c 696e 6720 696e 2e0d 0a20  e filling in... 
-000153d0: 2020 2020 2020 2069 676e 6f72 655f 7075         ignore_pu
-000153e0: 6e63 7475 6174 696f 6e73 203a 2062 6f6f  nctuations : boo
-000153f0: 6c2c 2064 6566 6175 6c74 2027 2227 2c2e  l, default '"',.
-00015400: 3f21 270d 0a20 2020 2020 2020 2020 2020  ?!'..           
-00015410: 2045 6e64 696e 6720 7075 6e63 7475 6174   Ending punctuat
-00015420: 696f 6e73 2074 6f20 6967 6e6f 7265 2069  ions to ignore i
-00015430: 6e20 7468 6520 6669 7273 7420 616e 6420  n the first and 
-00015440: 6c61 7374 2077 6f72 6420 6f66 2074 6865  last word of the
-00015450: 2067 6170 2074 6f20 6465 7465 726d 696e   gap to determin
-00015460: 6520 6f76 6572 6c61 7070 696e 6720 776f  e overlapping wo
-00015470: 7264 7320 746f 0d0a 2020 2020 2020 2020  rds to..        
-00015480: 2020 2020 7265 6d6f 7665 2062 6566 6f72      remove befor
-00015490: 6520 6669 6c6c 696e 6720 696e 2e0d 0a20  e filling in... 
-000154a0: 2020 2020 2020 2076 6572 626f 7365 3a0d         verbose:.
-000154b0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-000154c0: 7468 6572 2074 6f20 7072 696e 7420 6465  ther to print de
-000154d0: 7461 696c 206f 6620 7468 6520 6669 6c6c  tail of the fill
-000154e0: 6564 2063 6f6e 7465 6e74 2e0d 0a0d 0a20  ed content..... 
-000154f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-00015500: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-00015510: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-00015520: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-00015530: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-00015540: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-00015550: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-00015560: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-00015570: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00015580: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-00015590: 656c 662e 7365 676d 656e 7473 2920 3c20  elf.segments) < 
-000155a0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-000155b0: 7265 7475 726e 2073 656c 660d 0a20 2020  return self..   
-000155c0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000155d0: 6365 286f 7468 6572 5f72 6573 756c 742c  ce(other_result,
-000155e0: 2073 7472 293a 0d0a 2020 2020 2020 2020   str):..        
-000155f0: 2020 2020 6f74 6865 725f 7265 7375 6c74      other_result
-00015600: 203d 2057 6869 7370 6572 5265 7375 6c74   = WhisperResult
-00015610: 286f 7468 6572 5f72 6573 756c 7429 0d0a  (other_result)..
-00015620: 0d0a 2020 2020 2020 2020 6966 2073 7472  ..        if str
-00015630: 6970 3a0d 0a20 2020 2020 2020 2020 2020  ip:..           
-00015640: 2064 6566 2073 7472 6970 5f73 7061 6365   def strip_space
-00015650: 2877 293a 0d0a 2020 2020 2020 2020 2020  (w):..          
-00015660: 2020 2020 2020 7265 7475 726e 2077 2e73        return w.s
-00015670: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
-00015680: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00015690: 2020 2064 6566 2073 7472 6970 5f73 7061     def strip_spa
-000156a0: 6365 2877 293a 0d0a 2020 2020 2020 2020  ce(w):..        
-000156b0: 2020 2020 2020 2020 7265 7475 726e 2077          return w
-000156c0: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
-000156d0: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
-000156e0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-000156f0: 2070 746e 203d 2066 275b 7b69 676e 6f72   ptn = f'[{ignor
-00015700: 655f 7075 6e63 7475 6174 696f 6e73 7d5d  e_punctuations}]
-00015710: 2b24 270d 0a0d 0a20 2020 2020 2020 2020  +$'....         
-00015720: 2020 2064 6566 2073 7472 6970 5f70 756e     def strip_pun
-00015730: 6374 7561 7469 6f6e 7328 7729 3a0d 0a20  ctuations(w):.. 
-00015740: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00015750: 6574 7572 6e20 7265 2e73 7562 2870 746e  eturn re.sub(ptn
-00015760: 2c20 2727 2c20 7374 7269 705f 7370 6163  , '', strip_spac
-00015770: 6528 7729 290d 0a20 2020 2020 2020 2065  e(w))..        e
-00015780: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00015790: 2020 7374 7269 705f 7075 6e63 7475 6174    strip_punctuat
-000157a0: 696f 6e73 203d 2073 7472 6970 5f73 7061  ions = strip_spa
-000157b0: 6365 0d0a 0d0a 2020 2020 2020 2020 6966  ce....        if
-000157c0: 2063 6173 655f 7365 6e73 6974 6976 653a   case_sensitive:
-000157d0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000157e0: 7269 7020 3d20 7374 7269 705f 7075 6e63  rip = strip_punc
-000157f0: 7475 6174 696f 6e73 0d0a 2020 2020 2020  tuations..      
-00015800: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00015810: 2020 2020 2064 6566 2073 7472 6970 2877       def strip(w
-00015820: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00015830: 2020 2020 7265 7475 726e 2073 7472 6970      return strip
-00015840: 5f70 756e 6374 7561 7469 6f6e 7328 7729  _punctuations(w)
-00015850: 2e6c 6f77 6572 2829 0d0a 0d0a 2020 2020  .lower()....    
-00015860: 2020 2020 7365 675f 7061 6972 7320 3d20      seg_pairs = 
-00015870: 6c69 7374 2865 6e75 6d65 7261 7465 287a  list(enumerate(z
-00015880: 6970 2873 656c 662e 7365 676d 656e 7473  ip(self.segments
-00015890: 5b3a 2d31 5d2c 2073 656c 662e 7365 676d  [:-1], self.segm
-000158a0: 656e 7473 5b31 3a5d 2929 290d 0a20 2020  ents[1:])))..   
-000158b0: 2020 2020 2073 6567 5f70 6169 7273 2e69       seg_pairs.i
-000158c0: 6e73 6572 7428 302c 2028 2d31 2c20 284e  nsert(0, (-1, (N
-000158d0: 6f6e 652c 2073 656c 662e 7365 676d 656e  one, self.segmen
-000158e0: 7473 5b30 5d29 2929 0d0a 2020 2020 2020  ts[0])))..      
-000158f0: 2020 7365 675f 7061 6972 732e 6170 7065    seg_pairs.appe
-00015900: 6e64 2828 7365 675f 7061 6972 735b 2d31  nd((seg_pairs[-1
-00015910: 5d5b 305d 2b31 2c20 2873 656c 662e 7365  ][0]+1, (self.se
-00015920: 676d 656e 7473 5b2d 315d 2c20 4e6f 6e65  gments[-1], None
-00015930: 2929 290d 0a0d 0a20 2020 2020 2020 2063  )))....        c
-00015940: 6861 6e67 6573 203d 205b 5d0d 0a20 2020  hanges = []..   
-00015950: 2020 2020 2066 6f72 2069 2c20 2873 6567       for i, (seg
-00015960: 302c 2073 6567 3129 2069 6e20 7265 7665  0, seg1) in reve
-00015970: 7273 6564 2873 6567 5f70 6169 7273 293a  rsed(seg_pairs):
-00015980: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-00015990: 7273 745f 776f 7264 203d 204e 6f6e 6520  rst_word = None 
-000159a0: 6966 2073 6567 3020 6973 204e 6f6e 6520  if seg0 is None 
-000159b0: 656c 7365 2073 6567 302e 776f 7264 735b  else seg0.words[
-000159c0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
-000159d0: 206c 6173 745f 776f 7264 203d 204e 6f6e   last_word = Non
-000159e0: 6520 6966 2073 6567 3120 6973 204e 6f6e  e if seg1 is Non
-000159f0: 6520 656c 7365 2073 6567 312e 776f 7264  e else seg1.word
-00015a00: 735b 305d 0d0a 2020 2020 2020 2020 2020  s[0]..          
-00015a10: 2020 7374 6172 7420 3d20 286f 7468 6572    start = (other
-00015a20: 5f72 6573 756c 745b 305d 2e73 7461 7274  _result[0].start
-00015a30: 2069 6620 6669 7273 745f 776f 7264 2069   if first_word i
-00015a40: 7320 4e6f 6e65 2065 6c73 6520 6669 7273  s None else firs
-00015a50: 745f 776f 7264 2e65 6e64 290d 0a20 2020  t_word.end)..   
-00015a60: 2020 2020 2020 2020 2065 6e64 203d 206f           end = o
-00015a70: 7468 6572 5f72 6573 756c 745b 2d31 5d2e  ther_result[-1].
-00015a80: 656e 6420 6966 206c 6173 745f 776f 7264  end if last_word
-00015a90: 2069 7320 4e6f 6e65 2065 6c73 6520 6c61   is None else la
-00015aa0: 7374 5f77 6f72 642e 7374 6172 740d 0a20  st_word.start.. 
-00015ab0: 2020 2020 2020 2020 2020 2069 6620 656e             if en
-00015ac0: 6420 2d20 7374 6172 7420 3c3d 206d 696e  d - start <= min
-00015ad0: 5f67 6170 3a0d 0a20 2020 2020 2020 2020  _gap:..         
-00015ae0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00015af0: 0a20 2020 2020 2020 2020 2020 2067 6170  .            gap
-00015b00: 5f77 6f72 6473 203d 206f 7468 6572 5f72  _words = other_r
-00015b10: 6573 756c 742e 6765 745f 636f 6e74 656e  esult.get_conten
-00015b20: 745f 6279 5f74 696d 6528 2873 7461 7274  t_by_time((start
-00015b30: 2c20 656e 6429 290d 0a20 2020 2020 2020  , end))..       
-00015b40: 2020 2020 2069 6620 6669 7273 745f 776f       if first_wo
-00015b50: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
-00015b60: 6e64 2067 6170 5f77 6f72 6473 2061 6e64  nd gap_words and
-00015b70: 2073 7472 6970 2866 6972 7374 5f77 6f72   strip(first_wor
-00015b80: 642e 776f 7264 2920 3d3d 2073 7472 6970  d.word) == strip
-00015b90: 2867 6170 5f77 6f72 6473 5b30 5d2e 776f  (gap_words[0].wo
-00015ba0: 7264 293a 0d0a 2020 2020 2020 2020 2020  rd):..          
-00015bb0: 2020 2020 2020 6669 7273 745f 776f 7264        first_word
-00015bc0: 2e65 6e64 203d 2067 6170 5f77 6f72 6473  .end = gap_words
-00015bd0: 5b30 5d2e 656e 640d 0a20 2020 2020 2020  [0].end..       
-00015be0: 2020 2020 2020 2020 2067 6170 5f77 6f72           gap_wor
-00015bf0: 6473 203d 2067 6170 5f77 6f72 6473 5b31  ds = gap_words[1
-00015c00: 3a5d 0d0a 2020 2020 2020 2020 2020 2020  :]..            
-00015c10: 6966 206c 6173 745f 776f 7264 2069 7320  if last_word is 
-00015c20: 6e6f 7420 4e6f 6e65 2061 6e64 2067 6170  not None and gap
-00015c30: 5f77 6f72 6473 2061 6e64 2073 7472 6970  _words and strip
-00015c40: 286c 6173 745f 776f 7264 2e77 6f72 6429  (last_word.word)
-00015c50: 203d 3d20 7374 7269 7028 6761 705f 776f   == strip(gap_wo
-00015c60: 7264 735b 2d31 5d2e 776f 7264 293a 0d0a  rds[-1].word):..
-00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c80: 6c61 7374 5f77 6f72 642e 7374 6172 7420  last_word.start 
-00015c90: 3d20 6761 705f 776f 7264 735b 2d31 5d2e  = gap_words[-1].
-00015ca0: 7374 6172 740d 0a20 2020 2020 2020 2020  start..         
-00015cb0: 2020 2020 2020 2067 6170 5f77 6f72 6473         gap_words
-00015cc0: 203d 2067 6170 5f77 6f72 6473 5b3a 2d31   = gap_words[:-1
-00015cd0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-00015ce0: 6620 6e6f 7420 6761 705f 776f 7264 733a  f not gap_words:
-00015cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015d00: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00015d10: 2020 2020 2020 2020 6966 206c 6173 745f          if last_
-00015d20: 776f 7264 2069 7320 6e6f 7420 4e6f 6e65  word is not None
-00015d30: 2061 6e64 206c 6173 745f 776f 7264 2e73   and last_word.s
-00015d40: 7461 7274 203c 2067 6170 5f77 6f72 6473  tart < gap_words
-00015d50: 5b2d 315d 2e65 6e64 3a0d 0a20 2020 2020  [-1].end:..     
-00015d60: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-00015d70: 776f 7264 2e73 7461 7274 203d 2067 6170  word.start = gap
-00015d80: 5f77 6f72 6473 5b2d 315d 2e65 6e64 0d0a  _words[-1].end..
-00015d90: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00015da0: 7365 676d 656e 7473 203d 205b 6f74 6865  segments = [othe
-00015db0: 725f 7265 7375 6c74 5b67 6170 5f77 6f72  r_result[gap_wor
-00015dc0: 6473 5b30 5d2e 7365 676d 656e 745f 6964  ds[0].segment_id
-00015dd0: 5d2e 636f 7079 285b 5d29 5d0d 0a20 2020  ].copy([])]..   
-00015de0: 2020 2020 2020 2020 2066 6f72 206a 2c20           for j, 
-00015df0: 6e65 775f 776f 7264 2069 6e20 656e 756d  new_word in enum
-00015e00: 6572 6174 6528 6761 705f 776f 7264 7329  erate(gap_words)
-00015e10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015e20: 2020 206e 6577 5f77 6f72 645f 636f 7079     new_word_copy
-00015e30: 203d 206e 6577 5f77 6f72 642e 636f 7079   = new_word.copy
-00015e40: 2863 6f70 795f 746f 6b65 6e73 3d54 7275  (copy_tokens=Tru
-00015e50: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00015e60: 2020 2020 6966 206a 203d 3d20 3020 616e      if j == 0 an
-00015e70: 6420 6669 7273 745f 776f 7264 2069 7320  d first_word is 
-00015e80: 6e6f 7420 4e6f 6e65 2061 6e64 2066 6972  not None and fir
-00015e90: 7374 5f77 6f72 642e 656e 6420 3e20 6761  st_word.end > ga
-00015ea0: 705f 776f 7264 735b 305d 2e73 7461 7274  p_words[0].start
-00015eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015ec0: 2020 2020 2020 206e 6577 5f77 6f72 645f         new_word_
-00015ed0: 636f 7079 2e73 7461 7274 203d 2066 6972  copy.start = fir
-00015ee0: 7374 5f77 6f72 642e 656e 640d 0a20 2020  st_word.end..   
-00015ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015f00: 6e65 775f 7365 676d 656e 7473 5b2d 315d  new_segments[-1]
-00015f10: 2e69 6420 213d 206e 6577 5f77 6f72 642e  .id != new_word.
-00015f20: 7365 676d 656e 745f 6964 3a0d 0a20 2020  segment_id:..   
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 206e 6577 5f73 6567 6d65 6e74 732e 6170   new_segments.ap
-00015f50: 7065 6e64 286f 7468 6572 5f72 6573 756c  pend(other_resul
-00015f60: 745b 6e65 775f 776f 7264 2e73 6567 6d65  t[new_word.segme
-00015f70: 6e74 5f69 645d 2e63 6f70 7928 5b5d 2929  nt_id].copy([]))
-00015f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015f90: 2020 6e65 775f 7365 676d 656e 7473 5b2d    new_segments[-
-00015fa0: 315d 2e77 6f72 6473 2e61 7070 656e 6428  1].words.append(
-00015fb0: 6e65 775f 776f 7264 5f63 6f70 7929 0d0a  new_word_copy)..
-00015fc0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00015fd0: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00015fe0: 2020 2020 2020 2020 2063 6861 6e67 6573           changes
-00015ff0: 2e61 7070 656e 6428 275c 6e27 2e6a 6f69  .append('\n'.joi
-00016000: 6e28 2741 6464 6564 3a20 2720 2b20 732e  n('Added: ' + s.
-00016010: 746f 5f64 6973 706c 6179 5f73 7472 2854  to_display_str(T
-00016020: 7275 6529 2066 6f72 2073 2069 6e20 6e65  rue) for s in ne
-00016030: 775f 7365 676d 656e 7473 2929 0d0a 2020  w_segments))..  
-00016040: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00016050: 6567 6d65 6e74 7320 3d20 7365 6c66 2e73  egments = self.s
-00016060: 6567 6d65 6e74 735b 3a69 2b31 5d20 2b20  egments[:i+1] + 
-00016070: 6e65 775f 7365 676d 656e 7473 202b 2073  new_segments + s
-00016080: 656c 662e 7365 676d 656e 7473 5b69 2b31  elf.segments[i+1
-00016090: 3a5d 0d0a 2020 2020 2020 2020 6966 2063  :]..        if c
-000160a0: 6861 6e67 6573 3a0d 0a20 2020 2020 2020  hanges:..       
-000160b0: 2020 2020 2070 7269 6e74 2827 5c6e 272e       print('\n'.
-000160c0: 6a6f 696e 2872 6576 6572 7365 6428 6368  join(reversed(ch
-000160d0: 616e 6765 7329 2929 0d0a 2020 2020 2020  anges)))..      
-000160e0: 2020 7365 6c66 2e72 6561 7373 6967 6e5f    self.reassign_
-000160f0: 6964 7328 290d 0a0d 0a20 2020 2020 2020  ids()....       
-00016100: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00016110: 2020 2020 6465 6620 7265 6772 6f75 7028      def regroup(
-00016120: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00016130: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00016140: 2072 6567 726f 7570 5f61 6c67 6f3a 2055   regroup_algo: U
-00016150: 6e69 6f6e 5b73 7472 2c20 626f 6f6c 5d20  nion[str, bool] 
-00016160: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00016170: 2020 2020 2076 6572 626f 7365 3a20 626f       verbose: bo
-00016180: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-00016190: 2020 2020 2020 2020 206f 6e6c 795f 7368           only_sh
-000161a0: 6f77 3a20 626f 6f6c 203d 2046 616c 7365  ow: bool = False
-000161b0: 0d0a 2020 2020 2920 2d3e 2022 5768 6973  ..    ) -> "Whis
-000161c0: 7065 7252 6573 756c 7422 3a0d 0a20 2020  perResult":..   
-000161d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000161e0: 2020 5265 6772 6f75 7020 2869 6e2d 706c    Regroup (in-pl
-000161f0: 6163 6529 2077 6f72 6473 2069 6e74 6f20  ace) words into 
-00016200: 7365 676d 656e 7473 2e0d 0a0d 0a20 2020  segments.....   
-00016210: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-00016220: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00016230: 2d2d 2d0d 0a20 2020 2020 2020 2072 6567  ---..        reg
-00016240: 726f 7570 5f61 6c67 6f3a 2073 7472 206f  roup_algo: str o
-00016250: 7220 626f 6f6c 2c20 6465 6661 756c 7420  r bool, default 
-00016260: 2764 6127 0d0a 2020 2020 2020 2020 2020  'da'..          
-00016270: 2020 2053 7472 696e 6720 7265 7072 6573     String repres
-00016280: 656e 7461 7469 6f6e 206f 6620 6120 6375  entation of a cu
-00016290: 7374 6f6d 2072 6567 726f 7570 696e 6720  stom regrouping 
-000162a0: 616c 676f 7269 7468 6d20 6f72 2060 6054  algorithm or ``T
-000162b0: 7275 6560 6020 7573 6520 746f 2074 6865  rue`` use to the
-000162c0: 2064 6566 6175 6c74 2061 6c67 6f72 6974   default algorit
-000162d0: 686d 2027 6461 272e 0d0a 2020 2020 2020  hm 'da'...      
-000162e0: 2020 7665 7262 6f73 6520 3a20 626f 6f6c    verbose : bool
-000162f0: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
-00016300: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-00016310: 7468 6572 2074 6f20 7368 6f77 2061 6c6c  ther to show all
-00016320: 2074 6865 206d 6574 686f 6473 2061 6e64   the methods and
-00016330: 2061 7267 756d 656e 7473 2070 6172 7365   arguments parse
-00016340: 6420 6672 6f6d 2060 6072 6567 726f 7570  d from ``regroup
-00016350: 5f61 6c67 6f60 602e 0d0a 2020 2020 2020  _algo``...      
-00016360: 2020 6f6e 6c79 5f73 686f 7720 3a20 626f    only_show : bo
-00016370: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00016380: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-00016390: 6865 7468 6572 2074 6f20 7368 6f77 2074  hether to show t
-000163a0: 6865 2061 6c6c 206d 6574 686f 6473 2061  he all methods a
-000163b0: 6e64 2061 7267 756d 656e 7473 2070 6172  nd arguments par
-000163c0: 7365 6420 6672 6f6d 2060 6072 6567 726f  sed from ``regro
-000163d0: 7570 5f61 6c67 6f60 6020 7769 7468 6f75  up_algo`` withou
-000163e0: 7420 7275 6e6e 696e 6720 7468 6520 6d65  t running the me
-000163f0: 7468 6f64 730d 0a0d 0a20 2020 2020 2020  thods....       
-00016400: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00016410: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00016420: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
-00016430: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-00016440: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
-00016450: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
-00016460: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
-00016470: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
-00016480: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
-00016490: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
-000164a0: 2020 2020 2053 796e 7461 7820 666f 7220       Syntax for 
-000164b0: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-000164c0: 6174 696f 6e20 6f66 2063 7573 746f 6d20  ation of custom 
-000164d0: 7265 6772 6f75 7069 6e67 2061 6c67 6f72  regrouping algor
-000164e0: 6974 686d 2e0d 0a20 2020 2020 2020 2020  ithm...         
-000164f0: 2020 204d 6574 686f 6420 6b65 7973 3a0d     Method keys:.
-00016500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016510: 2073 673a 2073 706c 6974 5f62 795f 6761   sg: split_by_ga
-00016520: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-00016530: 2020 2073 703a 2073 706c 6974 5f62 795f     sp: split_by_
-00016540: 7075 6e63 7475 6174 696f 6e0d 0a20 2020  punctuation..   
-00016550: 2020 2020 2020 2020 2020 2020 2073 6c3a               sl:
-00016560: 2073 706c 6974 5f62 795f 6c65 6e67 7468   split_by_length
-00016570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016580: 2020 7364 3a20 7370 6c69 745f 6279 5f64    sd: split_by_d
-00016590: 7572 6174 696f 6e0d 0a20 2020 2020 2020  uration..       
-000165a0: 2020 2020 2020 2020 206d 673a 206d 6572           mg: mer
-000165b0: 6765 5f62 795f 6761 700d 0a20 2020 2020  ge_by_gap..     
-000165c0: 2020 2020 2020 2020 2020 206d 703a 206d             mp: m
-000165d0: 6572 6765 5f62 795f 7075 6e63 7475 6174  erge_by_punctuat
-000165e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000165f0: 2020 2020 206d 733a 206d 6572 6765 5f61       ms: merge_a
-00016600: 6c6c 5f73 6567 6d65 6e74 0d0a 2020 2020  ll_segment..    
-00016610: 2020 2020 2020 2020 2020 2020 636d 3a20              cm: 
-00016620: 636c 616d 705f 6d61 780d 0a20 2020 2020  clamp_max..     
-00016630: 2020 2020 2020 2020 2020 206c 3a20 6c6f             l: lo
-00016640: 636b 0d0a 2020 2020 2020 2020 2020 2020  ck..            
-00016650: 2020 2020 7573 3a20 756e 6c6f 636b 5f61      us: unlock_a
-00016660: 6c6c 5f73 6567 6d65 6e74 730d 0a20 2020  ll_segments..   
-00016670: 2020 2020 2020 2020 2020 2020 2064 613a               da:
-00016680: 2064 6566 6175 6c74 2061 6c67 6f72 6974   default algorit
-00016690: 686d 2028 636d 5f73 703d 2c2a 202f efbc  hm (cm_sp=,* /..
-000166a0: 8c5f 7367 3d2e 355f 6d67 3d2e 332b 335f  ._sg=.5_mg=.3+3_
-000166b0: 7370 3d2e 2a20 2fe3 8082 2f3f 2fef bc9f  sp=.* /.../?/...
-000166c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000166d0: 2020 2072 773a 2072 656d 6f76 655f 776f     rw: remove_wo
-000166e0: 7264 0d0a 2020 2020 2020 2020 2020 2020  rd..            
-000166f0: 2020 2020 7273 3a20 7265 6d6f 7665 5f73      rs: remove_s
-00016700: 6567 6d65 6e74 0d0a 2020 2020 2020 2020  egment..        
-00016710: 2020 2020 2020 2020 7270 3a20 7265 6d6f          rp: remo
-00016720: 7665 5f72 6570 6574 6974 696f 6e0d 0a20  ve_repetition.. 
-00016730: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00016740: 7773 3a20 7265 6d6f 7665 5f77 6f72 6473  ws: remove_words
-00016750: 5f62 795f 7374 720d 0a20 2020 2020 2020  _by_str..       
-00016760: 2020 2020 2020 2020 2066 673a 2066 696c           fg: fil
-00016770: 6c5f 696e 5f67 6170 730d 0a20 2020 2020  l_in_gaps..     
-00016780: 2020 2020 2020 204d 6574 6163 6861 7261         Metachara
-00016790: 6374 6572 733a 0d0a 2020 2020 2020 2020  cters:..        
-000167a0: 2020 2020 2020 2020 3d20 7365 7061 7261          = separa
-000167b0: 7465 7320 6120 6d65 7468 6f64 206b 6579  tes a method key
-000167c0: 2061 6e64 2069 7473 2061 7267 756d 656e   and its argumen
-000167d0: 7473 2028 6e6f 7420 7573 6564 2069 6620  ts (not used if 
-000167e0: 6e6f 2061 7267 756d 656e 7429 0d0a 2020  no argument)..  
-000167f0: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
-00016800: 7365 7061 7261 7465 7320 6d65 7468 6f64  separates method
-00016810: 206b 6579 7320 2861 6674 6572 2061 7267   keys (after arg
-00016820: 756d 656e 7473 2069 6620 7468 6572 6520  uments if there 
-00016830: 6172 6520 616e 7929 0d0a 2020 2020 2020  are any)..      
-00016840: 2020 2020 2020 2020 2020 2b20 7365 7061            + sepa
-00016850: 7261 7465 7320 6172 6775 6d65 6e74 7320  rates arguments 
-00016860: 666f 7220 6120 6d65 7468 6f64 206b 6579  for a method key
-00016870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016880: 2020 2f20 7365 7061 7261 7465 7320 616e    / separates an
-00016890: 2061 7267 756d 656e 7420 696e 746f 206c   argument into l
-000168a0: 6973 7420 6f66 2073 7472 696e 6773 0d0a  ist of strings..
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 2a20 7365 7061 7261 7465 7320 616e 2069  * separates an i
-000168d0: 7465 6d20 696e 206c 6973 7420 6f66 2073  tem in list of s
-000168e0: 7472 696e 6773 2069 6e74 6f20 6120 6e65  trings into a ne
-000168f0: 7374 6564 206c 6973 7420 6f66 2073 7472  sted list of str
-00016900: 696e 6773 0d0a 2020 2020 2020 2020 2020  ings..          
-00016910: 2020 4e6f 7465 733a 0d0a 2020 2020 2020    Notes:..      
-00016920: 2020 2020 2020 2d61 7267 756d 656e 7473        -arguments
-00016930: 2061 7265 2070 6172 7365 6420 706f 7369   are parsed posi
-00016940: 7469 6f6e 616c 6c79 0d0a 2020 2020 2020  tionally..      
-00016950: 2020 2020 2020 2d69 6620 6e6f 2061 7267        -if no arg
-00016960: 756d 656e 7420 6973 2070 726f 7669 6465  ument is provide
-00016970: 642c 2074 6865 2064 6566 6175 6c74 206f  d, the default o
-00016980: 6e65 7320 7769 6c6c 2062 6520 7573 6564  nes will be used
-00016990: 0d0a 2020 2020 2020 2020 2020 2020 2d75  ..            -u
-000169a0: 7365 2031 206f 7220 3020 746f 2072 6570  se 1 or 0 to rep
-000169b0: 7265 7365 6e74 2054 7275 6520 6f72 2046  resent True or F
-000169c0: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-000169d0: 2020 4578 616d 706c 6520 313a 0d0a 2020    Example 1:..  
-000169e0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000169f0: 7267 655f 6279 5f67 6170 282e 322c 2031  rge_by_gap(.2, 1
-00016a00: 302c 206c 6f63 6b3d 5472 7565 290d 0a20  0, lock=True).. 
-00016a10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016a20: 673d 2e32 2b31 302b 2b2b 310d 0a20 2020  g=.2+10+++1..   
-00016a30: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
-00016a40: 653a 205b 6c6f 636b 5d20 6973 2074 6865  e: [lock] is the
-00016a50: 2035 7468 2061 7267 756d 656e 7420 6865   5th argument he
-00016a60: 6e63 6520 7468 6520 3220 6d69 7373 696e  nce the 2 missin
-00016a70: 6720 6172 6775 6d65 6e74 7320 696e 6265  g arguments inbe
-00016a80: 7477 6565 6e20 7468 6520 7468 7265 6520  tween the three 
-00016a90: 2b20 6265 666f 7265 2031 0d0a 2020 2020  + before 1..    
-00016aa0: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
-00016ab0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-00016ac0: 2020 2020 7370 6c69 745f 6279 5f70 756e      split_by_pun
-00016ad0: 6374 7561 7469 6f6e 285b 2827 2e27 2c20  ctuation([('.', 
-00016ae0: 2720 2729 2c20 27e3 8082 272c 2027 3f27  ' '), '...', '?'
-00016af0: 2c20 27ef bc9f 275d 2c20 5472 7565 290d  , '...'], True).
-00016b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b10: 2073 703d 2e2a 202f e380 822f 3f2f efbc   sp=.* /.../?/..
-00016b20: 9f2b 310d 0a20 2020 2020 2020 2020 2020  .+1..           
-00016b30: 2045 7861 6d70 6c65 2033 3a0d 0a20 2020   Example 3:..   
-00016b40: 2020 2020 2020 2020 2020 2020 206d 6572               mer
-00016b50: 6765 5f61 6c6c 5f73 6567 6d65 6e74 7328  ge_all_segments(
-00016b60: 292e 7370 6c69 745f 6279 5f67 6170 282e  ).split_by_gap(.
-00016b70: 3529 2e6d 6572 6765 5f62 795f 6761 7028  5).merge_by_gap(
-00016b80: 2e31 352c 2033 290d 0a20 2020 2020 2020  .15, 3)..       
-00016b90: 2020 2020 2020 2020 206d 735f 7367 3d2e           ms_sg=.
-00016ba0: 355f 6d67 3d2e 3135 2b33 0d0a 2020 2020  5_mg=.15+3..    
-00016bb0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00016bc0: 2069 6620 7265 6772 6f75 705f 616c 676f   if regroup_algo
-00016bd0: 2069 7320 4661 6c73 653a 0d0a 2020 2020   is False:..    
-00016be0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00016bf0: 656c 660d 0a20 2020 2020 2020 2069 6620  elf..        if 
-00016c00: 7265 6772 6f75 705f 616c 676f 2069 7320  regroup_algo is 
-00016c10: 4e6f 6e65 206f 7220 7265 6772 6f75 705f  None or regroup_
-00016c20: 616c 676f 2069 7320 5472 7565 3a0d 0a20  algo is True:.. 
-00016c30: 2020 2020 2020 2020 2020 2072 6567 726f             regro
-00016c40: 7570 5f61 6c67 6f20 3d20 2764 6127 0d0a  up_algo = 'da'..
-00016c50: 0d0a 2020 2020 2020 2020 666f 7220 6d65  ..        for me
-00016c60: 7468 6f64 2c20 6b77 6172 6773 2c20 6d73  thod, kwargs, ms
-00016c70: 6720 696e 2073 656c 662e 7061 7273 655f  g in self.parse_
-00016c80: 7265 6772 6f75 705f 616c 676f 2872 6567  regroup_algo(reg
-00016c90: 726f 7570 5f61 6c67 6f2c 2069 6e63 6c75  roup_algo, inclu
-00016ca0: 6465 5f73 7472 3d76 6572 626f 7365 206f  de_str=verbose o
-00016cb0: 7220 6f6e 6c79 5f73 686f 7729 3a0d 0a20  r only_show):.. 
-00016cc0: 2020 2020 2020 2020 2020 2069 6620 6d73             if ms
-00016cd0: 673a 0d0a 2020 2020 2020 2020 2020 2020  g:..            
-00016ce0: 2020 2020 7072 696e 7428 6d73 6729 0d0a      print(msg)..
-00016cf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00016d00: 6f74 206f 6e6c 795f 7368 6f77 3a0d 0a20  ot only_show:.. 
-00016d10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016d20: 6574 686f 6428 2a2a 6b77 6172 6773 290d  ethod(**kwargs).
-00016d30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00016d40: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
-00016d50: 6620 7061 7273 655f 7265 6772 6f75 705f  f parse_regroup_
-00016d60: 616c 676f 2873 656c 662c 2072 6567 726f  algo(self, regro
-00016d70: 7570 5f61 6c67 6f3a 2073 7472 2c20 696e  up_algo: str, in
-00016d80: 636c 7564 655f 7374 723a 2062 6f6f 6c20  clude_str: bool 
-00016d90: 3d20 5472 7565 2920 2d3e 204c 6973 745b  = True) -> List[
-00016da0: 5475 706c 655b 4361 6c6c 6162 6c65 2c20  Tuple[Callable, 
-00016db0: 6469 6374 2c20 7374 725d 5d3a 0d0a 2020  dict, str]]:..  
-00016dc0: 2020 2020 2020 6d65 7468 6f64 7320 3d20        methods = 
-00016dd0: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
-00016de0: 2020 2073 673d 7365 6c66 2e73 706c 6974     sg=self.split
-00016df0: 5f62 795f 6761 702c 0d0a 2020 2020 2020  _by_gap,..      
-00016e00: 2020 2020 2020 7370 3d73 656c 662e 7370        sp=self.sp
-00016e10: 6c69 745f 6279 5f70 756e 6374 7561 7469  lit_by_punctuati
-00016e20: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-00016e30: 2073 6c3d 7365 6c66 2e73 706c 6974 5f62   sl=self.split_b
-00016e40: 795f 6c65 6e67 7468 2c0d 0a20 2020 2020  y_length,..     
-00016e50: 2020 2020 2020 2073 643d 7365 6c66 2e73         sd=self.s
-00016e60: 706c 6974 5f62 795f 6475 7261 7469 6f6e  plit_by_duration
-00016e70: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00016e80: 673d 7365 6c66 2e6d 6572 6765 5f62 795f  g=self.merge_by_
-00016e90: 6761 702c 0d0a 2020 2020 2020 2020 2020  gap,..          
-00016ea0: 2020 6d70 3d73 656c 662e 6d65 7267 655f    mp=self.merge_
-00016eb0: 6279 5f70 756e 6374 7561 7469 6f6e 2c0d  by_punctuation,.
-00016ec0: 0a20 2020 2020 2020 2020 2020 206d 733d  .            ms=
-00016ed0: 7365 6c66 2e6d 6572 6765 5f61 6c6c 5f73  self.merge_all_s
-00016ee0: 6567 6d65 6e74 732c 0d0a 2020 2020 2020  egments,..      
-00016ef0: 2020 2020 2020 636d 3d73 656c 662e 636c        cm=self.cl
-00016f00: 616d 705f 6d61 782c 0d0a 2020 2020 2020  amp_max,..      
-00016f10: 2020 2020 2020 7573 3d73 656c 662e 756e        us=self.un
-00016f20: 6c6f 636b 5f61 6c6c 5f73 6567 6d65 6e74  lock_all_segment
-00016f30: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00016f40: 6c3d 7365 6c66 2e6c 6f63 6b2c 0d0a 2020  l=self.lock,..  
-00016f50: 2020 2020 2020 2020 2020 7277 3d73 656c            rw=sel
-00016f60: 662e 7265 6d6f 7665 5f77 6f72 642c 0d0a  f.remove_word,..
-00016f70: 2020 2020 2020 2020 2020 2020 7273 3d73              rs=s
-00016f80: 656c 662e 7265 6d6f 7665 5f73 6567 6d65  elf.remove_segme
-00016f90: 6e74 2c0d 0a20 2020 2020 2020 2020 2020  nt,..           
-00016fa0: 2072 703d 7365 6c66 2e72 656d 6f76 655f   rp=self.remove_
-00016fb0: 7265 7065 7469 7469 6f6e 2c0d 0a20 2020  repetition,..   
-00016fc0: 2020 2020 2020 2020 2072 7773 3d73 656c           rws=sel
-00016fd0: 662e 7265 6d6f 7665 5f77 6f72 6473 5f62  f.remove_words_b
-00016fe0: 795f 7374 722c 0d0a 2020 2020 2020 2020  y_str,..        
-00016ff0: 2020 2020 6667 3d73 656c 662e 6669 6c6c      fg=self.fill
-00017000: 5f69 6e5f 6761 7073 2c0d 0a20 2020 2020  _in_gaps,..     
-00017010: 2020 2029 0d0a 2020 2020 2020 2020 6966     )..        if
-00017020: 206e 6f74 2072 6567 726f 7570 5f61 6c67   not regroup_alg
-00017030: 6f3a 0d0a 2020 2020 2020 2020 2020 2020  o:..            
-00017040: 7265 7475 726e 205b 5d0d 0a0d 0a20 2020  return []....   
-00017050: 2020 2020 2063 616c 6c73 203d 2072 6567       calls = reg
-00017060: 726f 7570 5f61 6c67 6f2e 7370 6c69 7428  roup_algo.split(
-00017070: 275f 2729 0d0a 2020 2020 2020 2020 6966  '_')..        if
-00017080: 2027 6461 2720 696e 2063 616c 6c73 3a0d   'da' in calls:.
-00017090: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-000170a0: 6175 6c74 5f63 616c 6c73 203d 2027 636d  ault_calls = 'cm
-000170b0: 5f73 703d 2c2a 202f efbc 8c5f 7367 3d2e  _sp=,* /..._sg=.
-000170c0: 355f 6d67 3d2e 332b 335f 7370 3d2e 2a20  5_mg=.3+3_sp=.* 
-000170d0: 2fe3 8082 2f3f 2fef bc9f 272e 7370 6c69  /.../?/...'.spli
-000170e0: 7428 275f 2729 0d0a 2020 2020 2020 2020  t('_')..        
-000170f0: 2020 2020 6361 6c6c 7320 3d20 6368 6169      calls = chai
-00017100: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
-00017110: 6465 6661 756c 745f 6361 6c6c 7320 6966  default_calls if
-00017120: 206d 6574 686f 6420 3d3d 2027 6461 2720   method == 'da' 
-00017130: 656c 7365 205b 6d65 7468 6f64 5d20 666f  else [method] fo
-00017140: 7220 6d65 7468 6f64 2069 6e20 6361 6c6c  r method in call
-00017150: 7329 0d0a 2020 2020 2020 2020 6f70 6572  s)..        oper
-00017160: 6174 696f 6e73 203d 205b 5d0d 0a20 2020  ations = []..   
-00017170: 2020 2020 2066 6f72 206d 6574 686f 6420       for method 
-00017180: 696e 2063 616c 6c73 3a0d 0a20 2020 2020  in calls:..     
-00017190: 2020 2020 2020 206d 6574 686f 642c 2061         method, a
-000171a0: 7267 7320 3d20 6d65 7468 6f64 2e73 706c  rgs = method.spl
-000171b0: 6974 2827 3d27 2c20 6d61 7873 706c 6974  it('=', maxsplit
-000171c0: 3d31 2920 6966 2027 3d27 2069 6e20 6d65  =1) if '=' in me
-000171d0: 7468 6f64 2065 6c73 6520 286d 6574 686f  thod else (metho
-000171e0: 642c 2027 2729 0d0a 2020 2020 2020 2020  d, '')..        
-000171f0: 2020 2020 6966 206d 6574 686f 6420 6e6f      if method no
-00017200: 7420 696e 206d 6574 686f 6473 3a0d 0a20  t in methods:.. 
-00017210: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017220: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-00017230: 7465 6445 7272 6f72 2866 277b 6d65 7468  tedError(f'{meth
-00017240: 6f64 7d20 6973 206e 6f74 206f 6e65 206f  od} is not one o
-00017250: 6620 7468 6520 6176 6169 6c61 626c 6520  f the available 
-00017260: 6d65 7468 6f64 733a 207b 7475 706c 6528  methods: {tuple(
-00017270: 6d65 7468 6f64 732e 6b65 7973 2829 297d  methods.keys())}
-00017280: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00017290: 6172 6773 203d 205b 5d20 6966 206c 656e  args = [] if len
-000172a0: 2861 7267 7329 203d 3d20 3020 656c 7365  (args) == 0 else
-000172b0: 206c 6973 7428 6d61 7028 7374 725f 746f   list(map(str_to
-000172c0: 5f76 616c 6964 5f74 7970 652c 2061 7267  _valid_type, arg
-000172d0: 732e 7370 6c69 7428 272b 2729 2929 0d0a  s.split('+')))..
-000172e0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000172f0: 6773 203d 207b 6b3a 2076 2066 6f72 206b  gs = {k: v for k
-00017300: 2c20 7620 696e 207a 6970 286d 6574 686f  , v in zip(metho
-00017310: 6473 5b6d 6574 686f 645d 2e5f 5f63 6f64  ds[method].__cod
-00017320: 655f 5f2e 636f 5f76 6172 6e61 6d65 735b  e__.co_varnames[
-00017330: 313a 5d2c 2061 7267 7329 2069 6620 7620  1:], args) if v 
-00017340: 6973 206e 6f74 204e 6f6e 657d 0d0a 2020  is not None}..  
-00017350: 2020 2020 2020 2020 2020 6966 2069 6e63            if inc
-00017360: 6c75 6465 5f73 7472 3a0d 0a20 2020 2020  lude_str:..     
-00017370: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00017380: 735f 7374 7220 3d20 272c 2027 2e6a 6f69  s_str = ', '.joi
-00017390: 6e28 6627 7b6b 7d3d 227b 767d 2227 2069  n(f'{k}="{v}"' i
-000173a0: 6620 6973 696e 7374 616e 6365 2876 2c20  f isinstance(v, 
-000173b0: 7374 7229 2065 6c73 6520 6627 7b6b 7d3d  str) else f'{k}=
-000173c0: 7b76 7d27 2066 6f72 206b 2c20 7620 696e  {v}' for k, v in
-000173d0: 206b 7761 7267 732e 6974 656d 7328 2929   kwargs.items())
-000173e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000173f0: 2020 6f70 5f73 7472 203d 2066 277b 6d65    op_str = f'{me
-00017400: 7468 6f64 735b 6d65 7468 6f64 5d2e 5f5f  thods[method].__
-00017410: 6e61 6d65 5f5f 7d28 7b6b 7761 7267 735f  name__}({kwargs_
-00017420: 7374 727d 2927 0d0a 2020 2020 2020 2020  str})'..        
-00017430: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00017440: 2020 2020 2020 2020 2020 206f 705f 7374             op_st
-00017450: 7220 3d20 4e6f 6e65 0d0a 2020 2020 2020  r = None..      
-00017460: 2020 2020 2020 6f70 6572 6174 696f 6e73        operations
-00017470: 2e61 7070 656e 6428 286d 6574 686f 6473  .append((methods
-00017480: 5b6d 6574 686f 645d 2c20 6b77 6172 6773  [method], kwargs
-00017490: 2c20 6f70 5f73 7472 2929 0d0a 0d0a 2020  , op_str))....  
-000174a0: 2020 2020 2020 7265 7475 726e 206f 7065        return ope
-000174b0: 7261 7469 6f6e 730d 0a0d 0a20 2020 2064  rations....    d
-000174c0: 6566 2066 696e 6428 7365 6c66 2c20 7061  ef find(self, pa
-000174d0: 7474 6572 6e3a 2073 7472 2c20 776f 7264  ttern: str, word
-000174e0: 5f6c 6576 656c 3d54 7275 652c 2066 6c61  _level=True, fla
-000174f0: 6773 3d4e 6f6e 6529 202d 3e20 2257 6869  gs=None) -> "Whi
-00017500: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
-00017510: 7322 3a0d 0a20 2020 2020 2020 2022 2222  s":..        """
-00017520: 0d0a 2020 2020 2020 2020 4669 6e64 2073  ..        Find s
-00017530: 6567 6d65 6e74 732f 776f 7264 7320 616e  egments/words an
-00017540: 6420 7469 6d65 7374 616d 7073 2077 6974  d timestamps wit
-00017550: 6820 7265 6775 6c61 7220 6578 7072 6573  h regular expres
-00017560: 7369 6f6e 2e0d 0a0d 0a20 2020 2020 2020  sion.....       
-00017570: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00017580: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
-00017590: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-000175a0: 203a 2073 7472 0d0a 2020 2020 2020 2020   : str..        
-000175b0: 2020 2020 5265 6745 7820 7061 7474 6572      RegEx patter
-000175c0: 6e20 746f 2073 6561 7263 6820 666f 722e  n to search for.
-000175d0: 0d0a 2020 2020 2020 2020 776f 7264 5f6c  ..        word_l
-000175e0: 6576 656c 203a 2062 6f6f 6c2c 2064 6566  evel : bool, def
-000175f0: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-00017600: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-00017610: 6f20 7365 6172 6368 2061 7420 776f 7264  o search at word
-00017620: 2d6c 6576 656c 2e0d 0a20 2020 2020 2020  -level...       
-00017630: 2066 6c61 6773 203a 206f 7074 696f 6e61   flags : optiona
-00017640: 6c0d 0a20 2020 2020 2020 2020 2020 2052  l..            R
-00017650: 6567 4578 2066 6c61 6773 2e0d 0a0d 0a20  egEx flags..... 
-00017660: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-00017670: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-00017680: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-00017690: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-000176a0: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
-000176b0: 6865 730d 0a20 2020 2020 2020 2020 2020  hes..           
-000176c0: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
-000176d0: 3a63 6c61 7373 3a60 7374 6162 6c65 5f77  :class:`stable_w
-000176e0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-000176f0: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
-00017700: 6573 6020 7769 7468 2077 6f72 642f 7365  es` with word/se
-00017710: 676d 656e 7420 7468 6174 206d 6174 6368  gment that match
-00017720: 2060 6070 6174 7465 726e 6060 2e0d 0a20   ``pattern``... 
-00017730: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00017740: 2020 2020 7265 7475 726e 2057 6869 7370      return Whisp
-00017750: 6572 5265 7375 6c74 4d61 7463 6865 7328  erResultMatches(
-00017760: 7365 6c66 292e 6669 6e64 2870 6174 7465  self).find(patte
-00017770: 726e 2c20 776f 7264 5f6c 6576 656c 3d77  rn, word_level=w
-00017780: 6f72 645f 6c65 7665 6c2c 2066 6c61 6773  ord_level, flags
-00017790: 3d66 6c61 6773 290d 0a0d 0a20 2020 2040  =flags)....    @
-000177a0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-000177b0: 6620 7465 7874 2873 656c 6629 3a0d 0a20  f text(self):.. 
-000177c0: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
-000177d0: 2e6a 6f69 6e28 732e 7465 7874 2066 6f72  .join(s.text for
-000177e0: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
-000177f0: 6e74 7329 0d0a 0d0a 2020 2020 4070 726f  nts)....    @pro
-00017800: 7065 7274 790d 0a20 2020 2064 6566 2072  perty..    def r
-00017810: 6567 726f 7570 5f68 6973 746f 7279 2873  egroup_history(s
-00017820: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
-00017830: 2073 616d 6520 7379 6e74 6178 2061 7320   same syntax as 
-00017840: 6060 7265 6772 6f75 705f 616c 676f 6060  ``regroup_algo``
-00017850: 2066 6f72 203a 6d65 7468 3a60 6072 6573   for :meth:``res
-00017860: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
-00017870: 742e 7265 6772 6f75 7060 0d0a 2020 2020  t.regroup`..    
-00017880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017890: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-000178a0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-000178b0: 790d 0a20 2020 2064 6566 206e 6f6e 7370  y..    def nonsp
-000178c0: 6565 6368 5f73 6563 7469 6f6e 7328 7365  eech_sections(se
-000178d0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-000178e0: 7475 726e 2073 656c 662e 5f6e 6f6e 7370  turn self._nonsp
-000178f0: 6565 6368 5f73 6563 7469 6f6e 730d 0a0d  eech_sections...
-00017900: 0a20 2020 2064 6566 2073 686f 775f 7265  .    def show_re
-00017910: 6772 6f75 705f 6869 7374 6f72 7928 7365  group_history(se
-00017920: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00017930: 220d 0a20 2020 2020 2020 2050 7269 6e74  "..        Print
-00017940: 2064 6574 6169 6c73 206f 6620 616c 6c20   details of all 
-00017950: 7265 6772 6f75 7069 6e67 206f 7065 7261  regrouping opera
-00017960: 7469 6f6e 7320 7468 6174 2062 6565 6e20  tions that been 
-00017970: 7065 7266 6f72 6d65 6420 6f6e 2064 6174  performed on dat
-00017980: 612e 0d0a 2020 2020 2020 2020 2222 220d  a...        """.
-00017990: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000179a0: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
-000179b0: 7374 6f72 793a 0d0a 2020 2020 2020 2020  story:..        
-000179c0: 2020 2020 7072 696e 7428 2752 6573 756c      print('Resul
-000179d0: 7420 6861 7320 6e6f 2068 6973 746f 7279  t has no history
-000179e0: 2e27 290d 0a20 2020 2020 2020 2066 6f72  .')..        for
-000179f0: 202a 5f2c 206d 7367 2069 6e20 7365 6c66   *_, msg in self
-00017a00: 2e70 6172 7365 5f72 6567 726f 7570 5f61  .parse_regroup_a
-00017a10: 6c67 6f28 7365 6c66 2e5f 7265 6772 6f75  lgo(self._regrou
-00017a20: 705f 6869 7374 6f72 7929 3a0d 0a20 2020  p_history):..   
-00017a30: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00017a40: 272e 7b6d 7367 7d27 290d 0a0d 0a20 2020  '.{msg}')....   
-00017a50: 2064 6566 205f 5f6c 656e 5f5f 2873 656c   def __len__(sel
-00017a60: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00017a70: 7572 6e20 6c65 6e28 7365 6c66 2e73 6567  urn len(self.seg
-00017a80: 6d65 6e74 7329 0d0a 0d0a 2020 2020 6465  ments)....    de
-00017a90: 6620 756e 6c6f 636b 5f61 6c6c 5f73 6567  f unlock_all_seg
-00017aa0: 6d65 6e74 7328 7365 6c66 293a 0d0a 2020  ments(self):..  
-00017ab0: 2020 2020 2020 666f 7220 7320 696e 2073        for s in s
-00017ac0: 656c 662e 7365 676d 656e 7473 3a0d 0a20  elf.segments:.. 
-00017ad0: 2020 2020 2020 2020 2020 2073 2e75 6e6c             s.unl
-00017ae0: 6f63 6b5f 616c 6c5f 776f 7264 7328 290d  ock_all_words().
-00017af0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017b00: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00017b10: 7365 745f 6375 7272 656e 745f 6173 5f6f  set_current_as_o
-00017b20: 7269 6728 7365 6c66 2c20 6b65 6570 5f6f  rig(self, keep_o
-00017b30: 7269 673a 2062 6f6f 6c20 3d20 4661 6c73  rig: bool = Fals
-00017b40: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00017b50: 0d0a 2020 2020 2020 2020 4f76 6572 7772  ..        Overwr
-00017b60: 6974 6520 616c 6c20 7661 6c75 6573 2069  ite all values i
-00017b70: 6e20 6060 6f72 695f 6469 6374 6060 2077  n ``ori_dict`` w
-00017b80: 6974 6820 6375 7272 656e 7420 7661 6c75  ith current valu
-00017b90: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
-00017ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00017bb0: 7269 5f64 6963 7420 3d20 7365 6c66 2e74  ri_dict = self.t
-00017bc0: 6f5f 6469 6374 286b 6565 705f 6f72 6967  o_dict(keep_orig
-00017bd0: 3d6b 6565 705f 6f72 6967 290d 0a0d 0a20  =keep_orig).... 
-00017be0: 2020 2064 6566 2072 6573 6574 2873 656c     def reset(sel
-00017bf0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00017c00: 0d0a 2020 2020 2020 2020 5265 7374 6f72  ..        Restor
-00017c10: 6520 616c 6c20 7661 6c75 6573 2074 6f20  e all values to 
-00017c20: 7468 6174 2061 7420 696e 6974 6961 6c69  that at initiali
-00017c30: 7a61 7469 6f6e 2069 6e20 6060 6f72 695f  zation in ``ori_
-00017c40: 6469 6374 6060 2e0d 0a20 2020 2020 2020  dict``...       
-00017c50: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-00017c60: 6c66 2e6c 616e 6775 6167 6520 3d20 7365  lf.language = se
-00017c70: 6c66 2e6f 7269 5f64 6963 742e 6765 7428  lf.ori_dict.get(
-00017c80: 276c 616e 6775 6167 6527 290d 0a20 2020  'language')..   
-00017c90: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-00017ca0: 7570 5f68 6973 746f 7279 203d 2027 270d  up_history = ''.
-00017cb0: 0a20 2020 2020 2020 2073 6567 6d65 6e74  .        segment
-00017cc0: 7320 3d20 7365 6c66 2e6f 7269 5f64 6963  s = self.ori_dic
-00017cd0: 742e 6765 7428 2773 6567 6d65 6e74 7327  t.get('segments'
-00017ce0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00017cf0: 7365 676d 656e 7473 203d 205b 5365 676d  segments = [Segm
-00017d00: 656e 7428 2a2a 732c 2069 676e 6f72 655f  ent(**s, ignore_
-00017d10: 756e 7573 6564 5f61 7267 733d 5472 7565  unused_args=True
-00017d20: 2920 666f 7220 7320 696e 2073 6567 6d65  ) for s in segme
-00017d30: 6e74 735d 2069 6620 7365 676d 656e 7473  nts] if segments
-00017d40: 2065 6c73 6520 5b5d 0d0a 2020 2020 2020   else []..      
-00017d50: 2020 6966 2073 656c 662e 5f66 6f72 6365    if self._force
-00017d60: 645f 6f72 6465 723a 0d0a 2020 2020 2020  d_order:..      
-00017d70: 2020 2020 2020 7365 6c66 2e66 6f72 6365        self.force
-00017d80: 5f6f 7264 6572 2829 0d0a 2020 2020 2020  _order()..      
-00017d90: 2020 7365 6c66 2e72 656d 6f76 655f 6e6f    self.remove_no
-00017da0: 5f77 6f72 645f 7365 676d 656e 7473 2861  _word_segments(a
-00017db0: 6e79 2873 6567 2e68 6173 5f77 6f72 6473  ny(seg.has_words
-00017dc0: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
-00017dd0: 2e73 6567 6d65 6e74 7329 290d 0a0d 0a20  .segments)).... 
-00017de0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00017df0: 2020 6465 6620 6861 735f 776f 7264 7328    def has_words(
-00017e00: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00017e10: 7265 7475 726e 2062 6f6f 6c28 7365 6c66  return bool(self
-00017e20: 2e73 6567 6d65 6e74 7329 2061 6e64 2061  .segments) and a
-00017e30: 6c6c 2873 6567 2e68 6173 5f77 6f72 6473  ll(seg.has_words
-00017e40: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
-00017e50: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
-00017e60: 2020 746f 5f73 7274 5f76 7474 203d 2072    to_srt_vtt = r
-00017e70: 6573 756c 745f 746f 5f73 7274 5f76 7474  esult_to_srt_vtt
-00017e80: 0d0a 2020 2020 746f 5f61 7373 203d 2072  ..    to_ass = r
-00017e90: 6573 756c 745f 746f 5f61 7373 0d0a 2020  esult_to_ass..  
-00017ea0: 2020 746f 5f74 7376 203d 2072 6573 756c    to_tsv = resul
-00017eb0: 745f 746f 5f74 7376 0d0a 2020 2020 746f  t_to_tsv..    to
-00017ec0: 5f74 7874 203d 2072 6573 756c 745f 746f  _txt = result_to
-00017ed0: 5f74 7874 0d0a 2020 2020 7361 7665 5f61  _txt..    save_a
-00017ee0: 735f 6a73 6f6e 203d 2073 6176 655f 6173  s_json = save_as
-00017ef0: 5f6a 736f 6e0d 0a0d 0a0d 0a63 6c61 7373  _json......class
-00017f00: 2053 6567 6d65 6e74 4d61 7463 683a 0d0a   SegmentMatch:..
-00017f10: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00017f20: 5f5f 280d 0a20 2020 2020 2020 2020 2020  __(..           
-00017f30: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00017f40: 2020 2020 7365 676d 656e 7473 3a20 556e      segments: Un
-00017f50: 696f 6e5b 4c69 7374 5b53 6567 6d65 6e74  ion[List[Segment
-00017f60: 5d2c 2053 6567 6d65 6e74 5d2c 0d0a 2020  ], Segment],..  
-00017f70: 2020 2020 2020 2020 2020 5f77 6f72 645f            _word_
-00017f80: 696e 6469 6365 733a 204c 6973 745b 4c69  indices: List[Li
-00017f90: 7374 5b69 6e74 5d5d 203d 204e 6f6e 652c  st[int]] = None,
-00017fa0: 0d0a 2020 2020 2020 2020 2020 2020 5f74  ..            _t
-00017fb0: 6578 745f 6d61 7463 683a 2073 7472 203d  ext_match: str =
-00017fc0: 204e 6f6e 650d 0a20 2020 2029 3a0d 0a20   None..    ):.. 
-00017fd0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
-00017fe0: 656e 7473 203d 205b 7365 676d 656e 7473  ents = [segments
-00017ff0: 5d20 6966 2069 7369 6e73 7461 6e63 6528  ] if isinstance(
-00018000: 7365 676d 656e 7473 2c20 5365 676d 656e  segments, Segmen
-00018010: 7429 2065 6c73 6520 7365 676d 656e 7473  t) else segments
-00018020: 0d0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-00018030: 6f72 645f 696e 6469 6365 7320 3d20 5b5d  ord_indices = []
-00018040: 2069 6620 5f77 6f72 645f 696e 6469 6365   if _word_indice
-00018050: 7320 6973 204e 6f6e 6520 656c 7365 205f  s is None else _
-00018060: 776f 7264 5f69 6e64 6963 6573 0d0a 2020  word_indices..  
-00018070: 2020 2020 2020 7365 6c66 2e77 6f72 6473        self.words
-00018080: 203d 205b 7365 6c66 2e73 6567 6d65 6e74   = [self.segment
-00018090: 735b 695d 2e77 6f72 6473 5b6a 5d20 666f  s[i].words[j] fo
-000180a0: 7220 692c 2069 6e64 6963 6573 2069 6e20  r i, indices in 
-000180b0: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
-000180c0: 6f72 645f 696e 6469 6365 7329 2066 6f72  ord_indices) for
-000180d0: 206a 2069 6e20 696e 6469 6365 735d 0d0a   j in indices]..
-000180e0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-000180f0: 656c 662e 776f 7264 7329 2021 3d20 303a  elf.words) != 0:
-00018100: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00018110: 6c66 2e74 6578 7420 3d20 2727 2e6a 6f69  lf.text = ''.joi
-00018120: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
-00018130: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-00018140: 735b 695d 2e77 6f72 6473 5b6a 5d2e 776f  s[i].words[j].wo
-00018150: 7264 0d0a 2020 2020 2020 2020 2020 2020  rd..            
-00018160: 2020 2020 666f 7220 692c 2069 6e64 6963      for i, indic
-00018170: 6573 2069 6e20 656e 756d 6572 6174 6528  es in enumerate(
-00018180: 7365 6c66 2e77 6f72 645f 696e 6469 6365  self.word_indice
-00018190: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000181a0: 2020 2020 666f 7220 6a20 696e 2069 6e64      for j in ind
-000181b0: 6963 6573 0d0a 2020 2020 2020 2020 2020  ices..          
-000181c0: 2020 290d 0a20 2020 2020 2020 2065 6c73    )..        els
-000181d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000181e0: 7365 6c66 2e74 6578 7420 3d20 2727 2e6a  self.text = ''.j
-000181f0: 6f69 6e28 7365 672e 7465 7874 2066 6f72  oin(seg.text for
-00018200: 2073 6567 2069 6e20 7365 6c66 2e73 6567   seg in self.seg
-00018210: 6d65 6e74 7329 0d0a 2020 2020 2020 2020  ments)..        
-00018220: 7365 6c66 2e74 6578 745f 6d61 7463 6820  self.text_match 
-00018230: 3d20 5f74 6578 745f 6d61 7463 680d 0a0d  = _text_match...
-00018240: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00018250: 2020 2020 6465 6620 7374 6172 7428 7365      def start(se
-00018260: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00018270: 7475 726e 2028 0d0a 2020 2020 2020 2020  turn (..        
-00018280: 2020 2020 7365 6c66 2e77 6f72 6473 5b30      self.words[0
-00018290: 5d2e 7374 6172 740d 0a20 2020 2020 2020  ].start..       
-000182a0: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
-000182b0: 2e77 6f72 6473 2920 213d 2030 2065 6c73  .words) != 0 els
-000182c0: 650d 0a20 2020 2020 2020 2020 2020 2028  e..            (
-000182d0: 7365 6c66 2e73 6567 6d65 6e74 735b 305d  self.segments[0]
-000182e0: 2e73 7461 7274 2069 6620 6c65 6e28 7365  .start if len(se
-000182f0: 6c66 2e73 6567 6d65 6e74 7329 2021 3d20  lf.segments) != 
-00018300: 3020 656c 7365 204e 6f6e 6529 0d0a 2020  0 else None)..  
-00018310: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
-00018320: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-00018330: 6620 656e 6428 7365 6c66 293a 0d0a 2020  f end(self):..  
-00018340: 2020 2020 2020 7265 7475 726e 2028 0d0a        return (..
-00018350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018360: 2e77 6f72 6473 5b2d 315d 2e65 6e64 0d0a  .words[-1].end..
-00018370: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00018380: 656e 2873 656c 662e 776f 7264 7329 2021  en(self.words) !
-00018390: 3d20 3020 656c 7365 0d0a 2020 2020 2020  = 0 else..      
-000183a0: 2020 2020 2020 2873 656c 662e 7365 676d        (self.segm
-000183b0: 656e 7473 5b2d 315d 2e65 6e64 2069 6620  ents[-1].end if 
-000183c0: 6c65 6e28 7365 6c66 2e73 6567 6d65 6e74  len(self.segment
-000183d0: 7329 2021 3d20 3020 656c 7365 204e 6f6e  s) != 0 else Non
-000183e0: 6529 0d0a 2020 2020 2020 2020 290d 0a0d  e)..        )...
-000183f0: 0a20 2020 2064 6566 205f 5f6c 656e 5f5f  .    def __len__
-00018400: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00018410: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
-00018420: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
-00018430: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-00018440: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00018450: 6574 7572 6e20 7365 6c66 2e5f 5f64 6963  eturn self.__dic
-00018460: 745f 5f2e 5f5f 7265 7072 5f5f 2829 0d0a  t__.__repr__()..
-00018470: 0d0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-00018480: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00018490: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-000184a0: 6469 6374 5f5f 2e5f 5f73 7472 5f5f 2829  dict__.__str__()
-000184b0: 0d0a 0d0a 0d0a 636c 6173 7320 5768 6973  ......class Whis
-000184c0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
-000184d0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-000184e0: 5265 6745 7820 6d61 7463 6865 7320 666f  RegEx matches fo
-000184f0: 7220 5768 6973 7065 7252 6573 756c 7473  r WhisperResults
-00018500: 2e0d 0a20 2020 2022 2222 0d0a 2020 2020  ...    """..    
-00018510: 2320 5573 6520 5768 6973 7065 7252 6573  # Use WhisperRes
-00018520: 756c 742e 6669 6e64 2829 2069 6e73 7465  ult.find() inste
-00018530: 6164 206f 6620 696e 7374 616e 7469 6174  ad of instantiat
-00018540: 696e 6720 7468 6973 2063 6c61 7373 2064  ing this class d
-00018550: 6972 6563 746c 792e 0d0a 2020 2020 6465  irectly...    de
-00018560: 6620 5f5f 696e 6974 5f5f 280d 0a20 2020  f __init__(..   
-00018570: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
-00018580: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-00018590: 6865 733a 2055 6e69 6f6e 5b4c 6973 745b  hes: Union[List[
-000185a0: 5365 676d 656e 744d 6174 6368 5d2c 2057  SegmentMatch], W
-000185b0: 6869 7370 6572 5265 7375 6c74 5d2c 0d0a  hisperResult],..
-000185c0: 2020 2020 2020 2020 2020 2020 5f73 6567              _seg
-000185d0: 6d65 6e74 5f69 6e64 6963 6573 3a20 4c69  ment_indices: Li
-000185e0: 7374 5b4c 6973 745b 696e 745d 5d20 3d20  st[List[int]] = 
-000185f0: 4e6f 6e65 0d0a 2020 2020 293a 0d0a 2020  None..    ):..  
-00018600: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00018610: 6e63 6528 6d61 7463 6865 732c 2057 6869  nce(matches, Whi
-00018620: 7370 6572 5265 7375 6c74 293a 0d0a 2020  sperResult):..  
-00018630: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018640: 6174 6368 6573 203d 206c 6973 7428 6d61  atches = list(ma
-00018650: 7028 5365 676d 656e 744d 6174 6368 2c20  p(SegmentMatch, 
-00018660: 6d61 7463 6865 732e 7365 676d 656e 7473  matches.segments
-00018670: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018680: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
-00018690: 6469 6365 7320 3d20 5b5b 695d 2066 6f72  dices = [[i] for
-000186a0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-000186b0: 6d61 7463 6865 732e 7365 676d 656e 7473  matches.segments
-000186c0: 2929 5d0d 0a20 2020 2020 2020 2065 6c73  ))]..        els
-000186d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000186e0: 7365 6c66 2e6d 6174 6368 6573 203d 206d  self.matches = m
-000186f0: 6174 6368 6573 0d0a 2020 2020 2020 2020  atches..        
-00018700: 2020 2020 6173 7365 7274 205f 7365 676d      assert _segm
-00018710: 656e 745f 696e 6469 6365 7320 6973 206e  ent_indices is n
-00018720: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
-00018730: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
-00018740: 7365 6c66 2e6d 6174 6368 6573 2920 3d3d  self.matches) ==
-00018750: 206c 656e 285f 7365 676d 656e 745f 696e   len(_segment_in
-00018760: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
-00018770: 2020 2020 6173 7365 7274 2061 6c6c 286c      assert all(l
-00018780: 656e 286d 6174 6368 2e73 6567 6d65 6e74  en(match.segment
-00018790: 7329 203d 3d20 6c65 6e28 5f73 6567 6d65  s) == len(_segme
-000187a0: 6e74 5f69 6e64 6963 6573 5b69 5d29 2066  nt_indices[i]) f
-000187b0: 6f72 2069 2c20 6d61 7463 6820 696e 2065  or i, match in e
-000187c0: 6e75 6d65 7261 7465 2873 656c 662e 6d61  numerate(self.ma
-000187d0: 7463 6865 7329 290d 0a20 2020 2020 2020  tches))..       
-000187e0: 2020 2020 2073 656c 662e 5f73 6567 6d65       self._segme
-000187f0: 6e74 5f69 6e64 6963 6573 203d 205f 7365  nt_indices = _se
-00018800: 676d 656e 745f 696e 6469 6365 730d 0a0d  gment_indices...
-00018810: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00018820: 2020 2020 6465 6620 7365 676d 656e 745f      def segment_
-00018830: 696e 6469 6365 7328 7365 6c66 293a 0d0a  indices(self):..
-00018840: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00018850: 656c 662e 5f73 6567 6d65 6e74 5f69 6e64  elf._segment_ind
-00018860: 6963 6573 0d0a 0d0a 2020 2020 6465 6620  ices....    def 
-00018870: 5f63 7572 725f 7365 675f 6772 6f75 7073  _curr_seg_groups
-00018880: 2873 656c 6629 202d 3e20 4c69 7374 5b4c  (self) -> List[L
-00018890: 6973 745b 5475 706c 655b 696e 742c 2053  ist[Tuple[int, S
-000188a0: 6567 6d65 6e74 5d5d 5d3a 0d0a 2020 2020  egment]]]:..    
-000188b0: 2020 2020 7365 675f 6772 6f75 7073 2c20      seg_groups, 
-000188c0: 6375 7272 5f73 6567 7320 3d20 5b5d 2c20  curr_segs = [], 
-000188d0: 5b5d 0d0a 2020 2020 2020 2020 6375 7272  []..        curr
-000188e0: 5f6d 6178 203d 202d 310d 0a20 2020 2020  _max = -1..     
-000188f0: 2020 2066 6f72 2073 6567 5f69 6e64 6963     for seg_indic
-00018900: 6573 2c20 6d61 7463 6820 696e 207a 6970  es, match in zip
-00018910: 2873 656c 662e 5f73 6567 6d65 6e74 5f69  (self._segment_i
-00018920: 6e64 6963 6573 2c20 7365 6c66 2e6d 6174  ndices, self.mat
-00018930: 6368 6573 293a 0d0a 2020 2020 2020 2020  ches):..        
-00018940: 2020 2020 666f 7220 692c 2073 6567 2069      for i, seg i
-00018950: 6e20 7a69 7028 736f 7274 6564 2873 6567  n zip(sorted(seg
-00018960: 5f69 6e64 6963 6573 292c 206d 6174 6368  _indices), match
-00018970: 2e73 6567 6d65 6e74 7329 3a0d 0a20 2020  .segments):..   
-00018980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018990: 6920 3e20 6375 7272 5f6d 6178 3a0d 0a20  i > curr_max:.. 
-000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189b0: 2020 2063 7572 725f 7365 6773 2e61 7070     curr_segs.app
-000189c0: 656e 6428 2869 2c20 7365 6729 290d 0a20  end((i, seg)).. 
-000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189e0: 2020 2069 6620 6920 2d20 3120 213d 2063     if i - 1 != c
-000189f0: 7572 725f 6d61 783a 0d0a 2020 2020 2020  urr_max:..      
-00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a10: 2020 7365 675f 6772 6f75 7073 2e61 7070    seg_groups.app
-00018a20: 656e 6428 6375 7272 5f73 6567 7329 0d0a  end(curr_segs)..
-00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a40: 2020 2020 2020 2020 6375 7272 5f73 6567          curr_seg
-00018a50: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00018a60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00018a70: 5f6d 6178 203d 2069 0d0a 0d0a 2020 2020  _max = i....    
-00018a80: 2020 2020 6966 2063 7572 725f 7365 6773      if curr_segs
-00018a90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00018aa0: 6567 5f67 726f 7570 732e 6170 7065 6e64  eg_groups.append
-00018ab0: 2863 7572 725f 7365 6773 290d 0a20 2020  (curr_segs)..   
-00018ac0: 2020 2020 2072 6574 7572 6e20 7365 675f       return seg_
-00018ad0: 6772 6f75 7073 0d0a 0d0a 2020 2020 6465  groups....    de
-00018ae0: 6620 6669 6e64 2873 656c 662c 2070 6174  f find(self, pat
-00018af0: 7465 726e 3a20 7374 722c 2077 6f72 645f  tern: str, word_
-00018b00: 6c65 7665 6c3d 5472 7565 2c20 666c 6167  level=True, flag
-00018b10: 733d 4e6f 6e65 2920 2d3e 2022 5768 6973  s=None) -> "Whis
-00018b20: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
-00018b30: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
-00018b40: 0a20 2020 2020 2020 2046 696e 6420 7365  .        Find se
-00018b50: 676d 656e 7473 2f77 6f72 6473 2061 6e64  gments/words and
-00018b60: 2074 696d 6573 7461 6d70 7320 7769 7468   timestamps with
-00018b70: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-00018b80: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
-00018b90: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00018ba0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00018bb0: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
-00018bc0: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
-00018bd0: 2020 2052 6567 4578 2070 6174 7465 726e     RegEx pattern
-00018be0: 2074 6f20 7365 6172 6368 2066 6f72 2e0d   to search for..
-00018bf0: 0a20 2020 2020 2020 2077 6f72 645f 6c65  .        word_le
-00018c00: 7665 6c20 3a20 626f 6f6c 2c20 6465 6661  vel : bool, defa
-00018c10: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-00018c20: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00018c30: 2073 6561 7263 6820 6174 2077 6f72 642d   search at word-
-00018c40: 6c65 7665 6c2e 0d0a 2020 2020 2020 2020  level...        
-00018c50: 666c 6167 7320 3a20 6f70 7469 6f6e 616c  flags : optional
-00018c60: 0d0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00018c70: 6745 7820 666c 6167 732e 0d0a 0d0a 2020  gEx flags.....  
-00018c80: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-00018c90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-00018ca0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
-00018cb0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-00018cc0: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
-00018cd0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-00018ce0: 416e 2069 6e73 7461 6e63 6520 6f66 203a  An instance of :
-00018cf0: 636c 6173 733a 6073 7461 626c 655f 7768  class:`stable_wh
-00018d00: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
-00018d10: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
-00018d20: 7360 2077 6974 6820 776f 7264 2f73 6567  s` with word/seg
-00018d30: 6d65 6e74 2074 6861 7420 6d61 7463 6820  ment that match 
-00018d40: 6060 7061 7474 6572 6e60 602e 0d0a 2020  ``pattern``...  
-00018d50: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-00018d60: 2020 2020 2073 6567 5f67 726f 7570 7320       seg_groups 
-00018d70: 3d20 7365 6c66 2e5f 6375 7272 5f73 6567  = self._curr_seg
-00018d80: 5f67 726f 7570 7328 290d 0a20 2020 2020  _groups()..     
-00018d90: 2020 206d 6174 6368 6573 3a20 4c69 7374     matches: List
-00018da0: 5b53 6567 6d65 6e74 4d61 7463 685d 203d  [SegmentMatch] =
-00018db0: 205b 5d0d 0a20 2020 2020 2020 206d 6174   []..        mat
-00018dc0: 6368 5f73 6567 5f69 6e64 6963 6573 3a20  ch_seg_indices: 
-00018dd0: 4c69 7374 5b4c 6973 745b 696e 745d 5d20  List[List[int]] 
-00018de0: 3d20 5b5d 0d0a 2020 2020 2020 2020 6966  = []..        if
-00018df0: 2077 6f72 645f 6c65 7665 6c3a 0d0a 2020   word_level:..  
-00018e00: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00018e10: 2061 6c6c 2861 6c6c 2873 6567 2e68 6173   all(all(seg.has
-00018e20: 5f77 6f72 6473 2066 6f72 2073 6567 2069  _words for seg i
-00018e30: 6e20 6d61 7463 682e 7365 676d 656e 7473  n match.segments
-00018e40: 2920 666f 7220 6d61 7463 6820 696e 2073  ) for match in s
-00018e50: 656c 662e 6d61 7463 6865 7329 3a0d 0a20  elf.matches):.. 
-00018e60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00018e70: 6172 6e69 6e67 732e 7761 726e 2827 4361  arnings.warn('Ca
-00018e80: 6e6e 6f74 2070 6572 666f 726d 2077 6f72  nnot perform wor
-00018e90: 642d 6c65 7665 6c20 7365 6172 6368 2077  d-level search w
-00018ea0: 6974 6820 7365 676d 656e 7428 7329 206d  ith segment(s) m
-00018eb0: 6973 7369 6e67 2077 6f72 6420 7469 6d65  issing word time
-00018ec0: 7374 616d 7073 2e27 290d 0a20 2020 2020  stamps.')..     
-00018ed0: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
-00018ee0: 6c65 7665 6c20 3d20 4661 6c73 650d 0a0d  level = False...
-00018ef0: 0a20 2020 2020 2020 2066 6f72 2073 6567  .        for seg
-00018f00: 7320 696e 2073 6567 5f67 726f 7570 733a  s in seg_groups:
-00018f10: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00018f20: 2077 6f72 645f 6c65 7665 6c3a 0d0a 2020   word_level:..  
-00018f30: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00018f40: 7873 203d 206c 6973 7428 6368 6169 6e2e  xs = list(chain.
-00018f50: 6672 6f6d 5f69 7465 7261 626c 6528 0d0a  from_iterable(..
-00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f70: 2020 2020 5b28 692c 206a 295d 2a6c 656e      [(i, j)]*len
-00018f80: 2877 6f72 642e 776f 7264 2920 666f 7220  (word.word) for 
-00018f90: 2869 2c20 7365 6729 2069 6e20 7365 6773  (i, seg) in segs
-00018fa0: 2066 6f72 206a 2c20 776f 7264 2069 6e20   for j, word in 
-00018fb0: 656e 756d 6572 6174 6528 7365 672e 776f  enumerate(seg.wo
-00018fc0: 7264 7329 0d0a 2020 2020 2020 2020 2020  rds)..          
-00018fd0: 2020 2020 2020 2929 0d0a 2020 2020 2020        ))..      
-00018fe0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00018ff0: 2027 272e 6a6f 696e 2877 6f72 642e 776f   ''.join(word.wo
-00019000: 7264 2066 6f72 2028 5f2c 2073 6567 2920  rd for (_, seg) 
-00019010: 696e 2073 6567 7320 666f 7220 776f 7264  in segs for word
-00019020: 2069 6e20 7365 672e 776f 7264 7329 0d0a   in seg.words)..
-00019030: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00019040: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019050: 2020 2069 6478 7320 3d20 6c69 7374 2863     idxs = list(c
-00019060: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
-00019070: 6c65 285b 2869 2c20 4e6f 6e65 295d 2a6c  le([(i, None)]*l
-00019080: 656e 2873 6567 2e74 6578 7429 2066 6f72  en(seg.text) for
-00019090: 2028 692c 2073 6567 2920 696e 2073 6567   (i, seg) in seg
-000190a0: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-000190b0: 2020 2020 2074 6578 7420 3d20 2727 2e6a       text = ''.j
-000190c0: 6f69 6e28 7365 672e 7465 7874 2066 6f72  oin(seg.text for
-000190d0: 2028 5f2c 2073 6567 2920 696e 2073 6567   (_, seg) in seg
-000190e0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000190f0: 6173 7365 7274 206c 656e 2869 6478 7329  assert len(idxs)
-00019100: 203d 3d20 6c65 6e28 7465 7874 290d 0a20   == len(text).. 
-00019110: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00019120: 7572 725f 6d61 7463 6820 696e 2072 652e  urr_match in re.
-00019130: 6669 6e64 6974 6572 2870 6174 7465 726e  finditer(pattern
-00019140: 2c20 7465 7874 2c20 666c 6167 733d 666c  , text, flags=fl
-00019150: 6167 7320 6f72 2030 293a 0d0a 2020 2020  ags or 0):..    
-00019160: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00019170: 742c 2065 6e64 203d 2063 7572 725f 6d61  t, end = curr_ma
-00019180: 7463 682e 7370 616e 2829 0d0a 2020 2020  tch.span()..    
-00019190: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000191a0: 5f69 6478 7320 3d20 6964 7873 5b73 7461  _idxs = idxs[sta
-000191b0: 7274 3a20 656e 645d 0d0a 2020 2020 2020  rt: end]..      
-000191c0: 2020 2020 2020 2020 2020 6375 7272 5f73            curr_s
-000191d0: 6567 5f69 6478 7320 3d20 736f 7274 6564  eg_idxs = sorted
-000191e0: 2873 6574 2869 5b30 5d20 666f 7220 6920  (set(i[0] for i 
-000191f0: 696e 2063 7572 725f 6964 7873 2929 0d0a  in curr_idxs))..
-00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019210: 6966 2077 6f72 645f 6c65 7665 6c3a 0d0a  if word_level:..
-00019220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019230: 2020 2020 6375 7272 5f77 6f72 645f 6964      curr_word_id
-00019240: 7873 203d 205b 0d0a 2020 2020 2020 2020  xs = [..        
-00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019260: 736f 7274 6564 2873 6574 286a 2066 6f72  sorted(set(j for
-00019270: 2069 2c20 6a20 696e 2063 7572 725f 6964   i, j in curr_id
-00019280: 7873 2069 6620 6920 3d3d 2073 6567 5f69  xs if i == seg_i
-00019290: 6478 2929 0d0a 2020 2020 2020 2020 2020  dx))..          
-000192a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000192b0: 7220 7365 675f 6964 7820 696e 2063 7572  r seg_idx in cur
-000192c0: 725f 7365 675f 6964 7873 0d0a 2020 2020  r_seg_idxs..    
-000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000192f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00019300: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00019310: 7272 5f77 6f72 645f 6964 7873 203d 204e  rr_word_idxs = N
-00019320: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-00019330: 2020 2020 206d 6174 6368 6573 2e61 7070       matches.app
-00019340: 656e 6428 5365 676d 656e 744d 6174 6368  end(SegmentMatch
-00019350: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00019360: 2020 2020 2020 2073 6567 6d65 6e74 733d         segments=
-00019370: 5b73 2066 6f72 2069 2c20 7320 696e 2073  [s for i, s in s
-00019380: 6567 7320 6966 2069 2069 6e20 6375 7272  egs if i in curr
-00019390: 5f73 6567 5f69 6478 735d 2c0d 0a20 2020  _seg_idxs],..   
-000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193b0: 205f 776f 7264 5f69 6e64 6963 6573 3d63   _word_indices=c
-000193c0: 7572 725f 776f 7264 5f69 6478 732c 0d0a  urr_word_idxs,..
-000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193e0: 2020 2020 5f74 6578 745f 6d61 7463 683d      _text_match=
-000193f0: 6375 7272 5f6d 6174 6368 2e67 726f 7570  curr_match.group
-00019400: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00019410: 2020 2020 2929 0d0a 2020 2020 2020 2020      ))..        
-00019420: 2020 2020 2020 2020 6d61 7463 685f 7365          match_se
-00019430: 675f 696e 6469 6365 732e 6170 7065 6e64  g_indices.append
-00019440: 2863 7572 725f 7365 675f 6964 7873 290d  (curr_seg_idxs).
-00019450: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019460: 5768 6973 7065 7252 6573 756c 744d 6174  WhisperResultMat
-00019470: 6368 6573 286d 6174 6368 6573 2c20 6d61  ches(matches, ma
-00019480: 7463 685f 7365 675f 696e 6469 6365 7329  tch_seg_indices)
-00019490: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6c65  ....    def __le
-000194a0: 6e5f 5f28 7365 6c66 293a 0d0a 2020 2020  n__(self):..    
-000194b0: 2020 2020 7265 7475 726e 206c 656e 2873      return len(s
-000194c0: 656c 662e 6d61 7463 6865 7329 0d0a 0d0a  elf.matches)....
-000194d0: 2020 2020 6465 6620 5f5f 626f 6f6c 5f5f      def __bool__
-000194e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000194f0: 2072 6574 7572 6e20 7365 6c66 2e5f 5f6c   return self.__l
-00019500: 656e 5f5f 2829 2021 3d20 300d 0a0d 0a20  en__() != 0.... 
-00019510: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
-00019520: 5f5f 2873 656c 662c 2069 6478 293a 0d0a  __(self, idx):..
-00019530: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00019540: 656c 662e 6d61 7463 6865 735b 6964 785d  elf.matches[idx]
-00019550: 0d0a                                     ..
+00011a30: 2020 6d61 785f 776f 7264 733d 6d61 785f    max_words=max_
+00011a40: 776f 7264 732c 0d0a 2020 2020 2020 2020  words,..        
+00011a50: 2020 2020 2020 2020 6576 656e 5f73 706c          even_spl
+00011a60: 6974 3d65 7665 6e5f 7370 6c69 742c 0d0a  it=even_split,..
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 696e 636c 7564 655f 6c6f 636b 3d69 6e63  include_lock=inc
+00011a90: 6c75 6465 5f6c 6f63 6b0d 0a20 2020 2020  lude_lock..     
+00011aa0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+00011ab0: 2020 2020 2020 206c 6f63 6b3d 6c6f 636b         lock=lock
+00011ac0: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+00011ad0: 6577 6c69 6e65 3d6e 6577 6c69 6e65 0d0a  ewline=newline..
+00011ae0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00011af0: 2020 2069 6620 7365 6c66 2e5f 7265 6772     if self._regr
+00011b00: 6f75 705f 6869 7374 6f72 793a 0d0a 2020  oup_history:..  
+00011b10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011b20: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
+00011b30: 2b3d 2027 5f27 0d0a 2020 2020 2020 2020  += '_'..        
+00011b40: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
+00011b50: 7374 6f72 7920 2b3d 2028 6627 736c 3d7b  story += (f'sl={
+00011b60: 6d61 785f 6368 6172 7320 6f72 2022 227d  max_chars or ""}
+00011b70: 2b7b 6d61 785f 776f 7264 7320 6f72 2022  +{max_words or "
+00011b80: 227d 2b7b 696e 7428 6576 656e 5f73 706c  "}+{int(even_spl
+00011b90: 6974 297d 2b7b 696e 7428 666f 7263 655f  it)}+{int(force_
+00011ba0: 6c65 6e29 7d27 0d0a 2020 2020 2020 2020  len)}'..        
+00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bc0: 2020 2020 2020 2020 2020 6627 2b7b 696e            f'+{in
+00011bd0: 7428 6c6f 636b 297d 2b7b 696e 7428 696e  t(lock)}+{int(in
+00011be0: 636c 7564 655f 6c6f 636b 297d 2b7b 696e  clude_lock)}+{in
+00011bf0: 7428 6e65 776c 696e 6529 7d27 290d 0a20  t(newline)}').. 
+00011c00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011c10: 6c66 0d0a 0d0a 2020 2020 6465 6620 7370  lf....    def sp
+00011c20: 6c69 745f 6279 5f64 7572 6174 696f 6e28  lit_by_duration(
+00011c30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00011c40: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00011c50: 206d 6178 5f64 7572 3a20 666c 6f61 742c   max_dur: float,
+00011c60: 0d0a 2020 2020 2020 2020 2020 2020 6576  ..            ev
+00011c70: 656e 5f73 706c 6974 3a20 626f 6f6c 203d  en_split: bool =
+00011c80: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
+00011c90: 2020 2020 666f 7263 655f 6c65 6e3a 2062      force_len: b
+00011ca0: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00011cb0: 2020 2020 2020 2020 2020 6c6f 636b 3a20            lock: 
+00011cc0: 626f 6f6c 203d 2046 616c 7365 2c0d 0a20  bool = False,.. 
+00011cd0: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
+00011ce0: 6465 5f6c 6f63 6b3a 2062 6f6f 6c20 3d20  de_lock: bool = 
+00011cf0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00011d00: 2020 2020 6e65 776c 696e 653a 2062 6f6f      newline: boo
+00011d10: 6c20 3d20 4661 6c73 650d 0a20 2020 2029  l = False..    )
+00011d20: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
+00011d30: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
+00011d40: 220d 0a20 2020 2020 2020 2053 706c 6974  "..        Split
+00011d50: 2028 696e 2d70 6c61 6365 2920 616e 7920   (in-place) any 
+00011d60: 7365 676d 656e 7420 7468 6174 2065 7863  segment that exc
+00011d70: 6565 6473 2060 606d 6178 5f64 7572 6060  eeds ``max_dur``
+00011d80: 2069 6e74 6f20 736d 616c 6c65 7220 7365   into smaller se
+00011d90: 676d 656e 7473 2e0d 0a0d 0a20 2020 2020  gments.....     
+00011da0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+00011db0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00011dc0: 2d0d 0a20 2020 2020 2020 206d 6178 5f64  -..        max_d
+00011dd0: 7572 203a 2066 6c6f 6174 0d0a 2020 2020  ur : float..    
+00011de0: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
+00011df0: 6475 7261 7469 6f6e 2028 696e 2073 6563  duration (in sec
+00011e00: 6f6e 6473 2920 7065 7220 7365 676d 656e  onds) per segmen
+00011e10: 742e 0d0a 2020 2020 2020 2020 6576 656e  t...        even
+00011e20: 5f73 706c 6974 203a 2062 6f6f 6c2c 2064  _split : bool, d
+00011e30: 6566 6175 6c74 2054 7275 650d 0a20 2020  efault True..   
+00011e40: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00011e50: 2074 6f20 6576 656e 6c79 2073 706c 6974   to evenly split
+00011e60: 2061 2073 6567 6d65 6e74 2069 6e20 6c65   a segment in le
+00011e70: 6e67 7468 2069 6620 6974 2065 7863 6565  ngth if it excee
+00011e80: 6473 2060 606d 6178 5f64 7572 6060 2e0d  ds ``max_dur``..
+00011e90: 0a20 2020 2020 2020 2066 6f72 6365 5f6c  .        force_l
+00011ea0: 656e 203a 2062 6f6f 6c2c 2064 6566 6175  en : bool, defau
+00011eb0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+00011ec0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00011ed0: 2066 6f72 6365 2061 2063 6f6e 7374 616e   force a constan
+00011ee0: 7420 6c65 6e67 7468 2066 6f72 2065 6163  t length for eac
+00011ef0: 6820 7365 676d 656e 7420 6578 6365 7074  h segment except
+00011f00: 2074 6865 206c 6173 7420 7365 676d 656e   the last segmen
+00011f10: 742e 0d0a 2020 2020 2020 2020 2020 2020  t...            
+00011f20: 5468 6973 2077 696c 6c20 6967 6e6f 7265  This will ignore
+00011f30: 2061 6c6c 2070 7265 7669 6f75 7320 6e6f   all previous no
+00011f40: 6e2d 6c6f 636b 6564 2073 6567 6d65 6e74  n-locked segment
+00011f50: 2062 6f75 6e64 6172 6965 732e 0d0a 2020   boundaries...  
+00011f60: 2020 2020 2020 6c6f 636b 203a 2062 6f6f        lock : boo
+00011f70: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00011f80: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00011f90: 6574 6865 7220 746f 2070 7265 7665 6e74  ether to prevent
+00011fa0: 2066 7574 7572 6520 7370 6c69 7473 2f6d   future splits/m
+00011fb0: 6572 6765 7320 6672 6f6d 2061 6c74 6572  erges from alter
+00011fc0: 696e 6720 6368 616e 6765 7320 6d61 6465  ing changes made
+00011fd0: 2062 7920 7468 6973 206d 6574 686f 642e   by this method.
+00011fe0: 0d0a 2020 2020 2020 2020 696e 636c 7564  ..        includ
+00011ff0: 655f 6c6f 636b 3a20 626f 6f6c 2c20 6465  e_lock: bool, de
+00012000: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+00012010: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00012020: 2074 6f20 696e 636c 7564 6520 7072 6576   to include prev
+00012030: 696f 7573 206c 6f63 6b20 6265 666f 7265  ious lock before
+00012040: 2073 706c 6974 7469 6e67 2062 6173 6564   splitting based
+00012050: 206f 6e20 6d61 785f 776f 7264 732c 2069   on max_words, i
+00012060: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
+00012070: 2046 616c 7365 6060 2e0d 0a20 2020 2020   False``...     
+00012080: 2020 2020 2020 2053 706c 6974 7469 6e67         Splitting
+00012090: 2077 696c 6c20 6265 2064 6f6e 6520 6166   will be done af
+000120a0: 7465 7220 7468 6520 6669 7273 7420 6e6f  ter the first no
+000120b0: 6e2d 6c6f 636b 6564 2077 6f72 6420 3e20  n-locked word > 
+000120c0: 6060 6d61 785f 6475 7260 602e 0d0a 2020  ``max_dur``...  
+000120d0: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
+000120e0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+000120f0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+00012100: 5768 6574 6865 7220 746f 2069 6e73 6572  Whether to inser
+00012110: 7420 6c69 6e65 2062 7265 616b 2061 7420  t line break at 
+00012120: 7468 6520 7370 6c69 7420 706f 696e 7473  the split points
+00012130: 2069 6e73 7465 6164 206f 6620 7370 6c69   instead of spli
+00012140: 7474 696e 6720 696e 746f 2073 6570 6172  tting into separ
+00012150: 6174 6520 7365 676d 656e 7473 2e0d 0a0d  ate segments....
+00012160: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00012170: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00012180: 2d0d 0a20 2020 2020 2020 2073 7461 626c  -..        stabl
+00012190: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+000121a0: 2e57 6869 7370 6572 5265 7375 6c74 0d0a  .WhisperResult..
+000121b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000121c0: 6375 7272 656e 7420 696e 7374 616e 6365  current instance
+000121d0: 2061 6674 6572 2074 6865 2063 6861 6e67   after the chang
+000121e0: 6573 2e0d 0a0d 0a20 2020 2020 2020 204e  es.....        N
+000121f0: 6f74 6573 0d0a 2020 2020 2020 2020 2d2d  otes..        --
+00012200: 2d2d 2d0d 0a20 2020 2020 2020 2049 6620  ---..        If 
+00012210: 6060 6576 656e 5f73 706c 6974 203d 2054  ``even_split = T
+00012220: 7275 6560 602c 2073 6567 6d65 6e74 7320  rue``, segments 
+00012230: 6361 6e20 7374 696c 6c20 6578 6365 6564  can still exceed
+00012240: 2060 606d 6178 5f64 7572 6060 2061 6e64   ``max_dur`` and
+00012250: 206c 6f63 6b65 6420 776f 7264 7320 7769   locked words wi
+00012260: 6c6c 2062 6520 6967 6e6f 7265 6420 746f  ll be ignored to
+00012270: 2061 766f 6964 0d0a 2020 2020 2020 2020   avoid..        
+00012280: 756e 6576 656e 2073 706c 6974 7469 6e67  uneven splitting
+00012290: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+000122a0: 2020 2020 2020 2020 6966 2066 6f72 6365          if force
+000122b0: 5f6c 656e 3a0d 0a20 2020 2020 2020 2020  _len:..         
+000122c0: 2020 2073 656c 662e 6d65 7267 655f 616c     self.merge_al
+000122d0: 6c5f 7365 676d 656e 7473 2829 0d0a 2020  l_segments()..  
+000122e0: 2020 2020 2020 7365 6c66 2e5f 7370 6c69        self._spli
+000122f0: 745f 7365 676d 656e 7473 280d 0a20 2020  t_segments(..   
+00012300: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+00012310: 783a 2078 2e67 6574 5f64 7572 6174 696f  x: x.get_duratio
+00012320: 6e5f 696e 6469 6365 7328 0d0a 2020 2020  n_indices(..    
+00012330: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00012340: 6475 723d 6d61 785f 6475 722c 0d0a 2020  dur=max_dur,..  
+00012350: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00012360: 656e 5f73 706c 6974 3d65 7665 6e5f 7370  en_split=even_sp
+00012370: 6c69 742c 0d0a 2020 2020 2020 2020 2020  lit,..          
+00012380: 2020 2020 2020 696e 636c 7564 655f 6c6f        include_lo
+00012390: 636b 3d69 6e63 6c75 6465 5f6c 6f63 6b0d  ck=include_lock.
+000123a0: 0a20 2020 2020 2020 2020 2020 2029 2c0d  .            ),.
+000123b0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+000123c0: 6b3d 6c6f 636b 2c0d 0a20 2020 2020 2020  k=lock,..       
+000123d0: 2020 2020 206e 6577 6c69 6e65 3d6e 6577       newline=new
+000123e0: 6c69 6e65 0d0a 2020 2020 2020 2020 290d  line..        ).
+000123f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012400: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
+00012410: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00012420: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
+00012430: 7374 6f72 7920 2b3d 2027 5f27 0d0a 2020  story += '_'..  
+00012440: 2020 2020 2020 7365 6c66 2e5f 7265 6772        self._regr
+00012450: 6f75 705f 6869 7374 6f72 7920 2b3d 2028  oup_history += (
+00012460: 6627 7364 3d7b 6d61 785f 6475 727d 2b7b  f'sd={max_dur}+{
+00012470: 696e 7428 6576 656e 5f73 706c 6974 297d  int(even_split)}
+00012480: 2b7b 696e 7428 666f 7263 655f 6c65 6e29  +{int(force_len)
+00012490: 7d27 0d0a 2020 2020 2020 2020 2020 2020  }'..            
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124b0: 2020 2020 2020 6627 2b7b 696e 7428 6c6f        f'+{int(lo
+000124c0: 636b 297d 2b7b 696e 7428 696e 636c 7564  ck)}+{int(includ
+000124d0: 655f 6c6f 636b 297d 2b7b 696e 7428 6e65  e_lock)}+{int(ne
+000124e0: 776c 696e 6529 7d27 290d 0a20 2020 2020  wline)}')..     
+000124f0: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
+00012500: 0d0a 2020 2020 6465 6620 636c 616d 705f  ..    def clamp_
+00012510: 6d61 7828 0d0a 2020 2020 2020 2020 2020  max(..          
+00012520: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00012530: 2020 2020 206d 6564 6975 6d5f 6661 6374       medium_fact
+00012540: 6f72 3a20 666c 6f61 7420 3d20 322e 352c  or: float = 2.5,
+00012550: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+00012560: 785f 6475 723a 2066 6c6f 6174 203d 204e  x_dur: float = N
+00012570: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00012580: 2020 636c 6970 5f73 7461 7274 3a20 4f70    clip_start: Op
+00012590: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+000125a0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+000125b0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+000125c0: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
+000125d0: 3e20 2257 6869 7370 6572 5265 7375 6c74  > "WhisperResult
+000125e0: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
+000125f0: 0a20 2020 2020 2020 2043 6c61 6d70 2061  .        Clamp a
+00012600: 6c6c 2077 6f72 6420 6475 7261 7469 6f6e  ll word duration
+00012610: 7320 6162 6f76 6520 6365 7274 6169 6e20  s above certain 
+00012620: 7661 6c75 652e 0d0a 0d0a 2020 2020 2020  value.....      
+00012630: 2020 5468 6973 2069 7320 6d6f 7374 2065    This is most e
+00012640: 6666 6563 7469 7665 2077 6865 6e20 6170  ffective when ap
+00012650: 706c 6965 6420 6265 666f 7265 2061 6e64  plied before and
+00012660: 2061 6674 6572 206f 7468 6572 2072 6567   after other reg
+00012670: 726f 7570 206f 7065 7261 7469 6f6e 732e  roup operations.
+00012680: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+00012690: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+000126a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+000126b0: 2020 2020 6d65 6469 756d 5f66 6163 746f      medium_facto
+000126c0: 7220 3a20 666c 6f61 742c 2064 6566 6175  r : float, defau
+000126d0: 6c74 2032 2e35 0d0a 2020 2020 2020 2020  lt 2.5..        
+000126e0: 2020 2020 436c 616d 7020 6475 7261 7469      Clamp durati
+000126f0: 6f6e 7320 6162 6f76 6520 2860 606d 6564  ons above (``med
+00012700: 6975 6d5f 6661 6374 6f72 6060 202a 206d  ium_factor`` * m
+00012710: 6564 6975 6d20 6475 7261 7469 6f6e 2920  edium duration) 
+00012720: 7065 7220 7365 676d 656e 742e 0d0a 2020  per segment...  
+00012730: 2020 2020 2020 2020 2020 4966 2060 606d            If ``m
+00012740: 6564 6975 6d5f 6661 6374 6f72 203d 204e  edium_factor = N
+00012750: 6f6e 652f 3060 6020 6f72 2073 6567 6d65  one/0`` or segme
+00012760: 6e74 2068 6173 206c 6573 7320 7468 616e  nt has less than
+00012770: 2033 2077 6f72 6473 2c20 6974 2077 696c   3 words, it wil
+00012780: 6c20 6265 2069 676e 6f72 6564 2061 6e64  l be ignored and
+00012790: 2075 7365 206f 6e6c 7920 6060 6d61 785f   use only ``max_
+000127a0: 6475 7260 602e 0d0a 2020 2020 2020 2020  dur``...        
+000127b0: 6d61 785f 6475 7220 3a20 666c 6f61 742c  max_dur : float,
+000127c0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+000127d0: 2020 2020 2020 2043 6c61 6d70 2064 7572         Clamp dur
+000127e0: 6174 696f 6e73 2061 626f 7665 2060 606d  ations above ``m
+000127f0: 6178 5f64 7572 6060 2e0d 0a20 2020 2020  ax_dur``...     
+00012800: 2020 2063 6c69 705f 7374 6172 7420 3a20     clip_start : 
+00012810: 626f 6f6c 206f 7220 4e6f 6e65 2c20 6465  bool or None, de
+00012820: 6661 756c 7420 4e6f 6e65 0d0a 2020 2020  fault None..    
+00012830: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00012840: 746f 2063 6c61 6d70 2074 6865 2073 7461  to clamp the sta
+00012850: 7274 206f 6620 6120 776f 7264 2e20 4966  rt of a word. If
+00012860: 2060 604e 6f6e 6560 602c 2063 6c61 6d70   ``None``, clamp
+00012870: 2074 6865 2073 7461 7274 206f 6620 6669   the start of fi
+00012880: 7273 7420 776f 7264 2061 6e64 2065 6e64  rst word and end
+00012890: 206f 6620 6c61 7374 2077 6f72 6420 7065   of last word pe
+000128a0: 720d 0a20 2020 2020 2020 2020 2020 2073  r..            s
+000128b0: 6567 6d65 6e74 2e0d 0a20 2020 2020 2020  egment...       
+000128c0: 2076 6572 626f 7365 203a 2062 6f6f 6c2c   verbose : bool,
+000128d0: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+000128e0: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+000128f0: 6865 7220 746f 2070 7269 6e74 206f 7574  her to print out
+00012900: 2074 6865 2074 696d 6573 7461 6d70 2063   the timestamp c
+00012910: 6861 6e67 6573 2e0d 0a0d 0a20 2020 2020  hanges.....     
+00012920: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+00012930: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00012940: 2020 2020 2073 7461 626c 655f 7768 6973       stable_whis
+00012950: 7065 722e 7265 7375 6c74 2e57 6869 7370  per.result.Whisp
+00012960: 6572 5265 7375 6c74 0d0a 2020 2020 2020  erResult..      
+00012970: 2020 2020 2020 5468 6520 6375 7272 656e        The curren
+00012980: 7420 696e 7374 616e 6365 2061 6674 6572  t instance after
+00012990: 2074 6865 2063 6861 6e67 6573 2e0d 0a20   the changes... 
+000129a0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000129b0: 2020 2020 6966 206e 6f74 2028 6d65 6469      if not (medi
+000129c0: 756d 5f66 6163 746f 7220 6f72 206d 6178  um_factor or max
+000129d0: 5f64 7572 293a 0d0a 2020 2020 2020 2020  _dur):..        
+000129e0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000129f0: 7272 6f72 2827 4174 206c 6561 7374 206f  rror('At least o
+00012a00: 6e65 206f 6620 666f 6c6c 6f77 696e 6720  ne of following 
+00012a10: 6172 6775 6d65 6e74 7320 7265 7175 6972  arguments requir
+00012a20: 6573 206e 6f6e 2d7a 6572 6f20 7661 6c75  es non-zero valu
+00012a30: 653a 206d 6564 6975 6d5f 6661 6374 6f72  e: medium_factor
+00012a40: 3b20 6d61 785f 6475 7227 290d 0a0d 0a20  ; max_dur').... 
+00012a50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00012a60: 6c66 2e68 6173 5f77 6f72 6473 3a0d 0a20  lf.has_words:.. 
+00012a70: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00012a80: 6e67 732e 7761 726e 2827 4361 6e6e 6f74  ngs.warn('Cannot
+00012a90: 2063 6c61 6d70 2064 7565 2074 6f20 6d69   clamp due to mi
+00012aa0: 7373 696e 672f 6e6f 2077 6f72 642d 7469  ssing/no word-ti
+00012ab0: 6d65 7374 616d 7073 2729 0d0a 2020 2020  mestamps')..    
+00012ac0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00012ad0: 656c 660d 0a0d 0a20 2020 2020 2020 2066  elf....        f
+00012ae0: 6f72 2073 6567 2069 6e20 7365 6c66 2e73  or seg in self.s
+00012af0: 6567 6d65 6e74 733a 0d0a 2020 2020 2020  egments:..      
+00012b00: 2020 2020 2020 6375 7272 5f6d 6178 5f64        curr_max_d
+00012b10: 7572 203d 204e 6f6e 650d 0a20 2020 2020  ur = None..     
+00012b20: 2020 2020 2020 2069 6620 6d65 6469 756d         if medium
+00012b30: 5f66 6163 746f 7220 616e 6420 6c65 6e28  _factor and len(
+00012b40: 7365 672e 776f 7264 7329 203e 2032 3a0d  seg.words) > 2:.
+00012b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b60: 2064 7572 6174 696f 6e73 203d 206e 702e   durations = np.
+00012b70: 6172 7261 7928 5b77 6f72 642e 6475 7261  array([word.dura
+00012b80: 7469 6f6e 2066 6f72 2077 6f72 6420 696e  tion for word in
+00012b90: 2073 6567 2e77 6f72 6473 5d29 0d0a 2020   seg.words])..  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 6475                du
+00012bb0: 7261 7469 6f6e 732e 736f 7274 2829 0d0a  rations.sort()..
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 6375 7272 5f6d 6178 5f64 7572 203d 206d  curr_max_dur = m
+00012be0: 6564 6975 6d5f 6661 6374 6f72 202a 2064  edium_factor * d
+00012bf0: 7572 6174 696f 6e73 5b6c 656e 2864 7572  urations[len(dur
+00012c00: 6174 696f 6e73 292f 2f32 202b 2031 5d0d  ations)//2 + 1].
+00012c10: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00012c20: 6620 6d61 785f 6475 7220 616e 6420 286e  f max_dur and (n
+00012c30: 6f74 2063 7572 725f 6d61 785f 6475 7220  ot curr_max_dur 
+00012c40: 6f72 2063 7572 725f 6d61 785f 6475 7220  or curr_max_dur 
+00012c50: 3e20 6d61 785f 6475 7229 3a0d 0a20 2020  > max_dur):..   
+00012c60: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012c70: 725f 6d61 785f 6475 7220 3d20 6d61 785f  r_max_dur = max_
+00012c80: 6475 720d 0a0d 0a20 2020 2020 2020 2020  dur....         
+00012c90: 2020 2069 6620 6e6f 7420 6375 7272 5f6d     if not curr_m
+00012ca0: 6178 5f64 7572 3a0d 0a20 2020 2020 2020  ax_dur:..       
+00012cb0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00012cc0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+00012cd0: 2069 6620 636c 6970 5f73 7461 7274 2069   if clip_start i
+00012ce0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00012cf0: 2020 2020 2020 2020 2073 6567 2e77 6f72           seg.wor
+00012d00: 6473 5b30 5d2e 636c 616d 705f 6d61 7828  ds[0].clamp_max(
+00012d10: 6375 7272 5f6d 6178 5f64 7572 2c20 636c  curr_max_dur, cl
+00012d20: 6970 5f73 7461 7274 3d54 7275 652c 2076  ip_start=True, v
+00012d30: 6572 626f 7365 3d76 6572 626f 7365 290d  erbose=verbose).
+00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d50: 2073 6567 2e77 6f72 6473 5b2d 315d 2e63   seg.words[-1].c
+00012d60: 6c61 6d70 5f6d 6178 2863 7572 725f 6d61  lamp_max(curr_ma
+00012d70: 785f 6475 722c 2063 6c69 705f 7374 6172  x_dur, clip_star
+00012d80: 743d 4661 6c73 652c 2076 6572 626f 7365  t=False, verbose
+00012d90: 3d76 6572 626f 7365 290d 0a20 2020 2020  =verbose)..     
+00012da0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00012db0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00012dc0: 7220 692c 2077 6f72 6420 696e 2065 6e75  r i, word in enu
+00012dd0: 6d65 7261 7465 2873 6567 2e77 6f72 6473  merate(seg.words
+00012de0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00012df0: 2020 2020 2020 2020 776f 7264 2e63 6c61          word.cla
+00012e00: 6d70 5f6d 6178 2863 7572 725f 6d61 785f  mp_max(curr_max_
+00012e10: 6475 722c 2063 6c69 705f 7374 6172 743d  dur, clip_start=
+00012e20: 636c 6970 5f73 7461 7274 2c20 7665 7262  clip_start, verb
+00012e30: 6f73 653d 7665 7262 6f73 6529 0d0a 0d0a  ose=verbose)....
+00012e40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012e50: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+00012e60: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00012e70: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+00012e80: 746f 7279 202b 3d20 275f 270d 0a20 2020  tory += '_'..   
+00012e90: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+00012ea0: 7570 5f68 6973 746f 7279 202b 3d20 6627  up_history += f'
+00012eb0: 636d 3d7b 6d65 6469 756d 5f66 6163 746f  cm={medium_facto
+00012ec0: 727d 2b7b 6d61 785f 6475 7220 6f72 2022  r}+{max_dur or "
+00012ed0: 227d 2b7b 636c 6970 5f73 7461 7274 206f  "}+{clip_start o
+00012ee0: 7220 2222 7d2b 7b69 6e74 2876 6572 626f  r ""}+{int(verbo
+00012ef0: 7365 297d 270d 0a20 2020 2020 2020 2072  se)}'..        r
+00012f00: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+00012f10: 2020 6465 6620 6c6f 636b 280d 0a20 2020    def lock(..   
+00012f20: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+00012f30: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00012f40: 7473 7769 7468 3a20 556e 696f 6e5b 7374  tswith: Union[st
+00012f50: 722c 204c 6973 745b 7374 725d 5d20 3d20  r, List[str]] = 
+00012f60: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00012f70: 2020 2065 6e64 7377 6974 683a 2055 6e69     endswith: Uni
+00012f80: 6f6e 5b73 7472 2c20 4c69 7374 5b73 7472  on[str, List[str
+00012f90: 5d5d 203d 204e 6f6e 652c 0d0a 2020 2020  ]] = None,..    
+00012fa0: 2020 2020 2020 2020 7269 6768 743a 2062          right: b
+00012fb0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00012fc0: 2020 2020 2020 2020 206c 6566 743a 2062           left: b
+00012fd0: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
+00012fe0: 2020 2020 2020 2020 2020 6361 7365 5f73            case_s
+00012ff0: 656e 7369 7469 7665 3a20 626f 6f6c 203d  ensitive: bool =
+00013000: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+00013010: 2020 2020 2073 7472 6970 3a20 626f 6f6c       strip: bool
+00013020: 203d 2054 7275 650d 0a20 2020 2029 202d   = True..    ) -
+00013030: 3e20 2257 6869 7370 6572 5265 7375 6c74  > "WhisperResult
+00013040: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
+00013050: 0a20 2020 2020 2020 204c 6f63 6b20 776f  .        Lock wo
+00013060: 7264 732f 7365 676d 656e 7473 2077 6974  rds/segments wit
+00013070: 6820 6d61 7463 6869 6e67 2070 7265 6669  h matching prefi
+00013080: 782f 7375 6666 6978 2074 6f20 7072 6576  x/suffix to prev
+00013090: 656e 7420 7370 6c69 7474 696e 672f 6d65  ent splitting/me
+000130a0: 7267 696e 672e 0d0a 0d0a 2020 2020 2020  rging.....      
+000130b0: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+000130c0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000130d0: 0d0a 2020 2020 2020 2020 7374 6172 7473  ..        starts
+000130e0: 7769 7468 3a20 7374 7220 6f72 206c 6973  with: str or lis
+000130f0: 7420 6f66 2073 7472 0d0a 2020 2020 2020  t of str..      
+00013100: 2020 2020 2020 5072 6566 6978 6573 2074        Prefixes t
+00013110: 6f20 6c6f 636b 2e0d 0a20 2020 2020 2020  o lock...       
+00013120: 2065 6e64 7377 6974 683a 2073 7472 206f   endswith: str o
+00013130: 7220 6c69 7374 206f 6620 7374 720d 0a20  r list of str.. 
+00013140: 2020 2020 2020 2020 2020 2053 7566 6669             Suffi
+00013150: 7865 7320 746f 206c 6f63 6b2e 0d0a 2020  xes to lock...  
+00013160: 2020 2020 2020 7269 6768 7420 3a20 626f        right : bo
+00013170: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00013180: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00013190: 6574 6865 7220 7072 6576 656e 7420 7370  ether prevent sp
+000131a0: 6c69 7473 2f6d 6572 6765 7320 7769 7468  lits/merges with
+000131b0: 2074 6865 206e 6578 7420 776f 7264 2f73   the next word/s
+000131c0: 6567 6d65 6e74 2e0d 0a20 2020 2020 2020  egment...       
+000131d0: 206c 6566 7420 3a20 626f 6f6c 2c20 6465   left : bool, de
+000131e0: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+000131f0: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00013200: 2070 7265 7665 6e74 2073 706c 6974 732f   prevent splits/
+00013210: 6d65 7267 6573 2077 6974 6820 7468 6520  merges with the 
+00013220: 7072 6576 696f 7573 2077 6f72 642f 7365  previous word/se
+00013230: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
+00013240: 6361 7365 5f73 656e 7369 7469 7665 203a  case_sensitive :
+00013250: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00013260: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00013270: 2020 5768 6574 6865 7220 746f 206d 6174    Whether to mat
+00013280: 6368 2074 6865 2063 6173 6520 6f66 2074  ch the case of t
+00013290: 6865 2070 7265 6669 7865 732f 7375 6666  he prefixes/suff
+000132a0: 6978 6573 2077 6974 6820 7468 6520 776f  ixes with the wo
+000132b0: 7264 732f 7365 676d 656e 7473 2e0d 0a20  rds/segments... 
+000132c0: 2020 2020 2020 2073 7472 6970 203a 2062         strip : b
+000132d0: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+000132e0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+000132f0: 6865 7468 6572 2074 6f20 6967 6e6f 7265  hether to ignore
+00013300: 2073 7061 6365 7320 6265 666f 7265 2061   spaces before a
+00013310: 6e64 2061 6674 6572 2062 6f74 6820 776f  nd after both wo
+00013320: 7264 732f 7365 676d 656e 7473 2061 6e64  rds/segments and
+00013330: 2070 7265 6669 7865 732f 7375 6666 6978   prefixes/suffix
+00013340: 6573 2e0d 0a0d 0a20 2020 2020 2020 2052  es.....        R
+00013350: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+00013360: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00013370: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
+00013380: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
+00013390: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
+000133a0: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
+000133b0: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
+000133c0: 2063 6861 6e67 6573 2e0d 0a20 2020 2020   changes...     
+000133d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000133e0: 6173 7365 7274 2073 7461 7274 7377 6974  assert startswit
+000133f0: 6820 6f72 2065 6e64 7377 6974 682c 2027  h or endswith, '
+00013400: 4d75 7374 2073 7065 6369 6679 205b 7374  Must specify [st
+00013410: 6172 7473 7769 7468 5d20 6f72 2f61 6e64  artswith] or/and
+00013420: 205b 656e 6473 7769 7468 5d2e 270d 0a20   [endswith].'.. 
+00013430: 2020 2020 2020 2073 7461 7274 7377 6974         startswit
+00013440: 6820 3d20 5b5d 2069 6620 7374 6172 7473  h = [] if starts
+00013450: 7769 7468 2069 7320 4e6f 6e65 2065 6c73  with is None els
+00013460: 6520 285b 7374 6172 7473 7769 7468 5d20  e ([startswith] 
+00013470: 6966 2069 7369 6e73 7461 6e63 6528 7374  if isinstance(st
+00013480: 6172 7473 7769 7468 2c20 7374 7229 2065  artswith, str) e
+00013490: 6c73 6520 7374 6172 7473 7769 7468 290d  lse startswith).
+000134a0: 0a20 2020 2020 2020 2065 6e64 7377 6974  .        endswit
+000134b0: 6820 3d20 5b5d 2069 6620 656e 6473 7769  h = [] if endswi
+000134c0: 7468 2069 7320 4e6f 6e65 2065 6c73 6520  th is None else 
+000134d0: 285b 656e 6473 7769 7468 5d20 6966 2069  ([endswith] if i
+000134e0: 7369 6e73 7461 6e63 6528 656e 6473 7769  sinstance(endswi
+000134f0: 7468 2c20 7374 7229 2065 6c73 6520 656e  th, str) else en
+00013500: 6473 7769 7468 290d 0a20 2020 2020 2020  dswith)..       
+00013510: 2069 6620 6e6f 7420 6361 7365 5f73 656e   if not case_sen
+00013520: 7369 7469 7665 3a0d 0a20 2020 2020 2020  sitive:..       
+00013530: 2020 2020 2073 7461 7274 7377 6974 6820       startswith 
+00013540: 3d20 5b74 2e6c 6f77 6572 2829 2066 6f72  = [t.lower() for
+00013550: 2074 2069 6e20 7374 6172 7473 7769 7468   t in startswith
+00013560: 5d0d 0a20 2020 2020 2020 2020 2020 2065  ]..            e
+00013570: 6e64 7377 6974 6820 3d20 5b74 2e6c 6f77  ndswith = [t.low
+00013580: 6572 2829 2066 6f72 2074 2069 6e20 656e  er() for t in en
+00013590: 6473 7769 7468 5d0d 0a20 2020 2020 2020  dswith]..       
+000135a0: 2069 6620 7374 7269 703a 0d0a 2020 2020   if strip:..    
+000135b0: 2020 2020 2020 2020 7374 6172 7473 7769          startswi
+000135c0: 7468 203d 205b 742e 7374 7269 7028 2920  th = [t.strip() 
+000135d0: 666f 7220 7420 696e 2073 7461 7274 7377  for t in startsw
+000135e0: 6974 685d 0d0a 2020 2020 2020 2020 2020  ith]..          
+000135f0: 2020 656e 6473 7769 7468 203d 205b 742e    endswith = [t.
+00013600: 7374 7269 7028 2920 666f 7220 7420 696e  strip() for t in
+00013610: 2065 6e64 7377 6974 685d 0d0a 2020 2020   endswith]..    
+00013620: 2020 2020 666f 7220 7061 7274 2069 6e20      for part in 
+00013630: 7365 6c66 2e61 6c6c 5f77 6f72 6473 5f6f  self.all_words_o
+00013640: 725f 7365 676d 656e 7473 2829 3a0d 0a20  r_segments():.. 
+00013650: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+00013660: 3d20 7061 7274 2e77 6f72 6420 6966 2068  = part.word if h
+00013670: 6173 6174 7472 2870 6172 742c 2027 776f  asattr(part, 'wo
+00013680: 7264 2729 2065 6c73 6520 7061 7274 2e74  rd') else part.t
+00013690: 6578 740d 0a20 2020 2020 2020 2020 2020  ext..           
+000136a0: 2069 6620 6e6f 7420 6361 7365 5f73 656e   if not case_sen
+000136b0: 7369 7469 7665 3a0d 0a20 2020 2020 2020  sitive:..       
+000136c0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+000136d0: 7465 7874 2e6c 6f77 6572 2829 0d0a 2020  text.lower()..  
+000136e0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+000136f0: 6970 3a0d 0a20 2020 2020 2020 2020 2020  ip:..           
+00013700: 2020 2020 2074 6578 7420 3d20 7465 7874       text = text
+00013710: 2e73 7472 6970 2829 0d0a 2020 2020 2020  .strip()..      
+00013720: 2020 2020 2020 666f 7220 7072 6566 6978        for prefix
+00013730: 2069 6e20 7374 6172 7473 7769 7468 3a0d   in startswith:.
+00013740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013750: 2069 6620 7465 7874 2e73 7461 7274 7377   if text.startsw
+00013760: 6974 6828 7072 6566 6978 293a 0d0a 2020  ith(prefix):..  
+00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013780: 2020 6966 2072 6967 6874 3a0d 0a20 2020    if right:..   
+00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137a0: 2020 2020 2070 6172 742e 6c6f 636b 5f72       part.lock_r
+000137b0: 6967 6874 2829 0d0a 2020 2020 2020 2020  ight()..        
+000137c0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000137d0: 6566 743a 0d0a 2020 2020 2020 2020 2020  eft:..          
+000137e0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+000137f0: 7274 2e6c 6f63 6b5f 6c65 6674 2829 0d0a  rt.lock_left()..
+00013800: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00013810: 7375 6666 6978 2069 6e20 656e 6473 7769  suffix in endswi
+00013820: 7468 3a0d 0a20 2020 2020 2020 2020 2020  th:..           
+00013830: 2020 2020 2069 6620 7465 7874 2e65 6e64       if text.end
+00013840: 7377 6974 6828 7375 6666 6978 293a 0d0a  swith(suffix):..
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 2020 2020 6966 2072 6967 6874 3a0d 0a20      if right:.. 
+00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013880: 2020 2020 2020 2070 6172 742e 6c6f 636b         part.lock
+00013890: 5f72 6967 6874 2829 0d0a 2020 2020 2020  _right()..      
+000138a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000138b0: 206c 6566 743a 0d0a 2020 2020 2020 2020   left:..        
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 7061 7274 2e6c 6f63 6b5f 6c65 6674 2829  part.lock_left()
+000138e0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+000138f0: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
+00013900: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00013910: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+00013920: 6973 746f 7279 202b 3d20 275f 270d 0a20  istory += '_'.. 
+00013930: 2020 2020 2020 2073 7461 7274 7377 6974         startswit
+00013940: 685f 7374 7220 3d20 2873 7461 7274 7377  h_str = (startsw
+00013950: 6974 6820 6966 2069 7369 6e73 7461 6e63  ith if isinstanc
+00013960: 6528 7374 6172 7473 7769 7468 2c20 7374  e(startswith, st
+00013970: 7229 2065 6c73 6520 272f 272e 6a6f 696e  r) else '/'.join
+00013980: 2873 7461 7274 7377 6974 6829 2920 6966  (startswith)) if
+00013990: 2073 7461 7274 7377 6974 6820 656c 7365   startswith else
+000139a0: 2022 220d 0a20 2020 2020 2020 2065 6e64   ""..        end
+000139b0: 7377 6974 685f 7374 7220 3d20 2865 6e64  swith_str = (end
+000139c0: 7377 6974 6820 6966 2069 7369 6e73 7461  swith if isinsta
+000139d0: 6e63 6528 656e 6473 7769 7468 2c20 7374  nce(endswith, st
+000139e0: 7229 2065 6c73 6520 272f 272e 6a6f 696e  r) else '/'.join
+000139f0: 2865 6e64 7377 6974 6829 2920 6966 2065  (endswith)) if e
+00013a00: 6e64 7377 6974 6820 656c 7365 2022 220d  ndswith else "".
+00013a10: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00013a20: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
+00013a30: 3d20 2866 276c 3d7b 7374 6172 7473 7769  = (f'l={startswi
+00013a40: 7468 5f73 7472 7d2b 7b65 6e64 7377 6974  th_str}+{endswit
+00013a50: 685f 7374 727d 270d 0a20 2020 2020 2020  h_str}'..       
+00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a70: 2020 2020 2020 2020 2020 2066 272b 7b69             f'+{i
+00013a80: 6e74 2872 6967 6874 297d 2b7b 696e 7428  nt(right)}+{int(
+00013a90: 6c65 6674 297d 2b7b 696e 7428 6361 7365  left)}+{int(case
+00013aa0: 5f73 656e 7369 7469 7665 297d 2b7b 696e  _sensitive)}+{in
+00013ab0: 7428 7374 7269 7029 7d27 290d 0a20 2020  t(strip)}')..   
+00013ac0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00013ad0: 0d0a 0d0a 2020 2020 6465 6620 7265 6d6f  ....    def remo
+00013ae0: 7665 5f77 6f72 6428 0d0a 2020 2020 2020  ve_word(..      
+00013af0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00013b00: 2020 2020 2020 2020 2077 6f72 643a 2055           word: U
+00013b10: 6e69 6f6e 5b57 6f72 6454 696d 696e 672c  nion[WordTiming,
+00013b20: 2054 7570 6c65 5b69 6e74 2c20 696e 745d   Tuple[int, int]
+00013b30: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00013b40: 7265 6173 7369 676e 5f69 6473 3a20 626f  reassign_ids: bo
+00013b50: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+00013b60: 2020 2020 2020 2020 7665 7262 6f73 653a          verbose:
+00013b70: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
+00013b80: 2020 2920 2d3e 2027 5768 6973 7065 7252    ) -> 'WhisperR
+00013b90: 6573 756c 7427 3a0d 0a20 2020 2020 2020  esult':..       
+00013ba0: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
+00013bb0: 6d6f 7665 2061 2077 6f72 642e 0d0a 0d0a  move a word.....
+00013bc0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00013bd0: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+00013be0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00013bf0: 776f 7264 203a 2057 6f72 6454 696d 696e  word : WordTimin
+00013c00: 6720 6f72 2074 7570 6c65 206f 6620 2869  g or tuple of (i
+00013c10: 6e74 2c20 696e 7429 0d0a 2020 2020 2020  nt, int)..      
+00013c20: 2020 2020 2020 496e 7374 616e 6365 206f        Instance o
+00013c30: 6620 3a63 6c61 7373 3a60 7374 6162 6c65  f :class:`stable
+00013c40: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+00013c50: 576f 7264 5469 6d69 6e67 6020 6f72 2074  WordTiming` or t
+00013c60: 7570 6c65 206f 6620 2873 6567 6d65 6e74  uple of (segment
+00013c70: 2069 6e64 6578 2c20 776f 7264 2069 6e64   index, word ind
+00013c80: 6578 292e 0d0a 2020 2020 2020 2020 7265  ex)...        re
+00013c90: 6173 7369 676e 5f69 6473 203a 2062 6f6f  assign_ids : boo
+00013ca0: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
+00013cb0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00013cc0: 7468 6572 2074 6f20 7265 6173 7369 676e  ther to reassign
+00013cd0: 2073 6567 6d65 6e74 2061 6e64 2077 6f72   segment and wor
+00013ce0: 6420 6964 7320 2869 6e64 6963 6573 2920  d ids (indices) 
+00013cf0: 6166 7465 7220 7265 6d6f 7669 6e67 2060  after removing `
+00013d00: 6077 6f72 6460 602e 0d0a 2020 2020 2020  `word``...      
+00013d10: 2020 7665 7262 6f73 6520 3a20 626f 6f6c    verbose : bool
+00013d20: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
+00013d30: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00013d40: 6865 7220 746f 2070 7269 6e74 2064 6574  her to print det
+00013d50: 6169 6c20 6f66 2074 6865 2072 656d 6f76  ail of the remov
+00013d60: 6564 2077 6f72 642e 0d0a 0d0a 2020 2020  ed word.....    
+00013d70: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+00013d80: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+00013d90: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
+00013da0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+00013db0: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
+00013dc0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+00013dd0: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
+00013de0: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
+00013df0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00013e00: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00013e10: 6365 2877 6f72 642c 2057 6f72 6454 696d  ce(word, WordTim
+00013e20: 696e 6729 3a0d 0a20 2020 2020 2020 2020  ing):..         
+00013e30: 2020 2069 6620 7365 6c66 5b77 6f72 642e     if self[word.
+00013e40: 7365 676d 656e 745f 6964 5d5b 776f 7264  segment_id][word
+00013e50: 2e69 645d 2069 7320 6e6f 7420 776f 7264  .id] is not word
+00013e60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00013e70: 2020 2073 656c 662e 7265 6173 7369 676e     self.reassign
+00013e80: 5f69 6473 2829 0d0a 2020 2020 2020 2020  _ids()..        
+00013e90: 2020 2020 2020 2020 6966 2073 656c 665b          if self[
+00013ea0: 776f 7264 2e73 6567 6d65 6e74 5f69 645d  word.segment_id]
+00013eb0: 5b77 6f72 642e 6964 5d20 6973 206e 6f74  [word.id] is not
+00013ec0: 2077 6f72 643a 0d0a 2020 2020 2020 2020   word:..        
+00013ed0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00013ee0: 6520 5661 6c75 6545 7272 6f72 2827 776f  e ValueError('wo
+00013ef0: 7264 206e 6f74 2069 6e20 7265 7375 6c74  rd not in result
+00013f00: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00013f10: 7365 675f 6964 2c20 776f 7264 5f69 6420  seg_id, word_id 
+00013f20: 3d20 776f 7264 2e73 6567 6d65 6e74 5f69  = word.segment_i
+00013f30: 642c 2077 6f72 642e 6964 0d0a 2020 2020  d, word.id..    
+00013f40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00013f50: 2020 2020 2020 2073 6567 5f69 642c 2077         seg_id, w
+00013f60: 6f72 645f 6964 203d 2077 6f72 640d 0a20  ord_id = word.. 
+00013f70: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
+00013f80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00013f90: 7072 696e 7428 6627 5265 6d6f 7665 643a  print(f'Removed:
+00013fa0: 207b 7365 6c66 5b73 6567 5f69 645d 5b77   {self[seg_id][w
+00013fb0: 6f72 645f 6964 5d2e 746f 5f64 6963 7428  ord_id].to_dict(
+00013fc0: 297d 2729 0d0a 2020 2020 2020 2020 6465  )}')..        de
+00013fd0: 6c20 7365 6c66 2e73 6567 6d65 6e74 735b  l self.segments[
+00013fe0: 7365 675f 6964 5d2e 776f 7264 735b 776f  seg_id].words[wo
+00013ff0: 7264 5f69 645d 0d0a 2020 2020 2020 2020  rd_id]..        
+00014000: 6966 206e 6f74 2072 6561 7373 6967 6e5f  if not reassign_
+00014010: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+00014020: 2020 7265 7475 726e 2073 656c 660d 0a20    return self.. 
+00014030: 2020 2020 2020 2069 6620 7365 6c66 5b73         if self[s
+00014040: 6567 5f69 645d 2e68 6173 5f77 6f72 6473  eg_id].has_words
+00014050: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00014060: 656c 665b 7365 675f 6964 5d2e 7265 6173  elf[seg_id].reas
+00014070: 7369 676e 5f69 6473 2829 0d0a 2020 2020  sign_ids()..    
+00014080: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00014090: 2020 2020 2020 2073 656c 662e 7265 6d6f         self.remo
+000140a0: 7665 5f6e 6f5f 776f 7264 5f73 6567 6d65  ve_no_word_segme
+000140b0: 6e74 7328 290d 0a20 2020 2020 2020 2072  nts()..        r
+000140c0: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+000140d0: 2020 6465 6620 7265 6d6f 7665 5f73 6567    def remove_seg
+000140e0: 6d65 6e74 280d 0a20 2020 2020 2020 2020  ment(..         
+000140f0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+00014100: 2020 2020 2020 7365 676d 656e 743a 2055        segment: U
+00014110: 6e69 6f6e 5b53 6567 6d65 6e74 2c20 696e  nion[Segment, in
+00014120: 745d 2c0d 0a20 2020 2020 2020 2020 2020  t],..           
+00014130: 2072 6561 7373 6967 6e5f 6964 733a 2062   reassign_ids: b
+00014140: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00014150: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+00014160: 3a20 626f 6f6c 203d 2054 7275 650d 0a20  : bool = True.. 
+00014170: 2020 2029 202d 3e20 2757 6869 7370 6572     ) -> 'Whisper
+00014180: 5265 7375 6c74 273a 0d0a 2020 2020 2020  Result':..      
+00014190: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
+000141a0: 656d 6f76 6520 6120 7365 676d 656e 742e  emove a segment.
+000141b0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+000141c0: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+000141d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+000141e0: 2020 2020 7365 676d 656e 7420 3a20 5365      segment : Se
+000141f0: 676d 656e 7420 6f72 2069 6e74 0d0a 2020  gment or int..  
+00014200: 2020 2020 2020 2020 2020 496e 7374 616e            Instan
+00014210: 6365 203a 636c 6173 733a 6073 7461 626c  ce :class:`stabl
+00014220: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+00014230: 2e53 6567 6d65 6e74 6020 6f72 2073 6567  .Segment` or seg
+00014240: 6d65 6e74 2069 6e64 6578 2e0d 0a20 2020  ment index...   
+00014250: 2020 2020 2072 6561 7373 6967 6e5f 6964       reassign_id
+00014260: 7320 3a20 626f 6f6c 2c20 6465 6661 756c  s : bool, defaul
+00014270: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+00014280: 2020 2020 5768 6574 6865 7220 746f 2072      Whether to r
+00014290: 6561 7373 6967 6e20 7365 676d 656e 7420  eassign segment 
+000142a0: 4944 7320 2869 6e64 6963 6573 2920 6166  IDs (indices) af
+000142b0: 7465 7220 7265 6d6f 7669 6e67 2060 6073  ter removing ``s
+000142c0: 6567 6d65 6e74 6060 2e0d 0a20 2020 2020  egment``...     
+000142d0: 2020 2076 6572 626f 7365 203a 2062 6f6f     verbose : boo
+000142e0: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
+000142f0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00014300: 7468 6572 2074 6f20 7072 696e 7420 6465  ther to print de
+00014310: 7461 696c 206f 6620 7468 6520 7265 6d6f  tail of the remo
+00014320: 7665 6420 776f 7264 2e0d 0a0d 0a20 2020  ved word.....   
+00014330: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00014340: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00014350: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+00014360: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+00014370: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
+00014380: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+00014390: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
+000143a0: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
+000143b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000143c0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000143d0: 6e63 6528 7365 676d 656e 742c 2053 6567  nce(segment, Seg
+000143e0: 6d65 6e74 293a 0d0a 2020 2020 2020 2020  ment):..        
+000143f0: 2020 2020 6966 2073 656c 665b 7365 676d      if self[segm
+00014400: 656e 742e 6964 5d20 6973 206e 6f74 2073  ent.id] is not s
+00014410: 6567 6d65 6e74 3a0d 0a20 2020 2020 2020  egment:..       
+00014420: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00014430: 6173 7369 676e 5f69 6473 2829 0d0a 2020  assign_ids()..  
+00014440: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014450: 2073 656c 665b 7365 676d 656e 742e 6964   self[segment.id
+00014460: 5d20 6973 206e 6f74 2073 6567 6d65 6e74  ] is not segment
+00014470: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014480: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00014490: 7565 4572 726f 7228 2773 6567 6d65 6e74  ueError('segment
+000144a0: 206e 6f74 2069 6e20 7265 7375 6c74 2729   not in result')
+000144b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000144c0: 676d 656e 7420 3d20 7365 676d 656e 742e  gment = segment.
+000144d0: 6964 0d0a 2020 2020 2020 2020 6966 2076  id..        if v
+000144e0: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+000144f0: 2020 2020 2070 7269 6e74 2866 2752 656d       print(f'Rem
+00014500: 6f76 6564 3a20 5b69 643a 7b73 656c 665b  oved: [id:{self[
+00014510: 7365 676d 656e 745d 2e69 647d 5d20 7b73  segment].id}] {s
+00014520: 656c 665b 7365 676d 656e 745d 2e74 6f5f  elf[segment].to_
+00014530: 6469 7370 6c61 795f 7374 7228 5472 7565  display_str(True
+00014540: 297d 2729 0d0a 2020 2020 2020 2020 6465  )}')..        de
+00014550: 6c20 7365 6c66 2e73 6567 6d65 6e74 735b  l self.segments[
+00014560: 7365 676d 656e 745d 0d0a 2020 2020 2020  segment]..      
+00014570: 2020 6966 206e 6f74 2072 6561 7373 6967    if not reassig
+00014580: 6e5f 6964 733a 0d0a 2020 2020 2020 2020  n_ids:..        
+00014590: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+000145a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000145b0: 6173 7369 676e 5f69 6473 2854 7275 652c  assign_ids(True,
+000145c0: 2073 7461 7274 3d73 6567 6d65 6e74 290d   start=segment).
+000145d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000145e0: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
+000145f0: 7265 6d6f 7665 5f72 6570 6574 6974 696f  remove_repetitio
+00014600: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
+00014610: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00014620: 2020 206d 6178 5f77 6f72 6473 3a20 696e     max_words: in
+00014630: 7420 3d20 312c 0d0a 2020 2020 2020 2020  t = 1,..        
+00014640: 2020 2020 6361 7365 5f73 656e 7369 7469      case_sensiti
+00014650: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
+00014660: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00014670: 7472 6970 3a20 626f 6f6c 203d 2054 7275  trip: bool = Tru
+00014680: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00014690: 6967 6e6f 7265 5f70 756e 6374 7561 7469  ignore_punctuati
+000146a0: 6f6e 733a 2073 7472 203d 2022 5c22 272c  ons: str = "\"',
+000146b0: 2e3f 2122 2c0d 0a20 2020 2020 2020 2020  .?!",..         
+000146c0: 2020 2065 7874 656e 645f 6475 7261 7469     extend_durati
+000146d0: 6f6e 3a20 626f 6f6c 203d 2054 7275 652c  on: bool = True,
+000146e0: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+000146f0: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
+00014700: 7565 0d0a 2020 2020 2920 2d3e 2027 5768  ue..    ) -> 'Wh
+00014710: 6973 7065 7252 6573 756c 7427 3a0d 0a20  isperResult':.. 
+00014720: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00014730: 2020 2020 5265 6d6f 7665 2077 6f72 6473      Remove words
+00014740: 2074 6861 7420 7265 7065 6174 2063 6f6e   that repeat con
+00014750: 7365 6375 7469 7665 6c79 2e0d 0a0d 0a20  secutively..... 
+00014760: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00014770: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00014780: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 206d  -----..        m
+00014790: 6178 5f77 6f72 6473 203a 2069 6e74 0d0a  ax_words : int..
+000147a0: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
+000147b0: 6d75 6d20 6e75 6d62 6572 206f 6620 776f  mum number of wo
+000147c0: 7264 7320 746f 206c 6f6f 6b20 666f 7220  rds to look for 
+000147d0: 636f 6e73 6563 7574 6976 656c 792e 0d0a  consecutively...
+000147e0: 2020 2020 2020 2020 6361 7365 5f73 656e          case_sen
+000147f0: 7369 7469 7665 203a 2062 6f6f 6c2c 2064  sitive : bool, d
+00014800: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
+00014810: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+00014820: 7220 7468 6520 6361 7365 206f 6620 776f  r the case of wo
+00014830: 7264 7320 6e65 6564 2074 6f20 6d61 7463  rds need to matc
+00014840: 6820 746f 2062 6520 636f 6e73 6964 6572  h to be consider
+00014850: 6564 2061 7320 7265 7065 7469 7469 6f6e  ed as repetition
+00014860: 2e0d 0a20 2020 2020 2020 2073 7472 6970  ...        strip
+00014870: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00014880: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00014890: 2020 2057 6865 7468 6572 2074 6f20 6967     Whether to ig
+000148a0: 6e6f 7265 2073 7061 6365 7320 6265 666f  nore spaces befo
+000148b0: 7265 2061 6e64 2061 6674 6572 2065 6163  re and after eac
+000148c0: 6820 776f 7264 2e0d 0a20 2020 2020 2020  h word...       
+000148d0: 2069 676e 6f72 655f 7075 6e63 7475 6174   ignore_punctuat
+000148e0: 696f 6e73 203a 2062 6f6f 6c2c 2064 6566  ions : bool, def
+000148f0: 6175 6c74 2027 2227 2c2e 3f21 270d 0a20  ault '"',.?!'.. 
+00014900: 2020 2020 2020 2020 2020 2045 6e64 696e             Endin
+00014910: 6720 7075 6e63 7475 6174 696f 6e73 2074  g punctuations t
+00014920: 6f20 6967 6e6f 7265 2e0d 0a20 2020 2020  o ignore...     
+00014930: 2020 2065 7874 656e 645f 6475 7261 7469     extend_durati
+00014940: 6f6e 3a20 626f 6f6c 2c20 6465 6661 756c  on: bool, defaul
+00014950: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+00014960: 2020 2020 5768 6574 6865 7220 746f 2065      Whether to e
+00014970: 7874 656e 6420 7468 6520 6475 7261 7469  xtend the durati
+00014980: 6f6e 206f 6620 7468 6520 7072 6576 696f  on of the previo
+00014990: 7573 2077 6f72 6420 746f 2063 6f76 6572  us word to cover
+000149a0: 2074 6865 2064 7572 6174 696f 6e20 6f66   the duration of
+000149b0: 2074 6865 2072 6570 6574 6974 696f 6e2e   the repetition.
+000149c0: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
+000149d0: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
+000149e0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+000149f0: 2020 2057 6865 7468 6572 2074 6f20 7072     Whether to pr
+00014a00: 696e 7420 6465 7461 696c 206f 6620 7468  int detail of th
+00014a10: 6520 7265 6d6f 7665 6420 7265 7065 7469  e removed repeti
+00014a20: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+00014a30: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
+00014a40: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00014a50: 2020 2020 7374 6162 6c65 5f77 6869 7370      stable_whisp
+00014a60: 6572 2e72 6573 756c 742e 5768 6973 7065  er.result.Whispe
+00014a70: 7252 6573 756c 740d 0a20 2020 2020 2020  rResult..       
+00014a80: 2020 2020 2054 6865 2063 7572 7265 6e74       The current
+00014a90: 2069 6e73 7461 6e63 6520 6166 7465 7220   instance after 
+00014aa0: 7468 6520 6368 616e 6765 732e 0d0a 2020  the changes...  
+00014ab0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00014ac0: 2020 2069 6620 6e6f 7420 7365 6c66 2e68     if not self.h
+00014ad0: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
+00014ae0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00014af0: 6c66 0d0a 0d0a 2020 2020 2020 2020 666f  lf....        fo
+00014b00: 7220 636f 756e 7420 696e 2072 616e 6765  r count in range
+00014b10: 2831 2c20 6d61 785f 776f 7264 7320 2b20  (1, max_words + 
+00014b20: 3129 3a0d 0a20 2020 2020 2020 2020 2020  1):..           
+00014b30: 2061 6c6c 5f77 6f72 6473 203d 2073 656c   all_words = sel
+00014b40: 662e 616c 6c5f 776f 7264 7328 290d 0a20  f.all_words().. 
+00014b50: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00014b60: 6e28 616c 6c5f 776f 7264 7329 203c 2032  n(all_words) < 2
+00014b70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014b80: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
+00014b90: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00014ba0: 776f 7264 735f 7374 7220 3d20 5b77 2e77  words_str = [w.w
+00014bb0: 6f72 6420 666f 7220 7720 696e 2061 6c6c  ord for w in all
+00014bc0: 5f77 6f72 6473 5d0d 0a20 2020 2020 2020  _words]..       
+00014bd0: 2020 2020 2069 6620 7374 7269 703a 0d0a       if strip:..
+00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bf0: 616c 6c5f 776f 7264 735f 7374 7220 3d20  all_words_str = 
+00014c00: 5b77 2e73 7472 6970 2829 2066 6f72 2077  [w.strip() for w
+00014c10: 2069 6e20 616c 6c5f 776f 7264 735f 7374   in all_words_st
+00014c20: 725d 0d0a 2020 2020 2020 2020 2020 2020  r]..            
+00014c30: 6966 2069 676e 6f72 655f 7075 6e63 7475  if ignore_punctu
+00014c40: 6174 696f 6e73 3a0d 0a20 2020 2020 2020  ations:..       
+00014c50: 2020 2020 2020 2020 2070 746e 203d 2066           ptn = f
+00014c60: 275b 7b69 676e 6f72 655f 7075 6e63 7475  '[{ignore_punctu
+00014c70: 6174 696f 6e73 7d5d 2b24 270d 0a20 2020  ations}]+$'..   
+00014c80: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00014c90: 5f77 6f72 6473 5f73 7472 203d 205b 7265  _words_str = [re
+00014ca0: 2e73 7562 2870 746e 2c20 2727 2c20 7729  .sub(ptn, '', w)
+00014cb0: 2066 6f72 2077 2069 6e20 616c 6c5f 776f   for w in all_wo
+00014cc0: 7264 735f 7374 725d 0d0a 2020 2020 2020  rds_str]..      
+00014cd0: 2020 2020 2020 6966 206e 6f74 2063 6173        if not cas
+00014ce0: 655f 7365 6e73 6974 6976 653a 0d0a 2020  e_sensitive:..  
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00014d00: 6c5f 776f 7264 735f 7374 7220 3d20 5b77  l_words_str = [w
+00014d10: 2e6c 6f77 6572 2829 2066 6f72 2077 2069  .lower() for w i
+00014d20: 6e20 616c 6c5f 776f 7264 735f 7374 725d  n all_words_str]
+00014d30: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
+00014d40: 7874 5f69 203d 204e 6f6e 650d 0a20 2020  xt_i = None..   
+00014d50: 2020 2020 2020 2020 2063 6861 6e67 6573           changes
+00014d60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00014d70: 2020 2066 6f72 2069 2069 6e20 7265 7665     for i in reve
+00014d80: 7273 6564 2872 616e 6765 2863 6f75 6e74  rsed(range(count
+00014d90: 2a32 2c20 6c65 6e28 616c 6c5f 776f 7264  *2, len(all_word
+00014da0: 735f 7374 7229 2b31 2929 3a0d 0a20 2020  s_str)+1)):..   
+00014db0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014dc0: 6e65 7874 5f69 2069 7320 6e6f 7420 4e6f  next_i is not No
+00014dd0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00014de0: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
+00014df0: 5f69 2021 3d20 693a 0d0a 2020 2020 2020  _i != i:..      
+00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e10: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00014e40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00014e50: 6578 745f 6920 3d20 4e6f 6e65 0d0a 2020  ext_i = None..  
+00014e60: 2020 2020 2020 2020 2020 2020 2020 7320                s 
+00014e70: 3d20 6920 2d20 636f 756e 740d 0a20 2020  = i - count..   
+00014e80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014e90: 616c 6c5f 776f 7264 735f 7374 725b 7320  all_words_str[s 
+00014ea0: 2d20 636f 756e 743a 735d 2021 3d20 616c  - count:s] != al
+00014eb0: 6c5f 776f 7264 735f 7374 725b 733a 695d  l_words_str[s:i]
+00014ec0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014ed0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00014ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ef0: 206e 6578 745f 6920 3d20 730d 0a20 2020   next_i = s..   
+00014f00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014f10: 6578 7465 6e64 5f64 7572 6174 696f 6e3a  extend_duration:
+00014f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014f30: 2020 2020 2020 616c 6c5f 776f 7264 735b        all_words[
+00014f40: 732d 315d 2e65 6e64 203d 2061 6c6c 5f77  s-1].end = all_w
+00014f50: 6f72 6473 5b69 2d31 5d2e 656e 640d 0a20  ords[i-1].end.. 
+00014f60: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014f70: 656d 705f 6368 616e 6765 7320 3d20 5b5d  emp_changes = []
+00014f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014f90: 2020 666f 7220 6a20 696e 2072 6576 6572    for j in rever
+00014fa0: 7365 6428 7261 6e67 6528 732c 2069 2929  sed(range(s, i))
+00014fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014fc0: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
+00014fd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00014fe0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00014ff0: 5f63 6861 6e67 6573 2e61 7070 656e 6428  _changes.append(
+00015000: 6627 2d20 7b61 6c6c 5f77 6f72 6473 5b6a  f'- {all_words[j
+00015010: 5d2e 746f 5f64 6963 7428 297d 2729 0d0a  ].to_dict()}')..
+00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015030: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
+00015040: 776f 7264 2861 6c6c 5f77 6f72 6473 5b6a  word(all_words[j
+00015050: 5d2c 2046 616c 7365 2c20 7665 7262 6f73  ], False, verbos
+00015060: 653d 4661 6c73 6529 0d0a 2020 2020 2020  e=False)..      
+00015070: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
+00015080: 705f 6368 616e 6765 733a 0d0a 2020 2020  p_changes:..    
+00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150a0: 6368 616e 6765 732e 6170 7065 6e64 280d  changes.append(.
+000150b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150c0: 2020 2020 2020 2020 2066 2752 656d 6f76           f'Remov
+000150d0: 653a 205b 7b66 6f72 6d61 745f 7469 6d65  e: [{format_time
+000150e0: 7374 616d 7028 616c 6c5f 776f 7264 735b  stamp(all_words[
+000150f0: 735d 2e73 7461 7274 297d 202d 3e20 7b66  s].start)} -> {f
+00015100: 6f72 6d61 745f 7469 6d65 7374 616d 7028  ormat_timestamp(
+00015110: 616c 6c5f 776f 7264 735b 692d 315d 2e65  all_words[i-1].e
+00015120: 6e64 297d 5d20 270d 0a20 2020 2020 2020  nd)}] '..       
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 202b 2027 272e 6a6f 696e 285f 772e 776f   + ''.join(_w.wo
+00015150: 7264 2066 6f72 205f 7720 696e 2061 6c6c  rd for _w in all
+00015160: 5f77 6f72 6473 5b73 3a69 5d29 202b 2027  _words[s:i]) + '
+00015170: 5c6e 270d 0a20 2020 2020 2020 2020 2020  \n'..           
+00015180: 2020 2020 2020 2020 2020 2020 202b 2027               + '
+00015190: 5c6e 272e 6a6f 696e 2872 6576 6572 7365  \n'.join(reverse
+000151a0: 6428 7465 6d70 5f63 6861 6e67 6573 2929  d(temp_changes))
+000151b0: 202b 2027 5c6e 270d 0a20 2020 2020 2020   + '\n'..       
+000151c0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 666f 7220 6930 2c20 6931 2069 6e20 7a69  for i0, i1 in zi
+000151f0: 7028 7261 6e67 6528 7320 2d20 636f 756e  p(range(s - coun
+00015200: 742c 2073 292c 2072 616e 6765 2873 2c20  t, s), range(s, 
+00015210: 6929 293a 0d0a 2020 2020 2020 2020 2020  i)):..          
+00015220: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00015230: 2861 6c6c 5f77 6f72 6473 5b69 305d 2e77  (all_words[i0].w
+00015240: 6f72 6429 203c 206c 656e 2861 6c6c 5f77  ord) < len(all_w
+00015250: 6f72 6473 5b69 315d 2e77 6f72 6429 3a0d  ords[i1].word):.
+00015260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015270: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
+00015280: 6473 5b69 315d 2e73 7461 7274 203d 2061  ds[i1].start = a
+00015290: 6c6c 5f77 6f72 6473 5b69 305d 2e73 7461  ll_words[i0].sta
+000152a0: 7274 0d0a 2020 2020 2020 2020 2020 2020  rt..            
+000152b0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000152c0: 776f 7264 735b 6931 5d2e 656e 6420 3d20  words[i1].end = 
+000152d0: 616c 6c5f 776f 7264 735b 6930 5d2e 656e  all_words[i0].en
+000152e0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+000152f0: 2020 2020 2020 2020 2020 205f 7369 642c             _sid,
+00015300: 205f 7769 6420 3d20 616c 6c5f 776f 7264   _wid = all_word
+00015310: 735b 6930 5d2e 7365 676d 656e 745f 6964  s[i0].segment_id
+00015320: 2c20 616c 6c5f 776f 7264 735b 6930 5d2e  , all_words[i0].
+00015330: 6964 0d0a 2020 2020 2020 2020 2020 2020  id..            
+00015340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015350: 2e73 6567 6d65 6e74 735b 5f73 6964 5d2e  .segments[_sid].
+00015360: 776f 7264 735b 5f77 6964 5d20 3d20 616c  words[_wid] = al
+00015370: 6c5f 776f 7264 735b 6931 5d0d 0a0d 0a20  l_words[i1].... 
+00015380: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
+00015390: 616e 6765 733a 0d0a 2020 2020 2020 2020  anges:..        
+000153a0: 2020 2020 2020 2020 7072 696e 7428 275c          print('\
+000153b0: 6e27 2e6a 6f69 6e28 7265 7665 7273 6564  n'.join(reversed
+000153c0: 2863 6861 6e67 6573 2929 290d 0a0d 0a20  (changes))).... 
+000153d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000153e0: 7265 6d6f 7665 5f6e 6f5f 776f 7264 5f73  remove_no_word_s
+000153f0: 6567 6d65 6e74 7328 7265 6173 7369 676e  egments(reassign
+00015400: 5f69 6473 3d46 616c 7365 290d 0a20 2020  _ids=False)..   
+00015410: 2020 2020 2073 656c 662e 7265 6173 7369       self.reassi
+00015420: 676e 5f69 6473 2829 0d0a 0d0a 2020 2020  gn_ids()....    
+00015430: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+00015440: 0a0d 0a20 2020 2064 6566 2072 656d 6f76  ...    def remov
+00015450: 655f 776f 7264 735f 6279 5f73 7472 280d  e_words_by_str(.
+00015460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015470: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+00015480: 776f 7264 733a 2055 6e69 6f6e 5b73 7472  words: Union[str
+00015490: 2c20 4c69 7374 5b73 7472 5d2c 204e 6f6e  , List[str], Non
+000154a0: 655d 2c0d 0a20 2020 2020 2020 2020 2020  e],..           
+000154b0: 2063 6173 655f 7365 6e73 6974 6976 653a   case_sensitive:
+000154c0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+000154d0: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+000154e0: 703a 2062 6f6f 6c20 3d20 5472 7565 2c0d  p: bool = True,.
+000154f0: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00015500: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
+00015510: 3a20 7374 7220 3d20 225c 2227 2c2e 3f21  : str = "\"',.?!
+00015520: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00015530: 6d69 6e5f 7072 6f62 3a20 666c 6f61 7420  min_prob: float 
+00015540: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00015550: 2020 2020 2066 696c 7465 7273 3a20 4361       filters: Ca
+00015560: 6c6c 6162 6c65 203d 204e 6f6e 652c 0d0a  llable = None,..
+00015570: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+00015580: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
+00015590: 0d0a 2020 2020 2920 2d3e 2027 5768 6973  ..    ) -> 'Whis
+000155a0: 7065 7252 6573 756c 7427 3a0d 0a20 2020  perResult':..   
+000155b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000155c0: 2020 5265 6d6f 7665 2077 6f72 6473 2074    Remove words t
+000155d0: 6861 7420 6d61 7463 6820 6060 776f 7264  hat match ``word
+000155e0: 7360 602e 0d0a 0d0a 2020 2020 2020 2020  s``.....        
+000155f0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00015600: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00015610: 2020 2020 2020 2020 776f 7264 7320 3a20          words : 
+00015620: 7374 7220 6f72 206c 6973 7420 6f66 2073  str or list of s
+00015630: 7472 206f 7220 4e6f 6e65 0d0a 2020 2020  tr or None..    
+00015640: 2020 2020 2020 2020 4120 776f 7264 206f          A word o
+00015650: 7220 6c69 7374 206f 6620 776f 7264 7320  r list of words 
+00015660: 746f 2072 656d 6f76 652e 6060 4e6f 6e65  to remove.``None
+00015670: 6060 2066 6f72 2061 6c6c 2077 6f72 6473  `` for all words
+00015680: 2074 6f20 6265 2070 6173 7365 6420 696e   to be passed in
+00015690: 746f 2060 6066 696c 7465 7273 6060 2e0d  to ``filters``..
+000156a0: 0a20 2020 2020 2020 2063 6173 655f 7365  .        case_se
+000156b0: 6e73 6974 6976 6520 3a20 626f 6f6c 2c20  nsitive : bool, 
+000156c0: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+000156d0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000156e0: 6572 2074 6865 2063 6173 6520 6f66 2077  er the case of w
+000156f0: 6f72 6473 206e 6565 6420 746f 206d 6174  ords need to mat
+00015700: 6368 2074 6f20 6265 2063 6f6e 7369 6465  ch to be conside
+00015710: 7265 6420 6173 2072 6570 6574 6974 696f  red as repetitio
+00015720: 6e2e 0d0a 2020 2020 2020 2020 7374 7269  n...        stri
+00015730: 7020 3a20 626f 6f6c 2c20 6465 6661 756c  p : bool, defaul
+00015740: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
+00015750: 2020 2020 5768 6574 6865 7220 746f 2069      Whether to i
+00015760: 676e 6f72 6520 7370 6163 6573 2062 6566  gnore spaces bef
+00015770: 6f72 6520 616e 6420 6166 7465 7220 6561  ore and after ea
+00015780: 6368 2077 6f72 642e 0d0a 2020 2020 2020  ch word...      
+00015790: 2020 6967 6e6f 7265 5f70 756e 6374 7561    ignore_punctua
+000157a0: 7469 6f6e 7320 3a20 626f 6f6c 2c20 6465  tions : bool, de
+000157b0: 6661 756c 7420 2722 272c 2e3f 2127 0d0a  fault '"',.?!'..
+000157c0: 2020 2020 2020 2020 2020 2020 456e 6469              Endi
+000157d0: 6e67 2070 756e 6374 7561 7469 6f6e 7320  ng punctuations 
+000157e0: 746f 2069 676e 6f72 652e 0d0a 2020 2020  to ignore...    
+000157f0: 2020 2020 6d69 6e5f 7072 6f62 203a 2066      min_prob : f
+00015800: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0d0a  loat, optional..
+00015810: 2020 2020 2020 2020 2020 2020 4163 7473              Acts
+00015820: 2061 7320 7468 6520 6669 7273 7420 6669   as the first fi
+00015830: 6c74 6572 2074 6865 2066 6f72 2074 6865  lter the for the
+00015840: 2077 6f72 6473 2074 6861 7420 6d61 7463   words that matc
+00015850: 6820 6060 776f 7264 7360 602e 2057 6f72  h ``words``. Wor
+00015860: 6473 2077 6974 6820 7072 6f62 6162 696c  ds with probabil
+00015870: 6974 7920 3c20 6060 6d69 6e5f 7072 6f62  ity < ``min_prob
+00015880: 6060 2077 696c 6c0d 0a20 2020 2020 2020  `` will..       
+00015890: 2020 2020 2062 6520 7265 6d6f 7665 6420       be removed 
+000158a0: 6966 2060 6066 696c 7465 7273 6060 2069  if ``filters`` i
+000158b0: 7320 6060 4e6f 6e65 6060 2c20 656c 7365  s ``None``, else
+000158c0: 2070 6173 7320 7468 6520 776f 7264 7320   pass the words 
+000158d0: 696e 746f 2060 6066 696c 7465 7273 6060  into ``filters``
+000158e0: 2e20 576f 7264 7320 7769 7468 6f75 7420  . Words without 
+000158f0: 7072 6f62 6162 696c 6974 7920 7769 6c6c  probability will
+00015900: 0d0a 2020 2020 2020 2020 2020 2020 6265  ..            be
+00015910: 2074 7265 6174 6564 2061 7320 6861 7669   treated as havi
+00015920: 6e67 2070 726f 6261 6269 6c69 7479 203c  ng probability <
+00015930: 2060 606d 696e 5f70 726f 6260 602e 0d0a   ``min_prob``...
+00015940: 2020 2020 2020 2020 6669 6c74 6572 7320          filters 
+00015950: 3a20 4361 6c6c 6162 6c65 2c20 6f70 7469  : Callable, opti
+00015960: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
+00015970: 2020 4120 6675 6e63 7469 6f6e 2074 6861    A function tha
+00015980: 7420 7461 6b65 7320 616e 2069 6e73 7461  t takes an insta
+00015990: 6e63 6520 6f66 203a 636c 6173 733a 6073  nce of :class:`s
+000159a0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
+000159b0: 7375 6c74 2e57 6f72 6454 696d 696e 6760  sult.WordTiming`
+000159c0: 2061 7320 6974 7320 6f6e 6c79 2061 7267   as its only arg
+000159d0: 756d 656e 742e 0d0a 2020 2020 2020 2020  ument...        
+000159e0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+000159f0: 6e20 6973 2063 7573 746f 6d20 6669 6c74  n is custom filt
+00015a00: 6572 2066 6f72 2074 6865 2077 6f72 6473  er for the words
+00015a10: 2074 6861 7420 6d61 7463 6820 6060 776f   that match ``wo
+00015a20: 7264 7360 6020 616e 6420 7765 7265 206e  rds`` and were n
+00015a30: 6f74 2063 6175 6768 7420 6279 2060 606d  ot caught by ``m
+00015a40: 696e 5f70 726f 6260 602e 0d0a 2020 2020  in_prob``...    
+00015a50: 2020 2020 7665 7262 6f73 653a 0d0a 2020      verbose:..  
+00015a60: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+00015a70: 7220 746f 2070 7269 6e74 2064 6574 6169  r to print detai
+00015a80: 6c20 6f66 2074 6865 2072 656d 6f76 6564  l of the removed
+00015a90: 2077 6f72 6473 2e0d 0a0d 0a20 2020 2020   words.....     
+00015aa0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+00015ab0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00015ac0: 2020 2020 2073 7461 626c 655f 7768 6973       stable_whis
+00015ad0: 7065 722e 7265 7375 6c74 2e57 6869 7370  per.result.Whisp
+00015ae0: 6572 5265 7375 6c74 0d0a 2020 2020 2020  erResult..      
+00015af0: 2020 2020 2020 5468 6520 6375 7272 656e        The curren
+00015b00: 7420 696e 7374 616e 6365 2061 6674 6572  t instance after
+00015b10: 2074 6865 2063 6861 6e67 6573 2e0d 0a20   the changes... 
+00015b20: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00015b30: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00015b40: 6861 735f 776f 7264 733a 0d0a 2020 2020  has_words:..    
+00015b50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00015b60: 656c 660d 0a20 2020 2020 2020 2069 6620  elf..        if 
+00015b70: 6973 696e 7374 616e 6365 2877 6f72 6473  isinstance(words
+00015b80: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
+00015b90: 2020 2020 2077 6f72 6473 203d 205b 776f       words = [wo
+00015ba0: 7264 735d 0d0a 2020 2020 2020 2020 616c  rds]..        al
+00015bb0: 6c5f 776f 7264 7320 3d20 7365 6c66 2e61  l_words = self.a
+00015bc0: 6c6c 5f77 6f72 6473 2829 0d0a 2020 2020  ll_words()..    
+00015bd0: 2020 2020 616c 6c5f 776f 7264 735f 7374      all_words_st
+00015be0: 7220 3d20 5b77 2e77 6f72 6420 666f 7220  r = [w.word for 
+00015bf0: 7720 696e 2061 6c6c 5f77 6f72 6473 5d0d  w in all_words].
+00015c00: 0a20 2020 2020 2020 2069 6620 7374 7269  .        if stri
+00015c10: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+00015c20: 616c 6c5f 776f 7264 735f 7374 7220 3d20  all_words_str = 
+00015c30: 5b77 2e73 7472 6970 2829 2066 6f72 2077  [w.strip() for w
+00015c40: 2069 6e20 616c 6c5f 776f 7264 735f 7374   in all_words_st
+00015c50: 725d 0d0a 2020 2020 2020 2020 2020 2020  r]..            
+00015c60: 776f 7264 7320 3d20 5b77 2e73 7472 6970  words = [w.strip
+00015c70: 2829 2066 6f72 2077 2069 6e20 776f 7264  () for w in word
+00015c80: 735d 0d0a 2020 2020 2020 2020 6966 2069  s]..        if i
+00015c90: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
+00015ca0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+00015cb0: 2070 746e 203d 2066 275b 7b69 676e 6f72   ptn = f'[{ignor
+00015cc0: 655f 7075 6e63 7475 6174 696f 6e73 7d5d  e_punctuations}]
+00015cd0: 2b24 270d 0a20 2020 2020 2020 2020 2020  +$'..           
+00015ce0: 2061 6c6c 5f77 6f72 6473 5f73 7472 203d   all_words_str =
+00015cf0: 205b 7265 2e73 7562 2870 746e 2c20 2727   [re.sub(ptn, ''
+00015d00: 2c20 7729 2066 6f72 2077 2069 6e20 616c  , w) for w in al
+00015d10: 6c5f 776f 7264 735f 7374 725d 0d0a 2020  l_words_str]..  
+00015d20: 2020 2020 2020 2020 2020 776f 7264 7320            words 
+00015d30: 3d20 5b72 652e 7375 6228 7074 6e2c 2027  = [re.sub(ptn, '
+00015d40: 272c 2077 2920 666f 7220 7720 696e 2077  ', w) for w in w
+00015d50: 6f72 6473 5d0d 0a20 2020 2020 2020 2069  ords]..        i
+00015d60: 6620 6e6f 7420 6361 7365 5f73 656e 7369  f not case_sensi
+00015d70: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
+00015d80: 2020 2061 6c6c 5f77 6f72 6473 5f73 7472     all_words_str
+00015d90: 203d 205b 772e 6c6f 7765 7228 2920 666f   = [w.lower() fo
+00015da0: 7220 7720 696e 2061 6c6c 5f77 6f72 6473  r w in all_words
+00015db0: 5f73 7472 5d0d 0a20 2020 2020 2020 2020  _str]..         
+00015dc0: 2020 2077 6f72 6473 203d 205b 772e 6c6f     words = [w.lo
+00015dd0: 7765 7228 2920 666f 7220 7720 696e 2077  wer() for w in w
+00015de0: 6f72 6473 5d0d 0a0d 0a20 2020 2020 2020  ords]....       
+00015df0: 2063 6861 6e67 6573 203d 205b 5d0d 0a20   changes = [].. 
+00015e00: 2020 2020 2020 2066 6f72 2069 2c20 7720         for i, w 
+00015e10: 696e 2072 6576 6572 7365 6428 6c69 7374  in reversed(list
+00015e20: 2865 6e75 6d65 7261 7465 2861 6c6c 5f77  (enumerate(all_w
+00015e30: 6f72 6473 5f73 7472 2929 293a 0d0a 2020  ords_str))):..  
+00015e40: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00015e50: 2028 776f 7264 7320 6973 204e 6f6e 6520   (words is None 
+00015e60: 6f72 2061 6e79 2877 203d 3d20 5f77 2066  or any(w == _w f
+00015e70: 6f72 205f 7720 696e 2077 6f72 6473 2929  or _w in words))
+00015e80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015e90: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+00015ea0: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
+00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ec0: 2020 2028 6d69 6e5f 7072 6f62 2069 7320     (min_prob is 
+00015ed0: 4e6f 6e65 206f 7220 616c 6c5f 776f 7264  None or all_word
+00015ee0: 735b 695d 2e70 726f 6261 6269 6c69 7479  s[i].probability
+00015ef0: 2069 7320 4e6f 6e65 206f 7220 6d69 6e5f   is None or min_
+00015f00: 7072 6f62 203e 2061 6c6c 5f77 6f72 6473  prob > all_words
+00015f10: 5b69 5d2e 7072 6f62 6162 696c 6974 7929  [i].probability)
+00015f20: 2061 6e64 0d0a 2020 2020 2020 2020 2020   and..          
+00015f30: 2020 2020 2020 2020 2020 2866 696c 7465            (filte
+00015f40: 7273 2069 7320 4e6f 6e65 206f 7220 6669  rs is None or fi
+00015f50: 6c74 6572 7328 616c 6c5f 776f 7264 735b  lters(all_words[
+00015f60: 695d 2929 0d0a 2020 2020 2020 2020 2020  i]))..          
+00015f70: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
+00015f80: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00015f90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015fa0: 2020 2020 2020 2063 6861 6e67 6573 2e61         changes.a
+00015fb0: 7070 656e 6428 6627 5265 6d6f 7665 643a  ppend(f'Removed:
+00015fc0: 207b 616c 6c5f 776f 7264 735b 695d 2e74   {all_words[i].t
+00015fd0: 6f5f 6469 6374 2829 7d27 290d 0a20 2020  o_dict()}')..   
+00015fe0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ff0: 662e 7265 6d6f 7665 5f77 6f72 6428 616c  f.remove_word(al
+00016000: 6c5f 776f 7264 735b 695d 2c20 4661 6c73  l_words[i], Fals
+00016010: 652c 2076 6572 626f 7365 3d46 616c 7365  e, verbose=False
+00016020: 290d 0a20 2020 2020 2020 2069 6620 6368  )..        if ch
+00016030: 616e 6765 733a 0d0a 2020 2020 2020 2020  anges:..        
+00016040: 2020 2020 7072 696e 7428 275c 6e27 2e6a      print('\n'.j
+00016050: 6f69 6e28 7265 7665 7273 6564 2863 6861  oin(reversed(cha
+00016060: 6e67 6573 2929 290d 0a20 2020 2020 2020  nges)))..       
+00016070: 2073 656c 662e 7265 6d6f 7665 5f6e 6f5f   self.remove_no_
+00016080: 776f 7264 5f73 6567 6d65 6e74 7328 290d  word_segments().
+00016090: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+000160a0: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+000160b0: 6620 6669 6c6c 5f69 6e5f 6761 7073 280d  f fill_in_gaps(.
+000160c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000160d0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+000160e0: 6f74 6865 725f 7265 7375 6c74 3a20 556e  other_result: Un
+000160f0: 696f 6e5b 2757 6869 7370 6572 5265 7375  ion['WhisperResu
+00016100: 6c74 272c 2073 7472 5d2c 0d0a 2020 2020  lt', str],..    
+00016110: 2020 2020 2020 2020 6d69 6e5f 6761 703a          min_gap:
+00016120: 2066 6c6f 6174 203d 2030 2e31 2c0d 0a20   float = 0.1,.. 
+00016130: 2020 2020 2020 2020 2020 2063 6173 655f             case_
+00016140: 7365 6e73 6974 6976 653a 2062 6f6f 6c20  sensitive: bool 
+00016150: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00016160: 2020 2020 2020 7374 7269 703a 2062 6f6f        strip: boo
+00016170: 6c20 3d20 5472 7565 2c0d 0a20 2020 2020  l = True,..     
+00016180: 2020 2020 2020 2069 676e 6f72 655f 7075         ignore_pu
+00016190: 6e63 7475 6174 696f 6e73 3a20 7374 7220  nctuations: str 
+000161a0: 3d20 225c 2227 2c2e 3f21 222c 0d0a 2020  = "\"',.?!",..  
+000161b0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+000161c0: 653a 2062 6f6f 6c20 3d20 5472 7565 0d0a  e: bool = True..
+000161d0: 2020 2020 2920 2d3e 2027 5768 6973 7065      ) -> 'Whispe
+000161e0: 7252 6573 756c 7427 3a0d 0a20 2020 2020  rResult':..     
+000161f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00016200: 4669 6c6c 2069 6e20 7365 676d 656e 7420  Fill in segment 
+00016210: 6761 7073 206c 6172 6765 7220 7468 616e  gaps larger than
+00016220: 2060 606d 696e 5f67 6170 6060 2077 6974   ``min_gap`` wit
+00016230: 6820 636f 6e74 656e 7420 6672 6f6d 2060  h content from `
+00016240: 606f 7468 6572 5f72 6573 756c 7460 6020  `other_result`` 
+00016250: 6174 2074 6865 2074 696d 6573 206f 6620  at the times of 
+00016260: 6761 7073 2e0d 0a0d 0a20 2020 2020 2020  gaps.....       
+00016270: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00016280: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+00016290: 0a20 2020 2020 2020 206f 7468 6572 5f72  .        other_r
+000162a0: 6573 756c 7420 3a20 5768 6973 7065 7252  esult : WhisperR
+000162b0: 6573 756c 7420 6f72 2073 7472 0d0a 2020  esult or str..  
+000162c0: 2020 2020 2020 2020 2020 416e 6f74 6865            Anothe
+000162d0: 7220 7472 616e 7363 7269 7074 696f 6e20  r transcription 
+000162e0: 7265 7375 6c74 2061 7320 616e 2069 6e73  result as an ins
+000162f0: 7461 6e63 6520 6f66 203a 636c 6173 733a  tance of :class:
+00016300: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
+00016310: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
+00016320: 7375 6c74 6020 6f72 2070 6174 6820 746f  sult` or path to
+00016330: 2074 6865 0d0a 2020 2020 2020 2020 2020   the..          
+00016340: 2020 4a53 4f4e 206f 6620 7468 6520 7265    JSON of the re
+00016350: 7375 6c74 2e0d 0a20 2020 2020 2020 206d  sult...        m
+00016360: 696e 5f67 6170 203a 2066 6c6f 6174 2c20  in_gap : float, 
+00016370: 6465 6661 756c 7420 302e 310d 0a20 2020  default 0.1..   
+00016380: 2020 2020 2020 2020 2054 6865 206d 696e           The min
+00016390: 696d 756d 2073 6563 6f6e 6473 206f 6620  imum seconds of 
+000163a0: 6120 6761 7020 6265 7477 6565 6e20 7365  a gap between se
+000163b0: 676d 656e 7473 2074 6861 7420 6d75 7374  gments that must
+000163c0: 2062 6520 6578 6365 6564 6564 2074 6f20   be exceeded to 
+000163d0: 6265 2066 696c 6c65 6420 696e 2e0d 0a20  be filled in... 
+000163e0: 2020 2020 2020 2063 6173 655f 7365 6e73         case_sens
+000163f0: 6974 6976 6520 3a20 626f 6f6c 2c20 6465  itive : bool, de
+00016400: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+00016410: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00016420: 2074 6f20 636f 6e73 6964 6572 2074 6865   to consider the
+00016430: 2063 6173 6520 6f66 2074 6865 2066 6972   case of the fir
+00016440: 7374 2061 6e64 206c 6173 7420 776f 7264  st and last word
+00016450: 206f 6620 7468 6520 6761 7020 746f 2064   of the gap to d
+00016460: 6574 6572 6d69 6e65 206f 7665 726c 6170  etermine overlap
+00016470: 7069 6e67 2077 6f72 6473 2074 6f20 7265  ping words to re
+00016480: 6d6f 7665 0d0a 2020 2020 2020 2020 2020  move..          
+00016490: 2020 6265 666f 7265 2066 696c 6c69 6e67    before filling
+000164a0: 2069 6e2e 0d0a 2020 2020 2020 2020 7374   in...        st
+000164b0: 7269 7020 3a20 626f 6f6c 2c20 6465 6661  rip : bool, defa
+000164c0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+000164d0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000164e0: 2069 676e 6f72 6520 7370 6163 6573 2062   ignore spaces b
+000164f0: 6566 6f72 6520 616e 6420 6166 7465 7220  efore and after 
+00016500: 7468 6520 6669 7273 7420 616e 6420 6c61  the first and la
+00016510: 7374 2077 6f72 6420 6f66 2074 6865 2067  st word of the g
+00016520: 6170 2074 6f20 6465 7465 726d 696e 6520  ap to determine 
+00016530: 6f76 6572 6c61 7070 696e 6720 776f 7264  overlapping word
+00016540: 730d 0a20 2020 2020 2020 2020 2020 2074  s..            t
+00016550: 6f20 7265 6d6f 7665 2062 6566 6f72 6520  o remove before 
+00016560: 6669 6c6c 696e 6720 696e 2e0d 0a20 2020  filling in...   
+00016570: 2020 2020 2069 676e 6f72 655f 7075 6e63       ignore_punc
+00016580: 7475 6174 696f 6e73 203a 2062 6f6f 6c2c  tuations : bool,
+00016590: 2064 6566 6175 6c74 2027 2227 2c2e 3f21   default '"',.?!
+000165a0: 270d 0a20 2020 2020 2020 2020 2020 2045  '..            E
+000165b0: 6e64 696e 6720 7075 6e63 7475 6174 696f  nding punctuatio
+000165c0: 6e73 2074 6f20 6967 6e6f 7265 2069 6e20  ns to ignore in 
+000165d0: 7468 6520 6669 7273 7420 616e 6420 6c61  the first and la
+000165e0: 7374 2077 6f72 6420 6f66 2074 6865 2067  st word of the g
+000165f0: 6170 2074 6f20 6465 7465 726d 696e 6520  ap to determine 
+00016600: 6f76 6572 6c61 7070 696e 6720 776f 7264  overlapping word
+00016610: 7320 746f 0d0a 2020 2020 2020 2020 2020  s to..          
+00016620: 2020 7265 6d6f 7665 2062 6566 6f72 6520    remove before 
+00016630: 6669 6c6c 696e 6720 696e 2e0d 0a20 2020  filling in...   
+00016640: 2020 2020 2076 6572 626f 7365 3a0d 0a20       verbose:.. 
+00016650: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00016660: 6572 2074 6f20 7072 696e 7420 6465 7461  er to print deta
+00016670: 696c 206f 6620 7468 6520 6669 6c6c 6564  il of the filled
+00016680: 2063 6f6e 7465 6e74 2e0d 0a0d 0a20 2020   content.....   
+00016690: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+000166a0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+000166b0: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+000166c0: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+000166d0: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
+000166e0: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+000166f0: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
+00016700: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
+00016710: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00016720: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
+00016730: 662e 7365 676d 656e 7473 2920 3c20 323a  f.segments) < 2:
+00016740: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00016750: 7475 726e 2073 656c 660d 0a20 2020 2020  turn self..     
+00016760: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00016770: 286f 7468 6572 5f72 6573 756c 742c 2073  (other_result, s
+00016780: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
+00016790: 2020 6f74 6865 725f 7265 7375 6c74 203d    other_result =
+000167a0: 2057 6869 7370 6572 5265 7375 6c74 286f   WhisperResult(o
+000167b0: 7468 6572 5f72 6573 756c 7429 0d0a 0d0a  ther_result)....
+000167c0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
+000167d0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000167e0: 6566 2073 7472 6970 5f73 7061 6365 2877  ef strip_space(w
+000167f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016800: 2020 2020 7265 7475 726e 2077 2e73 7472      return w.str
+00016810: 6970 2829 0d0a 2020 2020 2020 2020 656c  ip()..        el
+00016820: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00016830: 2064 6566 2073 7472 6970 5f73 7061 6365   def strip_space
+00016840: 2877 293a 0d0a 2020 2020 2020 2020 2020  (w):..          
+00016850: 2020 2020 2020 7265 7475 726e 2077 0d0a        return w..
+00016860: 0d0a 2020 2020 2020 2020 6966 2069 676e  ..        if ign
+00016870: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
+00016880: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00016890: 746e 203d 2066 275b 7b69 676e 6f72 655f  tn = f'[{ignore_
+000168a0: 7075 6e63 7475 6174 696f 6e73 7d5d 2b24  punctuations}]+$
+000168b0: 270d 0a0d 0a20 2020 2020 2020 2020 2020  '....           
+000168c0: 2064 6566 2073 7472 6970 5f70 756e 6374   def strip_punct
+000168d0: 7561 7469 6f6e 7328 7729 3a0d 0a20 2020  uations(w):..   
+000168e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000168f0: 7572 6e20 7265 2e73 7562 2870 746e 2c20  urn re.sub(ptn, 
+00016900: 2727 2c20 7374 7269 705f 7370 6163 6528  '', strip_space(
+00016910: 7729 290d 0a20 2020 2020 2020 2065 6c73  w))..        els
+00016920: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00016930: 7374 7269 705f 7075 6e63 7475 6174 696f  strip_punctuatio
+00016940: 6e73 203d 2073 7472 6970 5f73 7061 6365  ns = strip_space
+00016950: 0d0a 0d0a 2020 2020 2020 2020 6966 2063  ....        if c
+00016960: 6173 655f 7365 6e73 6974 6976 653a 0d0a  ase_sensitive:..
+00016970: 2020 2020 2020 2020 2020 2020 7374 7269              stri
+00016980: 7020 3d20 7374 7269 705f 7075 6e63 7475  p = strip_punctu
+00016990: 6174 696f 6e73 0d0a 2020 2020 2020 2020  ations..        
+000169a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000169b0: 2020 2064 6566 2073 7472 6970 2877 293a     def strip(w):
+000169c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000169d0: 2020 7265 7475 726e 2073 7472 6970 5f70    return strip_p
+000169e0: 756e 6374 7561 7469 6f6e 7328 7729 2e6c  unctuations(w).l
+000169f0: 6f77 6572 2829 0d0a 0d0a 2020 2020 2020  ower()....      
+00016a00: 2020 7365 675f 7061 6972 7320 3d20 6c69    seg_pairs = li
+00016a10: 7374 2865 6e75 6d65 7261 7465 287a 6970  st(enumerate(zip
+00016a20: 2873 656c 662e 7365 676d 656e 7473 5b3a  (self.segments[:
+00016a30: 2d31 5d2c 2073 656c 662e 7365 676d 656e  -1], self.segmen
+00016a40: 7473 5b31 3a5d 2929 290d 0a20 2020 2020  ts[1:])))..     
+00016a50: 2020 2073 6567 5f70 6169 7273 2e69 6e73     seg_pairs.ins
+00016a60: 6572 7428 302c 2028 2d31 2c20 284e 6f6e  ert(0, (-1, (Non
+00016a70: 652c 2073 656c 662e 7365 676d 656e 7473  e, self.segments
+00016a80: 5b30 5d29 2929 0d0a 2020 2020 2020 2020  [0])))..        
+00016a90: 7365 675f 7061 6972 732e 6170 7065 6e64  seg_pairs.append
+00016aa0: 2828 7365 675f 7061 6972 735b 2d31 5d5b  ((seg_pairs[-1][
+00016ab0: 305d 2b31 2c20 2873 656c 662e 7365 676d  0]+1, (self.segm
+00016ac0: 656e 7473 5b2d 315d 2c20 4e6f 6e65 2929  ents[-1], None))
+00016ad0: 290d 0a0d 0a20 2020 2020 2020 2063 6861  )....        cha
+00016ae0: 6e67 6573 203d 205b 5d0d 0a20 2020 2020  nges = []..     
+00016af0: 2020 2066 6f72 2069 2c20 2873 6567 302c     for i, (seg0,
+00016b00: 2073 6567 3129 2069 6e20 7265 7665 7273   seg1) in revers
+00016b10: 6564 2873 6567 5f70 6169 7273 293a 0d0a  ed(seg_pairs):..
+00016b20: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00016b30: 745f 776f 7264 203d 204e 6f6e 6520 6966  t_word = None if
+00016b40: 2073 6567 3020 6973 204e 6f6e 6520 656c   seg0 is None el
+00016b50: 7365 2073 6567 302e 776f 7264 735b 2d31  se seg0.words[-1
+00016b60: 5d0d 0a20 2020 2020 2020 2020 2020 206c  ]..            l
+00016b70: 6173 745f 776f 7264 203d 204e 6f6e 6520  ast_word = None 
+00016b80: 6966 2073 6567 3120 6973 204e 6f6e 6520  if seg1 is None 
+00016b90: 656c 7365 2073 6567 312e 776f 7264 735b  else seg1.words[
+00016ba0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00016bb0: 7374 6172 7420 3d20 286f 7468 6572 5f72  start = (other_r
+00016bc0: 6573 756c 745b 305d 2e73 7461 7274 2069  esult[0].start i
+00016bd0: 6620 6669 7273 745f 776f 7264 2069 7320  f first_word is 
+00016be0: 4e6f 6e65 2065 6c73 6520 6669 7273 745f  None else first_
+00016bf0: 776f 7264 2e65 6e64 290d 0a20 2020 2020  word.end)..     
+00016c00: 2020 2020 2020 2065 6e64 203d 206f 7468         end = oth
+00016c10: 6572 5f72 6573 756c 745b 2d31 5d2e 656e  er_result[-1].en
+00016c20: 6420 6966 206c 6173 745f 776f 7264 2069  d if last_word i
+00016c30: 7320 4e6f 6e65 2065 6c73 6520 6c61 7374  s None else last
+00016c40: 5f77 6f72 642e 7374 6172 740d 0a20 2020  _word.start..   
+00016c50: 2020 2020 2020 2020 2069 6620 656e 6420           if end 
+00016c60: 2d20 7374 6172 7420 3c3d 206d 696e 5f67  - start <= min_g
+00016c70: 6170 3a0d 0a20 2020 2020 2020 2020 2020  ap:..           
+00016c80: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00016c90: 2020 2020 2020 2020 2020 2067 6170 5f77             gap_w
+00016ca0: 6f72 6473 203d 206f 7468 6572 5f72 6573  ords = other_res
+00016cb0: 756c 742e 6765 745f 636f 6e74 656e 745f  ult.get_content_
+00016cc0: 6279 5f74 696d 6528 2873 7461 7274 2c20  by_time((start, 
+00016cd0: 656e 6429 290d 0a20 2020 2020 2020 2020  end))..         
+00016ce0: 2020 2069 6620 6669 7273 745f 776f 7264     if first_word
+00016cf0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00016d00: 2067 6170 5f77 6f72 6473 2061 6e64 2073   gap_words and s
+00016d10: 7472 6970 2866 6972 7374 5f77 6f72 642e  trip(first_word.
+00016d20: 776f 7264 2920 3d3d 2073 7472 6970 2867  word) == strip(g
+00016d30: 6170 5f77 6f72 6473 5b30 5d2e 776f 7264  ap_words[0].word
+00016d40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016d50: 2020 2020 6669 7273 745f 776f 7264 2e65      first_word.e
+00016d60: 6e64 203d 2067 6170 5f77 6f72 6473 5b30  nd = gap_words[0
+00016d70: 5d2e 656e 640d 0a20 2020 2020 2020 2020  ].end..         
+00016d80: 2020 2020 2020 2067 6170 5f77 6f72 6473         gap_words
+00016d90: 203d 2067 6170 5f77 6f72 6473 5b31 3a5d   = gap_words[1:]
+00016da0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00016db0: 206c 6173 745f 776f 7264 2069 7320 6e6f   last_word is no
+00016dc0: 7420 4e6f 6e65 2061 6e64 2067 6170 5f77  t None and gap_w
+00016dd0: 6f72 6473 2061 6e64 2073 7472 6970 286c  ords and strip(l
+00016de0: 6173 745f 776f 7264 2e77 6f72 6429 203d  ast_word.word) =
+00016df0: 3d20 7374 7269 7028 6761 705f 776f 7264  = strip(gap_word
+00016e00: 735b 2d31 5d2e 776f 7264 293a 0d0a 2020  s[-1].word):..  
+00016e10: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00016e20: 7374 5f77 6f72 642e 7374 6172 7420 3d20  st_word.start = 
+00016e30: 6761 705f 776f 7264 735b 2d31 5d2e 7374  gap_words[-1].st
+00016e40: 6172 740d 0a20 2020 2020 2020 2020 2020  art..           
+00016e50: 2020 2020 2067 6170 5f77 6f72 6473 203d       gap_words =
+00016e60: 2067 6170 5f77 6f72 6473 5b3a 2d31 5d0d   gap_words[:-1].
+00016e70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016e80: 6e6f 7420 6761 705f 776f 7264 733a 0d0a  not gap_words:..
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ea0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00016eb0: 2020 2020 2020 6966 206c 6173 745f 776f        if last_wo
+00016ec0: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
+00016ed0: 6e64 206c 6173 745f 776f 7264 2e73 7461  nd last_word.sta
+00016ee0: 7274 203c 2067 6170 5f77 6f72 6473 5b2d  rt < gap_words[-
+00016ef0: 315d 2e65 6e64 3a0d 0a20 2020 2020 2020  1].end:..       
+00016f00: 2020 2020 2020 2020 206c 6173 745f 776f           last_wo
+00016f10: 7264 2e73 7461 7274 203d 2067 6170 5f77  rd.start = gap_w
+00016f20: 6f72 6473 5b2d 315d 2e65 6e64 0d0a 2020  ords[-1].end..  
+00016f30: 2020 2020 2020 2020 2020 6e65 775f 7365            new_se
+00016f40: 676d 656e 7473 203d 205b 6f74 6865 725f  gments = [other_
+00016f50: 7265 7375 6c74 5b67 6170 5f77 6f72 6473  result[gap_words
+00016f60: 5b30 5d2e 7365 676d 656e 745f 6964 5d2e  [0].segment_id].
+00016f70: 636f 7079 285b 5d29 5d0d 0a20 2020 2020  copy([])]..     
+00016f80: 2020 2020 2020 2066 6f72 206a 2c20 6e65         for j, ne
+00016f90: 775f 776f 7264 2069 6e20 656e 756d 6572  w_word in enumer
+00016fa0: 6174 6528 6761 705f 776f 7264 7329 3a0d  ate(gap_words):.
+00016fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016fc0: 206e 6577 5f77 6f72 645f 636f 7079 203d   new_word_copy =
+00016fd0: 206e 6577 5f77 6f72 642e 636f 7079 2863   new_word.copy(c
+00016fe0: 6f70 795f 746f 6b65 6e73 3d54 7275 6529  opy_tokens=True)
+00016ff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017000: 2020 6966 206a 203d 3d20 3020 616e 6420    if j == 0 and 
+00017010: 6669 7273 745f 776f 7264 2069 7320 6e6f  first_word is no
+00017020: 7420 4e6f 6e65 2061 6e64 2066 6972 7374  t None and first
+00017030: 5f77 6f72 642e 656e 6420 3e20 6761 705f  _word.end > gap_
+00017040: 776f 7264 735b 305d 2e73 7461 7274 3a0d  words[0].start:.
+00017050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017060: 2020 2020 206e 6577 5f77 6f72 645f 636f       new_word_co
+00017070: 7079 2e73 7461 7274 203d 2066 6972 7374  py.start = first
+00017080: 5f77 6f72 642e 656e 640d 0a20 2020 2020  _word.end..     
+00017090: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+000170a0: 775f 7365 676d 656e 7473 5b2d 315d 2e69  w_segments[-1].i
+000170b0: 6420 213d 206e 6577 5f77 6f72 642e 7365  d != new_word.se
+000170c0: 676d 656e 745f 6964 3a0d 0a20 2020 2020  gment_id:..     
+000170d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000170e0: 6577 5f73 6567 6d65 6e74 732e 6170 7065  ew_segments.appe
+000170f0: 6e64 286f 7468 6572 5f72 6573 756c 745b  nd(other_result[
+00017100: 6e65 775f 776f 7264 2e73 6567 6d65 6e74  new_word.segment
+00017110: 5f69 645d 2e63 6f70 7928 5b5d 2929 0d0a  _id].copy([]))..
+00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017130: 6e65 775f 7365 676d 656e 7473 5b2d 315d  new_segments[-1]
+00017140: 2e77 6f72 6473 2e61 7070 656e 6428 6e65  .words.append(ne
+00017150: 775f 776f 7264 5f63 6f70 7929 0d0a 2020  w_word_copy)..  
+00017160: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+00017170: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+00017180: 2020 2020 2020 2063 6861 6e67 6573 2e61         changes.a
+00017190: 7070 656e 6428 275c 6e27 2e6a 6f69 6e28  ppend('\n'.join(
+000171a0: 2741 6464 6564 3a20 2720 2b20 732e 746f  'Added: ' + s.to
+000171b0: 5f64 6973 706c 6179 5f73 7472 2854 7275  _display_str(Tru
+000171c0: 6529 2066 6f72 2073 2069 6e20 6e65 775f  e) for s in new_
+000171d0: 7365 676d 656e 7473 2929 0d0a 2020 2020  segments))..    
+000171e0: 2020 2020 2020 2020 7365 6c66 2e73 6567          self.seg
+000171f0: 6d65 6e74 7320 3d20 7365 6c66 2e73 6567  ments = self.seg
+00017200: 6d65 6e74 735b 3a69 2b31 5d20 2b20 6e65  ments[:i+1] + ne
+00017210: 775f 7365 676d 656e 7473 202b 2073 656c  w_segments + sel
+00017220: 662e 7365 676d 656e 7473 5b69 2b31 3a5d  f.segments[i+1:]
+00017230: 0d0a 2020 2020 2020 2020 6966 2063 6861  ..        if cha
+00017240: 6e67 6573 3a0d 0a20 2020 2020 2020 2020  nges:..         
+00017250: 2020 2070 7269 6e74 2827 5c6e 272e 6a6f     print('\n'.jo
+00017260: 696e 2872 6576 6572 7365 6428 6368 616e  in(reversed(chan
+00017270: 6765 7329 2929 0d0a 2020 2020 2020 2020  ges)))..        
+00017280: 7365 6c66 2e72 6561 7373 6967 6e5f 6964  self.reassign_id
+00017290: 7328 290d 0a0d 0a20 2020 2020 2020 2072  s()....        r
+000172a0: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
+000172b0: 2020 6465 6620 7265 6772 6f75 7028 0d0a    def regroup(..
+000172c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000172d0: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+000172e0: 6567 726f 7570 5f61 6c67 6f3a 2055 6e69  egroup_algo: Uni
+000172f0: 6f6e 5b73 7472 2c20 626f 6f6c 5d20 3d20  on[str, bool] = 
+00017300: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00017310: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00017320: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00017330: 2020 2020 2020 206f 6e6c 795f 7368 6f77         only_show
+00017340: 3a20 626f 6f6c 203d 2046 616c 7365 0d0a  : bool = False..
+00017350: 2020 2020 2920 2d3e 2022 5768 6973 7065      ) -> "Whispe
+00017360: 7252 6573 756c 7422 3a0d 0a20 2020 2020  rResult":..     
+00017370: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00017380: 5265 6772 6f75 7020 2869 6e2d 706c 6163  Regroup (in-plac
+00017390: 6529 2077 6f72 6473 2069 6e74 6f20 7365  e) words into se
+000173a0: 676d 656e 7473 2e0d 0a0d 0a20 2020 2020  gments.....     
+000173b0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000173c0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000173d0: 2d0d 0a20 2020 2020 2020 2072 6567 726f  -..        regro
+000173e0: 7570 5f61 6c67 6f3a 2073 7472 206f 7220  up_algo: str or 
+000173f0: 626f 6f6c 2c20 6465 6661 756c 7420 2764  bool, default 'd
+00017400: 6127 0d0a 2020 2020 2020 2020 2020 2020  a'..            
+00017410: 2053 7472 696e 6720 7265 7072 6573 656e   String represen
+00017420: 7461 7469 6f6e 206f 6620 6120 6375 7374  tation of a cust
+00017430: 6f6d 2072 6567 726f 7570 696e 6720 616c  om regrouping al
+00017440: 676f 7269 7468 6d20 6f72 2060 6054 7275  gorithm or ``Tru
+00017450: 6560 6020 7573 6520 746f 2074 6865 2064  e`` use to the d
+00017460: 6566 6175 6c74 2061 6c67 6f72 6974 686d  efault algorithm
+00017470: 2027 6461 272e 0d0a 2020 2020 2020 2020   'da'...        
+00017480: 7665 7262 6f73 6520 3a20 626f 6f6c 2c20  verbose : bool, 
+00017490: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+000174a0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000174b0: 6572 2074 6f20 7368 6f77 2061 6c6c 2074  er to show all t
+000174c0: 6865 206d 6574 686f 6473 2061 6e64 2061  he methods and a
+000174d0: 7267 756d 656e 7473 2070 6172 7365 6420  rguments parsed 
+000174e0: 6672 6f6d 2060 6072 6567 726f 7570 5f61  from ``regroup_a
+000174f0: 6c67 6f60 602e 0d0a 2020 2020 2020 2020  lgo``...        
+00017500: 6f6e 6c79 5f73 686f 7720 3a20 626f 6f6c  only_show : bool
+00017510: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
+00017520: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00017530: 7468 6572 2074 6f20 7368 6f77 2074 6865  ther to show the
+00017540: 2061 6c6c 206d 6574 686f 6473 2061 6e64   all methods and
+00017550: 2061 7267 756d 656e 7473 2070 6172 7365   arguments parse
+00017560: 6420 6672 6f6d 2060 6072 6567 726f 7570  d from ``regroup
+00017570: 5f61 6c67 6f60 6020 7769 7468 6f75 7420  _algo`` without 
+00017580: 7275 6e6e 696e 6720 7468 6520 6d65 7468  running the meth
+00017590: 6f64 730d 0a0d 0a20 2020 2020 2020 2052  ods....        R
+000175a0: 6574 7572 6e73 0d0a 2020 2020 2020 2020  eturns..        
+000175b0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+000175c0: 2073 7461 626c 655f 7768 6973 7065 722e   stable_whisper.
+000175d0: 7265 7375 6c74 2e57 6869 7370 6572 5265  result.WhisperRe
+000175e0: 7375 6c74 0d0a 2020 2020 2020 2020 2020  sult..          
+000175f0: 2020 5468 6520 6375 7272 656e 7420 696e    The current in
+00017600: 7374 616e 6365 2061 6674 6572 2074 6865  stance after the
+00017610: 2063 6861 6e67 6573 2e0d 0a0d 0a20 2020   changes.....   
+00017620: 2020 2020 204e 6f74 6573 0d0a 2020 2020       Notes..    
+00017630: 2020 2020 2d2d 2d2d 2d0d 0a20 2020 2020      -----..     
+00017640: 2020 2053 796e 7461 7820 666f 7220 7374     Syntax for st
+00017650: 7269 6e67 2072 6570 7265 7365 6e74 6174  ring representat
+00017660: 696f 6e20 6f66 2063 7573 746f 6d20 7265  ion of custom re
+00017670: 6772 6f75 7069 6e67 2061 6c67 6f72 6974  grouping algorit
+00017680: 686d 2e0d 0a20 2020 2020 2020 2020 2020  hm...           
+00017690: 204d 6574 686f 6420 6b65 7973 3a0d 0a20   Method keys:.. 
+000176a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000176b0: 673a 2073 706c 6974 5f62 795f 6761 700d  g: split_by_gap.
+000176c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000176d0: 2073 703a 2073 706c 6974 5f62 795f 7075   sp: split_by_pu
+000176e0: 6e63 7475 6174 696f 6e0d 0a20 2020 2020  nctuation..     
+000176f0: 2020 2020 2020 2020 2020 2073 6c3a 2073             sl: s
+00017700: 706c 6974 5f62 795f 6c65 6e67 7468 0d0a  plit_by_length..
+00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017720: 7364 3a20 7370 6c69 745f 6279 5f64 7572  sd: split_by_dur
+00017730: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00017740: 2020 2020 2020 206d 673a 206d 6572 6765         mg: merge
+00017750: 5f62 795f 6761 700d 0a20 2020 2020 2020  _by_gap..       
+00017760: 2020 2020 2020 2020 206d 703a 206d 6572           mp: mer
+00017770: 6765 5f62 795f 7075 6e63 7475 6174 696f  ge_by_punctuatio
+00017780: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00017790: 2020 206d 733a 206d 6572 6765 5f61 6c6c     ms: merge_all
+000177a0: 5f73 6567 6d65 6e74 0d0a 2020 2020 2020  _segment..      
+000177b0: 2020 2020 2020 2020 2020 636d 3a20 636c            cm: cl
+000177c0: 616d 705f 6d61 780d 0a20 2020 2020 2020  amp_max..       
+000177d0: 2020 2020 2020 2020 206c 3a20 6c6f 636b           l: lock
+000177e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000177f0: 2020 7573 3a20 756e 6c6f 636b 5f61 6c6c    us: unlock_all
+00017800: 5f73 6567 6d65 6e74 730d 0a20 2020 2020  _segments..     
+00017810: 2020 2020 2020 2020 2020 2064 613a 2064             da: d
+00017820: 6566 6175 6c74 2061 6c67 6f72 6974 686d  efault algorithm
+00017830: 2028 636d 5f73 703d 2c2a 202f efbc 8c5f   (cm_sp=,* /..._
+00017840: 7367 3d2e 355f 6d67 3d2e 332b 335f 7370  sg=.5_mg=.3+3_sp
+00017850: 3d2e 2a20 2fe3 8082 2f3f 2fef bc9f 290d  =.* /.../?/...).
+00017860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017870: 2072 773a 2072 656d 6f76 655f 776f 7264   rw: remove_word
+00017880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017890: 2020 7273 3a20 7265 6d6f 7665 5f73 6567    rs: remove_seg
+000178a0: 6d65 6e74 0d0a 2020 2020 2020 2020 2020  ment..          
+000178b0: 2020 2020 2020 7270 3a20 7265 6d6f 7665        rp: remove
+000178c0: 5f72 6570 6574 6974 696f 6e0d 0a20 2020  _repetition..   
+000178d0: 2020 2020 2020 2020 2020 2020 2072 7773               rws
+000178e0: 3a20 7265 6d6f 7665 5f77 6f72 6473 5f62  : remove_words_b
+000178f0: 795f 7374 720d 0a20 2020 2020 2020 2020  y_str..         
+00017900: 2020 2020 2020 2066 673a 2066 696c 6c5f         fg: fill_
+00017910: 696e 5f67 6170 730d 0a20 2020 2020 2020  in_gaps..       
+00017920: 2020 2020 2020 2020 2070 3a20 7061 640d           p: pad.
+00017930: 0a20 2020 2020 2020 2020 2020 204d 6574  .            Met
+00017940: 6163 6861 7261 6374 6572 733a 0d0a 2020  acharacters:..  
+00017950: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+00017960: 7365 7061 7261 7465 7320 6120 6d65 7468  separates a meth
+00017970: 6f64 206b 6579 2061 6e64 2069 7473 2061  od key and its a
+00017980: 7267 756d 656e 7473 2028 6e6f 7420 7573  rguments (not us
+00017990: 6564 2069 6620 6e6f 2061 7267 756d 656e  ed if no argumen
+000179a0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000179b0: 2020 2020 5f20 7365 7061 7261 7465 7320      _ separates 
+000179c0: 6d65 7468 6f64 206b 6579 7320 2861 6674  method keys (aft
+000179d0: 6572 2061 7267 756d 656e 7473 2069 6620  er arguments if 
+000179e0: 7468 6572 6520 6172 6520 616e 7929 0d0a  there are any)..
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2b20 7365 7061 7261 7465 7320 6172 6775  + separates argu
+00017a10: 6d65 6e74 7320 666f 7220 6120 6d65 7468  ments for a meth
+00017a20: 6f64 206b 6579 0d0a 2020 2020 2020 2020  od key..        
+00017a30: 2020 2020 2020 2020 2f20 7365 7061 7261          / separa
+00017a40: 7465 7320 616e 2061 7267 756d 656e 7420  tes an argument 
+00017a50: 696e 746f 206c 6973 7420 6f66 2073 7472  into list of str
+00017a60: 696e 6773 0d0a 2020 2020 2020 2020 2020  ings..          
+00017a70: 2020 2020 2020 2a20 7365 7061 7261 7465        * separate
+00017a80: 7320 616e 2069 7465 6d20 696e 206c 6973  s an item in lis
+00017a90: 7420 6f66 2073 7472 696e 6773 2069 6e74  t of strings int
+00017aa0: 6f20 6120 6e65 7374 6564 206c 6973 7420  o a nested list 
+00017ab0: 6f66 2073 7472 696e 6773 0d0a 2020 2020  of strings..    
+00017ac0: 2020 2020 2020 2020 4e6f 7465 733a 0d0a          Notes:..
+00017ad0: 2020 2020 2020 2020 2020 2020 2d61 7267              -arg
+00017ae0: 756d 656e 7473 2061 7265 2070 6172 7365  uments are parse
+00017af0: 6420 706f 7369 7469 6f6e 616c 6c79 0d0a  d positionally..
+00017b00: 2020 2020 2020 2020 2020 2020 2d69 6620              -if 
+00017b10: 6e6f 2061 7267 756d 656e 7420 6973 2070  no argument is p
+00017b20: 726f 7669 6465 642c 2074 6865 2064 6566  rovided, the def
+00017b30: 6175 6c74 206f 6e65 7320 7769 6c6c 2062  ault ones will b
+00017b40: 6520 7573 6564 0d0a 2020 2020 2020 2020  e used..        
+00017b50: 2020 2020 2d75 7365 2031 206f 7220 3020      -use 1 or 0 
+00017b60: 746f 2072 6570 7265 7365 6e74 2054 7275  to represent Tru
+00017b70: 6520 6f72 2046 616c 7365 0d0a 2020 2020  e or False..    
+00017b80: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
+00017b90: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00017ba0: 2020 2020 6d65 7267 655f 6279 5f67 6170      merge_by_gap
+00017bb0: 282e 322c 2031 302c 206c 6f63 6b3d 5472  (.2, 10, lock=Tr
+00017bc0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00017bd0: 2020 2020 206d 673d 2e32 2b31 302b 2b2b       mg=.2+10+++
+00017be0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00017bf0: 2020 204e 6f74 653a 205b 6c6f 636b 5d20     Note: [lock] 
+00017c00: 6973 2074 6865 2035 7468 2061 7267 756d  is the 5th argum
+00017c10: 656e 7420 6865 6e63 6520 7468 6520 3220  ent hence the 2 
+00017c20: 6d69 7373 696e 6720 6172 6775 6d65 6e74  missing argument
+00017c30: 7320 696e 6265 7477 6565 6e20 7468 6520  s inbetween the 
+00017c40: 7468 7265 6520 2b20 6265 666f 7265 2031  three + before 1
+00017c50: 0d0a 2020 2020 2020 2020 2020 2020 4578  ..            Ex
+00017c60: 616d 706c 6520 323a 0d0a 2020 2020 2020  ample 2:..      
+00017c70: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
+00017c80: 6279 5f70 756e 6374 7561 7469 6f6e 285b  by_punctuation([
+00017c90: 2827 2e27 2c20 2720 2729 2c20 27e3 8082  ('.', ' '), '...
+00017ca0: 272c 2027 3f27 2c20 27ef bc9f 275d 2c20  ', '?', '...'], 
+00017cb0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00017cc0: 2020 2020 2020 2073 703d 2e2a 202f e380         sp=.* /..
+00017cd0: 822f 3f2f efbc 9f2b 310d 0a20 2020 2020  ./?/...+1..     
+00017ce0: 2020 2020 2020 2045 7861 6d70 6c65 2033         Example 3
+00017cf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017d00: 2020 206d 6572 6765 5f61 6c6c 5f73 6567     merge_all_seg
+00017d10: 6d65 6e74 7328 292e 7370 6c69 745f 6279  ments().split_by
+00017d20: 5f67 6170 282e 3529 2e6d 6572 6765 5f62  _gap(.5).merge_b
+00017d30: 795f 6761 7028 2e31 352c 2033 290d 0a20  y_gap(.15, 3).. 
+00017d40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017d50: 735f 7367 3d2e 355f 6d67 3d2e 3135 2b33  s_sg=.5_mg=.15+3
+00017d60: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00017d70: 2020 2020 2020 2069 6620 7265 6772 6f75         if regrou
+00017d80: 705f 616c 676f 2069 7320 4661 6c73 653a  p_algo is False:
+00017d90: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00017da0: 7475 726e 2073 656c 660d 0a20 2020 2020  turn self..     
+00017db0: 2020 2069 6620 7265 6772 6f75 705f 616c     if regroup_al
+00017dc0: 676f 2069 7320 4e6f 6e65 206f 7220 7265  go is None or re
+00017dd0: 6772 6f75 705f 616c 676f 2069 7320 5472  group_algo is Tr
+00017de0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00017df0: 2072 6567 726f 7570 5f61 6c67 6f20 3d20   regroup_algo = 
+00017e00: 2764 6127 0d0a 0d0a 2020 2020 2020 2020  'da'....        
+00017e10: 666f 7220 6d65 7468 6f64 2c20 6b77 6172  for method, kwar
+00017e20: 6773 2c20 6d73 6720 696e 2073 656c 662e  gs, msg in self.
+00017e30: 7061 7273 655f 7265 6772 6f75 705f 616c  parse_regroup_al
+00017e40: 676f 2872 6567 726f 7570 5f61 6c67 6f2c  go(regroup_algo,
+00017e50: 2069 6e63 6c75 6465 5f73 7472 3d76 6572   include_str=ver
+00017e60: 626f 7365 206f 7220 6f6e 6c79 5f73 686f  bose or only_sho
+00017e70: 7729 3a0d 0a20 2020 2020 2020 2020 2020  w):..           
+00017e80: 2069 6620 6d73 673a 0d0a 2020 2020 2020   if msg:..      
+00017e90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00017ea0: 6d73 6729 0d0a 2020 2020 2020 2020 2020  msg)..          
+00017eb0: 2020 6966 206e 6f74 206f 6e6c 795f 7368    if not only_sh
+00017ec0: 6f77 3a0d 0a20 2020 2020 2020 2020 2020  ow:..           
+00017ed0: 2020 2020 206d 6574 686f 6428 2a2a 6b77       method(**kw
+00017ee0: 6172 6773 290d 0a0d 0a20 2020 2020 2020  args)....       
+00017ef0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00017f00: 2020 2020 6465 6620 7061 7273 655f 7265      def parse_re
+00017f10: 6772 6f75 705f 616c 676f 2873 656c 662c  group_algo(self,
+00017f20: 2072 6567 726f 7570 5f61 6c67 6f3a 2073   regroup_algo: s
+00017f30: 7472 2c20 696e 636c 7564 655f 7374 723a  tr, include_str:
+00017f40: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
+00017f50: 204c 6973 745b 5475 706c 655b 4361 6c6c   List[Tuple[Call
+00017f60: 6162 6c65 2c20 6469 6374 2c20 7374 725d  able, dict, str]
+00017f70: 5d3a 0d0a 2020 2020 2020 2020 6d65 7468  ]:..        meth
+00017f80: 6f64 7320 3d20 6469 6374 280d 0a20 2020  ods = dict(..   
+00017f90: 2020 2020 2020 2020 2073 673d 7365 6c66           sg=self
+00017fa0: 2e73 706c 6974 5f62 795f 6761 702c 0d0a  .split_by_gap,..
+00017fb0: 2020 2020 2020 2020 2020 2020 7370 3d73              sp=s
+00017fc0: 656c 662e 7370 6c69 745f 6279 5f70 756e  elf.split_by_pun
+00017fd0: 6374 7561 7469 6f6e 2c0d 0a20 2020 2020  ctuation,..     
+00017fe0: 2020 2020 2020 2073 6c3d 7365 6c66 2e73         sl=self.s
+00017ff0: 706c 6974 5f62 795f 6c65 6e67 7468 2c0d  plit_by_length,.
+00018000: 0a20 2020 2020 2020 2020 2020 2073 643d  .            sd=
+00018010: 7365 6c66 2e73 706c 6974 5f62 795f 6475  self.split_by_du
+00018020: 7261 7469 6f6e 2c0d 0a20 2020 2020 2020  ration,..       
+00018030: 2020 2020 206d 673d 7365 6c66 2e6d 6572       mg=self.mer
+00018040: 6765 5f62 795f 6761 702c 0d0a 2020 2020  ge_by_gap,..    
+00018050: 2020 2020 2020 2020 6d70 3d73 656c 662e          mp=self.
+00018060: 6d65 7267 655f 6279 5f70 756e 6374 7561  merge_by_punctua
+00018070: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
+00018080: 2020 206d 733d 7365 6c66 2e6d 6572 6765     ms=self.merge
+00018090: 5f61 6c6c 5f73 6567 6d65 6e74 732c 0d0a  _all_segments,..
+000180a0: 2020 2020 2020 2020 2020 2020 636d 3d73              cm=s
+000180b0: 656c 662e 636c 616d 705f 6d61 782c 0d0a  elf.clamp_max,..
+000180c0: 2020 2020 2020 2020 2020 2020 7573 3d73              us=s
+000180d0: 656c 662e 756e 6c6f 636b 5f61 6c6c 5f73  elf.unlock_all_s
+000180e0: 6567 6d65 6e74 732c 0d0a 2020 2020 2020  egments,..      
+000180f0: 2020 2020 2020 6c3d 7365 6c66 2e6c 6f63        l=self.loc
+00018100: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
+00018110: 7277 3d73 656c 662e 7265 6d6f 7665 5f77  rw=self.remove_w
+00018120: 6f72 642c 0d0a 2020 2020 2020 2020 2020  ord,..          
+00018130: 2020 7273 3d73 656c 662e 7265 6d6f 7665    rs=self.remove
+00018140: 5f73 6567 6d65 6e74 2c0d 0a20 2020 2020  _segment,..     
+00018150: 2020 2020 2020 2072 703d 7365 6c66 2e72         rp=self.r
+00018160: 656d 6f76 655f 7265 7065 7469 7469 6f6e  emove_repetition
+00018170: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00018180: 7773 3d73 656c 662e 7265 6d6f 7665 5f77  ws=self.remove_w
+00018190: 6f72 6473 5f62 795f 7374 722c 0d0a 2020  ords_by_str,..  
+000181a0: 2020 2020 2020 2020 2020 6667 3d73 656c            fg=sel
+000181b0: 662e 6669 6c6c 5f69 6e5f 6761 7073 2c0d  f.fill_in_gaps,.
+000181c0: 0a20 2020 2020 2020 2020 2020 2070 3d73  .            p=s
+000181d0: 656c 662e 7061 642c 0d0a 2020 2020 2020  elf.pad,..      
+000181e0: 2020 290d 0a20 2020 2020 2020 2069 6620    )..        if 
+000181f0: 6e6f 7420 7265 6772 6f75 705f 616c 676f  not regroup_algo
+00018200: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00018210: 6574 7572 6e20 5b5d 0d0a 0d0a 2020 2020  eturn []....    
+00018220: 2020 2020 6361 6c6c 7320 3d20 7265 6772      calls = regr
+00018230: 6f75 705f 616c 676f 2e73 706c 6974 2827  oup_algo.split('
+00018240: 5f27 290d 0a20 2020 2020 2020 2069 6620  _')..        if 
+00018250: 2764 6127 2069 6e20 6361 6c6c 733a 0d0a  'da' in calls:..
+00018260: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00018270: 756c 745f 6361 6c6c 7320 3d20 2763 6d5f  ult_calls = 'cm_
+00018280: 7370 3d2c 2a20 2fef bc8c 5f73 673d 2e35  sp=,* /..._sg=.5
+00018290: 5f6d 673d 2e33 2b33 5f73 703d 2e2a 202f  _mg=.3+3_sp=.* /
+000182a0: e380 822f 3f2f efbc 9f27 2e73 706c 6974  .../?/...'.split
+000182b0: 2827 5f27 290d 0a20 2020 2020 2020 2020  ('_')..         
+000182c0: 2020 2063 616c 6c73 203d 2063 6861 696e     calls = chain
+000182d0: 2e66 726f 6d5f 6974 6572 6162 6c65 2864  .from_iterable(d
+000182e0: 6566 6175 6c74 5f63 616c 6c73 2069 6620  efault_calls if 
+000182f0: 6d65 7468 6f64 203d 3d20 2764 6127 2065  method == 'da' e
+00018300: 6c73 6520 5b6d 6574 686f 645d 2066 6f72  lse [method] for
+00018310: 206d 6574 686f 6420 696e 2063 616c 6c73   method in calls
+00018320: 290d 0a20 2020 2020 2020 206f 7065 7261  )..        opera
+00018330: 7469 6f6e 7320 3d20 5b5d 0d0a 2020 2020  tions = []..    
+00018340: 2020 2020 666f 7220 6d65 7468 6f64 2069      for method i
+00018350: 6e20 6361 6c6c 733a 0d0a 2020 2020 2020  n calls:..      
+00018360: 2020 2020 2020 6d65 7468 6f64 2c20 6172        method, ar
+00018370: 6773 203d 206d 6574 686f 642e 7370 6c69  gs = method.spli
+00018380: 7428 273d 272c 206d 6178 7370 6c69 743d  t('=', maxsplit=
+00018390: 3129 2069 6620 273d 2720 696e 206d 6574  1) if '=' in met
+000183a0: 686f 6420 656c 7365 2028 6d65 7468 6f64  hod else (method
+000183b0: 2c20 2727 290d 0a20 2020 2020 2020 2020  , '')..         
+000183c0: 2020 2069 6620 6d65 7468 6f64 206e 6f74     if method not
+000183d0: 2069 6e20 6d65 7468 6f64 733a 0d0a 2020   in methods:..  
+000183e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000183f0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00018400: 6564 4572 726f 7228 6627 7b6d 6574 686f  edError(f'{metho
+00018410: 647d 2069 7320 6e6f 7420 6f6e 6520 6f66  d} is not one of
+00018420: 2074 6865 2061 7661 696c 6162 6c65 206d   the available m
+00018430: 6574 686f 6473 3a20 7b74 7570 6c65 286d  ethods: {tuple(m
+00018440: 6574 686f 6473 2e6b 6579 7328 2929 7d27  ethods.keys())}'
+00018450: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+00018460: 7267 7320 3d20 5b5d 2069 6620 6c65 6e28  rgs = [] if len(
+00018470: 6172 6773 2920 3d3d 2030 2065 6c73 6520  args) == 0 else 
+00018480: 6c69 7374 286d 6170 2873 7472 5f74 6f5f  list(map(str_to_
+00018490: 7661 6c69 645f 7479 7065 2c20 6172 6773  valid_type, args
+000184a0: 2e73 706c 6974 2827 2b27 2929 290d 0a20  .split('+'))).. 
+000184b0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+000184c0: 7320 3d20 7b6b 3a20 7620 666f 7220 6b2c  s = {k: v for k,
+000184d0: 2076 2069 6e20 7a69 7028 6d65 7468 6f64   v in zip(method
+000184e0: 735b 6d65 7468 6f64 5d2e 5f5f 636f 6465  s[method].__code
+000184f0: 5f5f 2e63 6f5f 7661 726e 616d 6573 5b31  __.co_varnames[1
+00018500: 3a5d 2c20 6172 6773 2920 6966 2076 2069  :], args) if v i
+00018510: 7320 6e6f 7420 4e6f 6e65 7d0d 0a20 2020  s not None}..   
+00018520: 2020 2020 2020 2020 2069 6620 696e 636c           if incl
+00018530: 7564 655f 7374 723a 0d0a 2020 2020 2020  ude_str:..      
+00018540: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00018550: 5f73 7472 203d 2027 2c20 272e 6a6f 696e  _str = ', '.join
+00018560: 2866 277b 6b7d 3d22 7b76 7d22 2720 6966  (f'{k}="{v}"' if
+00018570: 2069 7369 6e73 7461 6e63 6528 762c 2073   isinstance(v, s
+00018580: 7472 2920 656c 7365 2066 277b 6b7d 3d7b  tr) else f'{k}={
+00018590: 767d 2720 666f 7220 6b2c 2076 2069 6e20  v}' for k, v in 
+000185a0: 6b77 6172 6773 2e69 7465 6d73 2829 290d  kwargs.items()).
+000185b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000185c0: 206f 705f 7374 7220 3d20 6627 7b6d 6574   op_str = f'{met
+000185d0: 686f 6473 5b6d 6574 686f 645d 2e5f 5f6e  hods[method].__n
+000185e0: 616d 655f 5f7d 287b 6b77 6172 6773 5f73  ame__}({kwargs_s
+000185f0: 7472 7d29 270d 0a20 2020 2020 2020 2020  tr})'..         
+00018600: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00018610: 2020 2020 2020 2020 2020 6f70 5f73 7472            op_str
+00018620: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+00018630: 2020 2020 206f 7065 7261 7469 6f6e 732e       operations.
+00018640: 6170 7065 6e64 2828 6d65 7468 6f64 735b  append((methods[
+00018650: 6d65 7468 6f64 5d2c 206b 7761 7267 732c  method], kwargs,
+00018660: 206f 705f 7374 7229 290d 0a0d 0a20 2020   op_str))....   
+00018670: 2020 2020 2072 6574 7572 6e20 6f70 6572       return oper
+00018680: 6174 696f 6e73 0d0a 0d0a 2020 2020 6465  ations....    de
+00018690: 6620 6669 6e64 2873 656c 662c 2070 6174  f find(self, pat
+000186a0: 7465 726e 3a20 7374 722c 2077 6f72 645f  tern: str, word_
+000186b0: 6c65 7665 6c3d 5472 7565 2c20 666c 6167  level=True, flag
+000186c0: 733d 4e6f 6e65 2920 2d3e 2022 5768 6973  s=None) -> "Whis
+000186d0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
+000186e0: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
+000186f0: 0a20 2020 2020 2020 2046 696e 6420 7365  .        Find se
+00018700: 676d 656e 7473 2f77 6f72 6473 2061 6e64  gments/words and
+00018710: 2074 696d 6573 7461 6d70 7320 7769 7468   timestamps with
+00018720: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
+00018730: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
+00018740: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00018750: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00018760: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
+00018770: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
+00018780: 2020 2052 6567 4578 2070 6174 7465 726e     RegEx pattern
+00018790: 2074 6f20 7365 6172 6368 2066 6f72 2e0d   to search for..
+000187a0: 0a20 2020 2020 2020 2077 6f72 645f 6c65  .        word_le
+000187b0: 7665 6c20 3a20 626f 6f6c 2c20 6465 6661  vel : bool, defa
+000187c0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+000187d0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000187e0: 2073 6561 7263 6820 6174 2077 6f72 642d   search at word-
+000187f0: 6c65 7665 6c2e 0d0a 2020 2020 2020 2020  level...        
+00018800: 666c 6167 7320 3a20 6f70 7469 6f6e 616c  flags : optional
+00018810: 0d0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00018820: 6745 7820 666c 6167 732e 0d0a 0d0a 2020  gEx flags.....  
+00018830: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+00018840: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+00018850: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+00018860: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+00018870: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
+00018880: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+00018890: 416e 2069 6e73 7461 6e63 6520 6f66 203a  An instance of :
+000188a0: 636c 6173 733a 6073 7461 626c 655f 7768  class:`stable_wh
+000188b0: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+000188c0: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
+000188d0: 7360 2077 6974 6820 776f 7264 2f73 6567  s` with word/seg
+000188e0: 6d65 6e74 2074 6861 7420 6d61 7463 6820  ment that match 
+000188f0: 6060 7061 7474 6572 6e60 602e 0d0a 2020  ``pattern``...  
+00018900: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00018910: 2020 2072 6574 7572 6e20 5768 6973 7065     return Whispe
+00018920: 7252 6573 756c 744d 6174 6368 6573 2873  rResultMatches(s
+00018930: 656c 6629 2e66 696e 6428 7061 7474 6572  elf).find(patter
+00018940: 6e2c 2077 6f72 645f 6c65 7665 6c3d 776f  n, word_level=wo
+00018950: 7264 5f6c 6576 656c 2c20 666c 6167 733d  rd_level, flags=
+00018960: 666c 6167 7329 0d0a 0d0a 2020 2020 4070  flags)....    @p
+00018970: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00018980: 2074 6578 7428 7365 6c66 293a 0d0a 2020   text(self):..  
+00018990: 2020 2020 2020 7265 7475 726e 2027 272e        return ''.
+000189a0: 6a6f 696e 2873 2e74 6578 7420 666f 7220  join(s.text for 
+000189b0: 7320 696e 2073 656c 662e 7365 676d 656e  s in self.segmen
+000189c0: 7473 290d 0a0d 0a20 2020 2040 7072 6f70  ts)....    @prop
+000189d0: 6572 7479 0d0a 2020 2020 6465 6620 7265  erty..    def re
+000189e0: 6772 6f75 705f 6869 7374 6f72 7928 7365  group_history(se
+000189f0: 6c66 293a 0d0a 2020 2020 2020 2020 2320  lf):..        # 
+00018a00: 7361 6d65 2073 796e 7461 7820 6173 2060  same syntax as `
+00018a10: 6072 6567 726f 7570 5f61 6c67 6f60 6020  `regroup_algo`` 
+00018a20: 666f 7220 3a6d 6574 683a 6060 7265 7375  for :meth:``resu
+00018a30: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
+00018a40: 2e72 6567 726f 7570 600d 0a20 2020 2020  .regroup`..     
+00018a50: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00018a60: 7265 6772 6f75 705f 6869 7374 6f72 790d  regroup_history.
+00018a70: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00018a80: 0d0a 2020 2020 6465 6620 6e6f 6e73 7065  ..    def nonspe
+00018a90: 6563 685f 7365 6374 696f 6e73 2873 656c  ech_sections(sel
+00018aa0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00018ab0: 7572 6e20 7365 6c66 2e5f 6e6f 6e73 7065  urn self._nonspe
+00018ac0: 6563 685f 7365 6374 696f 6e73 0d0a 0d0a  ech_sections....
+00018ad0: 2020 2020 6465 6620 7368 6f77 5f72 6567      def show_reg
+00018ae0: 726f 7570 5f68 6973 746f 7279 2873 656c  roup_history(sel
+00018af0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00018b00: 0d0a 2020 2020 2020 2020 5072 696e 7420  ..        Print 
+00018b10: 6465 7461 696c 7320 6f66 2061 6c6c 2072  details of all r
+00018b20: 6567 726f 7570 696e 6720 6f70 6572 6174  egrouping operat
+00018b30: 696f 6e73 2074 6861 7420 6265 656e 2070  ions that been p
+00018b40: 6572 666f 726d 6564 206f 6e20 6461 7461  erformed on data
+00018b50: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00018b60: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00018b70: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+00018b80: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
+00018b90: 2020 2070 7269 6e74 2827 5265 7375 6c74     print('Result
+00018ba0: 2068 6173 206e 6f20 6869 7374 6f72 792e   has no history.
+00018bb0: 2729 0d0a 2020 2020 2020 2020 666f 7220  ')..        for 
+00018bc0: 2a5f 2c20 6d73 6720 696e 2073 656c 662e  *_, msg in self.
+00018bd0: 7061 7273 655f 7265 6772 6f75 705f 616c  parse_regroup_al
+00018be0: 676f 2873 656c 662e 5f72 6567 726f 7570  go(self._regroup
+00018bf0: 5f68 6973 746f 7279 293a 0d0a 2020 2020  _history):..    
+00018c00: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00018c10: 2e7b 6d73 677d 2729 0d0a 0d0a 2020 2020  .{msg}')....    
+00018c20: 6465 6620 5f5f 6c65 6e5f 5f28 7365 6c66  def __len__(self
+00018c30: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00018c40: 726e 206c 656e 2873 656c 662e 7365 676d  rn len(self.segm
+00018c50: 656e 7473 290d 0a0d 0a20 2020 2064 6566  ents)....    def
+00018c60: 2075 6e6c 6f63 6b5f 616c 6c5f 7365 676d   unlock_all_segm
+00018c70: 656e 7473 2873 656c 6629 3a0d 0a20 2020  ents(self):..   
+00018c80: 2020 2020 2066 6f72 2073 2069 6e20 7365       for s in se
+00018c90: 6c66 2e73 6567 6d65 6e74 733a 0d0a 2020  lf.segments:..  
+00018ca0: 2020 2020 2020 2020 2020 732e 756e 6c6f            s.unlo
+00018cb0: 636b 5f61 6c6c 5f77 6f72 6473 2829 0d0a  ck_all_words()..
+00018cc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018cd0: 656c 660d 0a0d 0a20 2020 2064 6566 2073  elf....    def s
+00018ce0: 6574 5f63 7572 7265 6e74 5f61 735f 6f72  et_current_as_or
+00018cf0: 6967 2873 656c 662c 206b 6565 705f 6f72  ig(self, keep_or
+00018d00: 6967 3a20 626f 6f6c 203d 2046 616c 7365  ig: bool = False
+00018d10: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00018d20: 0a20 2020 2020 2020 204f 7665 7277 7269  .        Overwri
+00018d30: 7465 2061 6c6c 2076 616c 7565 7320 696e  te all values in
+00018d40: 2060 606f 7269 5f64 6963 7460 6020 7769   ``ori_dict`` wi
+00018d50: 7468 2063 7572 7265 6e74 2076 616c 7565  th current value
+00018d60: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
+00018d70: 0a20 2020 2020 2020 2073 656c 662e 6f72  .        self.or
+00018d80: 695f 6469 6374 203d 2073 656c 662e 746f  i_dict = self.to
+00018d90: 5f64 6963 7428 6b65 6570 5f6f 7269 673d  _dict(keep_orig=
+00018da0: 6b65 6570 5f6f 7269 6729 0d0a 0d0a 2020  keep_orig)....  
+00018db0: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
+00018dc0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+00018dd0: 0a20 2020 2020 2020 2052 6573 746f 7265  .        Restore
+00018de0: 2061 6c6c 2076 616c 7565 7320 746f 2074   all values to t
+00018df0: 6861 7420 6174 2069 6e69 7469 616c 697a  hat at initializ
+00018e00: 6174 696f 6e20 696e 2060 606f 7269 5f64  ation in ``ori_d
+00018e10: 6963 7460 602e 0d0a 2020 2020 2020 2020  ict``...        
+00018e20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00018e30: 662e 6c61 6e67 7561 6765 203d 2073 656c  f.language = sel
+00018e40: 662e 6f72 695f 6469 6374 2e67 6574 2827  f.ori_dict.get('
+00018e50: 6c61 6e67 7561 6765 2729 0d0a 2020 2020  language')..    
+00018e60: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
+00018e70: 705f 6869 7374 6f72 7920 3d20 2727 0d0a  p_history = ''..
+00018e80: 2020 2020 2020 2020 7365 676d 656e 7473          segments
+00018e90: 203d 2073 656c 662e 6f72 695f 6469 6374   = self.ori_dict
+00018ea0: 2e67 6574 2827 7365 676d 656e 7473 2729  .get('segments')
+00018eb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00018ec0: 6567 6d65 6e74 7320 3d20 5b53 6567 6d65  egments = [Segme
+00018ed0: 6e74 282a 2a73 2c20 6967 6e6f 7265 5f75  nt(**s, ignore_u
+00018ee0: 6e75 7365 645f 6172 6773 3d54 7275 6529  nused_args=True)
+00018ef0: 2066 6f72 2073 2069 6e20 7365 676d 656e   for s in segmen
+00018f00: 7473 5d20 6966 2073 6567 6d65 6e74 7320  ts] if segments 
+00018f10: 656c 7365 205b 5d0d 0a20 2020 2020 2020  else []..       
+00018f20: 2069 6620 7365 6c66 2e5f 666f 7263 6564   if self._forced
+00018f30: 5f6f 7264 6572 3a0d 0a20 2020 2020 2020  _order:..       
+00018f40: 2020 2020 2073 656c 662e 666f 7263 655f       self.force_
+00018f50: 6f72 6465 7228 290d 0a20 2020 2020 2020  order()..       
+00018f60: 2073 656c 662e 7265 6d6f 7665 5f6e 6f5f   self.remove_no_
+00018f70: 776f 7264 5f73 6567 6d65 6e74 7328 616e  word_segments(an
+00018f80: 7928 7365 672e 6861 735f 776f 7264 7320  y(seg.has_words 
+00018f90: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
+00018fa0: 7365 676d 656e 7473 2929 0d0a 0d0a 2020  segments))....  
+00018fb0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00018fc0: 2064 6566 2068 6173 5f77 6f72 6473 2873   def has_words(s
+00018fd0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00018fe0: 6574 7572 6e20 626f 6f6c 2873 656c 662e  eturn bool(self.
+00018ff0: 7365 676d 656e 7473 2920 616e 6420 616c  segments) and al
+00019000: 6c28 7365 672e 6861 735f 776f 7264 7320  l(seg.has_words 
+00019010: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
+00019020: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
+00019030: 2074 6f5f 7372 745f 7674 7420 3d20 7265   to_srt_vtt = re
+00019040: 7375 6c74 5f74 6f5f 7372 745f 7674 740d  sult_to_srt_vtt.
+00019050: 0a20 2020 2074 6f5f 6173 7320 3d20 7265  .    to_ass = re
+00019060: 7375 6c74 5f74 6f5f 6173 730d 0a20 2020  sult_to_ass..   
+00019070: 2074 6f5f 7473 7620 3d20 7265 7375 6c74   to_tsv = result
+00019080: 5f74 6f5f 7473 760d 0a20 2020 2074 6f5f  _to_tsv..    to_
+00019090: 7478 7420 3d20 7265 7375 6c74 5f74 6f5f  txt = result_to_
+000190a0: 7478 740d 0a20 2020 2073 6176 655f 6173  txt..    save_as
+000190b0: 5f6a 736f 6e20 3d20 7361 7665 5f61 735f  _json = save_as_
+000190c0: 6a73 6f6e 0d0a 0d0a 0d0a 636c 6173 7320  json......class 
+000190d0: 5365 676d 656e 744d 6174 6368 3a0d 0a0d  SegmentMatch:...
+000190e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000190f0: 5f28 0d0a 2020 2020 2020 2020 2020 2020  _(..            
+00019100: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00019110: 2020 2073 6567 6d65 6e74 733a 2055 6e69     segments: Uni
+00019120: 6f6e 5b4c 6973 745b 5365 676d 656e 745d  on[List[Segment]
+00019130: 2c20 5365 676d 656e 745d 2c0d 0a20 2020  , Segment],..   
+00019140: 2020 2020 2020 2020 205f 776f 7264 5f69           _word_i
+00019150: 6e64 6963 6573 3a20 4c69 7374 5b4c 6973  ndices: List[Lis
+00019160: 745b 696e 745d 5d20 3d20 4e6f 6e65 2c0d  t[int]] = None,.
+00019170: 0a20 2020 2020 2020 2020 2020 205f 7465  .            _te
+00019180: 7874 5f6d 6174 6368 3a20 7374 7220 3d20  xt_match: str = 
+00019190: 4e6f 6e65 0d0a 2020 2020 293a 0d0a 2020  None..    ):..  
+000191a0: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
+000191b0: 6e74 7320 3d20 5b73 6567 6d65 6e74 735d  nts = [segments]
+000191c0: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
+000191d0: 6567 6d65 6e74 732c 2053 6567 6d65 6e74  egments, Segment
+000191e0: 2920 656c 7365 2073 6567 6d65 6e74 730d  ) else segments.
+000191f0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
+00019200: 7264 5f69 6e64 6963 6573 203d 205b 5d20  rd_indices = [] 
+00019210: 6966 205f 776f 7264 5f69 6e64 6963 6573  if _word_indices
+00019220: 2069 7320 4e6f 6e65 2065 6c73 6520 5f77   is None else _w
+00019230: 6f72 645f 696e 6469 6365 730d 0a20 2020  ord_indices..   
+00019240: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
+00019250: 3d20 5b73 656c 662e 7365 676d 656e 7473  = [self.segments
+00019260: 5b69 5d2e 776f 7264 735b 6a5d 2066 6f72  [i].words[j] for
+00019270: 2069 2c20 696e 6469 6365 7320 696e 2065   i, indices in e
+00019280: 6e75 6d65 7261 7465 2873 656c 662e 776f  numerate(self.wo
+00019290: 7264 5f69 6e64 6963 6573 2920 666f 7220  rd_indices) for 
+000192a0: 6a20 696e 2069 6e64 6963 6573 5d0d 0a20  j in indices].. 
+000192b0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+000192c0: 6c66 2e77 6f72 6473 2920 213d 2030 3a0d  lf.words) != 0:.
+000192d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000192e0: 662e 7465 7874 203d 2027 272e 6a6f 696e  f.text = ''.join
+000192f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00019300: 2020 2073 656c 662e 7365 676d 656e 7473     self.segments
+00019310: 5b69 5d2e 776f 7264 735b 6a5d 2e77 6f72  [i].words[j].wor
+00019320: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00019330: 2020 2066 6f72 2069 2c20 696e 6469 6365     for i, indice
+00019340: 7320 696e 2065 6e75 6d65 7261 7465 2873  s in enumerate(s
+00019350: 656c 662e 776f 7264 5f69 6e64 6963 6573  elf.word_indices
+00019360: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019370: 2020 2066 6f72 206a 2069 6e20 696e 6469     for j in indi
+00019380: 6365 730d 0a20 2020 2020 2020 2020 2020  ces..           
+00019390: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
+000193a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000193b0: 656c 662e 7465 7874 203d 2027 272e 6a6f  elf.text = ''.jo
+000193c0: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
+000193d0: 7365 6720 696e 2073 656c 662e 7365 676d  seg in self.segm
+000193e0: 656e 7473 290d 0a20 2020 2020 2020 2073  ents)..        s
+000193f0: 656c 662e 7465 7874 5f6d 6174 6368 203d  elf.text_match =
+00019400: 205f 7465 7874 5f6d 6174 6368 0d0a 0d0a   _text_match....
+00019410: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00019420: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
+00019430: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00019440: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
+00019450: 2020 2073 656c 662e 776f 7264 735b 305d     self.words[0]
+00019460: 2e73 7461 7274 0d0a 2020 2020 2020 2020  .start..        
+00019470: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00019480: 776f 7264 7329 2021 3d20 3020 656c 7365  words) != 0 else
+00019490: 0d0a 2020 2020 2020 2020 2020 2020 2873  ..            (s
+000194a0: 656c 662e 7365 676d 656e 7473 5b30 5d2e  elf.segments[0].
+000194b0: 7374 6172 7420 6966 206c 656e 2873 656c  start if len(sel
+000194c0: 662e 7365 676d 656e 7473 2920 213d 2030  f.segments) != 0
+000194d0: 2065 6c73 6520 4e6f 6e65 290d 0a20 2020   else None)..   
+000194e0: 2020 2020 2029 0d0a 0d0a 2020 2020 4070       )....    @p
+000194f0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00019500: 2065 6e64 2873 656c 6629 3a0d 0a20 2020   end(self):..   
+00019510: 2020 2020 2072 6574 7572 6e20 280d 0a20       return (.. 
+00019520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019530: 776f 7264 735b 2d31 5d2e 656e 640d 0a20  words[-1].end.. 
+00019540: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00019550: 6e28 7365 6c66 2e77 6f72 6473 2920 213d  n(self.words) !=
+00019560: 2030 2065 6c73 650d 0a20 2020 2020 2020   0 else..       
+00019570: 2020 2020 2028 7365 6c66 2e73 6567 6d65       (self.segme
+00019580: 6e74 735b 2d31 5d2e 656e 6420 6966 206c  nts[-1].end if l
+00019590: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
+000195a0: 2920 213d 2030 2065 6c73 6520 4e6f 6e65  ) != 0 else None
+000195b0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
+000195c0: 2020 2020 6465 6620 5f5f 6c65 6e5f 5f28      def __len__(
+000195d0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000195e0: 7265 7475 726e 206c 656e 2873 656c 662e  return len(self.
+000195f0: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
+00019600: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+00019610: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00019620: 7475 726e 2073 656c 662e 5f5f 6469 6374  turn self.__dict
+00019630: 5f5f 2e5f 5f72 6570 725f 5f28 290d 0a0d  __.__repr__()...
+00019640: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+00019650: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00019660: 2072 6574 7572 6e20 7365 6c66 2e5f 5f64   return self.__d
+00019670: 6963 745f 5f2e 5f5f 7374 725f 5f28 290d  ict__.__str__().
+00019680: 0a0d 0a0d 0a63 6c61 7373 2057 6869 7370  .....class Whisp
+00019690: 6572 5265 7375 6c74 4d61 7463 6865 733a  erResultMatches:
+000196a0: 0d0a 2020 2020 2222 220d 0a20 2020 2052  ..    """..    R
+000196b0: 6567 4578 206d 6174 6368 6573 2066 6f72  egEx matches for
+000196c0: 2057 6869 7370 6572 5265 7375 6c74 732e   WhisperResults.
+000196d0: 0d0a 2020 2020 2222 220d 0a20 2020 2023  ..    """..    #
+000196e0: 2055 7365 2057 6869 7370 6572 5265 7375   Use WhisperResu
+000196f0: 6c74 2e66 696e 6428 2920 696e 7374 6561  lt.find() instea
+00019700: 6420 6f66 2069 6e73 7461 6e74 6961 7469  d of instantiati
+00019710: 6e67 2074 6869 7320 636c 6173 7320 6469  ng this class di
+00019720: 7265 6374 6c79 2e0d 0a20 2020 2064 6566  rectly...    def
+00019730: 205f 5f69 6e69 745f 5f28 0d0a 2020 2020   __init__(..    
+00019740: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+00019750: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00019760: 6573 3a20 556e 696f 6e5b 4c69 7374 5b53  es: Union[List[S
+00019770: 6567 6d65 6e74 4d61 7463 685d 2c20 5768  egmentMatch], Wh
+00019780: 6973 7065 7252 6573 756c 745d 2c0d 0a20  isperResult],.. 
+00019790: 2020 2020 2020 2020 2020 205f 7365 676d             _segm
+000197a0: 656e 745f 696e 6469 6365 733a 204c 6973  ent_indices: Lis
+000197b0: 745b 4c69 7374 5b69 6e74 5d5d 203d 204e  t[List[int]] = N
+000197c0: 6f6e 650d 0a20 2020 2029 3a0d 0a20 2020  one..    ):..   
+000197d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000197e0: 6365 286d 6174 6368 6573 2c20 5768 6973  ce(matches, Whis
+000197f0: 7065 7252 6573 756c 7429 3a0d 0a20 2020  perResult):..   
+00019800: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00019810: 7463 6865 7320 3d20 6c69 7374 286d 6170  tches = list(map
+00019820: 2853 6567 6d65 6e74 4d61 7463 682c 206d  (SegmentMatch, m
+00019830: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
+00019840: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00019850: 656c 662e 5f73 6567 6d65 6e74 5f69 6e64  elf._segment_ind
+00019860: 6963 6573 203d 205b 5b69 5d20 666f 7220  ices = [[i] for 
+00019870: 6920 696e 2072 616e 6765 286c 656e 286d  i in range(len(m
+00019880: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
+00019890: 295d 0d0a 2020 2020 2020 2020 656c 7365  )]..        else
+000198a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000198b0: 656c 662e 6d61 7463 6865 7320 3d20 6d61  elf.matches = ma
+000198c0: 7463 6865 730d 0a20 2020 2020 2020 2020  tches..         
+000198d0: 2020 2061 7373 6572 7420 5f73 6567 6d65     assert _segme
+000198e0: 6e74 5f69 6e64 6963 6573 2069 7320 6e6f  nt_indices is no
+000198f0: 7420 4e6f 6e65 0d0a 2020 2020 2020 2020  t None..        
+00019900: 2020 2020 6173 7365 7274 206c 656e 2873      assert len(s
+00019910: 656c 662e 6d61 7463 6865 7329 203d 3d20  elf.matches) == 
+00019920: 6c65 6e28 5f73 6567 6d65 6e74 5f69 6e64  len(_segment_ind
+00019930: 6963 6573 290d 0a20 2020 2020 2020 2020  ices)..         
+00019940: 2020 2061 7373 6572 7420 616c 6c28 6c65     assert all(le
+00019950: 6e28 6d61 7463 682e 7365 676d 656e 7473  n(match.segments
+00019960: 2920 3d3d 206c 656e 285f 7365 676d 656e  ) == len(_segmen
+00019970: 745f 696e 6469 6365 735b 695d 2920 666f  t_indices[i]) fo
+00019980: 7220 692c 206d 6174 6368 2069 6e20 656e  r i, match in en
+00019990: 756d 6572 6174 6528 7365 6c66 2e6d 6174  umerate(self.mat
+000199a0: 6368 6573 2929 0d0a 2020 2020 2020 2020  ches))..        
+000199b0: 2020 2020 7365 6c66 2e5f 7365 676d 656e      self._segmen
+000199c0: 745f 696e 6469 6365 7320 3d20 5f73 6567  t_indices = _seg
+000199d0: 6d65 6e74 5f69 6e64 6963 6573 0d0a 0d0a  ment_indices....
+000199e0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000199f0: 2020 2064 6566 2073 6567 6d65 6e74 5f69     def segment_i
+00019a00: 6e64 6963 6573 2873 656c 6629 3a0d 0a20  ndices(self):.. 
+00019a10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00019a20: 6c66 2e5f 7365 676d 656e 745f 696e 6469  lf._segment_indi
+00019a30: 6365 730d 0a0d 0a20 2020 2064 6566 205f  ces....    def _
+00019a40: 6375 7272 5f73 6567 5f67 726f 7570 7328  curr_seg_groups(
+00019a50: 7365 6c66 2920 2d3e 204c 6973 745b 4c69  self) -> List[Li
+00019a60: 7374 5b54 7570 6c65 5b69 6e74 2c20 5365  st[Tuple[int, Se
+00019a70: 676d 656e 745d 5d5d 3a0d 0a20 2020 2020  gment]]]:..     
+00019a80: 2020 2073 6567 5f67 726f 7570 732c 2063     seg_groups, c
+00019a90: 7572 725f 7365 6773 203d 205b 5d2c 205b  urr_segs = [], [
+00019aa0: 5d0d 0a20 2020 2020 2020 2063 7572 725f  ]..        curr_
+00019ab0: 6d61 7820 3d20 2d31 0d0a 2020 2020 2020  max = -1..      
+00019ac0: 2020 666f 7220 7365 675f 696e 6469 6365    for seg_indice
+00019ad0: 732c 206d 6174 6368 2069 6e20 7a69 7028  s, match in zip(
+00019ae0: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
+00019af0: 6469 6365 732c 2073 656c 662e 6d61 7463  dices, self.matc
+00019b00: 6865 7329 3a0d 0a20 2020 2020 2020 2020  hes):..         
+00019b10: 2020 2066 6f72 2069 2c20 7365 6720 696e     for i, seg in
+00019b20: 207a 6970 2873 6f72 7465 6428 7365 675f   zip(sorted(seg_
+00019b30: 696e 6469 6365 7329 2c20 6d61 7463 682e  indices), match.
+00019b40: 7365 676d 656e 7473 293a 0d0a 2020 2020  segments):..    
+00019b50: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00019b60: 203e 2063 7572 725f 6d61 783a 0d0a 2020   > curr_max:..  
+00019b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b80: 2020 6375 7272 5f73 6567 732e 6170 7065    curr_segs.appe
+00019b90: 6e64 2828 692c 2073 6567 2929 0d0a 2020  nd((i, seg))..  
+00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bb0: 2020 6966 2069 202d 2031 2021 3d20 6375    if i - 1 != cu
+00019bc0: 7272 5f6d 6178 3a0d 0a20 2020 2020 2020  rr_max:..       
+00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019be0: 2073 6567 5f67 726f 7570 732e 6170 7065   seg_groups.appe
+00019bf0: 6e64 2863 7572 725f 7365 6773 290d 0a20  nd(curr_segs).. 
+00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c10: 2020 2020 2020 2063 7572 725f 7365 6773         curr_segs
+00019c20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00019c30: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
+00019c40: 6d61 7820 3d20 690d 0a0d 0a20 2020 2020  max = i....     
+00019c50: 2020 2069 6620 6375 7272 5f73 6567 733a     if curr_segs:
+00019c60: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00019c70: 675f 6772 6f75 7073 2e61 7070 656e 6428  g_groups.append(
+00019c80: 6375 7272 5f73 6567 7329 0d0a 2020 2020  curr_segs)..    
+00019c90: 2020 2020 7265 7475 726e 2073 6567 5f67      return seg_g
+00019ca0: 726f 7570 730d 0a0d 0a20 2020 2064 6566  roups....    def
+00019cb0: 2066 696e 6428 7365 6c66 2c20 7061 7474   find(self, patt
+00019cc0: 6572 6e3a 2073 7472 2c20 776f 7264 5f6c  ern: str, word_l
+00019cd0: 6576 656c 3d54 7275 652c 2066 6c61 6773  evel=True, flags
+00019ce0: 3d4e 6f6e 6529 202d 3e20 2257 6869 7370  =None) -> "Whisp
+00019cf0: 6572 5265 7375 6c74 4d61 7463 6865 7322  erResultMatches"
+00019d00: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00019d10: 2020 2020 2020 2020 4669 6e64 2073 6567          Find seg
+00019d20: 6d65 6e74 732f 776f 7264 7320 616e 6420  ments/words and 
+00019d30: 7469 6d65 7374 616d 7073 2077 6974 6820  timestamps with 
+00019d40: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00019d50: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2050  on.....        P
+00019d60: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00019d70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00019d80: 2020 2020 2020 2070 6174 7465 726e 203a         pattern :
+00019d90: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00019da0: 2020 5265 6745 7820 7061 7474 6572 6e20    RegEx pattern 
+00019db0: 746f 2073 6561 7263 6820 666f 722e 0d0a  to search for...
+00019dc0: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
+00019dd0: 656c 203a 2062 6f6f 6c2c 2064 6566 6175  el : bool, defau
+00019de0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00019df0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00019e00: 7365 6172 6368 2061 7420 776f 7264 2d6c  search at word-l
+00019e10: 6576 656c 2e0d 0a20 2020 2020 2020 2066  evel...        f
+00019e20: 6c61 6773 203a 206f 7074 696f 6e61 6c0d  lags : optional.
+00019e30: 0a20 2020 2020 2020 2020 2020 2052 6567  .            Reg
+00019e40: 4578 2066 6c61 6773 2e0d 0a0d 0a20 2020  Ex flags.....   
+00019e50: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00019e60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00019e70: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+00019e80: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+00019e90: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
+00019ea0: 730d 0a20 2020 2020 2020 2020 2020 2041  s..            A
+00019eb0: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
+00019ec0: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
+00019ed0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+00019ee0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
+00019ef0: 6020 7769 7468 2077 6f72 642f 7365 676d  ` with word/segm
+00019f00: 656e 7420 7468 6174 206d 6174 6368 2060  ent that match `
+00019f10: 6070 6174 7465 726e 6060 2e0d 0a20 2020  `pattern``...   
+00019f20: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+00019f30: 2020 2020 7365 675f 6772 6f75 7073 203d      seg_groups =
+00019f40: 2073 656c 662e 5f63 7572 725f 7365 675f   self._curr_seg_
+00019f50: 6772 6f75 7073 2829 0d0a 2020 2020 2020  groups()..      
+00019f60: 2020 6d61 7463 6865 733a 204c 6973 745b    matches: List[
+00019f70: 5365 676d 656e 744d 6174 6368 5d20 3d20  SegmentMatch] = 
+00019f80: 5b5d 0d0a 2020 2020 2020 2020 6d61 7463  []..        matc
+00019f90: 685f 7365 675f 696e 6469 6365 733a 204c  h_seg_indices: L
+00019fa0: 6973 745b 4c69 7374 5b69 6e74 5d5d 203d  ist[List[int]] =
+00019fb0: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
+00019fc0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
+00019fd0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00019fe0: 616c 6c28 616c 6c28 7365 672e 6861 735f  all(all(seg.has_
+00019ff0: 776f 7264 7320 666f 7220 7365 6720 696e  words for seg in
+0001a000: 206d 6174 6368 2e73 6567 6d65 6e74 7329   match.segments)
+0001a010: 2066 6f72 206d 6174 6368 2069 6e20 7365   for match in se
+0001a020: 6c66 2e6d 6174 6368 6573 293a 0d0a 2020  lf.matches):..  
+0001a030: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+0001a040: 726e 696e 6773 2e77 6172 6e28 2743 616e  rnings.warn('Can
+0001a050: 6e6f 7420 7065 7266 6f72 6d20 776f 7264  not perform word
+0001a060: 2d6c 6576 656c 2073 6561 7263 6820 7769  -level search wi
+0001a070: 7468 2073 6567 6d65 6e74 2873 2920 6d69  th segment(s) mi
+0001a080: 7373 696e 6720 776f 7264 2074 696d 6573  ssing word times
+0001a090: 7461 6d70 732e 2729 0d0a 2020 2020 2020  tamps.')..      
+0001a0a0: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
+0001a0b0: 6576 656c 203d 2046 616c 7365 0d0a 0d0a  evel = False....
+0001a0c0: 2020 2020 2020 2020 666f 7220 7365 6773          for segs
+0001a0d0: 2069 6e20 7365 675f 6772 6f75 7073 3a0d   in seg_groups:.
+0001a0e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a0f0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
+0001a100: 2020 2020 2020 2020 2020 2020 2069 6478               idx
+0001a110: 7320 3d20 6c69 7374 2863 6861 696e 2e66  s = list(chain.f
+0001a120: 726f 6d5f 6974 6572 6162 6c65 280d 0a20  rom_iterable(.. 
+0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a140: 2020 205b 2869 2c20 6a29 5d2a 6c65 6e28     [(i, j)]*len(
+0001a150: 776f 7264 2e77 6f72 6429 2066 6f72 2028  word.word) for (
+0001a160: 692c 2073 6567 2920 696e 2073 6567 7320  i, seg) in segs 
+0001a170: 666f 7220 6a2c 2077 6f72 6420 696e 2065  for j, word in e
+0001a180: 6e75 6d65 7261 7465 2873 6567 2e77 6f72  numerate(seg.wor
+0001a190: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+0001a1a0: 2020 2020 2029 290d 0a20 2020 2020 2020       ))..       
+0001a1b0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+0001a1c0: 2727 2e6a 6f69 6e28 776f 7264 2e77 6f72  ''.join(word.wor
+0001a1d0: 6420 666f 7220 285f 2c20 7365 6729 2069  d for (_, seg) i
+0001a1e0: 6e20 7365 6773 2066 6f72 2077 6f72 6420  n segs for word 
+0001a1f0: 696e 2073 6567 2e77 6f72 6473 290d 0a20  in seg.words).. 
+0001a200: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001a210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a220: 2020 6964 7873 203d 206c 6973 7428 6368    idxs = list(ch
+0001a230: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
+0001a240: 6528 5b28 692c 204e 6f6e 6529 5d2a 6c65  e([(i, None)]*le
+0001a250: 6e28 7365 672e 7465 7874 2920 666f 7220  n(seg.text) for 
+0001a260: 2869 2c20 7365 6729 2069 6e20 7365 6773  (i, seg) in segs
+0001a270: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001a280: 2020 2020 7465 7874 203d 2027 272e 6a6f      text = ''.jo
+0001a290: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
+0001a2a0: 285f 2c20 7365 6729 2069 6e20 7365 6773  (_, seg) in segs
+0001a2b0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001a2c0: 7373 6572 7420 6c65 6e28 6964 7873 2920  ssert len(idxs) 
+0001a2d0: 3d3d 206c 656e 2874 6578 7429 0d0a 2020  == len(text)..  
+0001a2e0: 2020 2020 2020 2020 2020 666f 7220 6375            for cu
+0001a2f0: 7272 5f6d 6174 6368 2069 6e20 7265 2e66  rr_match in re.f
+0001a300: 696e 6469 7465 7228 7061 7474 6572 6e2c  inditer(pattern,
+0001a310: 2074 6578 742c 2066 6c61 6773 3d66 6c61   text, flags=fla
+0001a320: 6773 206f 7220 3029 3a0d 0a20 2020 2020  gs or 0):..     
+0001a330: 2020 2020 2020 2020 2020 2073 7461 7274             start
+0001a340: 2c20 656e 6420 3d20 6375 7272 5f6d 6174  , end = curr_mat
+0001a350: 6368 2e73 7061 6e28 290d 0a20 2020 2020  ch.span()..     
+0001a360: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
+0001a370: 6964 7873 203d 2069 6478 735b 7374 6172  idxs = idxs[star
+0001a380: 743a 2065 6e64 5d0d 0a20 2020 2020 2020  t: end]..       
+0001a390: 2020 2020 2020 2020 2063 7572 725f 7365           curr_se
+0001a3a0: 675f 6964 7873 203d 2073 6f72 7465 6428  g_idxs = sorted(
+0001a3b0: 7365 7428 695b 305d 2066 6f72 2069 2069  set(i[0] for i i
+0001a3c0: 6e20 6375 7272 5f69 6478 7329 290d 0a20  n curr_idxs)).. 
+0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a3e0: 6620 776f 7264 5f6c 6576 656c 3a0d 0a20  f word_level:.. 
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a400: 2020 2063 7572 725f 776f 7264 5f69 6478     curr_word_idx
+0001a410: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a430: 6f72 7465 6428 7365 7428 6a20 666f 7220  orted(set(j for 
+0001a440: 692c 206a 2069 6e20 6375 7272 5f69 6478  i, j in curr_idx
+0001a450: 7320 6966 2069 203d 3d20 7365 675f 6964  s if i == seg_id
+0001a460: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+0001a470: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001a480: 2073 6567 5f69 6478 2069 6e20 6375 7272   seg_idx in curr
+0001a490: 5f73 6567 5f69 6478 730d 0a20 2020 2020  _seg_idxs..     
+0001a4a0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0001a4b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a4c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001a4d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0001a4e0: 725f 776f 7264 5f69 6478 7320 3d20 4e6f  r_word_idxs = No
+0001a4f0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+0001a500: 2020 2020 6d61 7463 6865 732e 6170 7065      matches.appe
+0001a510: 6e64 2853 6567 6d65 6e74 4d61 7463 6828  nd(SegmentMatch(
+0001a520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a530: 2020 2020 2020 7365 676d 656e 7473 3d5b        segments=[
+0001a540: 7320 666f 7220 692c 2073 2069 6e20 7365  s for i, s in se
+0001a550: 6773 2069 6620 6920 696e 2063 7572 725f  gs if i in curr_
+0001a560: 7365 675f 6964 7873 5d2c 0d0a 2020 2020  seg_idxs],..    
+0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a580: 5f77 6f72 645f 696e 6469 6365 733d 6375  _word_indices=cu
+0001a590: 7272 5f77 6f72 645f 6964 7873 2c0d 0a20  rr_word_idxs,.. 
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 2020 205f 7465 7874 5f6d 6174 6368 3d63     _text_match=c
+0001a5c0: 7572 725f 6d61 7463 682e 6772 6f75 7028  urr_match.group(
+0001a5d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a5e0: 2020 2029 290d 0a20 2020 2020 2020 2020     ))..         
+0001a5f0: 2020 2020 2020 206d 6174 6368 5f73 6567         match_seg
+0001a600: 5f69 6e64 6963 6573 2e61 7070 656e 6428  _indices.append(
+0001a610: 6375 7272 5f73 6567 5f69 6478 7329 0d0a  curr_seg_idxs)..
+0001a620: 2020 2020 2020 2020 7265 7475 726e 2057          return W
+0001a630: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
+0001a640: 6865 7328 6d61 7463 6865 732c 206d 6174  hes(matches, mat
+0001a650: 6368 5f73 6567 5f69 6e64 6963 6573 290d  ch_seg_indices).
+0001a660: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
+0001a670: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+0001a680: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
+0001a690: 6c66 2e6d 6174 6368 6573 290d 0a0d 0a20  lf.matches).... 
+0001a6a0: 2020 2064 6566 205f 5f62 6f6f 6c5f 5f28     def __bool__(
+0001a6b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0001a6c0: 7265 7475 726e 2073 656c 662e 5f5f 6c65  return self.__le
+0001a6d0: 6e5f 5f28 2920 213d 2030 0d0a 0d0a 2020  n__() != 0....  
+0001a6e0: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
+0001a6f0: 5f28 7365 6c66 2c20 6964 7829 3a0d 0a20  _(self, idx):.. 
+0001a700: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001a710: 6c66 2e6d 6174 6368 6573 5b69 6478 5d0d  lf.matches[idx].
+0001a720: 0a                                       .
```

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/__init__.py` & `stable-ts-whisperless-2.17.3/stable_whisper/stabilization/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/nonvad.py` & `stable-ts-whisperless-2.17.3/stable_whisper/stabilization/nonvad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/silero_vad.py` & `stable-ts-whisperless-2.17.3/stable_whisper/stabilization/silero_vad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/utils.py` & `stable-ts-whisperless-2.17.3/stable_whisper/stabilization/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/text_output.py` & `stable-ts-whisperless-2.17.3/stable_whisper/text_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
     is_srt = (filepath is None or not filepath.lower().endswith('.vtt')) if vtt is None else not vtt
     if is_srt:
         segments2blocks = None
         to_word_level_string_callback = None
     else:
         def segments2blocks(segments):
             return 'WEBVTT\n\n' + '\n\n'.join(segment2vttblock(s, strip=strip) for i, s in enumerate(segments))
-        to_word_level_string_callback = to_vtt_word_level_segments if tag is None else tag
+        to_word_level_string_callback = to_vtt_word_level_segments if tag is None else None
 
     return result_to_any(
         result=result,
         filepath=filepath,
         filetype=('vtt', 'srt')[is_srt],
         segments2blocks=segments2blocks,
         segment_level=segment_level,
```

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/timing.py` & `stable-ts-whisperless-2.17.3/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/utils.py` & `stable-ts-whisperless-2.17.3/stable_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/video_output.py` & `stable-ts-whisperless-2.17.3/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/whisper_compatibility.py` & `stable-ts-whisperless-2.17.3/stable_whisper/whisper_compatibility.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/cli.py` & `stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/cli.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/faster_whisper.py` & `stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/hf_whisper.py` & `stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/hf_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/original_whisper.py` & `stable-ts-whisperless-2.17.3/stable_whisper/whisper_word_level/original_whisper.py`

 * *Files identical despite different names*

