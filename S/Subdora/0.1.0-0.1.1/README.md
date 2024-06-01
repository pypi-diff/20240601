# Comparing `tmp/subdora-0.1.0.tar.gz` & `tmp/subdora-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\Subdora\Subdora_v0.1.0\Package\Subdora\dist\.tmp-sd9arspo\subdora-0.1.0.tar", last modified: Sun May  5 09:50:48 2024, max compression
+gzip compressed data, was "C:\Users\laksh\OneDrive\Desktop\Subdora_v0.1.1\Package\Subdora\dist\.tmp-52wgadn7\subdora-0.1.1.tar", last modified: Sat Jun  1 12:05:31 2024, max compression
```

## Comparing `subdora-0.1.0.tar` & `subdora-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.873428 subdora-0.1.0/
--rw-rw-rw-   0        0        0      120 2024-05-01 09:50:01.000000 subdora-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2252 2024-05-05 09:50:48.853425 subdora-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1633 2024-05-05 09:38:09.000000 subdora-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:44.155395 subdora-0.1.0/Subdora/
--rw-rw-rw-   0        0        0       57 2024-05-03 12:30:53.000000 subdora-0.1.0/Subdora/__init__.py
--rw-rw-rw-   0        0        0     2583 2024-05-05 09:39:50.000000 subdora-0.1.0/Subdora/_subdora.py
--rw-rw-rw-   0        0        0     1808 2024-05-04 17:45:55.000000 subdora-0.1.0/Subdora/_subdora_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:43.988849 subdora-0.1.0/Subdora/corex64/
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:44.375887 subdora-0.1.0/Subdora/corex64/linux/
--rw-rw-rw-   0        0        0   132128 2024-05-03 12:14:40.000000 subdora-0.1.0/Subdora/corex64/linux/Subdora.so
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.797827 subdora-0.1.0/Subdora/corex64/win/
--rw-rw-rw-   0        0        0    65024 2024-05-05 08:20:34.000000 subdora-0.1.0/Subdora/corex64/win/Subdora.dll
--rw-rw-rw-   0        0        0   322672 2024-02-02 20:31:00.000000 subdora-0.1.0/Subdora/corex64/win/concrt140.dll
--rw-rw-rw-   0        0        0   346624 2024-01-07 18:32:18.000000 subdora-0.1.0/Subdora/corex64/win/libsodium.dll
--rw-rw-rw-   0        0        0   573008 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140.dll
--rw-rw-rw-   0        0        0    35920 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_1.dll
--rw-rw-rw-   0        0        0   268392 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_2.dll
--rw-rw-rw-   0        0        0    50280 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_atomic_wait.dll
--rw-rw-rw-   0        0        0    31856 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_codecvt_ids.dll
--rw-rw-rw-   0        0        0   412752 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcamp140.dll
--rw-rw-rw-   0        0        0   348784 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vccorlib140.dll
--rw-rw-rw-   0        0        0   196688 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcomp140.dll
--rw-rw-rw-   0        0        0   119376 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140.dll
--rw-rw-rw-   0        0        0    49744 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140_1.dll
--rw-rw-rw-   0        0        0    38512 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140_threads.dll
-drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.827339 subdora-0.1.0/Subdora.egg-info/
--rw-rw-rw-   0        0        0     2252 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2024-05-01 09:50:14.000000 subdora-0.1.0/project.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 09:50:48.873428 subdora-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1241 2024-05-05 09:38:54.000000 subdora-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.347924 subdora-0.1.1/
+-rw-rw-rw-   0        0        0      755 2024-05-27 05:25:18.000000 subdora-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3479 2024-06-01 12:05:31.346926 subdora-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2789 2024-06-01 12:04:47.000000 subdora-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.306193 subdora-0.1.1/Subdora/
+-rw-rw-rw-   0        0        0      104 2024-06-01 11:19:06.000000 subdora-0.1.1/Subdora/__init__.py
+-rw-rw-rw-   0        0        0     6198 2024-05-27 10:38:33.000000 subdora-0.1.1/Subdora/_subdora.py
+-rw-rw-rw-   0        0        0     1947 2024-06-01 11:38:52.000000 subdora-0.1.1/Subdora/_subdora_cli.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.296605 subdora-0.1.1/Subdora/corex64/
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.319260 subdora-0.1.1/Subdora/corex64/linux/
+-rw-rw-rw-   0        0        0   343968 2024-05-27 04:21:37.000000 subdora-0.1.1/Subdora/corex64/linux/Subdora.so
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.343682 subdora-0.1.1/Subdora/corex64/win/
+-rw-rw-rw-   0        0        0   168960 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/Subdora.dll
+-rw-rw-rw-   0        0        0   322672 2024-06-01 11:17:08.000000 subdora-0.1.1/Subdora/corex64/win/concrt140.dll
+-rw-rw-rw-   0        0        0   346624 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/libsodium.dll
+-rw-rw-rw-   0        0        0   573008 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/msvcp140.dll
+-rw-rw-rw-   0        0        0    35920 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/msvcp140_1.dll
+-rw-rw-rw-   0        0        0   268392 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/msvcp140_2.dll
+-rw-rw-rw-   0        0        0    50280 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/msvcp140_atomic_wait.dll
+-rw-rw-rw-   0        0        0    31856 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/msvcp140_codecvt_ids.dll
+-rw-rw-rw-   0        0        0   412752 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vcamp140.dll
+-rw-rw-rw-   0        0        0   348784 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vccorlib140.dll
+-rw-rw-rw-   0        0        0   196688 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vcomp140.dll
+-rw-rw-rw-   0        0        0   119376 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vcruntime140.dll
+-rw-rw-rw-   0        0        0    49744 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vcruntime140_1.dll
+-rw-rw-rw-   0        0        0    38512 2024-06-01 11:17:09.000000 subdora-0.1.1/Subdora/corex64/win/vcruntime140_threads.dll
+drwxrwxrwx   0        0        0        0 2024-06-01 12:05:31.345924 subdora-0.1.1/Subdora.egg-info/
+-rw-rw-rw-   0        0        0     3479 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 12:05:31.000000 subdora-0.1.1/Subdora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2024-05-23 10:31:56.000000 subdora-0.1.1/project.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:05:31.347924 subdora-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2024-05-27 05:07:06.000000 subdora-0.1.1/setup.py
```

### Comparing `subdora-0.1.0/PKG-INFO` & `subdora-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2053 7562  : 2.1..Name: Sub
 00000020: 646f 7261 0d0a 5665 7273 696f 6e3a 2030  dora..Version: 0
-00000030: 2e31 2e30 0d0a 5375 6d6d 6172 793a 2053  .1.0..Summary: S
+00000030: 2e31 2e31 0d0a 5375 6d6d 6172 793a 2053  .1.1..Summary: S
 00000040: 7562 646f 7261 203a 2041 2070 7974 686f  ubdora : A pytho
 00000050: 6e20 7061 636b 6167 6520 7468 6174 2074  n package that t
 00000060: 616b 6573 2063 6172 6520 6f66 206f 6266  akes care of obf
 00000070: 7573 6361 7469 6f6e 206f 6620 7079 7468  uscation of pyth
 00000080: 6f6e 2073 6372 6970 7473 0d0a 486f 6d65  on scripts..Home
 00000090: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 000000a0: 6974 6875 622e 636f 6d2f 4c61 6b73 6869  ithub.com/Lakshi
@@ -28,114 +28,191 @@
 000001b0: 696e 6720 5379 7374 656d 203a 3a20 556e  ing System :: Un
 000001c0: 6978 0d0a 436c 6173 7369 6669 6572 3a20  ix..Classifier: 
 000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 000001e0: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
 000001f0: 2057 696e 646f 7773 0d0a 4465 7363 7269   Windows..Descri
 00000200: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
 00000210: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000220: 6e0d 0a0d 0a0d 0a21 5b73 7562 646f 7261  n......![subdora
-00000230: 206c 6f67 6f5d 2868 7474 7073 3a2f 2f72   logo](https://r
-00000240: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000250: 7465 6e74 2e63 6f6d 2f4c 616b 7368 6974  tent.com/Lakshit
-00000260: 2d4b 6172 736f 6c69 7961 2f53 7562 646f  -Karsoliya/Subdo
-00000270: 7261 2f6d 6169 6e2f 6173 7365 7473 2f73  ra/main/assets/s
-00000280: 7562 646f 7261 2e70 6e67 2022 7375 6264  ubdora.png "subd
-00000290: 6f72 6120 6c6f 676f 2229 0d0d 0a0d 0d0a  ora logo")......
-000002a0: 3c68 313e 5375 6264 6f72 6120 302e 312e  <h1>Subdora 0.1.
-000002b0: 303c 2f68 313e 0d0d 0a3c 7020 7374 796c  0</h1>...<p styl
-000002c0: 653d 2263 6f6c 6f72 3a72 6564 3b66 6f6e  e="color:red;fon
-000002d0: 742d 7369 7a65 3a31 3270 783b 223e 2a2a  t-size:12px;">**
-000002e0: 2a54 6869 7320 7665 7273 696f 6e20 6f66  *This version of
-000002f0: 2073 7562 646f 7261 2069 7320 6e6f 7420   subdora is not 
-00000300: 6261 636b 7761 7264 2063 6f6d 7061 7469  backward compati
-00000310: 6162 6c65 2c20 6974 2069 7320 7265 636f  able, it is reco
-00000320: 6d6d 656e 6465 6420 746f 2075 7365 2074  mmended to use t
-00000330: 6865 206c 6174 6573 7420 7665 7269 736f  he latest veriso
-00000340: 6e20 6f66 2073 7562 646f 7261 203c 2f70  n of subdora </p
-00000350: 3e0d 0d0a 0d0d 0a3c 703e 5468 6973 2069  >......<p>This i
-00000360: 7320 7468 6520 5468 6972 6420 7265 6c65  s the Third rele
-00000370: 6173 6520 6f66 2073 7562 646f 7261 2e20  ase of subdora. 
-00000380: 5375 6264 6f72 6120 6973 2061 6e20 6f62  Subdora is an ob
-00000390: 6675 7363 6174 696f 6e20 746f 6f6c 2077  fuscation tool w
-000003a0: 6869 6368 206d 616b 6573 2073 6f75 7263  hich makes sourc
-000003b0: 6520 636f 6465 2076 6572 7920 6861 7264  e code very hard
-000003c0: 2074 6f20 696e 7465 7270 7261 7465 3c2f   to interprate</
-000003d0: 703e 0d0d 0a0d 0d0a 3c68 323e 496e 7374  p>......<h2>Inst
-000003e0: 616c 6c61 7469 6f6e 3c2f 6832 3e0d 0d0a  allation</h2>...
-000003f0: 0d0d 0a60 6060 0d0d 0a70 6970 2069 6e73  ...```...pip ins
-00000400: 7461 6c6c 2053 7562 646f 7261 0d0d 0a60  tall Subdora...`
-00000410: 6060 0d0d 0a0d 0d0a 3c68 323e 5375 7070  ``......<h2>Supp
-00000420: 6f72 7465 6420 4f53 3c2f 6832 3e0d 0d0a  orted OS</h2>...
-00000430: 0d0d 0a7c 2056 6572 7369 6f6e 207c 2041  ...| Version | A
-00000440: 726d 2020 207c 204c 696e 7578 2836 3429  rm   | Linux(64)
-00000450: 207c 2057 696e 646f 7773 2836 3429 207c   | Windows(64) |
-00000460: 0d0d 0a7c 3a2d 2d2d 2d2d 2d2d 3a7c 3a2d  ...|:-------:|:-
-00000470: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00000480: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  :|:-----------:|
-00000490: 0d0d 0a7c 2030 2e31 2e30 2020 207c 20e2  ...| 0.1.0   | .
-000004a0: 9d8c 2020 2020 7c20 e29c 94ef b88f 2020  ..    | ......  
-000004b0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-000004c0: 2020 2020 2020 207c 0d0d 0a7c 2030 2e30         |...| 0.0
-000004d0: 2e32 2020 207c 20e2 9d8c 2020 2020 7c20  .2   | ...    | 
-000004e0: e29c 94ef b88f 2020 2020 2020 2020 207c  ......         |
-000004f0: 20e2 9c94 efb8 8f20 2020 2020 2020 207c   ......        |
-00000500: 0d0d 0a7c 2030 2e30 2e31 2020 207c 20e2  ...| 0.0.1   | .
-00000510: 9d8c 2020 2020 7c20 e29c 94ef b88f 2020  ..    | ......  
-00000520: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00000530: 2020 2020 2020 207c 0d0d 0a0d 0d0a 0d0d         |........
-00000540: 0a3c 6832 3e57 6861 7427 7320 6e65 7720  .<h2>What's new 
-00000550: 696e 2076 302e 312e 303c 2f68 323e 0d0d  in v0.1.0</h2>..
-00000560: 0a0d 0d0a 2a20 4164 6420 7375 7070 6f72  ....* Add suppor
-00000570: 7420 666f 7220 636c 6920 746f 6f6c 200d  t for cli tool .
-00000580: 0d0a 2a20 4164 6420 6578 7069 7279 2074  ..* Add expiry t
-00000590: 696d 6520 6665 6174 7572 650d 0d0a 0d0d  ime feature.....
-000005a0: 0a0d 0d0a 3c68 323e 486f 7720 746f 2075  ....<h2>How to u
-000005b0: 7365 3c2f 6832 3e0d 0d0a 3c68 333e 436f  se</h2>...<h3>Co
-000005c0: 7265 2066 756e 6374 696f 6e61 6c69 7479  re functionality
-000005d0: 3c2f 6833 3e0d 0d0a 0d0d 0a3c 703e 3c62  </h3>......<p><b
-000005e0: 3e6f 6266 7573 6361 7469 6e67 206d 6169  >obfuscating mai
-000005f0: 6e2e 7079 2066 696c 653c 2f62 3e20 3c2f  n.py file</b> </
-00000600: 703e 0d0d 0a0d 0d0a 3c70 3e46 726f 6d20  p>......<p>From 
-00000610: 636f 6d6d 616e 6420 6c69 6e65 3c2f 703e  command line</p>
-00000620: 0d0d 0a0d 0d0a 3c63 6f64 653e 433a 5c3e  ......<code>C:\>
-00000630: 7375 6264 6f72 6120 2d2d 6f62 6675 7363  subdora --obfusc
-00000640: 6174 6520 6d61 696e 2e70 7920 2d2d 6974  ate main.py --it
-00000650: 7220 3130 202d 2d74 696d 6520 3130 6d3c  r 10 --time 10m<
-00000660: 2f63 6f64 653e 0d0d 0a0d 0d0a 3c70 3e46  /code>......<p>F
-00000670: 726f 6d20 7079 7468 6f6e 2066 696c 6520  rom python file 
-00000680: 3c2f 703e 0d0d 0a0d 0d0a 6060 6070 790d  </p>......```py.
-00000690: 0d0a 5375 6264 6f72 612e 7375 6264 6f72  ..Subdora.subdor
-000006a0: 615f 656e 636f 6465 5f66 696c 6528 226d  a_encode_file("m
-000006b0: 6169 6e2e 7079 222c 6e6f 5f6f 665f 6974  ain.py",no_of_it
-000006c0: 6572 6174 696f 6e73 2c65 7870 6972 795f  erations,expiry_
-000006d0: 7469 6d65 2923 2734 6d20 3468 2065 7463  time)#'4m 4h etc
-000006e0: 270d 0d0a 6060 600d 0d0a 0d0d 0a3c 703e  '...```......<p>
-000006f0: 3c62 3e54 6869 7320 7769 6c6c 2067 656e  <b>This will gen
-00000700: 6572 6174 6520 6120 6d61 696e 2e6d 7973  erate a main.mys
-00000710: 7420 6669 6c65 2069 6e20 6f72 6465 7220  t file in order 
-00000720: 746f 2065 7865 6375 7465 206d 7973 7420  to execute myst 
-00000730: 6669 6c65 3c2f 623e 3c2f 703e 0d0d 0a0d  file</b></p>....
-00000740: 0d0a 3c70 3e46 726f 6d20 636f 6d6d 616e  ..<p>From comman
-00000750: 6420 6c69 6e65 3c2f 703e 0d0d 0a0d 0d0a  d line</p>......
-00000760: 3c63 6f64 653e 433a 5c3e 7375 6264 6f72  <code>C:\>subdor
-00000770: 6120 2d2d 7275 6e20 6d61 696e 2e6d 7973  a --run main.mys
-00000780: 743c 2f63 6f64 653e 0d0d 0a0d 0d0a 3c70  t</code>......<p
-00000790: 3e46 726f 6d20 7079 7468 6f6e 2066 696c  >From python fil
-000007a0: 653c 2f70 3e0d 0d0a 0d0d 0a60 6060 7079  e</p>......```py
-000007b0: 0d0d 0a53 7562 646f 7261 2e73 7562 646f  ...Subdora.subdo
-000007c0: 7261 5f70 6172 7365 2822 6d61 696e 2e6d  ra_parse("main.m
-000007d0: 7973 7422 290d 0d0a 6060 600d 0d0a 0d0d  yst")...```.....
-000007e0: 0a3c 6833 3e0d 0d0a 0d0d 0a0d 0d0a 3c68  .<h3>.........<h
-000007f0: 333e 4665 6174 7572 6573 3c2f 6833 3e0d  3>Features</h3>.
-00000800: 0d0a 0d0d 0a2a 204f 6266 7573 6361 7469  .....* Obfuscati
-00000810: 6f6e 206f 6620 7079 7468 6f6e 2063 6f64  on of python cod
-00000820: 650d 0d0a 2a20 5375 7070 6f72 7420 436f  e...* Support Co
-00000830: 6465 2065 7870 6972 7920 4665 6174 7572  de expiry Featur
-00000840: 650d 0d0a 2a20 5375 7070 6f72 7420 6974  e...* Support it
-00000850: 6572 6174 696f 6e20 636f 756e 7465 720d  eration counter.
-00000860: 0d0a 2a20 5375 7070 6f72 7420 666f 7220  ..* Support for 
-00000870: 636c 6920 746f 6f6c 0d0d 0a2a 2053 7570  cli tool...* Sup
-00000880: 706f 7274 7320 6c6f 6164 696e 6720 6f62  ports loading ob
-00000890: 6675 7363 6174 6564 2063 6f64 6520 6173  fuscated code as
-000008a0: 206d 6f64 756c 6520 696e 2061 6e6f 7468   module in anoth
-000008b0: 6572 2070 7974 686f 6e20 7072 6f6a 6563  er python projec
-000008c0: 7473 0d0d 0a0d 0d0a 2020 0d0a            ts......  ..
+00000220: 6e0d 0a52 6571 7569 7265 732d 4469 7374  n..Requires-Dist
+00000230: 3a20 7069 6c6c 6f77 0d0a 0d0a 0d0a 215b  : pillow......![
+00000240: 7375 6264 6f72 6120 6c6f 676f 5d28 6874  subdora logo](ht
+00000250: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000260: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000270: 4c61 6b73 6869 742d 4b61 7273 6f6c 6979  Lakshit-Karsoliy
+00000280: 612f 5375 6264 6f72 612f 6d61 696e 2f61  a/Subdora/main/a
+00000290: 7373 6574 732f 7375 6264 6f72 612e 706e  ssets/subdora.pn
+000002a0: 6720 2273 7562 646f 7261 206c 6f67 6f22  g "subdora logo"
+000002b0: 290d 0d0a 0d0d 0a3c 6831 3e53 7562 646f  )......<h1>Subdo
+000002c0: 7261 2030 2e31 2e31 3c2f 6831 3e0d 0d0a  ra 0.1.1</h1>...
+000002d0: 3c70 2073 7479 6c65 3d22 636f 6c6f 723a  <p style="color:
+000002e0: 7265 643b 666f 6e74 2d73 697a 653a 3132  red;font-size:12
+000002f0: 7078 3b22 3e2a 2a2a 5468 6973 2076 6572  px;">***This ver
+00000300: 7369 6f6e 206f 6620 7375 6264 6f72 6120  sion of subdora 
+00000310: 6973 206e 6f74 2062 6163 6b77 6172 6420  is not backward 
+00000320: 636f 6d70 6174 6961 626c 652c 2069 7420  compatiable, it 
+00000330: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+00000340: 6f20 7573 6520 7468 6520 6c61 7465 7374  o use the latest
+00000350: 2076 6572 6973 6f6e 206f 6620 7375 6264   verison of subd
+00000360: 6f72 6120 3c2f 703e 0d0d 0a0d 0d0a 3c70  ora </p>......<p
+00000370: 3e54 6869 7320 6973 2074 6865 2054 6869  >This is the Thi
+00000380: 7264 2072 656c 6561 7365 206f 6620 7375  rd release of su
+00000390: 6264 6f72 612e 2053 7562 646f 7261 2069  bdora. Subdora i
+000003a0: 7320 616e 206f 6266 7573 6361 7469 6f6e  s an obfuscation
+000003b0: 2074 6f6f 6c20 7768 6963 6820 6d61 6b65   tool which make
+000003c0: 7320 736f 7572 6365 2063 6f64 6520 7665  s source code ve
+000003d0: 7279 2068 6172 6420 746f 2069 6e74 6572  ry hard to inter
+000003e0: 7072 6174 653c 2f70 3e0d 0d0a 0d0d 0a3c  prate</p>......<
+000003f0: 6832 3e49 6e73 7461 6c6c 6174 696f 6e3c  h2>Installation<
+00000400: 2f68 323e 0d0d 0a0d 0d0a 6060 600d 0d0a  /h2>......```...
+00000410: 7069 7020 696e 7374 616c 6c20 5375 6264  pip install Subd
+00000420: 6f72 610d 0d0a 6060 600d 0d0a 0d0d 0a3c  ora...```......<
+00000430: 6832 3e53 7570 706f 7274 6564 204f 533c  h2>Supported OS<
+00000440: 2f68 323e 0d0d 0a0d 0d0a 3c21 2d2d 207c  /h2>......<!-- |
+00000450: 2056 6572 7369 6f6e 207c 2041 726d 2020   Version | Arm  
+00000460: 207c 204c 696e 7578 2836 3429 207c 2057   | Linux(64) | W
+00000470: 696e 646f 7773 2836 3429 207c 0d0d 0a7c  indows(64) |...|
+00000480: 3a2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  :-------:|:-----
+00000490: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  :|:---------:|:-
+000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 0d0d 0a7c  ----------:|...|
+000004b0: 2030 2e31 2e31 2020 207c 20e2 9d8c 2020   0.1.1   | ...  
+000004c0: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+000004d0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+000004e0: 2020 207c 0d0d 0a7c 2030 2e31 2e30 2020     |...| 0.1.0  
+000004f0: 207c 20e2 9d8c 2020 2020 7c20 e29c 94ef   | ...    | ....
+00000500: b88f 2020 2020 2020 2020 207c 20e2 9c94  ..         | ...
+00000510: efb8 8f20 2020 2020 2020 207c 0d0d 0a7c  ...        |...|
+00000520: 2030 2e30 2e32 2020 207c 20e2 9d8c 2020   0.0.2   | ...  
+00000530: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00000540: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00000550: 2020 207c 0d0d 0a7c 2030 2e30 2e31 2020     |...| 0.0.1  
+00000560: 207c 20e2 9d8c 2020 2020 7c20 e29c 94ef   | ...    | ....
+00000570: b88f 2020 2020 2020 2020 207c 20e2 9c94  ..         | ...
+00000580: efb8 8f20 2020 2020 2020 207c 202d 2d3e  ...        | -->
+00000590: 0d0d 0a0d 0d0a 3c74 6162 6c65 3e0d 0d0a  ......<table>...
+000005a0: 2020 3c74 6865 6164 3e0d 0d0a 2020 2020    <thead>...    
+000005b0: 3c74 723e 0d0d 0a20 2020 2020 203c 7468  <tr>...      <th
+000005c0: 3e56 6572 7369 6f6e 3c2f 7468 3e0d 0d0a  >Version</th>...
+000005d0: 2020 2020 2020 3c74 683e 4172 6d3c 2f74        <th>Arm</t
+000005e0: 683e 0d0d 0a20 2020 2020 203c 7468 3e4c  h>...      <th>L
+000005f0: 696e 7578 2836 3429 3c2f 7468 3e0d 0d0a  inux(64)</th>...
+00000600: 2020 2020 2020 3c74 683e 5769 6e64 6f77        <th>Window
+00000610: 7328 3634 293c 2f74 683e 0d0d 0a20 2020  s(64)</th>...   
+00000620: 203c 2f74 723e 0d0d 0a20 203c 2f74 6865   </tr>...  </the
+00000630: 6164 3e0d 0d0a 2020 3c74 626f 6479 3e0d  ad>...  <tbody>.
+00000640: 0d0a 2020 2020 3c74 723e 0d0d 0a20 2020  ..    <tr>...   
+00000650: 2020 203c 7464 3e30 2e31 2e31 3c2f 7464     <td>0.1.1</td
+00000660: 3e0d 0d0a 2020 2020 2020 3c74 643e 2623  >...      <td>&#
+00000670: 3130 3036 303b 3c2f 7464 3e0d 0d0a 2020  10060;</td>...  
+00000680: 2020 2020 3c74 643e 2623 3130 3030 343b      <td>&#10004;
+00000690: 3c2f 7464 3e0d 0d0a 2020 2020 2020 3c74  </td>...      <t
+000006a0: 643e 2623 3130 3030 343b 3c2f 7464 3e0d  d>&#10004;</td>.
+000006b0: 0d0a 2020 2020 3c2f 7472 3e0d 0d0a 2020  ..    </tr>...  
+000006c0: 2020 3c74 723e 0d0d 0a20 2020 2020 203c    <tr>...      <
+000006d0: 7464 3e30 2e31 2e30 3c2f 7464 3e0d 0d0a  td>0.1.0</td>...
+000006e0: 2020 2020 2020 3c74 643e 2623 3130 3036        <td>&#1006
+000006f0: 303b 3c2f 7464 3e0d 0d0a 2020 2020 2020  0;</td>...      
+00000700: 3c74 643e 2623 3130 3030 343b 3c2f 7464  <td>&#10004;</td
+00000710: 3e0d 0d0a 2020 2020 2020 3c74 643e 2623  >...      <td>&#
+00000720: 3130 3030 343b 3c2f 7464 3e0d 0d0a 2020  10004;</td>...  
+00000730: 2020 3c2f 7472 3e0d 0d0a 2020 2020 3c74    </tr>...    <t
+00000740: 723e 0d0d 0a20 2020 2020 203c 7464 3e30  r>...      <td>0
+00000750: 2e30 2e32 3c2f 7464 3e0d 0d0a 2020 2020  .0.2</td>...    
+00000760: 2020 3c74 643e 2623 3130 3036 303b 3c2f    <td>&#10060;</
+00000770: 7464 3e0d 0d0a 2020 2020 2020 3c74 643e  td>...      <td>
+00000780: 2623 3130 3030 343b 3c2f 7464 3e0d 0d0a  &#10004;</td>...
+00000790: 2020 2020 2020 3c74 643e 2623 3130 3030        <td>&#1000
+000007a0: 343b 3c2f 7464 3e0d 0d0a 2020 2020 3c2f  4;</td>...    </
+000007b0: 7472 3e0d 0d0a 2020 2020 3c74 723e 0d0d  tr>...    <tr>..
+000007c0: 0a20 2020 2020 203c 7464 3e30 2e30 2e31  .      <td>0.0.1
+000007d0: 3c2f 7464 3e0d 0d0a 2020 2020 2020 3c74  </td>...      <t
+000007e0: 643e 2623 3130 3036 303b 3c2f 7464 3e0d  d>&#10060;</td>.
+000007f0: 0d0a 2020 2020 2020 3c74 643e 2623 3130  ..      <td>&#10
+00000800: 3030 343b 3c2f 7464 3e0d 0d0a 2020 2020  004;</td>...    
+00000810: 2020 3c74 643e 2623 3130 3030 343b 3c2f    <td>&#10004;</
+00000820: 7464 3e0d 0d0a 2020 2020 3c2f 7472 3e0d  td>...    </tr>.
+00000830: 0d0a 2020 3c2f 7462 6f64 793e 0d0d 0a3c  ..  </tbody>...<
+00000840: 2f74 6162 6c65 3e0d 0d0a 0d0d 0a0d 0d0a  /table>.........
+00000850: 0d0d 0a3c 6832 3e57 6861 7427 7320 6e65  ...<h2>What's ne
+00000860: 7720 696e 2076 302e 312e 313c 2f68 323e  w in v0.1.1</h2>
+00000870: 0d0d 0a0d 0d0a 2a20 6162 6c65 2074 6f20  ......* able to 
+00000880: 6f62 6675 7363 6174 6520 7079 7468 6f6e  obfuscate python
+00000890: 2073 6372 6970 7420 696e 746f 2069 6d61   script into ima
+000008a0: 6765 7320 7768 696c 6520 7265 7461 6e69  ges while retani
+000008b0: 6e67 2069 6e65 7261 7469 6f6e 2063 6f75  ng ineration cou
+000008c0: 6e74 6572 2061 6e64 2065 7870 6972 7920  nter and expiry 
+000008d0: 7469 6d65 200d 0d0a 2a20 4164 6420 7375  time ...* Add su
+000008e0: 7070 6f72 7420 666f 7220 636c 6920 746f  pport for cli to
+000008f0: 6f6c 200d 0d0a 2a20 4164 6420 6578 7069  ol ...* Add expi
+00000900: 7279 2074 696d 6520 6665 6174 7572 650d  ry time feature.
+00000910: 0d0a 0d0d 0a3c 6832 3e48 6f77 2074 6f20  .....<h2>How to 
+00000920: 7573 653c 2f68 323e 0d0d 0a3c 6833 3e43  use</h2>...<h3>C
+00000930: 6f72 6520 6675 6e63 7469 6f6e 616c 6974  ore functionalit
+00000940: 793c 2f68 333e 0d0d 0a0d 0d0a 3c70 3e3c  y</h3>......<p><
+00000950: 623e 6f62 6675 7363 6174 696e 6720 6d61  b>obfuscating ma
+00000960: 696e 2e70 7920 6669 6c65 3c2f 623e 203c  in.py file</b> <
+00000970: 2f70 3e0d 0d0a 0d0d 0a3c 703e 4672 6f6d  /p>......<p>From
+00000980: 2063 6f6d 6d61 6e64 206c 696e 653c 2f70   command line</p
+00000990: 3e0d 0d0a 0d0d 0a3c 636f 6465 3e43 3a5c  >......<code>C:\
+000009a0: 3e73 7562 646f 7261 202d 2d6f 6266 7573  >subdora --obfus
+000009b0: 6361 7465 206d 6169 6e2e 7079 202d 2d69  cate main.py --i
+000009c0: 7472 2031 3020 2d2d 7469 6d65 2031 306d  tr 10 --time 10m
+000009d0: 3c2f 636f 6465 3e0d 0d0a 0d0d 0a3c 703e  </code>......<p>
+000009e0: 4672 6f6d 2070 7974 686f 6e20 6669 6c65  From python file
+000009f0: 203c 2f70 3e0d 0d0a 0d0d 0a60 6060 7079   </p>......```py
+00000a00: 0d0d 0a53 7562 646f 7261 2e73 7562 646f  ...Subdora.subdo
+00000a10: 7261 5f65 6e63 6f64 655f 6669 6c65 2822  ra_encode_file("
+00000a20: 6d61 696e 2e70 7922 2c6e 6f5f 6f66 5f69  main.py",no_of_i
+00000a30: 7465 7261 7469 6f6e 732c 6578 7069 7279  terations,expiry
+00000a40: 5f74 696d 6529 2327 346d 2034 6820 6574  _time)#'4m 4h et
+00000a50: 6327 0d0d 0a60 6060 0d0d 0a0d 0d0a 3c70  c'...```......<p
+00000a60: 3e3c 623e 5468 6973 2077 696c 6c20 6765  ><b>This will ge
+00000a70: 6e65 7261 7465 2061 206d 6169 6e2e 6d79  nerate a main.my
+00000a80: 7374 2066 696c 6520 696e 206f 7264 6572  st file in order
+00000a90: 2074 6f20 6578 6563 7574 6520 6d79 7374   to execute myst
+00000aa0: 2066 696c 653c 2f62 3e3c 2f70 3e0d 0d0a   file</b></p>...
+00000ab0: 0d0d 0a3c 703e 4672 6f6d 2063 6f6d 6d61  ...<p>From comma
+00000ac0: 6e64 206c 696e 653c 2f70 3e0d 0d0a 0d0d  nd line</p>.....
+00000ad0: 0a3c 636f 6465 3e43 3a5c 3e73 7562 646f  .<code>C:\>subdo
+00000ae0: 7261 202d 2d72 756e 206d 6169 6e2e 6d79  ra --run main.my
+00000af0: 7374 3c2f 636f 6465 3e0d 0d0a 0d0d 0a3c  st</code>......<
+00000b00: 703e 4672 6f6d 2070 7974 686f 6e20 6669  p>From python fi
+00000b10: 6c65 3c2f 703e 0d0d 0a0d 0d0a 6060 6070  le</p>......```p
+00000b20: 790d 0d0a 5375 6264 6f72 612e 7375 6264  y...Subdora.subd
+00000b30: 6f72 615f 7061 7273 6528 226d 6169 6e2e  ora_parse("main.
+00000b40: 6d79 7374 2229 0d0d 0a60 6060 0d0d 0a0d  myst")...```....
+00000b50: 0d0a 3c70 3e3c 623e 456e 636f 6469 6e67  ..<p><b>Encoding
+00000b60: 2070 7974 686f 6e20 7363 7269 7074 2074   python script t
+00000b70: 6f20 696d 6167 653c 2f62 3e3c 2f70 3e0d  o image</b></p>.
+00000b80: 0d0a 3c70 3e2a 6f6e 6c79 2073 7570 706f  ..<p>*only suppo
+00000b90: 7274 7320 706e 6720 616e 6420 6a70 6720  rts png and jpg 
+00000ba0: 6669 6c65 733c 2f70 3e0d 0d0a 3c63 6f64  files</p>...<cod
+00000bb0: 653e 433a 3e73 7562 646f 7261 202d 2d6f  e>C:>subdora --o
+00000bc0: 6266 7573 6361 7465 206d 6169 6e2e 7079  bfuscate main.py
+00000bd0: 202d 2d69 6d67 2069 6d67 2e6a 7067 202d   --img img.jpg -
+00000be0: 2d69 7465 7261 7469 6f6e 7320 3520 2d2d  -iterations 5 --
+00000bf0: 7469 6d65 2035 6d3c 2f63 6f64 653e 0d0d  time 5m</code>..
+00000c00: 0a0d 0d0a 3c62 723e 3c70 3e54 6869 7320  ....<br><p>This 
+00000c10: 7769 6c6c 2067 656e 6572 6174 6520 6d61  will generate ma
+00000c20: 696e 2e70 6e67 2066 696c 6520 746f 2072  in.png file to r
+00000c30: 756e 2074 6865 2069 6d61 6765 2066 696c  un the image fil
+00000c40: 6520 7573 653c 2f70 3e0d 0d0a 0d0d 0a3c  e use</p>......<
+00000c50: 636f 6465 3e43 3a3e 2073 7562 646f 7261  code>C:> subdora
+00000c60: 202d 2d72 756e 206d 6169 6e2e 696d 673c   --run main.img<
+00000c70: 2f63 6f64 653e 0d0d 0a0d 0d0a 3c68 333e  /code>......<h3>
+00000c80: 0d0d 0a0d 0d0a 0d0d 0a3c 6833 3e46 6561  .........<h3>Fea
+00000c90: 7475 7265 733c 2f68 333e 0d0d 0a0d 0d0a  tures</h3>......
+00000ca0: 2a20 4f62 6675 7363 6174 696f 6e20 6f66  * Obfuscation of
+00000cb0: 2070 7974 686f 6e20 636f 6465 0d0d 0a2a   python code...*
+00000cc0: 206f 6266 7573 6361 7469 6f6e 206f 6620   obfuscation of 
+00000cd0: 7079 7468 6f6e 2063 6f64 6520 696e 746f  python code into
+00000ce0: 2069 6d61 6765 2066 696c 6573 0d0d 0a2a   image files...*
+00000cf0: 2053 7570 706f 7274 2043 6f64 6520 6578   Support Code ex
+00000d00: 7069 7279 2046 6561 7475 7265 0d0d 0a2a  piry Feature...*
+00000d10: 2053 7570 706f 7274 2069 7465 7261 7469   Support iterati
+00000d20: 6f6e 2063 6f75 6e74 6572 0d0d 0a2a 2053  on counter...* S
+00000d30: 7570 706f 7274 2066 6f72 2063 6c69 2074  upport for cli t
+00000d40: 6f6f 6c0d 0d0a 2a20 5375 7070 6f72 7473  ool...* Supports
+00000d50: 206c 6f61 6469 6e67 206f 6266 7573 6361   loading obfusca
+00000d60: 7465 6420 636f 6465 2061 7320 6d6f 6475  ted code as modu
+00000d70: 6c65 2069 6e20 616e 6f74 6865 7220 7079  le in another py
+00000d80: 7468 6f6e 2070 726f 6a65 6374 730d 0d0a  thon projects...
+00000d90: 0d0d 0a20 200d 0a                        ...  ..
```

### Comparing `subdora-0.1.0/Subdora/_subdora_cli.py` & `subdora-0.1.1/Subdora/_subdora_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import argparse
 import os 
 from datetime import datetime , timedelta  
-from ._subdora import subdora_parse , subdora_encode_file_cli
-
+from ._subdora import subdora_encode_file , subdora_encode_to_image , subdora_parse , subdora_parse_img 
 
+'''
+This is the main function that handles the cli related thing
+'''
 
 def main():
-    parser = argparse.ArgumentParser(description="8")
+    desc = '''
+    Subdora cli tool 
+    All subdora functionality on terminal 
+    usage :
+    type "subdora -h" to see full list of arguments
+    or visit https://github.com/Lakshit-Karsoliya/Subdora for usage and further query
+    '''
+    parser = argparse.ArgumentParser(description=desc)
 
     parser.add_argument("--obfuscate", type=str, help="python file going to be obfuscated")
-    parser.add_argument("--run",type=str,help=".myst file to run")
+    parser.add_argument("--img",type=str,help="image file which in which code is going to attached")
+    parser.add_argument("--run",type=str,help=".myst or .png file to run")
     parser.add_argument("--itr",type=int,help="iteration counter")
     parser.add_argument("--time",type=str,help="time of expiry")
 
     args = parser.parse_args()
 
-    py_file_arg , myst_file_arg , itr_arg , time_arg = args.obfuscate , args.run , args.itr , args.time 
+    py_file_arg, img_file_arg  , myst_file_arg , itr_arg , time_arg = args.obfuscate , args.img , args.run , args.itr , args.time 
 
-    if py_file_arg!=None and py_file_arg[-3:]==".py" and os.path.exists(os.path.abspath(py_file_arg)):
-        py_file = py_file_arg 
-        #going to obfuscate the fule usign func 1
-        if itr_arg==None:
-            itr = -100
-        if time_arg==None:
-            expiry_time = "INF"
-        if itr_arg!=None and isinstance(itr_arg,int):
-            itr = itr_arg 
-        if time_arg!=None and isinstance(time_arg, str) and (time_arg[-1] in ['m','h']) and isinstance(int(time_arg[:-1]), int):
-            current_time = datetime.now()
-            if time_arg[-1]=='m':
-                current_time += timedelta(minutes=int(time_arg[:-1]))
-            elif time_arg[-1]=='h':
-                current_time += timedelta(hours=int(time_arg[:-1]))
-            expiry_time = current_time.strftime("%a %b %d %H:%M:%S %Y")
-        
-        subdora_encode_file_cli(py_file,int(itr),expiry_time)
-        return
-
-    if myst_file_arg!=None and myst_file_arg[-5:]==".myst" and os.path.exists(myst_file_arg):
-        myst_file = myst_file_arg
-        # goint to run the myst file func 2
-        # dont care about other arguments 
-        subdora_parse(myst_file)
-        return
+    if py_file_arg!=None:
+        iterations = -100 if itr_arg == None else itr_arg 
+        exp_time = "INF" if time_arg == None else time_arg
+        if img_file_arg!=None:
+            subdora_encode_to_image(
+                py_file_arg,
+                img_file_arg,
+                iterations,
+                exp_time
+            )
+            return
+        else:
+            subdora_encode_file(
+                py_file_arg,
+                iterations,
+                exp_time
+            )
+            return
+    elif myst_file_arg!=None:
+        if myst_file_arg[-4:]=='myst':
+            subdora_parse(myst_file_arg)
+        elif myst_file_arg[-3:]=='png':
+            subdora_parse_img(myst_file_arg)
+        else:
+            print("Invalid Arguments")
+        return 
+    else:
+        print("Invalid Arguments")
```

### Comparing `subdora-0.1.0/Subdora/corex64/win/concrt140.dll` & `subdora-0.1.1/Subdora/corex64/win/concrt140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/libsodium.dll` & `subdora-0.1.1/Subdora/corex64/win/libsodium.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/msvcp140.dll` & `subdora-0.1.1/Subdora/corex64/win/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/msvcp140_1.dll` & `subdora-0.1.1/Subdora/corex64/win/msvcp140_1.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/msvcp140_2.dll` & `subdora-0.1.1/Subdora/corex64/win/msvcp140_2.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/msvcp140_atomic_wait.dll` & `subdora-0.1.1/Subdora/corex64/win/msvcp140_atomic_wait.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/msvcp140_codecvt_ids.dll` & `subdora-0.1.1/Subdora/corex64/win/msvcp140_codecvt_ids.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vcamp140.dll` & `subdora-0.1.1/Subdora/corex64/win/vcamp140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vccorlib140.dll` & `subdora-0.1.1/Subdora/corex64/win/vccorlib140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vcomp140.dll` & `subdora-0.1.1/Subdora/corex64/win/vcomp140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vcruntime140.dll` & `subdora-0.1.1/Subdora/corex64/win/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vcruntime140_1.dll` & `subdora-0.1.1/Subdora/corex64/win/vcruntime140_1.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora/corex64/win/vcruntime140_threads.dll` & `subdora-0.1.1/Subdora/corex64/win/vcruntime140_threads.dll`

 * *Files identical despite different names*

### Comparing `subdora-0.1.0/Subdora.egg-info/PKG-INFO` & `subdora-0.1.1/Subdora.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2053 7562  : 2.1..Name: Sub
 00000020: 646f 7261 0d0a 5665 7273 696f 6e3a 2030  dora..Version: 0
-00000030: 2e31 2e30 0d0a 5375 6d6d 6172 793a 2053  .1.0..Summary: S
+00000030: 2e31 2e31 0d0a 5375 6d6d 6172 793a 2053  .1.1..Summary: S
 00000040: 7562 646f 7261 203a 2041 2070 7974 686f  ubdora : A pytho
 00000050: 6e20 7061 636b 6167 6520 7468 6174 2074  n package that t
 00000060: 616b 6573 2063 6172 6520 6f66 206f 6266  akes care of obf
 00000070: 7573 6361 7469 6f6e 206f 6620 7079 7468  uscation of pyth
 00000080: 6f6e 2073 6372 6970 7473 0d0a 486f 6d65  on scripts..Home
 00000090: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 000000a0: 6974 6875 622e 636f 6d2f 4c61 6b73 6869  ithub.com/Lakshi
@@ -28,114 +28,191 @@
 000001b0: 696e 6720 5379 7374 656d 203a 3a20 556e  ing System :: Un
 000001c0: 6978 0d0a 436c 6173 7369 6669 6572 3a20  ix..Classifier: 
 000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 000001e0: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
 000001f0: 2057 696e 646f 7773 0d0a 4465 7363 7269   Windows..Descri
 00000200: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
 00000210: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000220: 6e0d 0a0d 0a0d 0a21 5b73 7562 646f 7261  n......![subdora
-00000230: 206c 6f67 6f5d 2868 7474 7073 3a2f 2f72   logo](https://r
-00000240: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000250: 7465 6e74 2e63 6f6d 2f4c 616b 7368 6974  tent.com/Lakshit
-00000260: 2d4b 6172 736f 6c69 7961 2f53 7562 646f  -Karsoliya/Subdo
-00000270: 7261 2f6d 6169 6e2f 6173 7365 7473 2f73  ra/main/assets/s
-00000280: 7562 646f 7261 2e70 6e67 2022 7375 6264  ubdora.png "subd
-00000290: 6f72 6120 6c6f 676f 2229 0d0d 0a0d 0d0a  ora logo")......
-000002a0: 3c68 313e 5375 6264 6f72 6120 302e 312e  <h1>Subdora 0.1.
-000002b0: 303c 2f68 313e 0d0d 0a3c 7020 7374 796c  0</h1>...<p styl
-000002c0: 653d 2263 6f6c 6f72 3a72 6564 3b66 6f6e  e="color:red;fon
-000002d0: 742d 7369 7a65 3a31 3270 783b 223e 2a2a  t-size:12px;">**
-000002e0: 2a54 6869 7320 7665 7273 696f 6e20 6f66  *This version of
-000002f0: 2073 7562 646f 7261 2069 7320 6e6f 7420   subdora is not 
-00000300: 6261 636b 7761 7264 2063 6f6d 7061 7469  backward compati
-00000310: 6162 6c65 2c20 6974 2069 7320 7265 636f  able, it is reco
-00000320: 6d6d 656e 6465 6420 746f 2075 7365 2074  mmended to use t
-00000330: 6865 206c 6174 6573 7420 7665 7269 736f  he latest veriso
-00000340: 6e20 6f66 2073 7562 646f 7261 203c 2f70  n of subdora </p
-00000350: 3e0d 0d0a 0d0d 0a3c 703e 5468 6973 2069  >......<p>This i
-00000360: 7320 7468 6520 5468 6972 6420 7265 6c65  s the Third rele
-00000370: 6173 6520 6f66 2073 7562 646f 7261 2e20  ase of subdora. 
-00000380: 5375 6264 6f72 6120 6973 2061 6e20 6f62  Subdora is an ob
-00000390: 6675 7363 6174 696f 6e20 746f 6f6c 2077  fuscation tool w
-000003a0: 6869 6368 206d 616b 6573 2073 6f75 7263  hich makes sourc
-000003b0: 6520 636f 6465 2076 6572 7920 6861 7264  e code very hard
-000003c0: 2074 6f20 696e 7465 7270 7261 7465 3c2f   to interprate</
-000003d0: 703e 0d0d 0a0d 0d0a 3c68 323e 496e 7374  p>......<h2>Inst
-000003e0: 616c 6c61 7469 6f6e 3c2f 6832 3e0d 0d0a  allation</h2>...
-000003f0: 0d0d 0a60 6060 0d0d 0a70 6970 2069 6e73  ...```...pip ins
-00000400: 7461 6c6c 2053 7562 646f 7261 0d0d 0a60  tall Subdora...`
-00000410: 6060 0d0d 0a0d 0d0a 3c68 323e 5375 7070  ``......<h2>Supp
-00000420: 6f72 7465 6420 4f53 3c2f 6832 3e0d 0d0a  orted OS</h2>...
-00000430: 0d0d 0a7c 2056 6572 7369 6f6e 207c 2041  ...| Version | A
-00000440: 726d 2020 207c 204c 696e 7578 2836 3429  rm   | Linux(64)
-00000450: 207c 2057 696e 646f 7773 2836 3429 207c   | Windows(64) |
-00000460: 0d0d 0a7c 3a2d 2d2d 2d2d 2d2d 3a7c 3a2d  ...|:-------:|:-
-00000470: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00000480: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  :|:-----------:|
-00000490: 0d0d 0a7c 2030 2e31 2e30 2020 207c 20e2  ...| 0.1.0   | .
-000004a0: 9d8c 2020 2020 7c20 e29c 94ef b88f 2020  ..    | ......  
-000004b0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-000004c0: 2020 2020 2020 207c 0d0d 0a7c 2030 2e30         |...| 0.0
-000004d0: 2e32 2020 207c 20e2 9d8c 2020 2020 7c20  .2   | ...    | 
-000004e0: e29c 94ef b88f 2020 2020 2020 2020 207c  ......         |
-000004f0: 20e2 9c94 efb8 8f20 2020 2020 2020 207c   ......        |
-00000500: 0d0d 0a7c 2030 2e30 2e31 2020 207c 20e2  ...| 0.0.1   | .
-00000510: 9d8c 2020 2020 7c20 e29c 94ef b88f 2020  ..    | ......  
-00000520: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00000530: 2020 2020 2020 207c 0d0d 0a0d 0d0a 0d0d         |........
-00000540: 0a3c 6832 3e57 6861 7427 7320 6e65 7720  .<h2>What's new 
-00000550: 696e 2076 302e 312e 303c 2f68 323e 0d0d  in v0.1.0</h2>..
-00000560: 0a0d 0d0a 2a20 4164 6420 7375 7070 6f72  ....* Add suppor
-00000570: 7420 666f 7220 636c 6920 746f 6f6c 200d  t for cli tool .
-00000580: 0d0a 2a20 4164 6420 6578 7069 7279 2074  ..* Add expiry t
-00000590: 696d 6520 6665 6174 7572 650d 0d0a 0d0d  ime feature.....
-000005a0: 0a0d 0d0a 3c68 323e 486f 7720 746f 2075  ....<h2>How to u
-000005b0: 7365 3c2f 6832 3e0d 0d0a 3c68 333e 436f  se</h2>...<h3>Co
-000005c0: 7265 2066 756e 6374 696f 6e61 6c69 7479  re functionality
-000005d0: 3c2f 6833 3e0d 0d0a 0d0d 0a3c 703e 3c62  </h3>......<p><b
-000005e0: 3e6f 6266 7573 6361 7469 6e67 206d 6169  >obfuscating mai
-000005f0: 6e2e 7079 2066 696c 653c 2f62 3e20 3c2f  n.py file</b> </
-00000600: 703e 0d0d 0a0d 0d0a 3c70 3e46 726f 6d20  p>......<p>From 
-00000610: 636f 6d6d 616e 6420 6c69 6e65 3c2f 703e  command line</p>
-00000620: 0d0d 0a0d 0d0a 3c63 6f64 653e 433a 5c3e  ......<code>C:\>
-00000630: 7375 6264 6f72 6120 2d2d 6f62 6675 7363  subdora --obfusc
-00000640: 6174 6520 6d61 696e 2e70 7920 2d2d 6974  ate main.py --it
-00000650: 7220 3130 202d 2d74 696d 6520 3130 6d3c  r 10 --time 10m<
-00000660: 2f63 6f64 653e 0d0d 0a0d 0d0a 3c70 3e46  /code>......<p>F
-00000670: 726f 6d20 7079 7468 6f6e 2066 696c 6520  rom python file 
-00000680: 3c2f 703e 0d0d 0a0d 0d0a 6060 6070 790d  </p>......```py.
-00000690: 0d0a 5375 6264 6f72 612e 7375 6264 6f72  ..Subdora.subdor
-000006a0: 615f 656e 636f 6465 5f66 696c 6528 226d  a_encode_file("m
-000006b0: 6169 6e2e 7079 222c 6e6f 5f6f 665f 6974  ain.py",no_of_it
-000006c0: 6572 6174 696f 6e73 2c65 7870 6972 795f  erations,expiry_
-000006d0: 7469 6d65 2923 2734 6d20 3468 2065 7463  time)#'4m 4h etc
-000006e0: 270d 0d0a 6060 600d 0d0a 0d0d 0a3c 703e  '...```......<p>
-000006f0: 3c62 3e54 6869 7320 7769 6c6c 2067 656e  <b>This will gen
-00000700: 6572 6174 6520 6120 6d61 696e 2e6d 7973  erate a main.mys
-00000710: 7420 6669 6c65 2069 6e20 6f72 6465 7220  t file in order 
-00000720: 746f 2065 7865 6375 7465 206d 7973 7420  to execute myst 
-00000730: 6669 6c65 3c2f 623e 3c2f 703e 0d0d 0a0d  file</b></p>....
-00000740: 0d0a 3c70 3e46 726f 6d20 636f 6d6d 616e  ..<p>From comman
-00000750: 6420 6c69 6e65 3c2f 703e 0d0d 0a0d 0d0a  d line</p>......
-00000760: 3c63 6f64 653e 433a 5c3e 7375 6264 6f72  <code>C:\>subdor
-00000770: 6120 2d2d 7275 6e20 6d61 696e 2e6d 7973  a --run main.mys
-00000780: 743c 2f63 6f64 653e 0d0d 0a0d 0d0a 3c70  t</code>......<p
-00000790: 3e46 726f 6d20 7079 7468 6f6e 2066 696c  >From python fil
-000007a0: 653c 2f70 3e0d 0d0a 0d0d 0a60 6060 7079  e</p>......```py
-000007b0: 0d0d 0a53 7562 646f 7261 2e73 7562 646f  ...Subdora.subdo
-000007c0: 7261 5f70 6172 7365 2822 6d61 696e 2e6d  ra_parse("main.m
-000007d0: 7973 7422 290d 0d0a 6060 600d 0d0a 0d0d  yst")...```.....
-000007e0: 0a3c 6833 3e0d 0d0a 0d0d 0a0d 0d0a 3c68  .<h3>.........<h
-000007f0: 333e 4665 6174 7572 6573 3c2f 6833 3e0d  3>Features</h3>.
-00000800: 0d0a 0d0d 0a2a 204f 6266 7573 6361 7469  .....* Obfuscati
-00000810: 6f6e 206f 6620 7079 7468 6f6e 2063 6f64  on of python cod
-00000820: 650d 0d0a 2a20 5375 7070 6f72 7420 436f  e...* Support Co
-00000830: 6465 2065 7870 6972 7920 4665 6174 7572  de expiry Featur
-00000840: 650d 0d0a 2a20 5375 7070 6f72 7420 6974  e...* Support it
-00000850: 6572 6174 696f 6e20 636f 756e 7465 720d  eration counter.
-00000860: 0d0a 2a20 5375 7070 6f72 7420 666f 7220  ..* Support for 
-00000870: 636c 6920 746f 6f6c 0d0d 0a2a 2053 7570  cli tool...* Sup
-00000880: 706f 7274 7320 6c6f 6164 696e 6720 6f62  ports loading ob
-00000890: 6675 7363 6174 6564 2063 6f64 6520 6173  fuscated code as
-000008a0: 206d 6f64 756c 6520 696e 2061 6e6f 7468   module in anoth
-000008b0: 6572 2070 7974 686f 6e20 7072 6f6a 6563  er python projec
-000008c0: 7473 0d0d 0a0d 0d0a 2020 0d0a            ts......  ..
+00000220: 6e0d 0a52 6571 7569 7265 732d 4469 7374  n..Requires-Dist
+00000230: 3a20 7069 6c6c 6f77 0d0a 0d0a 0d0a 215b  : pillow......![
+00000240: 7375 6264 6f72 6120 6c6f 676f 5d28 6874  subdora logo](ht
+00000250: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000260: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000270: 4c61 6b73 6869 742d 4b61 7273 6f6c 6979  Lakshit-Karsoliy
+00000280: 612f 5375 6264 6f72 612f 6d61 696e 2f61  a/Subdora/main/a
+00000290: 7373 6574 732f 7375 6264 6f72 612e 706e  ssets/subdora.pn
+000002a0: 6720 2273 7562 646f 7261 206c 6f67 6f22  g "subdora logo"
+000002b0: 290d 0d0a 0d0d 0a3c 6831 3e53 7562 646f  )......<h1>Subdo
+000002c0: 7261 2030 2e31 2e31 3c2f 6831 3e0d 0d0a  ra 0.1.1</h1>...
+000002d0: 3c70 2073 7479 6c65 3d22 636f 6c6f 723a  <p style="color:
+000002e0: 7265 643b 666f 6e74 2d73 697a 653a 3132  red;font-size:12
+000002f0: 7078 3b22 3e2a 2a2a 5468 6973 2076 6572  px;">***This ver
+00000300: 7369 6f6e 206f 6620 7375 6264 6f72 6120  sion of subdora 
+00000310: 6973 206e 6f74 2062 6163 6b77 6172 6420  is not backward 
+00000320: 636f 6d70 6174 6961 626c 652c 2069 7420  compatiable, it 
+00000330: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+00000340: 6f20 7573 6520 7468 6520 6c61 7465 7374  o use the latest
+00000350: 2076 6572 6973 6f6e 206f 6620 7375 6264   verison of subd
+00000360: 6f72 6120 3c2f 703e 0d0d 0a0d 0d0a 3c70  ora </p>......<p
+00000370: 3e54 6869 7320 6973 2074 6865 2054 6869  >This is the Thi
+00000380: 7264 2072 656c 6561 7365 206f 6620 7375  rd release of su
+00000390: 6264 6f72 612e 2053 7562 646f 7261 2069  bdora. Subdora i
+000003a0: 7320 616e 206f 6266 7573 6361 7469 6f6e  s an obfuscation
+000003b0: 2074 6f6f 6c20 7768 6963 6820 6d61 6b65   tool which make
+000003c0: 7320 736f 7572 6365 2063 6f64 6520 7665  s source code ve
+000003d0: 7279 2068 6172 6420 746f 2069 6e74 6572  ry hard to inter
+000003e0: 7072 6174 653c 2f70 3e0d 0d0a 0d0d 0a3c  prate</p>......<
+000003f0: 6832 3e49 6e73 7461 6c6c 6174 696f 6e3c  h2>Installation<
+00000400: 2f68 323e 0d0d 0a0d 0d0a 6060 600d 0d0a  /h2>......```...
+00000410: 7069 7020 696e 7374 616c 6c20 5375 6264  pip install Subd
+00000420: 6f72 610d 0d0a 6060 600d 0d0a 0d0d 0a3c  ora...```......<
+00000430: 6832 3e53 7570 706f 7274 6564 204f 533c  h2>Supported OS<
+00000440: 2f68 323e 0d0d 0a0d 0d0a 3c21 2d2d 207c  /h2>......<!-- |
+00000450: 2056 6572 7369 6f6e 207c 2041 726d 2020   Version | Arm  
+00000460: 207c 204c 696e 7578 2836 3429 207c 2057   | Linux(64) | W
+00000470: 696e 646f 7773 2836 3429 207c 0d0d 0a7c  indows(64) |...|
+00000480: 3a2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  :-------:|:-----
+00000490: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  :|:---------:|:-
+000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 0d0d 0a7c  ----------:|...|
+000004b0: 2030 2e31 2e31 2020 207c 20e2 9d8c 2020   0.1.1   | ...  
+000004c0: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+000004d0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+000004e0: 2020 207c 0d0d 0a7c 2030 2e31 2e30 2020     |...| 0.1.0  
+000004f0: 207c 20e2 9d8c 2020 2020 7c20 e29c 94ef   | ...    | ....
+00000500: b88f 2020 2020 2020 2020 207c 20e2 9c94  ..         | ...
+00000510: efb8 8f20 2020 2020 2020 207c 0d0d 0a7c  ...        |...|
+00000520: 2030 2e30 2e32 2020 207c 20e2 9d8c 2020   0.0.2   | ...  
+00000530: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00000540: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00000550: 2020 207c 0d0d 0a7c 2030 2e30 2e31 2020     |...| 0.0.1  
+00000560: 207c 20e2 9d8c 2020 2020 7c20 e29c 94ef   | ...    | ....
+00000570: b88f 2020 2020 2020 2020 207c 20e2 9c94  ..         | ...
+00000580: efb8 8f20 2020 2020 2020 207c 202d 2d3e  ...        | -->
+00000590: 0d0d 0a0d 0d0a 3c74 6162 6c65 3e0d 0d0a  ......<table>...
+000005a0: 2020 3c74 6865 6164 3e0d 0d0a 2020 2020    <thead>...    
+000005b0: 3c74 723e 0d0d 0a20 2020 2020 203c 7468  <tr>...      <th
+000005c0: 3e56 6572 7369 6f6e 3c2f 7468 3e0d 0d0a  >Version</th>...
+000005d0: 2020 2020 2020 3c74 683e 4172 6d3c 2f74        <th>Arm</t
+000005e0: 683e 0d0d 0a20 2020 2020 203c 7468 3e4c  h>...      <th>L
+000005f0: 696e 7578 2836 3429 3c2f 7468 3e0d 0d0a  inux(64)</th>...
+00000600: 2020 2020 2020 3c74 683e 5769 6e64 6f77        <th>Window
+00000610: 7328 3634 293c 2f74 683e 0d0d 0a20 2020  s(64)</th>...   
+00000620: 203c 2f74 723e 0d0d 0a20 203c 2f74 6865   </tr>...  </the
+00000630: 6164 3e0d 0d0a 2020 3c74 626f 6479 3e0d  ad>...  <tbody>.
+00000640: 0d0a 2020 2020 3c74 723e 0d0d 0a20 2020  ..    <tr>...   
+00000650: 2020 203c 7464 3e30 2e31 2e31 3c2f 7464     <td>0.1.1</td
+00000660: 3e0d 0d0a 2020 2020 2020 3c74 643e 2623  >...      <td>&#
+00000670: 3130 3036 303b 3c2f 7464 3e0d 0d0a 2020  10060;</td>...  
+00000680: 2020 2020 3c74 643e 2623 3130 3030 343b      <td>&#10004;
+00000690: 3c2f 7464 3e0d 0d0a 2020 2020 2020 3c74  </td>...      <t
+000006a0: 643e 2623 3130 3030 343b 3c2f 7464 3e0d  d>&#10004;</td>.
+000006b0: 0d0a 2020 2020 3c2f 7472 3e0d 0d0a 2020  ..    </tr>...  
+000006c0: 2020 3c74 723e 0d0d 0a20 2020 2020 203c    <tr>...      <
+000006d0: 7464 3e30 2e31 2e30 3c2f 7464 3e0d 0d0a  td>0.1.0</td>...
+000006e0: 2020 2020 2020 3c74 643e 2623 3130 3036        <td>&#1006
+000006f0: 303b 3c2f 7464 3e0d 0d0a 2020 2020 2020  0;</td>...      
+00000700: 3c74 643e 2623 3130 3030 343b 3c2f 7464  <td>&#10004;</td
+00000710: 3e0d 0d0a 2020 2020 2020 3c74 643e 2623  >...      <td>&#
+00000720: 3130 3030 343b 3c2f 7464 3e0d 0d0a 2020  10004;</td>...  
+00000730: 2020 3c2f 7472 3e0d 0d0a 2020 2020 3c74    </tr>...    <t
+00000740: 723e 0d0d 0a20 2020 2020 203c 7464 3e30  r>...      <td>0
+00000750: 2e30 2e32 3c2f 7464 3e0d 0d0a 2020 2020  .0.2</td>...    
+00000760: 2020 3c74 643e 2623 3130 3036 303b 3c2f    <td>&#10060;</
+00000770: 7464 3e0d 0d0a 2020 2020 2020 3c74 643e  td>...      <td>
+00000780: 2623 3130 3030 343b 3c2f 7464 3e0d 0d0a  &#10004;</td>...
+00000790: 2020 2020 2020 3c74 643e 2623 3130 3030        <td>&#1000
+000007a0: 343b 3c2f 7464 3e0d 0d0a 2020 2020 3c2f  4;</td>...    </
+000007b0: 7472 3e0d 0d0a 2020 2020 3c74 723e 0d0d  tr>...    <tr>..
+000007c0: 0a20 2020 2020 203c 7464 3e30 2e30 2e31  .      <td>0.0.1
+000007d0: 3c2f 7464 3e0d 0d0a 2020 2020 2020 3c74  </td>...      <t
+000007e0: 643e 2623 3130 3036 303b 3c2f 7464 3e0d  d>&#10060;</td>.
+000007f0: 0d0a 2020 2020 2020 3c74 643e 2623 3130  ..      <td>&#10
+00000800: 3030 343b 3c2f 7464 3e0d 0d0a 2020 2020  004;</td>...    
+00000810: 2020 3c74 643e 2623 3130 3030 343b 3c2f    <td>&#10004;</
+00000820: 7464 3e0d 0d0a 2020 2020 3c2f 7472 3e0d  td>...    </tr>.
+00000830: 0d0a 2020 3c2f 7462 6f64 793e 0d0d 0a3c  ..  </tbody>...<
+00000840: 2f74 6162 6c65 3e0d 0d0a 0d0d 0a0d 0d0a  /table>.........
+00000850: 0d0d 0a3c 6832 3e57 6861 7427 7320 6e65  ...<h2>What's ne
+00000860: 7720 696e 2076 302e 312e 313c 2f68 323e  w in v0.1.1</h2>
+00000870: 0d0d 0a0d 0d0a 2a20 6162 6c65 2074 6f20  ......* able to 
+00000880: 6f62 6675 7363 6174 6520 7079 7468 6f6e  obfuscate python
+00000890: 2073 6372 6970 7420 696e 746f 2069 6d61   script into ima
+000008a0: 6765 7320 7768 696c 6520 7265 7461 6e69  ges while retani
+000008b0: 6e67 2069 6e65 7261 7469 6f6e 2063 6f75  ng ineration cou
+000008c0: 6e74 6572 2061 6e64 2065 7870 6972 7920  nter and expiry 
+000008d0: 7469 6d65 200d 0d0a 2a20 4164 6420 7375  time ...* Add su
+000008e0: 7070 6f72 7420 666f 7220 636c 6920 746f  pport for cli to
+000008f0: 6f6c 200d 0d0a 2a20 4164 6420 6578 7069  ol ...* Add expi
+00000900: 7279 2074 696d 6520 6665 6174 7572 650d  ry time feature.
+00000910: 0d0a 0d0d 0a3c 6832 3e48 6f77 2074 6f20  .....<h2>How to 
+00000920: 7573 653c 2f68 323e 0d0d 0a3c 6833 3e43  use</h2>...<h3>C
+00000930: 6f72 6520 6675 6e63 7469 6f6e 616c 6974  ore functionalit
+00000940: 793c 2f68 333e 0d0d 0a0d 0d0a 3c70 3e3c  y</h3>......<p><
+00000950: 623e 6f62 6675 7363 6174 696e 6720 6d61  b>obfuscating ma
+00000960: 696e 2e70 7920 6669 6c65 3c2f 623e 203c  in.py file</b> <
+00000970: 2f70 3e0d 0d0a 0d0d 0a3c 703e 4672 6f6d  /p>......<p>From
+00000980: 2063 6f6d 6d61 6e64 206c 696e 653c 2f70   command line</p
+00000990: 3e0d 0d0a 0d0d 0a3c 636f 6465 3e43 3a5c  >......<code>C:\
+000009a0: 3e73 7562 646f 7261 202d 2d6f 6266 7573  >subdora --obfus
+000009b0: 6361 7465 206d 6169 6e2e 7079 202d 2d69  cate main.py --i
+000009c0: 7472 2031 3020 2d2d 7469 6d65 2031 306d  tr 10 --time 10m
+000009d0: 3c2f 636f 6465 3e0d 0d0a 0d0d 0a3c 703e  </code>......<p>
+000009e0: 4672 6f6d 2070 7974 686f 6e20 6669 6c65  From python file
+000009f0: 203c 2f70 3e0d 0d0a 0d0d 0a60 6060 7079   </p>......```py
+00000a00: 0d0d 0a53 7562 646f 7261 2e73 7562 646f  ...Subdora.subdo
+00000a10: 7261 5f65 6e63 6f64 655f 6669 6c65 2822  ra_encode_file("
+00000a20: 6d61 696e 2e70 7922 2c6e 6f5f 6f66 5f69  main.py",no_of_i
+00000a30: 7465 7261 7469 6f6e 732c 6578 7069 7279  terations,expiry
+00000a40: 5f74 696d 6529 2327 346d 2034 6820 6574  _time)#'4m 4h et
+00000a50: 6327 0d0d 0a60 6060 0d0d 0a0d 0d0a 3c70  c'...```......<p
+00000a60: 3e3c 623e 5468 6973 2077 696c 6c20 6765  ><b>This will ge
+00000a70: 6e65 7261 7465 2061 206d 6169 6e2e 6d79  nerate a main.my
+00000a80: 7374 2066 696c 6520 696e 206f 7264 6572  st file in order
+00000a90: 2074 6f20 6578 6563 7574 6520 6d79 7374   to execute myst
+00000aa0: 2066 696c 653c 2f62 3e3c 2f70 3e0d 0d0a   file</b></p>...
+00000ab0: 0d0d 0a3c 703e 4672 6f6d 2063 6f6d 6d61  ...<p>From comma
+00000ac0: 6e64 206c 696e 653c 2f70 3e0d 0d0a 0d0d  nd line</p>.....
+00000ad0: 0a3c 636f 6465 3e43 3a5c 3e73 7562 646f  .<code>C:\>subdo
+00000ae0: 7261 202d 2d72 756e 206d 6169 6e2e 6d79  ra --run main.my
+00000af0: 7374 3c2f 636f 6465 3e0d 0d0a 0d0d 0a3c  st</code>......<
+00000b00: 703e 4672 6f6d 2070 7974 686f 6e20 6669  p>From python fi
+00000b10: 6c65 3c2f 703e 0d0d 0a0d 0d0a 6060 6070  le</p>......```p
+00000b20: 790d 0d0a 5375 6264 6f72 612e 7375 6264  y...Subdora.subd
+00000b30: 6f72 615f 7061 7273 6528 226d 6169 6e2e  ora_parse("main.
+00000b40: 6d79 7374 2229 0d0d 0a60 6060 0d0d 0a0d  myst")...```....
+00000b50: 0d0a 3c70 3e3c 623e 456e 636f 6469 6e67  ..<p><b>Encoding
+00000b60: 2070 7974 686f 6e20 7363 7269 7074 2074   python script t
+00000b70: 6f20 696d 6167 653c 2f62 3e3c 2f70 3e0d  o image</b></p>.
+00000b80: 0d0a 3c70 3e2a 6f6e 6c79 2073 7570 706f  ..<p>*only suppo
+00000b90: 7274 7320 706e 6720 616e 6420 6a70 6720  rts png and jpg 
+00000ba0: 6669 6c65 733c 2f70 3e0d 0d0a 3c63 6f64  files</p>...<cod
+00000bb0: 653e 433a 3e73 7562 646f 7261 202d 2d6f  e>C:>subdora --o
+00000bc0: 6266 7573 6361 7465 206d 6169 6e2e 7079  bfuscate main.py
+00000bd0: 202d 2d69 6d67 2069 6d67 2e6a 7067 202d   --img img.jpg -
+00000be0: 2d69 7465 7261 7469 6f6e 7320 3520 2d2d  -iterations 5 --
+00000bf0: 7469 6d65 2035 6d3c 2f63 6f64 653e 0d0d  time 5m</code>..
+00000c00: 0a0d 0d0a 3c62 723e 3c70 3e54 6869 7320  ....<br><p>This 
+00000c10: 7769 6c6c 2067 656e 6572 6174 6520 6d61  will generate ma
+00000c20: 696e 2e70 6e67 2066 696c 6520 746f 2072  in.png file to r
+00000c30: 756e 2074 6865 2069 6d61 6765 2066 696c  un the image fil
+00000c40: 6520 7573 653c 2f70 3e0d 0d0a 0d0d 0a3c  e use</p>......<
+00000c50: 636f 6465 3e43 3a3e 2073 7562 646f 7261  code>C:> subdora
+00000c60: 202d 2d72 756e 206d 6169 6e2e 696d 673c   --run main.img<
+00000c70: 2f63 6f64 653e 0d0d 0a0d 0d0a 3c68 333e  /code>......<h3>
+00000c80: 0d0d 0a0d 0d0a 0d0d 0a3c 6833 3e46 6561  .........<h3>Fea
+00000c90: 7475 7265 733c 2f68 333e 0d0d 0a0d 0d0a  tures</h3>......
+00000ca0: 2a20 4f62 6675 7363 6174 696f 6e20 6f66  * Obfuscation of
+00000cb0: 2070 7974 686f 6e20 636f 6465 0d0d 0a2a   python code...*
+00000cc0: 206f 6266 7573 6361 7469 6f6e 206f 6620   obfuscation of 
+00000cd0: 7079 7468 6f6e 2063 6f64 6520 696e 746f  python code into
+00000ce0: 2069 6d61 6765 2066 696c 6573 0d0d 0a2a   image files...*
+00000cf0: 2053 7570 706f 7274 2043 6f64 6520 6578   Support Code ex
+00000d00: 7069 7279 2046 6561 7475 7265 0d0d 0a2a  piry Feature...*
+00000d10: 2053 7570 706f 7274 2069 7465 7261 7469   Support iterati
+00000d20: 6f6e 2063 6f75 6e74 6572 0d0d 0a2a 2053  on counter...* S
+00000d30: 7570 706f 7274 2066 6f72 2063 6c69 2074  upport for cli t
+00000d40: 6f6f 6c0d 0d0a 2a20 5375 7070 6f72 7473  ool...* Supports
+00000d50: 206c 6f61 6469 6e67 206f 6266 7573 6361   loading obfusca
+00000d60: 7465 6420 636f 6465 2061 7320 6d6f 6475  ted code as modu
+00000d70: 6c65 2069 6e20 616e 6f74 6865 7220 7079  le in another py
+00000d80: 7468 6f6e 2070 726f 6a65 6374 730d 0d0a  thon projects...
+00000d90: 0d0d 0a20 200d 0a                        ...  ..
```

### Comparing `subdora-0.1.0/Subdora.egg-info/SOURCES.txt` & `subdora-0.1.1/Subdora.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Subdora/__init__.py
 Subdora/_subdora.py
 Subdora/_subdora_cli.py
 Subdora.egg-info/PKG-INFO
 Subdora.egg-info/SOURCES.txt
 Subdora.egg-info/dependency_links.txt
 Subdora.egg-info/entry_points.txt
+Subdora.egg-info/requires.txt
 Subdora.egg-info/top_level.txt
 Subdora/corex64/linux/Subdora.so
 Subdora/corex64/win/Subdora.dll
 Subdora/corex64/win/concrt140.dll
 Subdora/corex64/win/libsodium.dll
 Subdora/corex64/win/msvcp140.dll
 Subdora/corex64/win/msvcp140_1.dll
```

### Comparing `subdora-0.1.0/setup.py` & `subdora-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'Subdora : A python package that takes care of obfuscation of python scripts'
 LONG_DESCRIPTION = long_description
 
 
 setup(
         name="Subdora", 
         version=VERSION,
         author="Lakshit Karsoliya",
         author_email="lakshitkumar220@gmail.com",
         description=DESCRIPTION,
         long_description_content_type="text/markdown",
 
         long_description=LONG_DESCRIPTION,
         url='https://github.com/Lakshit-Karsoliya/Subdora',
-        requires=[],
+        # requires=[],
 
-        packages=find_packages(),
-        include_package_data=True,
         
         keywords=['python', 'file encryption','security','obfuscation'],
         classifiers= [
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: Unix",
             "Operating System :: Microsoft :: Windows",
         ],
+        install_requires=["pillow"],
+        packages=find_packages(),
+        include_package_data=True,
         entry_points={
             "console_scripts":["subdora = Subdora._subdora_cli:main"],
         }
 )
```

