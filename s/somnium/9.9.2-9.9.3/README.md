# Comparing `tmp/somnium-9.9.2.tar.gz` & `tmp/somnium-9.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somnium-9.9.2.tar", last modified: Fri Sep  1 11:34:35 2023, max compression
+gzip compressed data, was "somnium-9.9.3.tar", last modified: Sat Jun  1 08:20:23 2024, max compression
```

## Comparing `somnium-9.9.2.tar` & `somnium-9.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-01 11:34:35.308000 somnium-9.9.2/
--rw-rw-rw-   0        0        0       19 2022-07-25 10:16:20.000000 somnium-9.9.2/LICENSE
--rw-rw-rw-   0        0        0     1514 2023-09-01 11:34:35.308000 somnium-9.9.2/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-09-01 10:02:15.000000 somnium-9.9.2/README.md
--rw-rw-rw-   0        0        0      103 2022-07-25 10:16:08.000000 somnium-9.9.2/pyproject.toml
--rw-rw-rw-   0        0        0      720 2023-09-01 11:34:35.316000 somnium-9.9.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-01 11:34:34.957000 somnium-9.9.2/src/
-drwxrwxrwx   0        0        0        0 2023-09-01 11:34:35.075000 somnium-9.9.2/src/somnium/
--rw-rw-rw-   0        0        0       30 2023-04-14 11:43:25.000000 somnium-9.9.2/src/somnium/__init__.py
--rw-rw-rw-   0        0        0     5429 2023-09-01 10:02:23.000000 somnium-9.9.2/src/somnium/__main__.py
-drwxrwxrwx   0        0        0        0 2023-09-01 11:34:35.306000 somnium-9.9.2/src/somnium/sync/
--rw-rw-rw-   0        0        0       30 2023-04-14 11:43:25.000000 somnium-9.9.2/src/somnium/sync/__init__.py
--rw-rw-rw-   0        0        0     6415 2023-09-01 11:33:11.000000 somnium-9.9.2/src/somnium/sync/__main__.py
-drwxrwxrwx   0        0        0        0 2023-09-01 11:34:35.250000 somnium-9.9.2/src/somnium.egg-info/
--rw-rw-rw-   0        0        0     1514 2023-09-01 11:34:34.000000 somnium-9.9.2/src/somnium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-09-01 11:34:34.000000 somnium-9.9.2/src/somnium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-01 11:34:34.000000 somnium-9.9.2/src/somnium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-09-01 11:34:34.000000 somnium-9.9.2/src/somnium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-09-01 11:34:34.000000 somnium-9.9.2/src/somnium.egg-info/top_level.txt
+drwxrwxrwx   0 odium     (1000) odium     (1000)        0 2024-06-01 08:20:23.852831 somnium-9.9.3/
+-rwxrwxrwx   0 odium     (1000) odium     (1000)       19 2022-07-25 10:16:20.000000 somnium-9.9.3/LICENSE
+-rwxrwxrwx   0 odium     (1000) odium     (1000)     1567 2024-06-01 08:20:23.849831 somnium-9.9.3/PKG-INFO
+-rwxrwxrwx   0 odium     (1000) odium     (1000)      935 2023-09-01 10:02:15.000000 somnium-9.9.3/README.md
+-rwxrwxrwx   0 odium     (1000) odium     (1000)      103 2022-07-25 10:16:08.000000 somnium-9.9.3/pyproject.toml
+-rwxrwxrwx   0 odium     (1000) odium     (1000)      743 2024-06-01 08:20:23.855831 somnium-9.9.3/setup.cfg
+drwxrwxrwx   0 odium     (1000) odium     (1000)        0 2024-06-01 08:20:23.636832 somnium-9.9.3/src/
+drwxrwxrwx   0 odium     (1000) odium     (1000)        0 2024-06-01 08:20:23.706831 somnium-9.9.3/src/somnium/
+-rwxrwxrwx   0 odium     (1000) odium     (1000)       30 2023-04-14 11:43:25.000000 somnium-9.9.3/src/somnium/__init__.py
+-rwxrwxrwx   0 odium     (1000) odium     (1000)     5429 2023-09-01 10:02:23.000000 somnium-9.9.3/src/somnium/__main__.py
+drwxrwxrwx   0 odium     (1000) odium     (1000)        0 2024-06-01 08:20:23.828830 somnium-9.9.3/src/somnium/sync/
+-rwxrwxrwx   0 odium     (1000) odium     (1000)       30 2023-04-14 11:43:25.000000 somnium-9.9.3/src/somnium/sync/__init__.py
+-rwxrwxrwx   0 odium     (1000) odium     (1000)     6415 2023-09-01 11:33:11.000000 somnium-9.9.3/src/somnium/sync/__main__.py
+drwxrwxrwx   0 odium     (1000) odium     (1000)        0 2024-06-01 08:20:23.842830 somnium-9.9.3/src/somnium.egg-info/
+-rwxrwxrwx   0 odium     (1000) odium     (1000)     1567 2024-06-01 08:20:23.000000 somnium-9.9.3/src/somnium.egg-info/PKG-INFO
+-rwxrwxrwx   0 odium     (1000) odium     (1000)      322 2024-06-01 08:20:23.000000 somnium-9.9.3/src/somnium.egg-info/SOURCES.txt
+-rwxrwxrwx   0 odium     (1000) odium     (1000)        1 2024-06-01 08:20:23.000000 somnium-9.9.3/src/somnium.egg-info/dependency_links.txt
+-rwxrwxrwx   0 odium     (1000) odium     (1000)       39 2024-06-01 08:20:23.000000 somnium-9.9.3/src/somnium.egg-info/requires.txt
+-rwxrwxrwx   0 odium     (1000) odium     (1000)        8 2024-06-01 08:20:23.000000 somnium-9.9.3/src/somnium.egg-info/top_level.txt
```

### Comparing `somnium-9.9.2/README.md` & `somnium-9.9.3/README.md`

 * *Files identical despite different names*

### Comparing `somnium-9.9.2/setup.cfg` & `somnium-9.9.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2073 6f6d 6e69 756d 0d0a 7665 7273   = somnium..vers
-00000020: 696f 6e20 3d20 392e 392e 320d 0a61 7574  ion = 9.9.2..aut
-00000030: 686f 7220 3d20 6f64 690d 0a61 7574 686f  hor = odi..autho
-00000040: 725f 656d 6169 6c20 3d20 6976 7578 6579  r_email = ivuxey
-00000050: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
-00000060: 7269 7074 696f 6e20 3d20 4372 6561 7465  ription = Create
-00000070: 2062 6561 7574 6966 756c 2061 7274 776f   beautiful artwo
-00000080: 726b 2075 7369 6e67 2074 6865 2070 6f77  rk using the pow
-00000090: 6572 206f 6620 4149 2e0d 0a6b 6579 776f  er of AI...keywo
-000000a0: 7264 7320 3d20 6169 2c20 7374 6162 6c65  rds = ai, stable
-000000b0: 6469 6666 7573 696f 6e2c 2064 7265 616d  diffusion, dream
-000000c0: 2c20 736f 6d6e 6975 6d0d 0a6c 6f6e 675f  , somnium..long_
-000000d0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000e0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000100: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000110: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000120: 6c20 3d20 6874 7470 733a 2f2f 6f64 6975  l = https://odiu
-00000130: 6d2e 7573 0d0a 6c69 6365 6e73 6520 3d20  m.us..license = 
-00000140: 4d49 540d 0a70 726f 6a65 6374 5f75 726c  MIT..project_url
-00000150: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000160: 6572 203d 2068 7474 7073 3a2f 2f74 2e6d  er = https://t.m
-00000170: 652f 6665 656c 6465 640d 0a63 6c61 7373  e/feelded..class
-00000180: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001b0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001d0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-000001e0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001f0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-00000200: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000210: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000220: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000230: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000240: 7569 7265 7320 3d20 3e3d 332e 350d 0a69  uires = >=3.5..i
-00000250: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000260: 3d20 0d0a 0968 746d 6c5f 7465 6c65 6772  = ...html_telegr
-00000270: 6170 685f 706f 7374 6572 0d0a 0d0a 5b6f  aph_poster....[o
-00000280: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000290: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-000002a0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
-000002b0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000002c0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 736f 6d6e 6975 6d0a 7665 7273 696f  = somnium.versio
+00000020: 6e20 3d20 392e 392e 330a 6175 7468 6f72  n = 9.9.3.author
+00000030: 203d 206f 6469 0a61 7574 686f 725f 656d   = odi.author_em
+00000040: 6169 6c20 3d20 6976 7578 6579 4067 6d61  ail = ivuxey@gma
+00000050: 696c 2e63 6f6d 0a64 6573 6372 6970 7469  il.com.descripti
+00000060: 6f6e 203d 2043 7265 6174 6520 6265 6175  on = Create beau
+00000070: 7469 6675 6c20 6172 7477 6f72 6b20 7573  tiful artwork us
+00000080: 696e 6720 7468 6520 706f 7765 7220 6f66  ing the power of
+00000090: 2041 492e 0a6b 6579 776f 7264 7320 3d20   AI..keywords = 
+000000a0: 6169 2c20 7374 6162 6c65 6469 6666 7573  ai, stablediffus
+000000b0: 696f 6e2c 2064 7265 616d 2c20 736f 6d6e  ion, dream, somn
+000000c0: 6975 6d0a 6c6f 6e67 5f64 6573 6372 6970  ium.long_descrip
+000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000e0: 444d 452e 6d64 0a6c 6f6e 675f 6465 7363  DME.md.long_desc
+000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000110: 646f 776e 0a75 726c 203d 2068 7474 7073  down.url = https
+00000120: 3a2f 2f74 2e6d 652f 6578 6563 616c 0a6c  ://t.me/execal.l
+00000130: 6963 656e 7365 203d 204d 4954 0a70 726f  icense = MIT.pro
+00000140: 6a65 6374 5f75 726c 7320 3d20 0a09 536f  ject_urls = ..So
+00000150: 7572 6365 203d 2068 7474 7073 3a2f 2f67  urce = https://g
+00000160: 6974 6875 622e 636f 6d2f 7661 7574 680a  ithub.com/vauth.
+00000170: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000180: 7474 7073 3a2f 2f74 2e6d 652f 6665 656c  ttps://t.me/feel
+00000190: 6465 640a 636c 6173 7369 6669 6572 7320  ded.classifiers 
+000001a0: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
+000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001c0: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
+000001d0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001e0: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+000001f0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000200: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000210: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
+00000220: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+00000230: 2073 7263 0a70 6163 6b61 6765 7320 3d20   src.packages = 
+00000240: 6669 6e64 3a0a 7079 7468 6f6e 5f72 6571  find:.python_req
+00000250: 7569 7265 7320 3d20 3e3d 332e 350a 696e  uires = >=3.5.in
+00000260: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000270: 200a 096c 786d 6c5b 6874 6d6c 5f63 6c65   ..lxml[html_cle
+00000280: 616e 5d0a 0968 746d 6c5f 7465 6c65 6772  an]..html_telegr
+00000290: 6170 685f 706f 7374 6572 0a0a 5b6f 7074  aph_poster..[opt
+000002a0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000002b0: 6e64 5d0a 7768 6572 6520 3d20 7372 630a  nd].where = src.
+000002c0: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
+000002d0: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
+000002e0: 6520 3d20 300a 0a                        e = 0..
```

### Comparing `somnium-9.9.2/src/somnium/__main__.py` & `somnium-9.9.3/src/somnium/__main__.py`

 * *Files identical despite different names*

### Comparing `somnium-9.9.2/src/somnium/sync/__main__.py` & `somnium-9.9.3/src/somnium/sync/__main__.py`

 * *Files identical despite different names*

