# Comparing `tmp/ipyslides-3.9.7.tar.gz` & `tmp/ipyslides-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.9.7.tar", last modified: Wed May 29 17:26:55 2024, max compression
+gzip compressed data, was "ipyslides-3.9.9.tar", last modified: Sat Jun  1 21:05:20 2024, max compression
```

## Comparing `ipyslides-3.9.7.tar` & `ipyslides-3.9.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:26:55.801293 ipyslides-3.9.7/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.7/LICENSE
--rw-rw-rw-   0        0        0     5391 2024-05-29 17:26:55.797514 ipyslides-3.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     4502 2024-05-29 16:58:11.000000 ipyslides-3.9.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:26:55.678015 ipyslides-3.9.7/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.7/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-29 17:05:35.000000 ipyslides-3.9.7/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:26:55.789079 ipyslides-3.9.7/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.7/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41105 2024-05-28 00:21:37.000000 ipyslides-3.9.7/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     6170 2024-05-28 17:17:01.000000 ipyslides-3.9.7/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    32996 2024-05-29 17:23:51.000000 ipyslides-3.9.7/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7555 2024-05-29 17:23:33.000000 ipyslides-3.9.7/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.7/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.7/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0     7909 2024-05-29 16:48:43.000000 ipyslides-3.9.7/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:26:55.790440 ipyslides-3.9.7/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12576 2024-05-18 23:11:33.000000 ipyslides-3.9.7/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1874 2024-05-28 17:40:55.000000 ipyslides-3.9.7/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.7/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2620 2024-05-28 17:24:24.000000 ipyslides-3.9.7/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    11908 2024-05-19 16:37:54.000000 ipyslides-3.9.7/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23555 2024-05-18 22:39:20.000000 ipyslides-3.9.7/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28835 2024-05-11 22:18:50.000000 ipyslides-3.9.7/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.7/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    16285 2024-05-28 00:22:32.000000 ipyslides-3.9.7/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    12575 2024-05-29 17:10:54.000000 ipyslides-3.9.7/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    47882 2024-05-29 17:13:38.000000 ipyslides-3.9.7/ipyslides/core.py
--rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.7/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.9.7/ipyslides/source.py
--rw-rw-rw-   0        0        0    29793 2024-05-29 15:38:52.000000 ipyslides-3.9.7/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.9.7/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.9.7/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:26:55.747060 ipyslides-3.9.7/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5391 2024-05-29 17:26:55.000000 ipyslides-3.9.7/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-29 17:26:55.000000 ipyslides-3.9.7/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:26:55.000000 ipyslides-3.9.7/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-29 17:26:55.000000 ipyslides-3.9.7/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 17:26:55.000000 ipyslides-3.9.7/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 17:26:55.801293 ipyslides-3.9.7/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.586967 ipyslides-3.9.9/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.9.9/LICENSE
+-rw-rw-rw-   0        0        0     5273 2024-06-01 21:05:20.583478 ipyslides-3.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4384 2024-06-01 21:03:10.000000 ipyslides-3.9.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.483573 ipyslides-3.9.9/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.9.9/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-06-01 20:52:13.000000 ipyslides-3.9.9/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.576357 ipyslides-3.9.9/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.9.9/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40933 2024-06-01 20:56:10.000000 ipyslides-3.9.9/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     6170 2024-05-28 17:17:01.000000 ipyslides-3.9.9/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    32648 2024-06-01 20:54:40.000000 ipyslides-3.9.9/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7555 2024-05-29 17:23:33.000000 ipyslides-3.9.9/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6606 2024-05-10 05:07:47.000000 ipyslides-3.9.9/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-10 05:35:36.000000 ipyslides-3.9.9/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0     7689 2024-05-30 18:07:59.000000 ipyslides-3.9.9/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.578362 ipyslides-3.9.9/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    11354 2024-05-30 18:06:53.000000 ipyslides-3.9.9/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1874 2024-05-28 17:40:55.000000 ipyslides-3.9.9/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3563 2024-05-18 22:39:26.000000 ipyslides-3.9.9/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2616 2024-06-01 18:25:46.000000 ipyslides-3.9.9/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    11995 2024-06-01 20:27:13.000000 ipyslides-3.9.9/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    23214 2024-06-01 19:11:51.000000 ipyslides-3.9.9/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    27096 2024-06-01 20:01:52.000000 ipyslides-3.9.9/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28407 2024-05-19 17:34:36.000000 ipyslides-3.9.9/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    16171 2024-06-01 20:22:44.000000 ipyslides-3.9.9/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    12534 2024-06-01 20:52:21.000000 ipyslides-3.9.9/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    46692 2024-06-01 20:07:57.000000 ipyslides-3.9.9/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18527 2024-05-08 17:02:50.000000 ipyslides-3.9.9/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     8776 2024-06-01 18:12:25.000000 ipyslides-3.9.9/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29785 2024-06-01 20:26:23.000000 ipyslides-3.9.9/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14549 2024-06-01 18:28:02.000000 ipyslides-3.9.9/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28897 2024-06-01 18:27:10.000000 ipyslides-3.9.9/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:05:20.548353 ipyslides-3.9.9/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5273 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 21:05:19.000000 ipyslides-3.9.9/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 21:05:20.586967 ipyslides-3.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.9.9/setup.py
```

### Comparing `ipyslides-3.9.7/LICENSE` & `ipyslides-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/PKG-INFO` & `ipyslides-3.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.7
+Version: 3.9.9
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
@@ -32,15 +32,14 @@
 </svg>
 
 # IPySlides
 
 Create interactive slides programatically in [Jupyter](https://jupyter.org/)/[Voila](https://voila.readthedocs.io/en/stable/) with all kind of rich content. 
 
 - Launch Example Notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/massgh/ipyslides/HEAD?labpath=demo.ipynb)
-- See a [Demo Notebook](https://www.kaggle.com/massgh/ipyslides) at [Kaggle](https://www.kaggle.com/massgh)
 - Watch a [Youtube Video](https://www.youtube.com/watch?v=thgLGl14-tg)
 - See [PDF-Slides](Slides.pdf)
 ![Overview](slide.png)
 
 ---
 # Changelog
 You can see upto date documentation via `ipyslides.Slides().docs()`, so no additional changelog is created.
@@ -99,15 +98,15 @@
 ---
 # Speaker Notes
 - You can turn on speaker notes with a `Show Notes` check in setting panel. See module `Slides.notes` for details or see examples in `Slides.demo()`. 
 
 > Notes is an experimantal feature, so use at your own risk. Avoid if you can.
 
 ---
-# Known Limitations
+# Caveats!
 - Since Markdown is parsed using python (and we do not run notebook from outside e.g. with nbconvert), markdown cells are of no use. A better alternative is linking a markodwn file using `Slides.sync_with_file` and slides auto update when you save your edits. You can still write markdown in code cell with slide magic `%%slide number -m` to add to slides. 
 - Slide number is necessary to be tracked by user in notebook, because cells are not linked to each other and multiple runs of a cell can lead to adding many slides with same content. Inside python scripts that run in linear fashion, you can use `Slides.[next_number,next_slide,next_frames,next_from_markdown]`.
 - Bounding box of slides for screenshots should be set by user (if not in fullscreen).
 
 ---
 
 # Acknowledgements
```

### Comparing `ipyslides-3.9.7/README.md` & `ipyslides-3.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,245 +38,237 @@
 00000250: 4269 6e64 6572 5d28 6874 7470 733a 2f2f  Binder](https://
 00000260: 6d79 6269 6e64 6572 2e6f 7267 2f62 6164  mybinder.org/bad
 00000270: 6765 5f6c 6f67 6f2e 7376 6729 5d28 6874  ge_logo.svg)](ht
 00000280: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
 00000290: 7267 2f76 322f 6768 2f6d 6173 7367 682f  rg/v2/gh/massgh/
 000002a0: 6970 7973 6c69 6465 732f 4845 4144 3f6c  ipyslides/HEAD?l
 000002b0: 6162 7061 7468 3d64 656d 6f2e 6970 796e  abpath=demo.ipyn
-000002c0: 6229 0d0a 2d20 5365 6520 6120 5b44 656d  b)..- See a [Dem
-000002d0: 6f20 4e6f 7465 626f 6f6b 5d28 6874 7470  o Notebook](http
-000002e0: 733a 2f2f 7777 772e 6b61 6767 6c65 2e63  s://www.kaggle.c
-000002f0: 6f6d 2f6d 6173 7367 682f 6970 7973 6c69  om/massgh/ipysli
-00000300: 6465 7329 2061 7420 5b4b 6167 676c 655d  des) at [Kaggle]
-00000310: 2868 7474 7073 3a2f 2f77 7777 2e6b 6167  (https://www.kag
-00000320: 676c 652e 636f 6d2f 6d61 7373 6768 290d  gle.com/massgh).
-00000330: 0a2d 2057 6174 6368 2061 205b 596f 7574  .- Watch a [Yout
-00000340: 7562 6520 5669 6465 6f5d 2868 7474 7073  ube Video](https
-00000350: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
-00000360: 6f6d 2f77 6174 6368 3f76 3d74 6867 4c47  om/watch?v=thgLG
-00000370: 6c31 342d 7467 290d 0a2d 2053 6565 205b  l14-tg)..- See [
-00000380: 5044 462d 536c 6964 6573 5d28 536c 6964  PDF-Slides](Slid
-00000390: 6573 2e70 6466 290d 0a21 5b4f 7665 7276  es.pdf)..![Overv
-000003a0: 6965 775d 2873 6c69 6465 2e70 6e67 290d  iew](slide.png).
-000003b0: 0a0d 0a2d 2d2d 0d0a 2320 4368 616e 6765  ...---..# Change
-000003c0: 6c6f 670d 0a59 6f75 2063 616e 2073 6565  log..You can see
-000003d0: 2075 7074 6f20 6461 7465 2064 6f63 756d   upto date docum
-000003e0: 656e 7461 7469 6f6e 2076 6961 2060 6970  entation via `ip
-000003f0: 7973 6c69 6465 732e 536c 6964 6573 2829  yslides.Slides()
-00000400: 2e64 6f63 7328 2960 2c20 736f 206e 6f20  .docs()`, so no 
-00000410: 6164 6469 7469 6f6e 616c 2063 6861 6e67  additional chang
-00000420: 656c 6f67 2069 7320 6372 6561 7465 642e  elog is created.
-00000430: 0d0a 0d0a 2d2d 2d0d 0a23 2049 6e73 7461  ....---..# Insta
-00000440: 6c6c 0d0a 6060 6073 6865 6c6c 0d0a 3e20  ll..```shell..> 
-00000450: 7069 7020 696e 7374 616c 6c20 6970 7973  pip install ipys
-00000460: 6c69 6465 730d 0a3e 2070 6970 2069 6e73  lides..> pip ins
-00000470: 7461 6c6c 2069 7079 736c 6964 6573 5b65  tall ipyslides[e
-00000480: 7874 7261 5d0d 0a60 6060 0d0a 466f 7220  xtra]..```..For 
-00000490: 6465 7665 6c6f 706d 656e 7420 696e 7374  development inst
-000004a0: 616c 6c2c 2063 6c6f 6e65 2074 6869 7320  all, clone this 
-000004b0: 7265 706f 7369 746f 7279 2061 6e64 2074  repository and t
-000004c0: 6865 6e0d 0a60 6060 7368 656c 6c0d 0a3e  hen..```shell..>
-000004d0: 2063 6420 6970 7973 6c69 6465 730d 0a3e   cd ipyslides..>
-000004e0: 2070 6970 2069 6e73 7461 6c6c 202d 6520   pip install -e 
-000004f0: 2e0d 0a60 6060 0d0a 0d0a 2d2d 2d0d 0a23  ...```....---..#
-00000500: 2048 6f77 2074 6f20 5573 650d 0a49 6e20   How to Use..In 
-00000510: 4a75 7079 7465 7220 4e6f 7465 626f 6f6b  Jupyter Notebook
-00000520: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  :..```python..im
-00000530: 706f 7274 2069 7079 736c 6964 6573 2061  port ipyslides a
-00000540: 7320 6973 640d 0a73 6c69 6465 7320 3d20  s isd..slides = 
-00000550: 6973 642e 536c 6964 6573 2829 0d0a 6060  isd.Slides()..``
-00000560: 600d 0a2d 2d2d 0d0a 0d0a 2320 4372 6561  `..---....# Crea
-00000570: 7469 6e67 2053 6c69 6465 730d 0a50 6c65  ting Slides..Ple
-00000580: 6173 6520 6c6f 6f6b 2061 7420 7477 6f20  ase look at two 
-00000590: 7072 6573 656e 7461 7469 6f6e 7320 7072  presentations pr
-000005a0: 6f76 6964 6564 2077 6974 6820 6053 6c69  ovided with `Sli
-000005b0: 6465 732e 646f 6373 2829 602c 2060 536c  des.docs()`, `Sl
-000005c0: 6964 6573 2e64 656d 6f28 2960 2074 6f20  ides.demo()` to 
-000005d0: 7365 6520 686f 7720 736c 6964 6573 2061  see how slides a
-000005e0: 7265 2063 7265 6174 6564 2e20 4d6f 7265  re created. More
-000005f0: 6f76 6572 2069 6e73 7472 7563 7469 6f6e  over instruction
-00000600: 2069 6e20 7365 7474 696e 6773 2070 616e   in settings pan
-00000610: 656c 2061 7265 2061 7420 796f 7572 2066  el are at your f
-00000620: 696e 6765 7220 7469 7073 2e0d 0a0d 0a0d  inger tips......
-00000630: 0a2d 2d2d 0d0a 2320 436f 6e74 656e 7420  .---..# Content 
-00000640: 5479 7065 7320 746f 2045 6d62 6564 0d0a  Types to Embed..
-00000650: 596f 7520 6361 6e20 656d 6265 6420 616e  You can embed an
-00000660: 7974 6869 6e67 2074 6861 7420 796f 7520  ything that you 
-00000670: 6361 6e20 696e 636c 7564 6520 696e 204a  can include in J
-00000680: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
-00000690: 6c69 6b65 2069 7079 7769 6467 6574 732c  like ipywidgets,
-000006a0: 2048 544d 4c2c 2050 4446 2c20 5669 6465   HTML, PDF, Vide
-000006b0: 6f73 2065 7463 2e2c 696e 636c 7564 696e  os etc.,includin
-000006c0: 6720 6a75 7079 7465 7220 6e6f 7465 626f  g jupyter notebo
-000006d0: 6f6b 2069 7473 656c 6621 200d 0a0d 0a2d  ok itself! ....-
-000006e0: 2049 5079 7468 6f6e 2044 6973 706c 6179   IPython Display
-000006f0: 204f 626a 6563 7473 2c20 7365 6520 6049   Objects, see `I
-00000700: 5079 7468 6f6e 6020 6d6f 6475 6c65 2e0d  Python` module..
-00000710: 0a2d 2050 6c6f 7473 2061 6e64 204f 7468  .- Plots and Oth
-00000720: 6572 2044 6174 6120 5479 7065 7320 286d  er Data Types (m
-00000730: 6174 706c 6f74 6c69 622c 2070 6c6f 746c  atplotlib, plotl
-00000740: 7920 6574 632e 290d 0a2d 204a 7570 7974  y etc.)..- Jupyt
-00000750: 6572 2049 6e74 6572 6163 7469 7665 2057  er Interactive W
-00000760: 6964 6765 7473 2028 6970 7977 6964 6765  idgets (ipywidge
-00000770: 7473 2c20 6271 706c 6f74 2065 6374 2e29  ts, bqplot ect.)
-00000780: 0d0a 2d20 4375 7374 6f6d 2061 6e64 2054  ..- Custom and T
-00000790: 6869 7264 2050 6172 7479 204f 626a 6563  hird Party Objec
-000007a0: 7473 2820 7768 6963 6820 6172 6520 6e6f  ts( which are no
-000007b0: 7420 696d 706c 656d 656e 7465 6420 696e  t implemented in
-000007c0: 2074 6869 7320 6c69 6272 6172 7929 0d0a   this library)..
-000007d0: 2020 2020 2d20 596f 7520 6361 6e20 6469      - You can di
-000007e0: 7370 6c61 7920 7769 7468 2060 6469 7370  splay with `disp
-000007f0: 6c61 7960 2063 6f6d 6d61 6e64 206f 7220  lay` command or 
-00000800: 6c69 6272 6172 7927 7320 7370 6563 6966  library's specif
-00000810: 6963 2064 6973 706c 6179 206d 6574 686f  ic display metho
-00000820: 642e 0d0a 2020 2020 2d20 596f 7520 6361  d...    - You ca
-00000830: 6e20 7365 7269 616c 697a 6520 6375 7374  n serialize cust
-00000840: 6f6d 206f 626a 6563 7473 2074 6f20 4854  om objects to HT
-00000850: 4d4c 2075 7369 6e67 2060 536c 6964 6573  ML using `Slides
-00000860: 2e73 6572 6961 6c69 7a65 7260 2041 5049  .serializer` API
-00000870: 2e0d 0a2d 2059 6f75 2063 616e 2065 7874  ...- You can ext
-00000880: 656e 6420 6d61 726b 646f 776e 2073 796e  end markdown syn
-00000890: 7461 7820 7573 696e 6720 6053 6c69 6465  tax using `Slide
-000008a0: 732e 6578 7465 6e64 6572 6020 4150 492e  s.extender` API.
-000008b0: 2053 6565 2073 6f6d 6520 676f 6f64 2065   See some good e
-000008c0: 7874 656e 7369 6f6e 7320 746f 2061 6464  xtensions to add
-000008d0: 2066 726f 6d20 5b50 794d 646f 776e 5d28   from [PyMdown](
-000008e0: 6874 7470 733a 2f2f 6661 6365 6c65 7373  https://faceless
-000008f0: 7573 6572 2e67 6974 6875 622e 696f 2f70  user.github.io/p
-00000900: 796d 646f 776e 2d65 7874 656e 7369 6f6e  ymdown-extension
-00000910: 732f 292e 0d0a 0d0a 0d0a 2d2d 2d0d 0a23  s/).......---..#
-00000920: 2050 4446 2070 7269 6e74 696e 670d 0a54   PDF printing..T
-00000930: 6f20 696e 636c 7564 6520 616c 6c20 7479  o include all ty
-00000940: 7065 206f 6620 6f62 6a65 6374 7320 796f  pe of objects yo
-00000950: 7520 6e65 6564 2074 6f20 6d61 6b65 2050  u need to make P
-00000960: 4446 206d 616e 7561 6c6c 792e 0d0a 5265  DF manually...Re
-00000970: 6164 2069 6e73 7472 7563 7469 6f6e 7320  ad instructions 
-00000980: 6279 2063 6c69 636b 696e 6720 e284 b9ef  by clicking ....
-00000990: b88f 2062 7574 746f 6e20 696e 2071 7569  .. button in qui
-000009a0: 636b 206d 656e 752e 2053 6565 205b 5044  ck menu. See [PD
-000009b0: 462d 536c 6964 6573 5d28 4950 7953 6c69  F-Slides](IPySli
-000009c0: 6465 732d 5072 696e 742e 7064 6629 0d0a  des-Print.pdf)..
-000009d0: 4966 2079 6f75 206a 7573 7420 6861 7665  If you just have
-000009e0: 2048 544d 4c20 6f62 6a65 6374 7320 6c69   HTML objects li
-000009f0: 6b65 2060 6d61 7470 6c6f 746f 6c69 6220  ke `matplotolib 
-00000a00: 706c 6f74 7360 2c20 6069 6d61 6765 7360  plots`, `images`
-00000a10: 2c20 6070 6c6f 746c 7960 2c20 6062 6f6b  , `plotly`, `bok
-00000a20: 6568 6020 6368 6172 7473 2065 7463 2e20  eh` charts etc. 
-00000a30: 616e 6420 6e6f 7420 736f 6d65 7468 696e  and not somethin
-00000a40: 6720 6c69 6b65 2060 6970 7977 6964 6765  g like `ipywidge
-00000a50: 7473 602c 2073 6565 206e 6578 7420 7365  ts`, see next se
-00000a60: 6374 696f 6e2e 0d0a 0d0a 2d2d 2d0d 0a23  ction.....---..#
-00000a70: 2048 544d 4c2f 5044 4620 536c 6964 6573   HTML/PDF Slides
-00000a80: 0d0a 2d20 5573 6520 6073 6c69 6465 732e  ..- Use `slides.
-00000a90: 6578 706f 7274 5f68 746d 6c60 2074 6f20  export_html` to 
-00000aa0: 6275 696c 6420 7374 6174 6963 2073 6c69  build static sli
-00000ab0: 6465 7320 7468 6174 2079 6f75 2063 616e  des that you can
-00000ac0: 2070 7269 6e74 2061 7320 7765 6c6c 2e0d   print as well..
-00000ad0: 0a2d 2043 6f6e 7465 6e74 2076 6172 6965  .- Content varie
-00000ae0: 7479 2066 6f72 2065 7870 6f72 7420 6973  ty for export is
-00000af0: 206c 696d 6974 6564 2e20 5769 6467 6574   limited. Widget
-00000b00: 7320 6361 6e20 6e6f 7420 6265 2065 7870  s can not be exp
-00000b10: 6f72 7465 6420 756e 6c65 7373 2061 6e20  orted unless an 
-00000b20: 616c 7465 726e 6174 6976 6520 7265 7072  alternative repr
-00000b30: 6573 656e 7461 7469 6f6e 2069 7320 6769  esentation is gi
-00000b40: 7665 6e20 6279 2060 536c 6964 6573 2e61  ven by `Slides.a
-00000b50: 6c74 2877 6964 6765 742c 2066 756e 6328  lt(widget, func(
-00000b60: 7769 6467 6574 2929 602e 0d0a 2d20 5061  widget))`...- Pa
-00000b70: 7065 7220 7769 6474 6820 666f 7220 7072  per width for pr
-00000b80: 696e 7469 6e67 2069 7320 3130 2069 6e63  inting is 10 inc
-00000b90: 6820 2832 3534 6d6d 2920 616e 6420 6865  h (254mm) and he
-00000ba0: 6967 6874 2069 7320 6465 7465 726d 696e  ight is determin
-00000bb0: 6564 2062 7920 6173 7065 6374 2072 6174  ed by aspect rat
-00000bc0: 696f 206f 6620 736c 6964 6573 2e0d 0a2d  io of slides...-
-00000bd0: 2055 7365 2060 5361 7665 2061 7320 5044   Use `Save as PD
-00000be0: 4660 2069 6e20 6272 6f77 7365 7220 746f  F` in browser to
-00000bf0: 206d 616b 6520 6c69 6e6b 7320 776f 726b   make links work
-00000c00: 2069 6e20 6f75 7075 7420 5044 462e 0d0a   in ouput PDF...
-00000c10: 0d0a 2d2d 2d0d 0a23 2053 7065 616b 6572  ..---..# Speaker
-00000c20: 204e 6f74 6573 0d0a 2d20 596f 7520 6361   Notes..- You ca
-00000c30: 6e20 7475 726e 206f 6e20 7370 6561 6b65  n turn on speake
-00000c40: 7220 6e6f 7465 7320 7769 7468 2061 2060  r notes with a `
-00000c50: 5368 6f77 204e 6f74 6573 6020 6368 6563  Show Notes` chec
-00000c60: 6b20 696e 2073 6574 7469 6e67 2070 616e  k in setting pan
-00000c70: 656c 2e20 5365 6520 6d6f 6475 6c65 2060  el. See module `
-00000c80: 536c 6964 6573 2e6e 6f74 6573 6020 666f  Slides.notes` fo
-00000c90: 7220 6465 7461 696c 7320 6f72 2073 6565  r details or see
-00000ca0: 2065 7861 6d70 6c65 7320 696e 2060 536c   examples in `Sl
-00000cb0: 6964 6573 2e64 656d 6f28 2960 2e20 0d0a  ides.demo()`. ..
-00000cc0: 0d0a 3e20 4e6f 7465 7320 6973 2061 6e20  ..> Notes is an 
-00000cd0: 6578 7065 7269 6d61 6e74 616c 2066 6561  experimantal fea
-00000ce0: 7475 7265 2c20 736f 2075 7365 2061 7420  ture, so use at 
-00000cf0: 796f 7572 206f 776e 2072 6973 6b2e 2041  your own risk. A
-00000d00: 766f 6964 2069 6620 796f 7520 6361 6e2e  void if you can.
-00000d10: 0d0a 0d0a 2d2d 2d0d 0a23 204b 6e6f 776e  ....---..# Known
-00000d20: 204c 696d 6974 6174 696f 6e73 0d0a 2d20   Limitations..- 
-00000d30: 5369 6e63 6520 4d61 726b 646f 776e 2069  Since Markdown i
-00000d40: 7320 7061 7273 6564 2075 7369 6e67 2070  s parsed using p
-00000d50: 7974 686f 6e20 2861 6e64 2077 6520 646f  ython (and we do
-00000d60: 206e 6f74 2072 756e 206e 6f74 6562 6f6f   not run noteboo
-00000d70: 6b20 6672 6f6d 206f 7574 7369 6465 2065  k from outside e
-00000d80: 2e67 2e20 7769 7468 206e 6263 6f6e 7665  .g. with nbconve
-00000d90: 7274 292c 206d 6172 6b64 6f77 6e20 6365  rt), markdown ce
-00000da0: 6c6c 7320 6172 6520 6f66 206e 6f20 7573  lls are of no us
-00000db0: 652e 2041 2062 6574 7465 7220 616c 7465  e. A better alte
-00000dc0: 726e 6174 6976 6520 6973 206c 696e 6b69  rnative is linki
-00000dd0: 6e67 2061 206d 6172 6b6f 6477 6e20 6669  ng a markodwn fi
-00000de0: 6c65 2075 7369 6e67 2060 536c 6964 6573  le using `Slides
-00000df0: 2e73 796e 635f 7769 7468 5f66 696c 6560  .sync_with_file`
-00000e00: 2061 6e64 2073 6c69 6465 7320 6175 746f   and slides auto
-00000e10: 2075 7064 6174 6520 7768 656e 2079 6f75   update when you
-00000e20: 2073 6176 6520 796f 7572 2065 6469 7473   save your edits
-00000e30: 2e20 596f 7520 6361 6e20 7374 696c 6c20  . You can still 
-00000e40: 7772 6974 6520 6d61 726b 646f 776e 2069  write markdown i
-00000e50: 6e20 636f 6465 2063 656c 6c20 7769 7468  n code cell with
-00000e60: 2073 6c69 6465 206d 6167 6963 2060 2525   slide magic `%%
-00000e70: 736c 6964 6520 6e75 6d62 6572 202d 6d60  slide number -m`
-00000e80: 2074 6f20 6164 6420 746f 2073 6c69 6465   to add to slide
-00000e90: 732e 200d 0a2d 2053 6c69 6465 206e 756d  s. ..- Slide num
-00000ea0: 6265 7220 6973 206e 6563 6573 7361 7279  ber is necessary
-00000eb0: 2074 6f20 6265 2074 7261 636b 6564 2062   to be tracked b
-00000ec0: 7920 7573 6572 2069 6e20 6e6f 7465 626f  y user in notebo
-00000ed0: 6f6b 2c20 6265 6361 7573 6520 6365 6c6c  ok, because cell
-00000ee0: 7320 6172 6520 6e6f 7420 6c69 6e6b 6564  s are not linked
-00000ef0: 2074 6f20 6561 6368 206f 7468 6572 2061   to each other a
-00000f00: 6e64 206d 756c 7469 706c 6520 7275 6e73  nd multiple runs
-00000f10: 206f 6620 6120 6365 6c6c 2063 616e 206c   of a cell can l
-00000f20: 6561 6420 746f 2061 6464 696e 6720 6d61  ead to adding ma
-00000f30: 6e79 2073 6c69 6465 7320 7769 7468 2073  ny slides with s
-00000f40: 616d 6520 636f 6e74 656e 742e 2049 6e73  ame content. Ins
-00000f50: 6964 6520 7079 7468 6f6e 2073 6372 6970  ide python scrip
-00000f60: 7473 2074 6861 7420 7275 6e20 696e 206c  ts that run in l
-00000f70: 696e 6561 7220 6661 7368 696f 6e2c 2079  inear fashion, y
-00000f80: 6f75 2063 616e 2075 7365 2060 536c 6964  ou can use `Slid
-00000f90: 6573 2e5b 6e65 7874 5f6e 756d 6265 722c  es.[next_number,
-00000fa0: 6e65 7874 5f73 6c69 6465 2c6e 6578 745f  next_slide,next_
-00000fb0: 6672 616d 6573 2c6e 6578 745f 6672 6f6d  frames,next_from
-00000fc0: 5f6d 6172 6b64 6f77 6e5d 602e 0d0a 2d20  _markdown]`...- 
-00000fd0: 426f 756e 6469 6e67 2062 6f78 206f 6620  Bounding box of 
-00000fe0: 736c 6964 6573 2066 6f72 2073 6372 6565  slides for scree
-00000ff0: 6e73 686f 7473 2073 686f 756c 6420 6265  nshots should be
-00001000: 2073 6574 2062 7920 7573 6572 2028 6966   set by user (if
-00001010: 206e 6f74 2069 6e20 6675 6c6c 7363 7265   not in fullscre
-00001020: 656e 292e 0d0a 0d0a 2d2d 2d0d 0a0d 0a23  en).....---....#
-00001030: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
-00001040: 730d 0a2d 2053 6c69 6465 7320 6170 706c  s..- Slides appl
-00001050: 6963 6174 696f 6e20 6973 2062 6173 6564  ication is based
-00001060: 206f 6e20 5b69 7079 7769 6467 6574 735d   on [ipywidgets]
-00001070: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001080: 636f 6d2f 6a75 7079 7465 722d 7769 6467  com/jupyter-widg
-00001090: 6574 732f 6970 7977 6964 6765 7473 292e  ets/ipywidgets).
-000010a0: 0d0a 2d20 5269 6368 2064 6973 706c 6179  ..- Rich display
-000010b0: 206d 6563 6861 6e69 736d 2c20 616e 6420   mechanism, and 
-000010c0: 636f 6c6c 6563 7469 6f6e 206f 6620 6365  collection of ce
-000010d0: 6c6c 206f 7574 7075 7420 746f 2073 6c69  ll output to sli
-000010e0: 6465 7320 6865 6176 696c 7920 7265 6c79  des heavily rely
-000010f0: 206f 6e20 5b49 5079 7468 6f6e 5d28 6874   on [IPython](ht
-00001100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001110: 2f69 7079 7468 6f6e 2f69 7079 7468 6f6e  /ipython/ipython
-00001120: 292e 0d0a 2d20 5b50 7974 686f 6e2d 4d61  )...- [Python-Ma
-00001130: 726b 646f 776e 5d28 6874 7470 733a 2f2f  rkdown](https://
-00001140: 7079 7468 6f6e 2d6d 6172 6b64 6f77 6e2e  python-markdown.
-00001150: 6769 7468 7562 2e69 6f2f 2920 6973 2065  github.io/) is e
-00001160: 7874 656e 7369 6c79 2075 7365 6420 666f  xtensily used fo
-00001170: 7220 636f 6e74 656e 7420 616e 6420 6578  r content and ex
-00001180: 7465 6e64 6564 2077 6865 7265 206e 6565  tended where nee
-00001190: 6465 642e 0d0a                           ded...
+000002c0: 6229 0d0a 2d20 5761 7463 6820 6120 5b59  b)..- Watch a [Y
+000002d0: 6f75 7475 6265 2056 6964 656f 5d28 6874  outube Video](ht
+000002e0: 7470 733a 2f2f 7777 772e 796f 7574 7562  tps://www.youtub
+000002f0: 652e 636f 6d2f 7761 7463 683f 763d 7468  e.com/watch?v=th
+00000300: 674c 476c 3134 2d74 6729 0d0a 2d20 5365  gLGl14-tg)..- Se
+00000310: 6520 5b50 4446 2d53 6c69 6465 735d 2853  e [PDF-Slides](S
+00000320: 6c69 6465 732e 7064 6629 0d0a 215b 4f76  lides.pdf)..![Ov
+00000330: 6572 7669 6577 5d28 736c 6964 652e 706e  erview](slide.pn
+00000340: 6729 0d0a 0d0a 2d2d 2d0d 0a23 2043 6861  g)....---..# Cha
+00000350: 6e67 656c 6f67 0d0a 596f 7520 6361 6e20  ngelog..You can 
+00000360: 7365 6520 7570 746f 2064 6174 6520 646f  see upto date do
+00000370: 6375 6d65 6e74 6174 696f 6e20 7669 6120  cumentation via 
+00000380: 6069 7079 736c 6964 6573 2e53 6c69 6465  `ipyslides.Slide
+00000390: 7328 292e 646f 6373 2829 602c 2073 6f20  s().docs()`, so 
+000003a0: 6e6f 2061 6464 6974 696f 6e61 6c20 6368  no additional ch
+000003b0: 616e 6765 6c6f 6720 6973 2063 7265 6174  angelog is creat
+000003c0: 6564 2e0d 0a0d 0a2d 2d2d 0d0a 2320 496e  ed.....---..# In
+000003d0: 7374 616c 6c0d 0a60 6060 7368 656c 6c0d  stall..```shell.
+000003e0: 0a3e 2070 6970 2069 6e73 7461 6c6c 2069  .> pip install i
+000003f0: 7079 736c 6964 6573 0d0a 3e20 7069 7020  pyslides..> pip 
+00000400: 696e 7374 616c 6c20 6970 7973 6c69 6465  install ipyslide
+00000410: 735b 6578 7472 615d 0d0a 6060 600d 0a46  s[extra]..```..F
+00000420: 6f72 2064 6576 656c 6f70 6d65 6e74 2069  or development i
+00000430: 6e73 7461 6c6c 2c20 636c 6f6e 6520 7468  nstall, clone th
+00000440: 6973 2072 6570 6f73 6974 6f72 7920 616e  is repository an
+00000450: 6420 7468 656e 0d0a 6060 6073 6865 6c6c  d then..```shell
+00000460: 0d0a 3e20 6364 2069 7079 736c 6964 6573  ..> cd ipyslides
+00000470: 0d0a 3e20 7069 7020 696e 7374 616c 6c20  ..> pip install 
+00000480: 2d65 202e 0d0a 6060 600d 0a0d 0a2d 2d2d  -e ...```....---
+00000490: 0d0a 2320 486f 7720 746f 2055 7365 0d0a  ..# How to Use..
+000004a0: 496e 204a 7570 7974 6572 204e 6f74 6562  In Jupyter Noteb
+000004b0: 6f6f 6b3a 0d0a 6060 6070 7974 686f 6e0d  ook:..```python.
+000004c0: 0a69 6d70 6f72 7420 6970 7973 6c69 6465  .import ipyslide
+000004d0: 7320 6173 2069 7364 0d0a 736c 6964 6573  s as isd..slides
+000004e0: 203d 2069 7364 2e53 6c69 6465 7328 290d   = isd.Slides().
+000004f0: 0a60 6060 0d0a 2d2d 2d0d 0a0d 0a23 2043  .```..---....# C
+00000500: 7265 6174 696e 6720 536c 6964 6573 0d0a  reating Slides..
+00000510: 506c 6561 7365 206c 6f6f 6b20 6174 2074  Please look at t
+00000520: 776f 2070 7265 7365 6e74 6174 696f 6e73  wo presentations
+00000530: 2070 726f 7669 6465 6420 7769 7468 2060   provided with `
+00000540: 536c 6964 6573 2e64 6f63 7328 2960 2c20  Slides.docs()`, 
+00000550: 6053 6c69 6465 732e 6465 6d6f 2829 6020  `Slides.demo()` 
+00000560: 746f 2073 6565 2068 6f77 2073 6c69 6465  to see how slide
+00000570: 7320 6172 6520 6372 6561 7465 642e 204d  s are created. M
+00000580: 6f72 656f 7665 7220 696e 7374 7275 6374  oreover instruct
+00000590: 696f 6e20 696e 2073 6574 7469 6e67 7320  ion in settings 
+000005a0: 7061 6e65 6c20 6172 6520 6174 2079 6f75  panel are at you
+000005b0: 7220 6669 6e67 6572 2074 6970 732e 0d0a  r finger tips...
+000005c0: 0d0a 0d0a 2d2d 2d0d 0a23 2043 6f6e 7465  ....---..# Conte
+000005d0: 6e74 2054 7970 6573 2074 6f20 456d 6265  nt Types to Embe
+000005e0: 640d 0a59 6f75 2063 616e 2065 6d62 6564  d..You can embed
+000005f0: 2061 6e79 7468 696e 6720 7468 6174 2079   anything that y
+00000600: 6f75 2063 616e 2069 6e63 6c75 6465 2069  ou can include i
+00000610: 6e20 4a75 7079 7465 7220 6e6f 7465 626f  n Jupyter notebo
+00000620: 6f6b 206c 696b 6520 6970 7977 6964 6765  ok like ipywidge
+00000630: 7473 2c20 4854 4d4c 2c20 5044 462c 2056  ts, HTML, PDF, V
+00000640: 6964 656f 7320 6574 632e 2c69 6e63 6c75  ideos etc.,inclu
+00000650: 6469 6e67 206a 7570 7974 6572 206e 6f74  ding jupyter not
+00000660: 6562 6f6f 6b20 6974 7365 6c66 2120 0d0a  ebook itself! ..
+00000670: 0d0a 2d20 4950 7974 686f 6e20 4469 7370  ..- IPython Disp
+00000680: 6c61 7920 4f62 6a65 6374 732c 2073 6565  lay Objects, see
+00000690: 2060 4950 7974 686f 6e60 206d 6f64 756c   `IPython` modul
+000006a0: 652e 0d0a 2d20 506c 6f74 7320 616e 6420  e...- Plots and 
+000006b0: 4f74 6865 7220 4461 7461 2054 7970 6573  Other Data Types
+000006c0: 2028 6d61 7470 6c6f 746c 6962 2c20 706c   (matplotlib, pl
+000006d0: 6f74 6c79 2065 7463 2e29 0d0a 2d20 4a75  otly etc.)..- Ju
+000006e0: 7079 7465 7220 496e 7465 7261 6374 6976  pyter Interactiv
+000006f0: 6520 5769 6467 6574 7320 2869 7079 7769  e Widgets (ipywi
+00000700: 6467 6574 732c 2062 7170 6c6f 7420 6563  dgets, bqplot ec
+00000710: 742e 290d 0a2d 2043 7573 746f 6d20 616e  t.)..- Custom an
+00000720: 6420 5468 6972 6420 5061 7274 7920 4f62  d Third Party Ob
+00000730: 6a65 6374 7328 2077 6869 6368 2061 7265  jects( which are
+00000740: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
+00000750: 2069 6e20 7468 6973 206c 6962 7261 7279   in this library
+00000760: 290d 0a20 2020 202d 2059 6f75 2063 616e  )..    - You can
+00000770: 2064 6973 706c 6179 2077 6974 6820 6064   display with `d
+00000780: 6973 706c 6179 6020 636f 6d6d 616e 6420  isplay` command 
+00000790: 6f72 206c 6962 7261 7279 2773 2073 7065  or library's spe
+000007a0: 6369 6669 6320 6469 7370 6c61 7920 6d65  cific display me
+000007b0: 7468 6f64 2e0d 0a20 2020 202d 2059 6f75  thod...    - You
+000007c0: 2063 616e 2073 6572 6961 6c69 7a65 2063   can serialize c
+000007d0: 7573 746f 6d20 6f62 6a65 6374 7320 746f  ustom objects to
+000007e0: 2048 544d 4c20 7573 696e 6720 6053 6c69   HTML using `Sli
+000007f0: 6465 732e 7365 7269 616c 697a 6572 6020  des.serializer` 
+00000800: 4150 492e 0d0a 2d20 596f 7520 6361 6e20  API...- You can 
+00000810: 6578 7465 6e64 206d 6172 6b64 6f77 6e20  extend markdown 
+00000820: 7379 6e74 6178 2075 7369 6e67 2060 536c  syntax using `Sl
+00000830: 6964 6573 2e65 7874 656e 6465 7260 2041  ides.extender` A
+00000840: 5049 2e20 5365 6520 736f 6d65 2067 6f6f  PI. See some goo
+00000850: 6420 6578 7465 6e73 696f 6e73 2074 6f20  d extensions to 
+00000860: 6164 6420 6672 6f6d 205b 5079 4d64 6f77  add from [PyMdow
+00000870: 6e5d 2868 7474 7073 3a2f 2f66 6163 656c  n](https://facel
+00000880: 6573 7375 7365 722e 6769 7468 7562 2e69  essuser.github.i
+00000890: 6f2f 7079 6d64 6f77 6e2d 6578 7465 6e73  o/pymdown-extens
+000008a0: 696f 6e73 2f29 2e0d 0a0d 0a0d 0a2d 2d2d  ions/).......---
+000008b0: 0d0a 2320 5044 4620 7072 696e 7469 6e67  ..# PDF printing
+000008c0: 0d0a 546f 2069 6e63 6c75 6465 2061 6c6c  ..To include all
+000008d0: 2074 7970 6520 6f66 206f 626a 6563 7473   type of objects
+000008e0: 2079 6f75 206e 6565 6420 746f 206d 616b   you need to mak
+000008f0: 6520 5044 4620 6d61 6e75 616c 6c79 2e0d  e PDF manually..
+00000900: 0a52 6561 6420 696e 7374 7275 6374 696f  .Read instructio
+00000910: 6e73 2062 7920 636c 6963 6b69 6e67 20e2  ns by clicking .
+00000920: 84b9 efb8 8f20 6275 7474 6f6e 2069 6e20  ..... button in 
+00000930: 7175 6963 6b20 6d65 6e75 2e20 5365 6520  quick menu. See 
+00000940: 5b50 4446 2d53 6c69 6465 735d 2849 5079  [PDF-Slides](IPy
+00000950: 536c 6964 6573 2d50 7269 6e74 2e70 6466  Slides-Print.pdf
+00000960: 290d 0a49 6620 796f 7520 6a75 7374 2068  )..If you just h
+00000970: 6176 6520 4854 4d4c 206f 626a 6563 7473  ave HTML objects
+00000980: 206c 696b 6520 606d 6174 706c 6f74 6f6c   like `matplotol
+00000990: 6962 2070 6c6f 7473 602c 2060 696d 6167  ib plots`, `imag
+000009a0: 6573 602c 2060 706c 6f74 6c79 602c 2060  es`, `plotly`, `
+000009b0: 626f 6b65 6860 2063 6861 7274 7320 6574  bokeh` charts et
+000009c0: 632e 2061 6e64 206e 6f74 2073 6f6d 6574  c. and not somet
+000009d0: 6869 6e67 206c 696b 6520 6069 7079 7769  hing like `ipywi
+000009e0: 6467 6574 7360 2c20 7365 6520 6e65 7874  dgets`, see next
+000009f0: 2073 6563 7469 6f6e 2e0d 0a0d 0a2d 2d2d   section.....---
+00000a00: 0d0a 2320 4854 4d4c 2f50 4446 2053 6c69  ..# HTML/PDF Sli
+00000a10: 6465 730d 0a2d 2055 7365 2060 736c 6964  des..- Use `slid
+00000a20: 6573 2e65 7870 6f72 745f 6874 6d6c 6020  es.export_html` 
+00000a30: 746f 2062 7569 6c64 2073 7461 7469 6320  to build static 
+00000a40: 736c 6964 6573 2074 6861 7420 796f 7520  slides that you 
+00000a50: 6361 6e20 7072 696e 7420 6173 2077 656c  can print as wel
+00000a60: 6c2e 0d0a 2d20 436f 6e74 656e 7420 7661  l...- Content va
+00000a70: 7269 6574 7920 666f 7220 6578 706f 7274  riety for export
+00000a80: 2069 7320 6c69 6d69 7465 642e 2057 6964   is limited. Wid
+00000a90: 6765 7473 2063 616e 206e 6f74 2062 6520  gets can not be 
+00000aa0: 6578 706f 7274 6564 2075 6e6c 6573 7320  exported unless 
+00000ab0: 616e 2061 6c74 6572 6e61 7469 7665 2072  an alternative r
+00000ac0: 6570 7265 7365 6e74 6174 696f 6e20 6973  epresentation is
+00000ad0: 2067 6976 656e 2062 7920 6053 6c69 6465   given by `Slide
+00000ae0: 732e 616c 7428 7769 6467 6574 2c20 6675  s.alt(widget, fu
+00000af0: 6e63 2877 6964 6765 7429 2960 2e0d 0a2d  nc(widget))`...-
+00000b00: 2050 6170 6572 2077 6964 7468 2066 6f72   Paper width for
+00000b10: 2070 7269 6e74 696e 6720 6973 2031 3020   printing is 10 
+00000b20: 696e 6368 2028 3235 346d 6d29 2061 6e64  inch (254mm) and
+00000b30: 2068 6569 6768 7420 6973 2064 6574 6572   height is deter
+00000b40: 6d69 6e65 6420 6279 2061 7370 6563 7420  mined by aspect 
+00000b50: 7261 7469 6f20 6f66 2073 6c69 6465 732e  ratio of slides.
+00000b60: 0d0a 2d20 5573 6520 6053 6176 6520 6173  ..- Use `Save as
+00000b70: 2050 4446 6020 696e 2062 726f 7773 6572   PDF` in browser
+00000b80: 2074 6f20 6d61 6b65 206c 696e 6b73 2077   to make links w
+00000b90: 6f72 6b20 696e 206f 7570 7574 2050 4446  ork in ouput PDF
+00000ba0: 2e0d 0a0d 0a2d 2d2d 0d0a 2320 5370 6561  .....---..# Spea
+00000bb0: 6b65 7220 4e6f 7465 730d 0a2d 2059 6f75  ker Notes..- You
+00000bc0: 2063 616e 2074 7572 6e20 6f6e 2073 7065   can turn on spe
+00000bd0: 616b 6572 206e 6f74 6573 2077 6974 6820  aker notes with 
+00000be0: 6120 6053 686f 7720 4e6f 7465 7360 2063  a `Show Notes` c
+00000bf0: 6865 636b 2069 6e20 7365 7474 696e 6720  heck in setting 
+00000c00: 7061 6e65 6c2e 2053 6565 206d 6f64 756c  panel. See modul
+00000c10: 6520 6053 6c69 6465 732e 6e6f 7465 7360  e `Slides.notes`
+00000c20: 2066 6f72 2064 6574 6169 6c73 206f 7220   for details or 
+00000c30: 7365 6520 6578 616d 706c 6573 2069 6e20  see examples in 
+00000c40: 6053 6c69 6465 732e 6465 6d6f 2829 602e  `Slides.demo()`.
+00000c50: 200d 0a0d 0a3e 204e 6f74 6573 2069 7320   ....> Notes is 
+00000c60: 616e 2065 7870 6572 696d 616e 7461 6c20  an experimantal 
+00000c70: 6665 6174 7572 652c 2073 6f20 7573 6520  feature, so use 
+00000c80: 6174 2079 6f75 7220 6f77 6e20 7269 736b  at your own risk
+00000c90: 2e20 4176 6f69 6420 6966 2079 6f75 2063  . Avoid if you c
+00000ca0: 616e 2e0d 0a0d 0a2d 2d2d 0d0a 2320 4361  an.....---..# Ca
+00000cb0: 7665 6174 7321 0d0a 2d20 5369 6e63 6520  veats!..- Since 
+00000cc0: 4d61 726b 646f 776e 2069 7320 7061 7273  Markdown is pars
+00000cd0: 6564 2075 7369 6e67 2070 7974 686f 6e20  ed using python 
+00000ce0: 2861 6e64 2077 6520 646f 206e 6f74 2072  (and we do not r
+00000cf0: 756e 206e 6f74 6562 6f6f 6b20 6672 6f6d  un notebook from
+00000d00: 206f 7574 7369 6465 2065 2e67 2e20 7769   outside e.g. wi
+00000d10: 7468 206e 6263 6f6e 7665 7274 292c 206d  th nbconvert), m
+00000d20: 6172 6b64 6f77 6e20 6365 6c6c 7320 6172  arkdown cells ar
+00000d30: 6520 6f66 206e 6f20 7573 652e 2041 2062  e of no use. A b
+00000d40: 6574 7465 7220 616c 7465 726e 6174 6976  etter alternativ
+00000d50: 6520 6973 206c 696e 6b69 6e67 2061 206d  e is linking a m
+00000d60: 6172 6b6f 6477 6e20 6669 6c65 2075 7369  arkodwn file usi
+00000d70: 6e67 2060 536c 6964 6573 2e73 796e 635f  ng `Slides.sync_
+00000d80: 7769 7468 5f66 696c 6560 2061 6e64 2073  with_file` and s
+00000d90: 6c69 6465 7320 6175 746f 2075 7064 6174  lides auto updat
+00000da0: 6520 7768 656e 2079 6f75 2073 6176 6520  e when you save 
+00000db0: 796f 7572 2065 6469 7473 2e20 596f 7520  your edits. You 
+00000dc0: 6361 6e20 7374 696c 6c20 7772 6974 6520  can still write 
+00000dd0: 6d61 726b 646f 776e 2069 6e20 636f 6465  markdown in code
+00000de0: 2063 656c 6c20 7769 7468 2073 6c69 6465   cell with slide
+00000df0: 206d 6167 6963 2060 2525 736c 6964 6520   magic `%%slide 
+00000e00: 6e75 6d62 6572 202d 6d60 2074 6f20 6164  number -m` to ad
+00000e10: 6420 746f 2073 6c69 6465 732e 200d 0a2d  d to slides. ..-
+00000e20: 2053 6c69 6465 206e 756d 6265 7220 6973   Slide number is
+00000e30: 206e 6563 6573 7361 7279 2074 6f20 6265   necessary to be
+00000e40: 2074 7261 636b 6564 2062 7920 7573 6572   tracked by user
+00000e50: 2069 6e20 6e6f 7465 626f 6f6b 2c20 6265   in notebook, be
+00000e60: 6361 7573 6520 6365 6c6c 7320 6172 6520  cause cells are 
+00000e70: 6e6f 7420 6c69 6e6b 6564 2074 6f20 6561  not linked to ea
+00000e80: 6368 206f 7468 6572 2061 6e64 206d 756c  ch other and mul
+00000e90: 7469 706c 6520 7275 6e73 206f 6620 6120  tiple runs of a 
+00000ea0: 6365 6c6c 2063 616e 206c 6561 6420 746f  cell can lead to
+00000eb0: 2061 6464 696e 6720 6d61 6e79 2073 6c69   adding many sli
+00000ec0: 6465 7320 7769 7468 2073 616d 6520 636f  des with same co
+00000ed0: 6e74 656e 742e 2049 6e73 6964 6520 7079  ntent. Inside py
+00000ee0: 7468 6f6e 2073 6372 6970 7473 2074 6861  thon scripts tha
+00000ef0: 7420 7275 6e20 696e 206c 696e 6561 7220  t run in linear 
+00000f00: 6661 7368 696f 6e2c 2079 6f75 2063 616e  fashion, you can
+00000f10: 2075 7365 2060 536c 6964 6573 2e5b 6e65   use `Slides.[ne
+00000f20: 7874 5f6e 756d 6265 722c 6e65 7874 5f73  xt_number,next_s
+00000f30: 6c69 6465 2c6e 6578 745f 6672 616d 6573  lide,next_frames
+00000f40: 2c6e 6578 745f 6672 6f6d 5f6d 6172 6b64  ,next_from_markd
+00000f50: 6f77 6e5d 602e 0d0a 2d20 426f 756e 6469  own]`...- Boundi
+00000f60: 6e67 2062 6f78 206f 6620 736c 6964 6573  ng box of slides
+00000f70: 2066 6f72 2073 6372 6565 6e73 686f 7473   for screenshots
+00000f80: 2073 686f 756c 6420 6265 2073 6574 2062   should be set b
+00000f90: 7920 7573 6572 2028 6966 206e 6f74 2069  y user (if not i
+00000fa0: 6e20 6675 6c6c 7363 7265 656e 292e 0d0a  n fullscreen)...
+00000fb0: 0d0a 2d2d 2d0d 0a0d 0a23 2041 636b 6e6f  ..---....# Ackno
+00000fc0: 776c 6564 6765 6d65 6e74 730d 0a2d 2053  wledgements..- S
+00000fd0: 6c69 6465 7320 6170 706c 6963 6174 696f  lides applicatio
+00000fe0: 6e20 6973 2062 6173 6564 206f 6e20 5b69  n is based on [i
+00000ff0: 7079 7769 6467 6574 735d 2868 7474 7073  pywidgets](https
+00001000: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00001010: 7079 7465 722d 7769 6467 6574 732f 6970  pyter-widgets/ip
+00001020: 7977 6964 6765 7473 292e 0d0a 2d20 5269  ywidgets)...- Ri
+00001030: 6368 2064 6973 706c 6179 206d 6563 6861  ch display mecha
+00001040: 6e69 736d 2c20 616e 6420 636f 6c6c 6563  nism, and collec
+00001050: 7469 6f6e 206f 6620 6365 6c6c 206f 7574  tion of cell out
+00001060: 7075 7420 746f 2073 6c69 6465 7320 6865  put to slides he
+00001070: 6176 696c 7920 7265 6c79 206f 6e20 5b49  avily rely on [I
+00001080: 5079 7468 6f6e 5d28 6874 7470 733a 2f2f  Python](https://
+00001090: 6769 7468 7562 2e63 6f6d 2f69 7079 7468  github.com/ipyth
+000010a0: 6f6e 2f69 7079 7468 6f6e 292e 0d0a 2d20  on/ipython)...- 
+000010b0: 5b50 7974 686f 6e2d 4d61 726b 646f 776e  [Python-Markdown
+000010c0: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
+000010d0: 2d6d 6172 6b64 6f77 6e2e 6769 7468 7562  -markdown.github
+000010e0: 2e69 6f2f 2920 6973 2065 7874 656e 7369  .io/) is extensi
+000010f0: 6c79 2075 7365 6420 666f 7220 636f 6e74  ly used for cont
+00001100: 656e 7420 616e 6420 6578 7465 6e64 6564  ent and extended
+00001110: 2077 6865 7265 206e 6565 6465 642e 0d0a   where needed...
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/_layout_css.py` & `ipyslides-3.9.9/ipyslides/_base/_layout_css.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,14 @@
                 },
                 "^.CaptureMode": {
                     ".TopBar.Outside, .SlideArea .goto-button, .Sfresh-Btn": {
                         "visibility": "hidden !important"
                     },  # Hide in screenshot
                     ".Menu-Box" : {"display": "none !important",},
                 },
-                "^.PresentMode .SlideBox .SlideArea .ProxyPasteBtns": {
-                    "display": "none !important"
-                },  # Hide in presentation mode
                 "^.FullWindow, ^.FullScreen": {
                     ".Width-Slider, .Source-Btn": {"display": "none !important"},
                 },
                 "^.FullScreen": {
                     ".FullWindow-Btn": {"display": "none !important"},
                 },
                 "@keyframes heart-beat": {
@@ -566,24 +563,24 @@
                 'rect.tl-frame__body': { # Due to lack of dark mode in widget
                     'fill':'var(--primary-bg)',
                     'stroke':'var(--secondary-bg)',
                 },
             },
             ".Arrows": {
                 ".fa.fa-chevron-left": Icon(
-                    "chevron", color=accent_color, size="32px", rotation=180
+                    "chevron", color=accent_color, size="36px", rotation=180
                 ).css,
                 ".fa.fa-chevron-right": Icon(
-                    "chevron", color=accent_color, size="32px", rotation=0
+                    "chevron", color=accent_color, size="36px", rotation=0
                 ).css,
                 ".fa.fa-chevron-up": Icon(
-                    "chevron", color=accent_color, size="32px", rotation=-90
+                    "chevron", color=accent_color, size="36px", rotation=-90
                 ).css,  # Why SVG rotation is clockwise?
                 ".fa.fa-chevron-down": Icon(
-                    "chevron", color=accent_color, size="32px", rotation=90
+                    "chevron", color=accent_color, size="36px", rotation=90
                 ).css,
             },
             ".Settings-Btn": {
                 ".fa.fa-plus": Icon("settings", color=accent_color, size=_icons_size).css,
                 ".fa.fa-minus": Icon("close", color=accent_color, size=_icons_size).css,
             },
             ".Toc-Btn": {
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/_widgets.py` & `ipyslides-3.9.9/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/base.py` & `ipyslides-3.9.9/ipyslides/_base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class BaseSlides:
     def __init__(self):
         self._warnings = [] # Will be printed at end of building slides
         self._uid = f'{self.__class__.__name__}-{id(self)}' # Unique ID for this instance to have CSS, should be before settings
         self.__widgets = Widgets()
         self.__screenshot = ScreenShot(self.__widgets)
-        self.clipboard_image = self.__screenshot.clipboard_image # For easy access
+        self.clip_image = self.__screenshot.clip_image # For easy access
         self.__navigation = Navigation(self.__widgets) # Not accessed later, just for actions
         self.__settings = LayoutSettings(self, self.__widgets)
         self.export_html = _HhtmlExporter(self).export_html
         self.__notes = Notes(self, self.__widgets) # Needs main class for access to notes
         
         self.toast_html = self.widgets.htmls.toast
         
@@ -107,16 +107,15 @@
         **Following syntax works only under currently building slide:**
         
         - alert`notes\`This is slide notes\``  to add notes to current slide
         - alert`cite\`key\`` to add citation to current slide. citations are automatically added in suitable place and should be set once using `Slides.set_citations` function.
         - With citations mode set as 'footnote', you can add alert`refs\`ncol\`` to add citations anywhere on slide. If ncol is not given, it will be picked from layout settings.
         - alert`section\`content\`` to add a section that will appear in the table of contents.
         - alert`toc\`Table of content header text\`` to add a table of contents. For block type toc, see below.
-        - alert`proxy\`placeholder text\`` to add a proxy that can be updated later with `Slides.proxies[index].capture` contextmanager. Useful to keep placeholders for plots in markdwon.
-        - alert`peoxy\`[Button Text]\`` to add a proxy that can be replaced by pasting image from clipboard later.
+        - alert`proxy\`placeholder text\`` to add a proxy that can be updated later with `Slides.get(slide_number).proxies[index].capture` contextmanager or a shortcut `Slides.capture_proxy(slides_number, proxy_index)`. Useful to keep placeholders for plots/widgets in markdwon.
         - Triple dashes `---` is used to split markdown text in slides inside `from_markdown(start, content)` function.
         - Double dashes `--` is used to split markdown text in frames.
         
         Block table of contents with extra content can be added as follows:
                                                
         ```markdown
          ```toc Table of contents
@@ -224,15 +223,15 @@
             if name in func.__code__.co_names:
                 self._warnings.append(f'UserWarning: Output of `{name}` function under `on_load` may be lost while presenting. I hope you know what you are doing!')
         
         if 'settings' in func.__code__.co_names:
             self._warnings.append(f'UserWarning: Changing settings under `on_load` may have side effects on all slides. I hope you know what you are doing!')
         
         self.verify_running('on_load decorator can only be used inside slide constructor!')
-        self.running._on_load_private(func) # This to make sure if code is correct before adding it to slide
+        self.this._on_load_private(func) # This to make sure if code is correct before adding it to slide
     
     def on_refresh(self,func):
         """
         Decorator for inserting dynamic content on slide, define a function with no arguments.
         Content updates when `slide.update_display` is called or when `Slides.refresh` is called.
         ::: note-tip
             You can use it to dynamically fetch a value from a database or API while presenting, without having to run the cell again.
@@ -257,15 +256,15 @@
             Use `ipywidgets.interact/interactive` if you need extra control widgets beyond just a refresh.
         """
         return self._dynamic_private(func, tag = '_has_widgets', hide_refresher = False)
     
     def _dynamic_private(self, func, tag = None, hide_refresher = False):
         "Not for user use, internal function for other dynamic content decorators with their own tags."
         self.verify_running('Dynamic content can only be used inside slide constructor!')
-        return self.running._dynamic_private(func, tag = tag, hide_refresher = hide_refresher)
+        return self.this._dynamic_private(func, tag = tag, hide_refresher = hide_refresher)
         
     def _update_tmp_output(self, *objs):
         "Used for CSS/animations etc. HTML widget does not work properly."
         if self.is_jupyter_session():
             self.widgets._tmp_out.clear_output(wait=True)
             with self.widgets._tmp_out:
                 display(*objs)
@@ -294,15 +293,15 @@
             Use `Slides.sync_with_file` to auto update slides as markdown content changes.
         
         ::: note-info
             Use this function with 'next_' prefix to enable auto numbeing of slides inside python file.
         
         **Returns**: A tuple of handles to slides created. These handles can be used to access slides and set properties on them.
         """
-        if self.running:
+        if self.this:
             raise RuntimeError('Creating new slides under an already running slide context is not allowed!')
         
         if not isinstance(content, str): #check path later or it will throw error
             raise TypeError(f"content expects a makrdown text block, got {content!r}")
         
         if not trusted:
             lines = content.splitlines()
@@ -399,15 +398,15 @@
         return demo_slides(self)
         
         
     def docs(self):
         "Create presentation from docs of IPySlides."
         self.close_view() # Close any previous view to speed up loading 10x faster on average
         self.clear() # Clear previous content
-        self.create(*range(23)) # Create slides faster
+        self.create(*range(22)) # Create slides faster
         
         from ..core import Slides
 
         self.set_citations({'A': 'Citation A', 'B': 'Citation B'}, mode = 'footnote')
         self.settings.set_footer('IPySlides Documentation')
 
         with self.title(): # Title
@@ -445,15 +444,15 @@
         
         with self.next_slide(), self.code.context():
             self.write(self.fmt('`{self.version!r}` `{self.xmd_syntax}`'))
             
         with self.next_slide():
             self.write('## Adding Content')
             self.write('Besides functions below, you can add content to slides with `%%xmd`,`%xmd` as well.\n{.note .info}')
-            self.write([self.classed(self.doc(self.write,'Slides'),'block-green'), self.doc(self.parse,'Slides'),self.doc(self.clipboard_image,'Slides')])
+            self.write([self.classed(self.doc(self.write,'Slides'),'block-green'), self.doc(self.parse,'Slides'),self.doc(self.clip_image,'Slides')])
         
         with self.next_slide():
             self.write('## Adding Speaker Notes')
             (skipper := self.goto_button('Skip to Dynamic Content')).display()
             self.write([f'You can use alert`notes\`notes content\`` in markdown.\n{{.note .success}}\n',
                        'This is experimental feature, and may not work as expected.\n{.note-error .error}'])
             self.doc(self.notes,'Slides.notes', members = True, itself = False).display()
@@ -466,15 +465,15 @@
         
         with self.next_slide(): 
             self.write('## Layout and Theme Settings')
             self.doc(self.settings,'Slides.settings', members=True,itself = False).display()
                 
         with self.next_slide():
             self.write('## Useful Functions for Rich Content section`?Useful Functions for alert`Rich Content`?`')
-            self.doc(self.clipboard_image,'Slides').display()
+            self.doc(self.clip_image,'Slides').display()
             self.run_doc(self.alt,'Slides')
             
             members = sorted((
                 'alert block bokeh2html bullets classed format_html fmt color cols details doc sub sup '
                 'today error enable_zoom format_css highlight html iframe image keep_format notify plt2html '
                 'raw rows set_dir sig textbox suppress_output suppress_stdout svg vspace'
             ).split())
@@ -488,21 +487,20 @@
                 `Slides.settings.set_layout(..., ncol_refs = int)`. cite`A`
                        
                 Add sections in slides to separate content by alert`section\`text\``. Corresponding table of contents
                 can be added with alert`toc\`title\``/alert`\`\`\`toc title\\n summary of current section \\n\`\`\``.
             ''')
             self.doc(self, 'Slides', members = ['set_citations'], itself = False).display()
             
-        with self.next_slide() as s:
+        with self.next_slide():
             skipper.set_target() # Set target for skip button
             self.write('## Dynamic Content')
             self.run_doc(self.on_refresh,'Slides')
             self.run_doc(self.on_load,'Slides')
-            s.get_source().display()
-            
+            self.this.get_source().display() # this refers to slide being built
     
         with self.next_slide():
             self.write('## Content Styling')
             with self.code.context(returns = True) as c:
                 self.write(('You can **style**{.error} or **color[teal]`colorize`** your *content*{: style="color:hotpink;"} and *color[hotpink,yellow]`text`*. ' 
                        'Provide **CSS**{.info} for that using `.format_css` or use some of the available styles. '
                        'See these **styles**{.success} with `.css_styles` property as below:'))
@@ -519,15 +517,15 @@
         ```javascript
         import React, { Component } from "react";
         ```
         proxy`source code of slide will be updated here later using slide_handle.proxies[0].capture contextmanager`
         ''', trusted= True)
         
         # Update proxy with source code
-        with s8.proxies[0].capture(): # Capture to proxy
+        with s8.proxies[0].capture(): # or with self.capture_proxy(s8.number, 0):
             s8.get_source().display()
         
         with self.next_slide():
             self.write('## Loading from File/Exporting to HTML section`Loading from File/Exporting to HTML`')
             self.write('You can parse and view a markdown file. The output you can save by exporting notebook in other formats.\n{.note .info}')
             self.write([self.doc(attr,'Slides') for attr in (self.sync_with_file,self.from_markdown,self.demo,self.docs,self.export_html)])
         
@@ -542,20 +540,14 @@
             )
             self.write('If you need to serialize your own or third party objects not serialized by this module, you can use `@Slides.serializer.register` to serialize them to html.\n{.note .info}')
             self.doc(self.serializer,'Slides.serializer', members = True, itself = False).display()
             self.write('**You can also extend markdown syntax** using `markdown extensions`, ([See here](https://python-markdown.github.io/extensions/) and others to install, then use as below):')
             self.doc(self.extender,'Slides.extender', members = True, itself = False).display()
         
         with self.next_slide():
-            self.write('## Keys and Shortcuts\n'
-                '- You can use `Slides.current` to access a slide currently in view.\n'
-                '- You can use `Slides.running` to access the slide currently being built,'
-                ' so you can set CSS, aminations etc.', key_combs)
-        
-        with self.next_slide():
             self.write('''
             ## Focus on what matters
             - There is a zoom button on top bar which enables zooming of certain elements. This can be toggled by `Z` key.
             - Most of supported elements are zoomable by default like images, matplotlib, bokeh, PIL image, altair plotly, dataframe, etc.
             - You can also enable zooming for an object/widget by wrapping it inside `Slide.enable_zoom` function conveniently.
             - You can also enable by manully adding `zoom-self`, `zoom-child` classes to an element. To prevent zooming under as `zoom-child` class, use `no-zoom` class.
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/export_html.py` & `ipyslides-3.9.9/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/export_template.py` & `ipyslides-3.9.9/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/icons.py` & `ipyslides-3.9.9/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/intro.py` & `ipyslides-3.9.9/ipyslides/_base/intro.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,18 +122,14 @@
 ::: note-tip
     In JupyterLab, right click on the slides and select `Create New View for Output` for optimized display.
 
 **Key Bindings**{{.success}} {_Icon("pencil", color="var(--accent-color)", rotation=45)}
 
 {key_combs}
 
-::: note
-    - You can also swipe left/right from edges of screen ( within `±50px` edge range) on touch devices to change slides.
-    - In exported slides, bottom-right includes few buttons to jump accross slides.
-
 #### PDF Printing (by screen capture)
 {how_to_print}
 
 {how_to_slide}
 
 ::: note-warning
     Restart Kernel if you make mistake in slide numbers to avoid hidden state problem.
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/js/interaction.js` & `ipyslides-3.9.9/ipyslides/_base/js/interaction.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -17,47 +17,14 @@
 }
 
 function hideLaser(box, cursor) {
     cursor.style.display = 'none'; // hide in place
     box.onmousemove = null;
 }
 
-function touchSwiper(box, model) {
-    let startX = 0;
-    let endX = 0;
-    let startY = 0;
-    let endY = 0;
-
-    box.addEventListener('touchstart', function(event) {
-        startX = event.changedTouches[0].screenX;
-        startY = event.changedTouches[0].screenY;
-    }, false);
-
-    box.addEventListener('touchend', function(event) {
-        endX = event.changedTouches[0].screenX;
-        endY = event.changedTouches[0].screenY;
-        handleGesture();
-    }, false);
-
-    function handleGesture() {
-        let bbox = box.getBoundingClientRect(); // Swipe only from edges
-        if (Math.abs(endY - startY) < 20) {
-            // Y axis is not important but we should avoid X component of touch for a long y-scroll
-            if ((endX - startX) < -40 && startX > (bbox.right - 50)) {
-                model.set("msg_topy", "NEXT"); // align-left Swipe to Next
-            };
-
-            if ((endX - startX) > 40 && startX < (bbox.left + 50)) {
-                model.set("msg_topy", "PREV"); // Right Swipe to Prev
-            };
-            model.save_changes();
-        };
-    };
-};
-
 const keyMessage = {
     's': 'SCAP', // Screenshot
     'f': 'TFS', // Toggle Fullscreen with F but with click from button
     'z': 'ZOOM', // Enable zooming items
     'g': 'TPAN', // Setting panel
     'k': 'KSC', // keyboard shortcuts
     'l': 'TLSR', // L toggle laser
@@ -272,17 +239,14 @@
         box.onmouseleave = function() {
             box.blur();
         };
 
         // Keyboard events
         keyboardEvents(box, model);
 
-        // Touch Events are experimental
-        touchSwiper(box, model);
-
         // handle scale of slides size
         handleScale(box);
 
         // Remove other views without closing comm
         keepThisViewOnly(box);
 
         // Sends a message if fullscreen is changed by some other mechanism
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/js/notes.js` & `ipyslides-3.9.9/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/navigation.py` & `ipyslides-3.9.9/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/notes.py` & `ipyslides-3.9.9/ipyslides/_base/notes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         self.notes_check = self.widgets.checks.notes
         self.notes_check.observe(self.__open_close_notes, names=['value'])
         
     def insert(self, content):
         """Add notes to current slide. Content could be any object except javascript and interactive widgets.
         ::: note-tip     
             In markdown, you can use alert`notes\`notes content\``."""
-        if self.main.running is None:
+        if self.main.this is None:
             raise RuntimeError('Notes can only be added inside a slide constructor.')
         
         with suppress(BaseException): # Would work on next run, may not first
-            self.main.running._notes = self.main.format_html(content)._repr_html_()
+            self.main.this._notes = self.main.format_html(content)._repr_html_()
     __call__ = insert # Can be called as function
     
     def display(self):
         def set_value(content):
             bg = self.main.settings.colors.get('primary_bg','white')
             fg = self.main.settings.colors.get('primary_fg','black')
             bg2 = self.main.settings.colors.get('secondary_bg','#181818')
@@ -36,16 +36,16 @@
         }}
         .columns {{columns: 2 auto;font-family: {font};}}
         .columns > div > * {{background: {bg2};padding:0.2em;font-size:110%;border-left: 2px inset {bg};}}
         .columns > div:first-child::before {{content:'This Slide';font-size:80%;font-weight:bold;}}
         .columns > div:last-child::before {{content:'Next Slide';font-size:80%;font-weight:bold;}}
         </style>{content}"""
 
-        this_notes = self.main.current.notes 
-        next_slide_index = (self.main.current.index + 1) % len(self.main)
+        this_notes = self.main._current.notes 
+        next_slide_index = (self.main._current.index + 1) % len(self.main)
         if next_slide_index > 0: # Don't loop notes back
             next_notes = self.main[next_slide_index].notes
         else:
             next_notes = ''
 
         notes = self.main.cols(this_notes,next_notes)
         self.widgets.notes.value = set_value(notes)
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/screenshot.py` & `ipyslides-3.9.9/ipyslides/_base/screenshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,22 +109,27 @@
         short, res = (h, w/11) if w > h else (w, h/11) # letter page size landscape else portrait
         
         if short/res > 8.25: # if short side out of page, bring inside A4 size so work for both A4/Letter
             return short/8.25  # change resolution to shrink pages size to fit for print,long side already inside page
         
         return res   # Return previous resolution
     
-    def capture(self,btn):
-        "Saves screenshot of current slide into self.__images dictionary when corresponding button clicked. Use in fullscreen mode or set bbox using `.capture_setup`."
+    def capture(self,btn = None):
+        "Saves screenshot of current slide when corresponding button clicked. Returns captured image if called in a cell directly!"
         with self.capture_mode():
             sleep(0.05) # Just for above clearance of widgets views
             if self.widgets.sliders.progress.label not in self.__images:
                 self.__images[self.widgets.sliders.progress.label] = [] # container to store images
             
-            self.__images[self.widgets.sliders.progress.label].append(ImageGrab.grab(bbox = None)) # Append to existing list
+            im = ImageGrab.grab(bbox = None)
+            if btn is None:
+                return im
+            else: # called by button
+                self.__images[self.widgets.sliders.progress.label].append(im) # Append to existing list
+
     
     def __sort_images(self):
         ims = [] #sorting
         for label, _ in self.widgets.sliders.progress.options:
             if label in self.__images:
                 ims = [*ims,*self.__images[label]]
 
@@ -183,15 +188,15 @@
             
             self.__images = {} # Cleaned up
             
         
         self.widgets.ddowns.clear.value = 'None' # important to get back after operation
     
     
-    def clipboard_image(self, filename, quality = 95, overwrite = False):
+    def clip_image(self, filename, quality = 95, overwrite = False):
         """Save image from clipboard to file with a given quality. 
         On next run, it loads from saved file under `notebook-dir/.ipyslides-assets/clips`. 
         Useful to add screenshots from system into IPython. You can use overwite to overwrite existing file.
         You can add saved clips using a "clip:" prefix in path in `Slides.image("clip:filename.png")` function and also in markdown.
         
         - Output can be directly used in `write` command.
         - Converts to PIL image using `.to_pil()`.
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/settings.py` & `ipyslides-3.9.9/ipyslides/_base/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.btn_fscreen.observe(self._on_icon_change, names=["icon"])
         self.btn_zoom.observe(self._push_zoom, names=["value"])
         self.btn_laser.observe(self._toggle_laser, names=["value"])
         self.reflow_check.observe(self._update_theme, names=["value"])
         self.btn_draw.observe(self._toggle_overlay, names=["value"])
         self.btn_menu.observe(self._toggle_menu, names = ["value"])
         self.widgets.checks.navgui.observe(self._toggle_nav_gui, names=["value"])
-        self.widgets.checks.proxy.observe(self._toggle_proxy_buttons, names=["value"])
         self._update_theme(change = "aspect")  # Trigger Theme with aspect changed as well
         self.set_code_theme()  # Trigger CSS in it, must
         self.set_layout(center=True)  # Trigger this as well
         self._update_size(change=None)  # Trigger this as well
 
     def _close_quick_menu(self):
         "Need for actions on all buttons inside menu."
@@ -91,21 +90,14 @@
         return self._widgets  # To avoid breaking code by user
 
     def _toggle_nav_gui(self, change):
         if change["new"]:  # It's checked then hide
             self.show_nav_gui(True)
         else:
             self.show_nav_gui(False)
-
-    def _toggle_proxy_buttons(self, change):
-        if change["new"]:
-            self.widgets.mainbox.remove_class("PresentMode")  # Show if checked
-        else:
-            self.widgets.mainbox.add_class("PresentMode")
-
     
     def set_toggles(self,
         nav_gui = True,
         reflow_content = False, 
         notes = False, 
         notifications = True, 
         proxy_buttons = True,
@@ -257,17 +249,17 @@
         if text is None or text == "":
             self._footer_kws["text"] = ""  # assign to text
         elif text and isinstance(text, str):
             self._footer_kws["text"] = text  # assign to text
         else:
             raise TypeError(f"text should be string or None, not {type(text)}")
 
-        if self._slides.current:
+        if self._slides._current:
             self._get_footer(
-                self._slides.current, update_widget=True
+                self._slides._current, update_widget=True
             )  # Update footer immediately if slide there
         return self # for chaining set_methods
 
     def _get_footer(self, slide, update_widget=False):
         "Get footer text. `slide` is a slide object."
         if (type(slide).__name__ != "Slide") and (
             type(slide).__module__.split(".")[0] != "ipyslides"
@@ -307,21 +299,21 @@
         if not isinstance(aspect, (int,float)):
             raise TypeError("aspect should be int/float of ratio width/height.")
         self._layout = {'cwidth':width, 'scroll': scroll, 'centered': center, 'aspect': aspect, 'ncol_refs': ncol_refs}
         self._update_size(change = None) # will reset theme and send RESCALE message
         return self # for chaining set_methods
 
     def show_nav_gui(self, visible = True):
-        """Show/Hide navigation GUI, keyboard or touch still work. Hover on left-bottom corner to acess settings."""
+        """Show/Hide navigation GUI, keyboard still work. Hover on left-bottom corner to acess settings."""
         self.widgets.controls.layout.visibility = "visible" if visible else "hidden"
         self.widgets.checks.navgui.value = True if visible else False
         self.widgets.iw.msg_tojs = 'RESCALE' # sets padding etc
 
         if not visible:
-            self._slides.notify("Navigation controls hidden. But keyboard and touch gestures are working!")
+            self._slides.notify("Navigation controls hidden. But keyboard is still working!")
         
 
     def _update_size(self, change):
         self.widgets.mainbox.layout.height = "{}vw".format(
             int(self.width_slider.value / self._layout["aspect"])
         )
         self.widgets.mainbox.layout.width = "{}vw".format(self.width_slider.value)
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/slide.py` & `ipyslides-3.9.9/ipyslides/_base/slide.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Slide Object, should not be instantiated directly"""
 
 import sys, time
 from contextlib import contextmanager, suppress
-from ipywidgets import Layout, Button, HBox, VBox, Label
+from ipywidgets import Layout, Button, HBox
 
 from IPython.display import display
 from IPython.core.ultratb import FormattedTB
 
 
 from . import styles
-from ..utils import XTML, html, color, _format_css, _sub_doc, _css_docstring
+from ..utils import XTML, html, alert, _format_css, _sub_doc, _css_docstring
 from ..writer import _fmt_html
 from ..xmd import capture_content
 from .widgets import Output # not from ipywidget
 
 class _EmptyCaptured: outputs = [] # Just for initialization
 
 def _expand_objs(outputs, context):
@@ -149,43 +149,14 @@
         
         if slide._app.in_proxy:
             raise RuntimeError("Can't place proxy inside another proxy being captured.")
         
         self._slide = slide
         self._to_display = self
         self._text = text.strip() # Remove leading and trailing spaces
-        
-        if self._text.startswith('[') and self._text.endswith(']'):
-            self._text = self._text[1:-1]
-            btn1 = Button(description = 'Paste', layout = Layout(width='auto'))
-            btn2 = Button(description = 'Paste for Export Only', layout = Layout(width='auto'))
-            btns = VBox([Label(f'Paste Proxy: "{self._text}"'), HBox([btn1, btn2])], layout = Layout(width='auto',border='1px solid var(--accent-color)')).add_class('ProxyPasteBtns')
-            self._to_display = btns
-            
-            def on_click(btn):
-                try:
-                    im = self._slide._app.clipboard_image(f'attachment:{id(self)}.png', overwrite = True).to_html()
-                        
-                    with self.capture(): # capture if successful above, otherwise don't
-                        display(self._to_display) # keep buttons there to replace later, won't be displayed in export
-                        if btn is btn1: 
-                            im.display()
-                            btn1.description = 'Replace ?'
-                            btn2.description = 'Paste for Export Only'
-                        elif btn is btn2:
-                            html('div', [im], className='export-only',style = '').display()
-                            btn2.description =  'Pasted for Export Only: Replace ?'
-                            btn1.description = 'Paste'
-                            
-                except: 
-                    self._slide._app.notify('No supported image on clipboard to paste!')
-                    
-            btn1.on_click(on_click)
-            btn2.on_click(on_click)
-        
         self._outputs = []
         self._key = str(len(self._slide._proxies))
         self._slide._proxies[self._key] = self
         self._columns = {} 
         self._exportables = {}
         display(self._to_display, metadata= {'Proxy': self._key}) 
         
@@ -195,18 +166,18 @@
     @property
     def text(self): return self._text # Useful if user wants to filter proxies
     
     @property
     def slide(self): return self._slide # Useful if user wants to test if proxy is in slide
     
     def __repr__(self):
-        return f'Proxy(text = {self._text!r}, slide = {self._slide!r})'
+        return f'Proxy(text = {self._text!r}, slide_number = {self._slide.number}, proxy_index = {self._key})'
     
     def _repr_html_(self): # This is called when displayed
-        return color(f'Proxy(text = {self._text!r}, slide = {self._slide!r})',fg='var(--accent-color)').value
+        return alert(repr(self)).value
     
     @property
     def outputs(self):
         "Returns the outputs of the proxy, if it has been replaced."
         if self._outputs:
             return self._outputs 
         with capture_content() as captured:
@@ -218,15 +189,15 @@
         for out in self.outputs:
             content += _fmt_html(out)
         return content
     
     @contextmanager
     def capture(self):
         "Context manager to capture output to current prpxy. Use it like this: with proxy.capture(): ... after a slide is already created."
-        if self._slide._app.running:
+        if self._slide._app.this:
             raise RuntimeError("Can't use Proxy.capture() contextmanager inside a slide constructor.")
         
         self._columns = {} # Reset columns
         self._exportables = {} # Reset exportables
         self._slide._app._in_proxy = self # Used to get print statements to work in order and coulm aware
         try:
             with capture_content() as captured:
@@ -518,15 +489,15 @@
     def set_css(self,props : dict):
         """Attributes at the root level of the dictionary will be applied to the slide. You can add CSS classes by `Slide.set_dom_classes`.
         use `ipyslides.Slides.settings.set_css` to set CSS for all slides at once.
         {css_docstring}"""
         self._css = _format_css(props, allow_root_attrs = True)
         
         # See effect of changes
-        if not self._app.running: # Otherwise it has side effects
+        if not self._app.this: # Otherwise it has side effects
             if self._app._slidelabel != self.label:
                 self._app._slidelabel = self.label # Go there to see effects
             else:
                 self._app._update_tmp_output(self.animation, self._css)
 
     def set_dom_classes(self, add=None, remove=None):
         "Sett CSS classes on this slide separated by space. classes are remove first and add after it."
@@ -580,15 +551,15 @@
     def set_animation(self, name):
         "Set animation of this slide. Provide None if need to stop animation."
         if name is None:
             self._animation = html('style', '')
         elif isinstance(name,str) and name in styles.animations:
             self._animation = html('style',self._instance_animation(name))
             # See effect of changes
-            if not self._app.running: # Otherwise it has side effects
+            if not self._app.this: # Otherwise it has side effects
                 if self._app._slidelabel != self.label:
                     self._app._slidelabel = self.label # Go there to see effects
                 else:
                     self._app._update_tmp_output(self._animation, self.css)
         else:
             self._animation = None # It should be None, not '' or don't throw error here
```

### Comparing `ipyslides-3.9.7/ipyslides/_base/styles.py` & `ipyslides-3.9.9/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/_base/widgets.py` & `ipyslides-3.9.9/ipyslides/_base/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     menu    = ipw.ToggleButton(icon='plus',value = False, tooltip ='Toggle Quick Menu').add_class('Menu-Btn').add_class('Menu-Item')        
 
 @dataclass(frozen=True)
 class _Htmls:
     """
     Instantiate under `Widgets` class only.
     """
-    footer  = HTML('<p>Put Your Info Here using `slides.settings.set_footer` function</p>',layout=Layout(margin='0')).add_class('Footer') # Zero margin is important
+    footer  = HTML('Add short info here using `slides.settings.set_footer` function',layout=Layout(margin='0')).add_class('Footer') # Zero margin is important
     theme   = HTML(html('style',styles.style_css(styles.theme_colors['Inherit'])).value)
     main    = HTML(html('style',_layout_css.layout_css(styles.theme_colors['Inherit']['accent_color'], 16/9)).value) # Will be update in theme as well
     window  = HTML(html('style','').value) # Should be separate CSS, need class to handle disconnect options
     loading = HTML(layout=Layout(display='none')).add_class('Loading') #SVG Animation in it
     logo    = HtmlWidget('').add_class('LogoHtml')
     toast   = HtmlWidget('').add_class('Toast') # For notifications
     cursor  = HtmlWidget('').add_class('LaserPointer') # For beautiful cursor
@@ -103,15 +103,14 @@
     """
     Instantiate under `Widgets` class only.
     """
     reflow  = ipw.Checkbox(value=False,description='Reflow Content',layout=auto_layout)
     notes   = ipw.Checkbox(value=False,description='Notes',layout=auto_layout) # do not observe, just keep track when slides work
     toast   = ipw.Checkbox(value = True, description='Notifications',layout=auto_layout)
     focus   = ipw.Checkbox(value = True, description='Auto Focus',layout=auto_layout)
-    proxy   = ipw.Checkbox(value = True, description='Proxy Buttons',layout=auto_layout)
     navgui  = ipw.Checkbox(value = True, description='Show Nav. GUI',layout=auto_layout)
 
 @dataclass(frozen=True)
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
@@ -192,15 +191,15 @@
             VBox([
                 HTML('<b>Layout and Theme</b>',layout = _html_layout),
                 self.sliders.fontsize,
                 self.sliders.width,
                 self.ddowns.theme,
                 HTML('<b>Additional Features</b>',layout = _html_layout),
                 self.checks.notes,self.checks.toast,self.checks.reflow,
-                self.checks.proxy,self.checks.navgui,self.checks.focus,
+                self.checks.navgui,self.checks.focus,
                 HTML('<b>HTML File Export</b>',layout = _html_layout),
                 self.buttons.export,
                 HTML(html('details',[html('summary','<b>Screenshot Export</b>'), how_to_print]).value,layout = _html_layout),
                 self.ddowns.clear,
                 self.buttons.cap_all,
                 self.buttons.crop,
                 self.buttons.pdf,
```

### Comparing `ipyslides-3.9.7/ipyslides/_demo.py` & `ipyslides-3.9.9/ipyslides/_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             fig, ax = plt.subplots()
             x = np.linspace(0,obj+1,50+10*(idx+1))
             ax.plot(x,np.sin(x));
             ax.set_title(f'$f(x)=\sin(x)$, 0 < x < {idx+1}')
             ax.set_axis_off()
             slides.notes.insert(f'## This is under @frames decorator!')
 
-        slides.write([f'### This is Slide {slides.running.number}.{idx}\n and we are animating matplotlib',
+        slides.write([f'### This is Slide {slides.this.number}.{idx}\n and we are animating matplotlib',
                       s.show_lines([idx]),
                       'cite`This` refs`1`'
                       ],ax,widths=[40,60])
         if idx == 0: #Only show source code of first frame
             s.show_lines([5]).display()
 
     slides.next_from_markdown('section`Controlling Content on Frames` toc`### Contents`')
@@ -198,15 +198,15 @@
     @slides.next_frames(*boxes, repeat=False)
     def f(idx, obj):
         slides.write('# Frames with \n#### `repeat = False`')
         slides.write(obj)
 
     @slides.next_frames(*boxes, repeat=True)
     def f(idx, obj):
-        slides.running.set_animation(None) #Disable animation for showing bullets list
+        slides.this.set_animation(None) #Disable animation for showing bullets list
         slides.write('# Frames with \n#### `repeat = True` and Fancy Bullet List')
         slides.bullets(obj, marker='💘').display()
 
     @slides.next_frames(*boxes, repeat=[(0,1),(2,3)])
     def f(idx, obj):
         slides.write('# Frames with \n#### `repeat = [(0,1),(2,3)]`')
         slides.write(*obj)
@@ -244,16 +244,16 @@
                 |r1 |r2 |r3 |
                 ''',
             ], 
             [
                 '### Widgets',
                 slides.alt(ipw.IntSlider(),lambda w: f'<input type="range" min="{w.min}" max="{w.max}" value="{w.value}">'), # alt only works with widgets, but below display tricks works with any object
                 lambda: display(ipw.Button(description='Click to do nothing'),metadata = {'text/html': '<button>Click to do nothing</button>'}), # This is a hack to display button as html in exported slides
-                ipw.Checkbox(description='Select to do nothing',indent=False), # screenshot of this will be pasted in proxy below to export html
-                'proxy`[Paste Checkbox Screenshot Here]`'
+                ipw.Checkbox(description='Select to do nothing',indent=False), 
+                'proxy`Paste Checkbox Screenshot Here with Slides.clip_image function`'
             ]
         )
         s.get_source().display(True)
 
     slides.next_from_markdown(slides.fmt('''
     %++
     ## $ \LaTeX $ in Slides
```

### Comparing `ipyslides-3.9.7/ipyslides/core.py` & `ipyslides-3.9.9/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
             )
 
         self._cite_mode = 'footnote'
 
         self._slides_dict = (
             {}
         )  # Initialize slide dictionary, updated by user or by _setup.
-        self._reverse_mapping = {"0": "0"}  # display number -> input number of slide
         self._iterable = []  # self._collect_slides() # Collect internally
         self._nslides = 0  # Real number of slides
         self._max_index = 0  # Maximum index including frames
         self._running_slide = (
             None  # For Notes, citations etc in markdown, controlled in Slide class
         )
         self._next_number = (
@@ -139,15 +138,15 @@
     def _set_running(self, slide):
         "Context manager to set running slide and turns back to previous."
         if slide and not isinstance(
             slide, Slide
         ):  # None is acceptable to hold running slide in other function
             raise TypeError(f"slide must be None or Slide, got {type(slide)}")
 
-        old = self.running
+        old = self.this
         self._running_slide = slide
         try:
             yield
         finally:
             self._running_slide = old
 
     @contextmanager
@@ -156,15 +155,15 @@
         with self._set_running(None):
             yield
 
     def run_cell(self, cell, **kwargs):
         """Run cell and return result. Use this instead of IPython's run_cell for extra controls."""
         self._unregister_postrun_cell() # important to avoid putting contnet on slides
         output = self.shell.run_cell(cell, **kwargs)
-        if self.running: # there was post_run_cell under building slides
+        if self.this: # there was post_run_cell under building slides
             self._register_postrun_cell() # should be back
         return output
     
     def _post_run_cell(self, result):
         self._unregister_postrun_cell() # it will be initialized from next building slides
         if result.error_before_exec or result.error_in_exec:
             return  # Do not display if there is an error
@@ -186,16 +185,16 @@
             self.shell.events.unregister("post_run_cell", self._post_run_cell)
     
     def _register_postrun_cell(self):
         with suppress(Exception): 
             self.shell.events.register("post_run_cell", self._post_run_cell)
         
     def _jump_to_source_cell(self, btn):
-        if hasattr(self.current, '_scroll_btn'):
-            self.current._scroll_btn.focus()
+        if hasattr(self._current, '_scroll_btn'):
+            self._current._scroll_btn.focus()
         else:
             self.notify('No source cell found!')
 
     def _setup(self):
         # Only in Jupyter Notebook
         if self.shell and self.shell.__class__.__name__ != "TerminalInteractiveShell":
             if self._max_index == 0:  # prevent overwrite
@@ -212,35 +211,37 @@
     def __iter__(self):  # This is must have for exporting
         return iter(self._iterable)
 
     def __len__(self):
         return len(self._iterable)
 
     def __getitem__(self, key):
-        "Get slide by index or key(written on slide's bottom)."
+        "Get slide by index or slice. Use Slides.get func to access slides by number they were created with."
         if isinstance(key, int):
             return self._iterable[key]
-        elif isinstance(key, str):
-            frame = None
-            if "." in key:
-                key, frame = key.split(".")
-
-            if key in self._reverse_mapping:
-                _slide = self._slides_dict[self._reverse_mapping[key]]
-                if frame:
-                    _slide = _slide.frames[int(frame) - 1]
-                return _slide
-            else:
-                raise KeyError(f"Key {key} not found.")
         elif isinstance(key, slice):
             return self._iterable[key.start : key.stop : key.step]
 
         raise KeyError(
-            "Slide could be accessed by index, slice or key, got {}".format(key)
+            f"A slide could be accessed by index or slice, got {type(key)},\n"
+            "Use `Slides.get` function to access slides by number they were created with."
         )
+    
+    def get(self, slide_number):
+        "Access a slide by given slide number. Use this instead of indexing if adding extra content to a slide such as CSS."
+        if isinstance(slide_number,int):
+            key = str(slide_number)
+            if key in self._slides_dict:
+                return self._slides_dict[key]
+            else:
+                raise KeyError(f"Slide with number {slide_number} was never created or may be deleted!")
+        else:
+            raise TypeError(f"slide_number should be interger by which slide was created, got {type(slide_number)}")
+    
+    __call__ = get  # like paranthesis indexing
 
     def __del__(self):
         for k, v in globals():
             if isinstance(v, Slides):
                 del globals()[k]
 
         for k, v in locals():
@@ -266,21 +267,20 @@
         return utils.get_child_dir('.ipyslides-assets', create = True)
     
     @property
     def cite_mode(self):
         return self._cite_mode
 
     @property
-    def current(self):
-        "Access current visible slide and use operations like set_css etc."
+    def _current(self):
         return self._iterable[self._slideindex]
 
     @property
-    def running(self):
-        "Access slide currently being built. Useful inside frames decorator."
+    def this(self):
+        "Access slide currently being built. Useful for operations like set_css etc."
         return self._running_slide
 
     @property
     def in_proxy(self):
         "Check if proxy is capturing output."
         return getattr(self, "_in_proxy", None)
 
@@ -292,15 +292,15 @@
     @property
     def draw_button(self):
         "Get a button to reveal drawing board easily from slide. Like it lets you remeber to draw now."
         return self.widgets.toggles.draw
 
     def verify_running(self, error_msg=""):
         "Verify if slide is being built, otherwise raise error."
-        if self.running is None:
+        if self.this is None:
             raise RuntimeError(
                 error_msg or "This operation is only allowed under slide constructor."
             )
 
     def _add_clean_title(self):
         with suppress(BaseException):  # need to avoid any errors
             with _build_slide(self, "0") as s:
@@ -323,21 +323,16 @@
 
         self._unregister_postrun_cell() # no need in initialization functions 
         self.refresh()  # cleans up initialization setup and tocs/other things
 
     def clear(self):
         "Clear all slides. This will also clear resources including citations, sections."
         self._slides_dict = {}  # Clear slides
-        _ = [
-            self.__dict__.pop(s, None) for s in getattr(self, "_links_dict", {})
-        ]  # clear slides attributes
         self.set_citations({})  # Clears citations from disk too
-        self._next_number = (
-            0  # Reset slide number to 0, because user will overwrite title page.
-        )
+        self._next_number = 0  # Reset slide number to 0, because user will overwrite title page.
         self._add_clean_title()  # Add clean title page without messing with resources.
 
     def _cite(self, keys):
         self.verify_running("Citations can be added only inside a slide constructor!")
         citeds = [self._cite_key(key.strip()) for key in keys.split(',')] # avoid whitespaces around key
 
         if self.cite_mode == "inline":
@@ -345,20 +340,20 @@
         
         return '<sup>,</sup>'.join(citeds) 
 
     def _cite_key(self, key):
         """Use markdown syntax cite`key` to add citations since output has to be inline. 
         Citations corresponding to keys used can be added by ` Slides.set_citations ` method.
         """
-        cited = _Citation(slide=self.running, key=key)
+        cited = _Citation(slide=self.this, key=key)
 
         if self.cite_mode == "inline":
             return cited.inline_value  # Just write here
         else: # Set _id for citation in footnote mode
-            cited._id = list(self.running._citations.keys()).index(key) + 1 # Get index of key from unsorted ones
+            cited._id = list(self.this._citations.keys()).index(key) + 1 # Get index of key from unsorted ones
 
         # Return string otherwise will be on different place, avoid newline here
         return f'<a href="#{key}" class="citelink"><sup id ="{key}-back" style="color:var(--accent-color) !important;">{cited._id}</sup></a>'
     
     def _set_ctns(self, d):
         # Here other formatting does not work for citations
         new_citations = {k: self.parse(v, returns = True) for k, v in d.items()}
@@ -424,42 +419,42 @@
 
     def section(self, text):
         """Add section key to presentation that will appear in table of contents. In markdown, use section`content` syntax.
         Sections can be written as table of contents.
         """
         self.verify_running("Sections can be added only inside a slide constructor!")
 
-        self.running._section = text  # assign before updating toc
+        self.this._section = text  # assign before updating toc
         
         for s in self[:]:
             if (
-                getattr(s, "_toced", False) and s != self.running
+                getattr(s, "_toced", False) and s != self.this
             ):  # self will be built of course at end
                 s.update_display(go_there=False)
  
     def toc(self, title='## Contents {.align-left}', extra = None):
         "You can also use markdown syntax to add it like toc`title` or ```toc title\n extra\n```. Extra is passed to write command in right column."
         def fmt_sec(s, _class):
             return XTML(f'''<li class="toc-item {_class}">
                 <a href="#{s._sec_id}" class="export-only">{s._section}</a>
                 <span class="jupyter-only">{s._section}</span></li>''')
 
         def toc_handler():
             sections = []
             this_index = (
-                self[:].index(self.running)
-                if self.running in self[:]
-                else self.running.number
+                self[:].index(self.this)
+                if self.this in self[:]
+                else self.this.number
             )  # Monkey patching index, would work on next run
             for slide in self[:this_index]:
                 if slide._section:
                     sections.append(fmt_sec(slide,"prev"))
 
-            if self.running._section:
-                sections.append(fmt_sec(self.running,"this"))
+            if self.this._section:
+                sections.append(fmt_sec(self.this,"this"))
             elif sections:
                 sections[-1] = XTML(
                     sections[-1].value.replace("toc-item prev", "toc-item this")
                 )
 
             for slide in self[this_index + 1 :]:
                 if slide._section:
@@ -554,19 +549,19 @@
         "Set current slide label"
         with suppress(BaseException):  # May not be ready yet
             self.progress_slider.label = value
 
     @property
     def _sectionindex(self):
         "Get current section index"
-        if self.current._section:
-            return self.current.index
+        if self._current._section:
+            return self._current.index
         else:
             idxs = [
-                s.index for s in self[: self.current.index] if s._section
+                s.index for s in self[: self._current.index] if s._section
             ]  # Get all section indexes before current slide
             return idxs[-1] if idxs else 0  # Get last section index
 
     def _switch_slide(self, old_index, new_index):  
         uclass = f".{self.uid} .TOC"
         _objs = [
             self._iterable[new_index].css,
@@ -607,25 +602,22 @@
                 "InView-Last"
             ).add_class("InView-Other")
 
         if self._iterable and change:
             self.notes.display()  # Display notes first
             self.notify('x') # clear notification
             self._switch_slide(old_index=change["old"], new_index=change["new"])
-            self.current.run_on_load()  # Run on_load setup after switching slide, it updates footer as well
+            self._current.run_on_load()  # Run on_load setup after switching slide, it updates footer as well
 
     def refresh(self):
         "Auto Refresh whenever you create new slide or you can force refresh it"
         self._iterable = self._collect_slides()  # would be at least one title slide
         if not self._iterable:
             self.progress_slider.options = [("0", 0)]  # Clear options
             self.widgets.slidebox.children = []  # Clear older slides
-            _ = [
-                self.__dict__.pop(s, None) for s in getattr(self, "_links_dict", {})
-            ]  # clear slides attributes
             return None
 
         n_last = float(self._iterable[-1].label)
         self._nslides = int(n_last)  # Avoid frames number
         self._max_index = len(self._iterable) - 1  # This includes all frames
 
         # Now update progress bar
@@ -638,48 +630,32 @@
         self.widgets.slidebox.children = [it._widget for it in self._iterable]
         for i, s in enumerate(self._iterable):
             s._index = i  # Update index
 
         self._update_dynamic_content(None)  # Update dynamic content including widgets
         self._update_toc()  # Update table of content if any
 
-        # This is useful for readily available objects with slides instead of indexing.
-        old_links = getattr(self, "_links_dict", {})
-        _ = [self.__dict__.pop(s, None) for s in old_links]  # Remove old links
-        self._links_dict = {
-            f"s{item.label}".replace(".", "_"): item
-            for item in self._iterable
-            if item.label
-        }
-        self.__dict__.update(self._links_dict)  # Add new links
-
         if not any(['ShowSlide' in c._dom_classes for c in self.widgets.slidebox.children]):
             self.widgets.slidebox.children[0].add_class('ShowSlide')
 
         self.widgets.iw.msg_tojs = 'SwitchView' # Trigger view
 
     def proxy(self, text):
-        """Place a proxy placeholder in your slide and returns it's `handle`. This is useful when you want to update the placeholder later.
-        Use `Slides.proxies[index].capture` or `handle.capture` contextmanager to update the placeholder.
-        ::: note-tip
-            - Use square brackets around text like `proxy('[Button Text]')` to create a button that can paste image from clipboard. This is useful to export screenshots of widgets in a given state.
-            - Show/hide the proxy buttons by a checkbox `Proxy Buttons` in settings panel once you are done with pasting and ready to export/present.
+        """Place a proxy placeholder in your slide and return it's `handle`. This is useful when you want to update the placeholder later.
+        Use `Slides.capture_proxy(slide_number, proxy_index)` or `handle.capture` contextmanager to update the placeholder.
+        Use this in markdown as well by proxy `text` syntax.
         """
         self.verify_running(
             "proxy placeholder can only be used in a slide constructor!"
         )
-        return self.running._proxy_private(text)
-
-    @property
-    def proxies(self):
-        "Returns all placeholder proxies accross all slides."
-        _phs = []
-        for s in self._iterable:
-            _phs.extend(s.proxies)
-        return tuple(_phs)
+        return self.this._proxy_private(text)
+    
+    def capture_proxy(self, slide_number, proxy_index):
+        "This is a shortcut for `Slides.get(slide_number).proxies[proxy_index].capture()`."
+        return self.get(slide_number).proxies[proxy_index].capture()
 
     # defining magics and context managers
     def _slide(self, line, cell):
         """Capture content of a cell as `slide`.
             ---------------- Cell ----------------
             %%slide 1
             #python code here
@@ -723,18 +699,18 @@
             if len(frames) > 1 and repeat:
                 frames = ["\n".join([frames[0], *frames[1:i]]) for i in range(2, len(frames) + 1)]
             
             self._editing_index = None
             
             @self.frames(int(slide_number_str), *frames, repeat=False) # here repeat handled above
             def make_slide(idx, frm):
-                if (self.running.markdown != frm) or (idx == 0):
-                    self._editing_index = self.running.index # Go to latest editing markdown frame, or start of frames
+                if (self.this.markdown != frm) or (idx == 0):
+                    self._editing_index = self.this.index # Go to latest editing markdown frame, or start of frames
 
-                self.running.set_source(frm, "markdown")  # Update source beofore parsing content to make it available to user inside markdown too
+                self.this.set_source(frm, "markdown")  # Update source beofore parsing content to make it available to user inside markdown too
                 parse(xtr.copy_ns(cell, frm), returns = False)
             
             if self._editing_index is not None:
                 self.navigate_to(self._editing_index)
             
             delattr(self, '_editing_index')
 
@@ -845,15 +821,15 @@
         ```
 
         **Parameters**
 
         - slide_number: (int) slide number to insert frames on.
         - objs: expanded by * (list, tuple) of objects to write on frames. If repeat is False, only one frame is generated for each obj.
         - repeat: (bool, list, tuple) If False, only one frame is generated for each obj.
-            If True, one frame are generated in sequence of ojects linke `[a,b,c]` will generate 3 frames with [a], [a,b], [a,b,c] to given in function and will be written top to bottom.
+            If True, one frame are generated in sequence of ojects like `[a,b,c]` will generate 3 frames with [a], [a,b], [a,b,c] to given in function and will be written top to bottom.
             If list or tuple, it will be used as the sequence of frames to generate and number of frames = len(repeat).
             [(0,1),(1,2)] will generate 2 frames with [a,b] and [b,c] to given in function and will be written top to bottom or the way you write in your function.
         
         No return of defined function required, if any, only should be display/show etc.
         
         ::: note-info
             Use this function with 'next_' prefix to enable auto numbeing of slides inside python file.
@@ -937,15 +913,14 @@
 
         nslide = 0  # start of slides - 1
         for i in range(1, _max_range):
             if i in val_keys:
                 nslide = nslide + 1  # should be added before slide
                 self._slides_dict[f"{i}"]._label = f"{nslide}"
                 slides_iterable.append(self._slides_dict[f"{i}"])
-                self._reverse_mapping[str(nslide)] = str(i)
 
                 # Read Frames
                 frames = self._slides_dict[f"{i}"].frames
                 for j, frame in enumerate(frames, start=1):
                     jj = f"{j}" if len(frames) < 10 else f"{j:02}"  # 99 frames max
                     frame._label = f"{nslide}.{jj}"  # Label for frames
                     slides_iterable.append(frame)
@@ -1030,18 +1005,15 @@
     
     def next_number(self):
         "Get next slide number if need inside a .py file, e.g. in slide magic or explicit numbering."
         if self.inside_jupyter_notebook(self.next_number): 
             raise Exception("'next_number' should be used inside a .py file only!")
         return self._next_number
 
-    def AutoSlides(self):
-        raise Exception("This function is deprecated. Use Slides."
-        "[next_number, next_slide, next_frames, next_from_markdown] in python file for automatic numbering")
-        
+
 # Make available as Singleton Slides
 _private_instance = Slides()  # Singleton in use namespace
 # This is overwritten below to just have a singleton
 
 
 class Slides:
     _version = (
```

### Comparing `ipyslides-3.9.7/ipyslides/formatters.py` & `ipyslides-3.9.9/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/ipyslides/source.py` & `ipyslides-3.9.9/ipyslides/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,20 +92,18 @@
 def _str2code(text,language='python',name=None,**kwargs):
     "Only reads plain text source code, return source object with `show_lines` and `focus_lines` methods."
     out = SourceCode(highlight(text,language = language, name = name, **kwargs).value)
     out.raw = text
     return out
 
 class Code:
-    current = None
     def __init__(self,*args,**kwargs):
         raise Exception("""This class is not meant to be instantiated.
         Use cls.context() to get a context manager for source.
-        Use cls.current to get the current source object.
-        Use cls.create(obj) to get a source code from text, file or callable. Or explicitly:
+        Use cls.cast(obj) to get a source code from text, file or callable. Or explicitly:
             - cls.from_file(filename) to get a source object from a file.
             - cls.from_string(string) to get a source object from a string.
             - cls.from_callable(callable) to get a source object from a callable.
         """)
     
     @classmethod
     def cast(cls, obj, language='python',name=None, **kwargs):
@@ -117,16 +115,15 @@
                 return cls.from_string(obj, language=language,name=name, **kwargs)
         else:
             return cls.from_callable(obj, **kwargs)
     
     @classmethod
     def from_string(cls,text,language='python',name=None,**kwargs):
         "Creates source object from string. `name` is alternate used name for language. `kwargs` are passed to `ipyslides.formatter.highlight`."
-        cls.current = _str2code(text,language=language,name=name,**kwargs)
-        return cls.current
+        return _str2code(text,language=language,name=name,**kwargs)
     
     @classmethod
     def from_file(cls, filename,language = None,name = None,**kwargs):
         """Returns source object with `show_lines` and `focus_lines` methods. `name` is alternate used name for language.  
         `kwargs` are passed to `ipyslides.formatter.highlight`.     
         
         It tries to auto detect lanaguage from filename extension, if `language` is not given.
@@ -138,39 +135,37 @@
             lexer = None
             with suppress(BaseException):
                 lexer = pygments.lexers.get_lexer_by_name(_lang)
                 
             if lexer is None:
                 raise Exception(f'Failed to detect language from file {filename!r}. Use language argument!')
             
-        cls.current = _file2code(filename,language = _lang,name = _title,**kwargs)
-        return cls.current
+        return _file2code(filename,language = _lang,name = _title,**kwargs)
     
     @classmethod       
     def from_callable(cls, callable,**kwargs):
         "Returns source object from a given callable [class,function,module,method etc.] with `show_lines` and `focus_lines` methods. `kwargs` are passed to `ipyslides.formatter.highlight`"
         for _type in ['class','function','module','method','builtin','generator']:
             if getattr(inspect,f'is{_type}')(callable):
                 source = inspect.getsource(callable)
-                cls.current = _str2code(source,language='python',name=None)
-                return cls.current
+                return _str2code(source,language='python',name=None)
             
         # If things above do not work, raise error
         raise TypeError(f"Object {callable} is not callable!")
     
     @classmethod
     @contextmanager 
     def context(cls, returns = False, **kwargs): 
         """Execute and displays source code in the context manager. `kwargs` are passed to `ipyslides.formatter.highlight` function.
         Useful when source is written inside context manager itself.
         If `returns` is False (by default), then source is displayed before the output of code. Otherwise you can assign the source to a variable and display it later anywhere.
         
         **Usage**:
         ```python
-        with source.context(returns = True) as s: #if not used as `s`, still it is stored `source.current` attribute.`
+        with source.context(returns = True) as s: 
             do_something()
             write(s) # or s.display(), write(s)
             
         #s.raw, s.value are accesible attributes.
         #s.focus_lines, s.show_lines are methods that are used to show selective lines.
         ```
         """ 
@@ -196,14 +191,13 @@
                 with_node = node
                 break
 
         n2 = with_node.body[-1].end_lineno #can include multiline expressions in python 3.8+
         source = textwrap.dedent(''.join(lines[n1:][:n2 - offset]))
         source_html = SourceCode(highlight(source,language = 'python', **kwargs).value)
         source_html.raw = source # raw source code
-        cls.current = source_html
         
         if not returns:
             source_html.display()
         
         yield source_html
```

### Comparing `ipyslides-3.9.7/ipyslides/utils.py` & `ipyslides-3.9.9/ipyslides/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
     """Displays PNG/JPEG files or image data etc, `kwrags` are passed to IPython.display.Image. 
     You can provide following to `data` parameter:
         
     - An opened PIL image. Useful for image operations and then direct writing to slides. 
     - A file path to image file.
     - A url to image file.
     - A str/bytes object containing image data.  
-    - A str like "clip:image.png" will load an image saved using `Slides.clipboard_image('image.png')`. 
+    - A str like "clip:image.png" will load an image saved using `Slides.clip_image('image.png')`. 
 
     If `as_figure = False` caption is not used.
     """
     if isinstance(width,int):
         width = f'{width}px'
     
     if isinstance(data, str) and data.startswith("clip:"):
@@ -521,15 +521,15 @@
     wr = Writer(*objs,widths = widths) # Displayed
     wr._box.add_class('block' + (f'-{suffix}' if suffix else '')) # Add class to box
     if make_grid:
         wr._box.layout.display = 'grid' # Make it grid
         wr._box.layout.grid_gap = '1em 0px' # Remove extra gap in columns, but keep row gap
         wr._extra_style = 'style="display:grid;grid-gap:1em 0px;"' # Add extra style to box for export html to use
         
-    if not any([(wr._slides and wr._slides.running), wr._in_proxy]):
+    if not any([(wr._slides and wr._slides.this), wr._in_proxy]):
         return wr.update_display() # Update in usual cell to have widgets working
     
 def block(*objs, widths = None): 
     """
     Format a block like in LATEX beamer with `objs` in columns and immediately display it. Format rows by given an obj as list of objects.   
     ::: block
         - Block is automatically displayed and returns nothing.
```

### Comparing `ipyslides-3.9.7/ipyslides/writer.py` & `ipyslides-3.9.9/ipyslides/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,26 @@
             className='goto-button export-only'
         )
     
         display(self._button, metadata = {'DOMWidget': '---'})
         display(alt_link) # Hidden from slides
         
     def set_target(self, force = False):
-        if not self._app.running:
+        "Set target slide of goto button. Returns itself."
+        if not self._app.this:
             raise RuntimeError("GotoButton's target can be set only inside a slide constructor!")
         if self._button._TargetSlide and not force:
             raise RuntimeError("GotoButton's target can be set only once! Use `force=True` to link here and remove previous link.")
         
         if force:
             self._button._TargetSlide._target_id = None # Remove previous link
         
-        self._button._TargetSlide = self._app.running
+        self._button._TargetSlide = self._app.this
         self._button._TargetSlide._target_id = self._target_id # Set new link
+        return self 
     
 class AltForWidget(CustomDisplay):
     def __init__(self, widget, func):
         if not isinstance(widget, ipw.DOMWidget):
             raise TypeError(f'widget should be a widget, got {widget!r}')
         if not callable(func):
             raise TypeError(f'func should be a callable, got {func!r}')
@@ -75,15 +77,15 @@
         return 'AltForWidget(widget, func)'
         
     def _ipython_display_(self):
         return self.display()
         
     def display(self):
         slides = get_slides_instance()
-        if slides and (context := (slides.in_proxy or slides.running)):
+        if slides and (context := (slides.in_proxy or slides.this)):
             display(context._exp4widget(self._widget, self._func))
         else:
             display(self._widget, metadata = {'DOMWidget': '---'}) # Display widget under slides/notebook anywhere
         
 def _fmt_html(output):
     "Format captured rich output and others to html if possible. Used in other modules too."
     if hasattr(output, 'fmt_html'): # Columns
@@ -109,15 +111,15 @@
         
         try:
             self.__class__._in_write = True # To prevent write from being called inside write, specially by lambda function
             self._cols = self._capture_objs(*objs, widths = widths) # run after getting slides instance
         finally:
             self.__class__._in_write = False
             
-        self._slide = self._slides.running if self._slides else None
+        self._slide = self._slides.this if self._slides else None
         self._in_proxy = getattr(self._slides, '_in_proxy', None) # slide itself can be Non, so get via getattr
         self._in_dproxy = getattr(self._slides, '_in_dproxy', None)
         self._context = (self._in_dproxy if self._in_dproxy else self._slide) or self._in_proxy # order strictly matters
         
         if len(objs) == 1:
             display(*self._cols[0]['outputs']) # If only one column, display it directly
         else:
@@ -150,15 +152,15 @@
                     if isinstance(c,str):
                         parse(c, returns = False)
                     elif isinstance(c, CustomDisplay):
                         c.display() # Handles all custom display classes like alt, goto_button etc.
                     elif callable(c) and c.__name__ == '<lambda>':
                         _ = c() # If c is a lambda function, call it and it will dispatch whatever is inside, ignore output
                     elif isinstance(c, ipw.DOMWidget): # Should be a displayable widget, not just Widget
-                        if self._slides and self._slides.running:
+                        if self._slides and self._slides.this:
                             if (func := serializer.get_func(c)):
                                 self._slides.alt(c, func).display() # Alternative representation will be available on export, specially for ipw.HTML
                             else:
                                 display(c, metadata = {'DOMWidget': '---'}) # Display only widget
                         else:
                             display(c, metadata = {'DOMWidget': '---'}) # Display only widget outside slide buuilder
                     else:
@@ -244,15 +246,15 @@
         - `write` is a robust command that can handle most of the cases. If nothing works, `repr(obj)` will be displayed.
         - You can avoid `repr(obj)` by `lambda: func()` e.g. `lambda: plt.show()`.
         - You can use `display(obj, metadata = {'text/html': 'html repr by user'})` for any object to display object as it is and export its HTML representation in metadata.
         - A single string passed to `write` is equivalent to `parse` command.
         - You can add mini columns inside a column by markdown syntax or `Slides.cols`, but content type is limited in that case.
     """
     wr = Writer(*objs,widths = widths)
-    if not any([(wr._slides and wr._slides.running), wr._in_proxy, len(objs) == 1]):
+    if not any([(wr._slides and wr._slides.this), wr._in_proxy, len(objs) == 1]):
         return wr.update_display() # Update in usual cell to have widgets working, but not single object which displays outside of box
 
 # Patch for interact/interactive patching to show in output
 
 def _interact_ipython_display(self):
     def fmt_output_html(w):
         return serializer.get_func(w.out)(w.out)
```

### Comparing `ipyslides-3.9.7/ipyslides/xmd.py` & `ipyslides-3.9.9/ipyslides/xmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,16 @@
             f"pr = slide_instance.proxy({match!r})", instance_name="slide_instance"
         )  # assign to avoid __repr__ output in markdown
         text_chunk = text_chunk.replace(f"proxy`{match}`", block, 1)
     
     # Footnotes at place user likes
     all_matches = re.findall(r"refs\`([\d+]?)\`", text_chunk) # match digit or empty
     for match in all_matches:
-        slide_instance.running._refs_consumed = True
-        _cits = ''.join(v.value for v in sorted(slide_instance.running._citations.values(), key=lambda x: x._id))
+        slide_instance.this._refs_consumed = True
+        _cits = ''.join(v.value for v in sorted(slide_instance.this._citations.values(), key=lambda x: x._id))
         out = f"<div class='Citations' style='column-count: {match} !important;'>{_cits}</div>"
         text_chunk = text_chunk.replace(f"refs`{match}`", out, 1)
 
     return text_chunk
 
 class HtmlFormatter(string.Formatter):
     def format_field(self, value, format_spec):
@@ -357,15 +357,15 @@
             xmd 
         )  # Remove leading spaces from each line, better for writing under indented blocks
         xmd = re.sub("\\\`", "&#96;", xmd)  # Escape backticks
         xmd = self._resolve_nested(
             xmd
         )  # Resolve nested objects in form func`?text?` to func`html_repr`
 
-        if self._slides and self._slides.running:
+        if self._slides and self._slides.this: # under building slide
             xmd = resolve_objs_on_slide(
                 self._slides, xmd
             )  # Resolve objects in xmd related to current slide
 
 
         # After resolve_objs_on_slide, xmd can have code blocks which may not be passed from suitable context
         if (r"\n```python run" in xmd) and self._returns: # Do not match nested blocks, r"" is important
```

### Comparing `ipyslides-3.9.7/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.9.9/ipyslides.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.9.7
+Version: 3.9.9
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
@@ -32,15 +32,14 @@
 </svg>
 
 # IPySlides
 
 Create interactive slides programatically in [Jupyter](https://jupyter.org/)/[Voila](https://voila.readthedocs.io/en/stable/) with all kind of rich content. 
 
 - Launch Example Notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/massgh/ipyslides/HEAD?labpath=demo.ipynb)
-- See a [Demo Notebook](https://www.kaggle.com/massgh/ipyslides) at [Kaggle](https://www.kaggle.com/massgh)
 - Watch a [Youtube Video](https://www.youtube.com/watch?v=thgLGl14-tg)
 - See [PDF-Slides](Slides.pdf)
 ![Overview](slide.png)
 
 ---
 # Changelog
 You can see upto date documentation via `ipyslides.Slides().docs()`, so no additional changelog is created.
@@ -99,15 +98,15 @@
 ---
 # Speaker Notes
 - You can turn on speaker notes with a `Show Notes` check in setting panel. See module `Slides.notes` for details or see examples in `Slides.demo()`. 
 
 > Notes is an experimantal feature, so use at your own risk. Avoid if you can.
 
 ---
-# Known Limitations
+# Caveats!
 - Since Markdown is parsed using python (and we do not run notebook from outside e.g. with nbconvert), markdown cells are of no use. A better alternative is linking a markodwn file using `Slides.sync_with_file` and slides auto update when you save your edits. You can still write markdown in code cell with slide magic `%%slide number -m` to add to slides. 
 - Slide number is necessary to be tracked by user in notebook, because cells are not linked to each other and multiple runs of a cell can lead to adding many slides with same content. Inside python scripts that run in linear fashion, you can use `Slides.[next_number,next_slide,next_frames,next_from_markdown]`.
 - Bounding box of slides for screenshots should be set by user (if not in fullscreen).
 
 ---
 
 # Acknowledgements
```

### Comparing `ipyslides-3.9.7/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.9.9/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.9.7/setup.py` & `ipyslides-3.9.9/setup.py`

 * *Files identical despite different names*

