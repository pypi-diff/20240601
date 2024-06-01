# Comparing `tmp/posuto-2024.4.0.tar.gz` & `tmp/posuto-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posuto-2024.4.0.tar", last modified: Sun Mar 31 07:27:42 2024, max compression
+gzip compressed data, was "posuto-2024.5.0.tar", last modified: Wed May  1 09:26:20 2024, max compression
```

## Comparing `posuto-2024.4.0.tar` & `posuto-2024.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.544276 posuto-2024.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.432277 posuto-2024.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 07:27:12.000000 posuto-2024.4.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.432277 posuto-2024.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-31 07:27:12.000000 posuto-2024.4.0/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-31 07:27:12.000000 posuto-2024.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-31 07:27:12.000000 posuto-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-31 07:27:12.000000 posuto-2024.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-31 07:27:12.000000 posuto-2024.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-31 07:27:42.544276 posuto-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-03-31 07:27:12.000000 posuto-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.432277 posuto-2024.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-31 07:27:12.000000 posuto-2024.4.0/examples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)   295014 2024-03-31 07:27:12.000000 posuto-2024.4.0/postcharacter.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.544276 posuto-2024.4.0/posuto/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-31 07:27:12.000000 posuto-2024.4.0/posuto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127) 13054406 2024-03-31 07:27:29.000000 posuto-2024.4.0/posuto/officedata.json
--rw-r--r--   0 runner    (1001) docker     (127) 83853312 2024-03-31 07:27:29.000000 posuto-2024.4.0/posuto/postaldata.db
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-31 07:27:12.000000 posuto-2024.4.0/posuto/posuto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-03-31 07:27:12.000000 posuto-2024.4.0/posuto/prep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.544276 posuto-2024.4.0/posuto/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-31 07:27:12.000000 posuto-2024.4.0/posuto/tests/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:27:42.544276 posuto-2024.4.0/posuto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-31 07:27:42.000000 posuto-2024.4.0/posuto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-31 07:27:42.000000 posuto-2024.4.0/posuto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 07:27:42.000000 posuto-2024.4.0/posuto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 07:27:42.000000 posuto-2024.4.0/posuto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-31 07:27:12.000000 posuto-2024.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-31 07:27:42.544276 posuto-2024.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 07:27:12.000000 posuto-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.463960 posuto-2024.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.347961 posuto-2024.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 09:25:46.000000 posuto-2024.5.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.347961 posuto-2024.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-01 09:25:46.000000 posuto-2024.5.0/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-01 09:25:46.000000 posuto-2024.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 09:25:46.000000 posuto-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-01 09:25:46.000000 posuto-2024.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-01 09:25:46.000000 posuto-2024.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-01 09:26:20.463960 posuto-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-01 09:25:46.000000 posuto-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.347961 posuto-2024.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 09:25:46.000000 posuto-2024.5.0/examples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295014 2024-05-01 09:25:46.000000 posuto-2024.5.0/postcharacter.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.463960 posuto-2024.5.0/posuto/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 09:25:46.000000 posuto-2024.5.0/posuto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 13053678 2024-05-01 09:26:05.000000 posuto-2024.5.0/posuto/officedata.json
+-rw-r--r--   0 runner    (1001) docker     (127) 83857408 2024-05-01 09:26:05.000000 posuto-2024.5.0/posuto/postaldata.db
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-01 09:25:46.000000 posuto-2024.5.0/posuto/posuto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-05-01 09:25:46.000000 posuto-2024.5.0/posuto/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.463960 posuto-2024.5.0/posuto/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-01 09:25:46.000000 posuto-2024.5.0/posuto/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:26:20.463960 posuto-2024.5.0/posuto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-01 09:26:20.000000 posuto-2024.5.0/posuto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 09:26:20.000000 posuto-2024.5.0/posuto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:26:20.000000 posuto-2024.5.0/posuto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 09:26:20.000000 posuto-2024.5.0/posuto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 09:25:46.000000 posuto-2024.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 09:26:20.463960 posuto-2024.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 09:25:46.000000 posuto-2024.5.0/setup.py
```

### Comparing `posuto-2024.4.0/.github/workflows/linux.yml` & `posuto-2024.5.0/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/.gitignore` & `posuto-2024.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/LICENSE` & `posuto-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/Makefile` & `posuto-2024.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/PKG-INFO` & `posuto-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `posuto-2024.4.0/README.md` & `posuto-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/postcharacter.png` & `posuto-2024.5.0/postcharacter.png`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/posuto/officedata.json` & `posuto-2024.5.0/posuto/officedata.json`

 * *Files 0% similar despite different names*

```diff
@@ -2374,14 +2374,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシチュウオウク",
     "neighborhood_kana": "キタ２ジョウニシ",
     "alternates": []
   },
+  "0608654": {
+    "jis": "01101",
+    "kana": "ミツビシシヨウジ カブシキガイシヤ ホツカイドウシシヤ",
+    "name": "三菱商事　株式会社　北海道支社",
+    "prefecture": "北海道",
+    "city": "札幌市中央区",
+    "neighborhood": "北二条西",
+    "banchi": "4丁目",
+    "postal_code": "0608654",
+    "old_code": "060  ",
+    "post_office": "札幌中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ホッカイドウ",
+    "city_kana": "サッポロシチュウオウク",
+    "neighborhood_kana": "キタ２ジョウニシ",
+    "alternates": []
+  },
   "0608503": {
     "jis": "01101",
     "kana": "メデイカルプラザサツポロ",
     "name": "メディカルプラザ札幌",
     "prefecture": "北海道",
     "city": "札幌市中央区",
     "neighborhood": "北五条西",
@@ -2640,33 +2659,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシチュウオウク",
     "neighborhood_kana": "キタ１２ジョウニシ",
     "alternates": []
   },
-  "0608720": {
-    "jis": "01101",
-    "kana": "ノムラシヨウケン カブシキガイシヤ サツポロシテン",
-    "name": "野村證券　株式会社　札幌支店",
-    "prefecture": "北海道",
-    "city": "札幌市中央区",
-    "neighborhood": "北三条西",
-    "banchi": "4丁目(札幌中央郵便局私書箱第23号)",
-    "postal_code": "0608720",
-    "old_code": "06091",
-    "post_office": "札幌中央",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ホッカイドウ",
-    "city_kana": "サッポロシチュウオウク",
-    "neighborhood_kana": "キタ３ジョウニシ",
-    "alternates": []
-  },
   "0608651": {
     "jis": "01101",
     "kana": "ホクレン ノウギヨウキヨウドウクミアイレンゴウカイ",
     "name": "ホクレン　農業協同組合連合会",
     "prefecture": "北海道",
     "city": "札幌市中央区",
     "neighborhood": "北四条西",
@@ -2735,33 +2735,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシチュウオウク",
     "neighborhood_kana": "キタ１ジョウニシ",
     "alternates": []
   },
-  "0608654": {
-    "jis": "01101",
-    "kana": "ミツビシシヨウジ カブシキガイシヤ ホツカイドウシシヤ",
-    "name": "三菱商事　株式会社　北海道支社",
-    "prefecture": "北海道",
-    "city": "札幌市中央区",
-    "neighborhood": "北二条西",
-    "banchi": "4丁目(札幌中央郵便局私書箱第45号)",
-    "postal_code": "0608654",
-    "old_code": "06091",
-    "post_office": "札幌中央",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ホッカイドウ",
-    "city_kana": "サッポロシチュウオウク",
-    "neighborhood_kana": "キタ２ジョウニシ",
-    "alternates": []
-  },
   "0648503": {
     "jis": "01101",
     "kana": "アツミコウギヨウ カブシキガイシヤ",
     "name": "渥美工業　（株）",
     "prefecture": "北海道",
     "city": "札幌市中央区",
     "neighborhood": "南六条西",
@@ -25156,33 +25137,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "0368555": {
-    "jis": "02202",
-    "kana": "トウホクデンリヨク カブシキガイシヤ ヒロサキエイギヨウシヨ",
-    "name": "東北電力　株式会社　弘前営業所",
-    "prefecture": "青森県",
-    "city": "弘前市",
-    "neighborhood": "大字本町",
-    "banchi": "1",
-    "postal_code": "0368555",
-    "old_code": "036  ",
-    "post_office": "弘前",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "0368777": {
     "jis": "02202",
     "kana": "トウホクデンリヨクネツトワ-ク カブシキガイシヤ ヒロサキデンリヨクセンタ-",
     "name": "東北電力ネットワーク　株式会社　弘前電力センター",
     "prefecture": "青森県",
     "city": "弘前市",
     "neighborhood": "大字本町",
@@ -26032,33 +25994,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アオモリケン",
     "city_kana": "ハチノヘシ",
     "neighborhood_kana": "ミナトタカダイ",
     "alternates": []
   },
-  "0318550": {
-    "jis": "02203",
-    "kana": "トウホクデンリヨク カブシキガイシヤ ハチノヘエイギヨウシヨ",
-    "name": "東北電力　株式会社　八戸営業所",
-    "prefecture": "青森県",
-    "city": "八戸市",
-    "neighborhood": "大字堤町",
-    "banchi": "11-2",
-    "postal_code": "0318550",
-    "old_code": "031  ",
-    "post_office": "八戸",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "0318538": {
     "jis": "02203",
     "kana": "ナガサキヤ ハチノヘテン",
     "name": "長崎屋　八戸店",
     "prefecture": "青森県",
     "city": "八戸市",
     "neighborhood": "江陽",
@@ -44806,14 +44749,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "フクシマシ",
     "neighborhood_kana": "サカエマチ",
     "alternates": []
   },
+  "9608603": {
+    "jis": "07201",
+    "kana": "カブシキガイシヤ ミズホギンコウ フクシマシテン",
+    "name": "株式会社　みずほ銀行　福島支店",
+    "prefecture": "福島県",
+    "city": "福島市",
+    "neighborhood": "置賜町",
+    "banchi": "6番20号",
+    "postal_code": "9608603",
+    "old_code": "960  ",
+    "post_office": "福島中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "フクシマケン",
+    "city_kana": "フクシマシ",
+    "neighborhood_kana": "オキタマチョウ",
+    "alternates": []
+  },
   "9608520": {
     "jis": "07201",
     "kana": "カブシキガイシヤ ヤクルトホンシヤ フクシマコウジヨウ",
     "name": "株式会社　ヤクルト本社　福島工場",
     "prefecture": "福島県",
     "city": "福島市",
     "neighborhood": "黒岩",
@@ -46250,33 +46212,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "フクシマシ",
     "neighborhood_kana": "オオタマチ",
     "alternates": []
   },
-  "9608603": {
-    "jis": "07201",
-    "kana": "カブシキガイシヤ ミズホギンコウ フクシマシテン",
-    "name": "株式会社　みずほ銀行　福島支店",
-    "prefecture": "福島県",
-    "city": "福島市",
-    "neighborhood": "置賜町",
-    "banchi": "6番20号(福島中央郵便局私書箱第41号)",
-    "postal_code": "9608603",
-    "old_code": "96091",
-    "post_office": "福島中央",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクシマケン",
-    "city_kana": "フクシマシ",
-    "neighborhood_kana": "オキタマチョウ",
-    "alternates": []
-  },
   "9608610": {
     "jis": "07201",
     "kana": "サトウコウギヨウ カブシキガイシヤ",
     "name": "佐藤工業　株式会社",
     "prefecture": "福島県",
     "city": "福島市",
     "neighborhood": "泉",
@@ -47371,14 +47314,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "カイセイ",
     "alternates": []
   },
+  "9638611": {
+    "jis": "07203",
+    "kana": "ガツコウホウジン セイセンガクシヤ オウウダイガク",
+    "name": "学校法人　晴川学舎　奥羽大学",
+    "prefecture": "福島県",
+    "city": "郡山市",
+    "neighborhood": "富田町",
+    "banchi": "字三角堂31-1",
+    "postal_code": "9638611",
+    "old_code": "963  ",
+    "post_office": "郡山",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "フクシマケン",
+    "city_kana": "コオリヤマシ",
+    "neighborhood_kana": "トミタマチ",
+    "alternates": []
+  },
   "9638501": {
     "jis": "07203",
     "kana": "コウエキザイダンホウジン ホシソウゴウビヨウイン",
     "name": "公益財団法人　星総合病院",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "向河原町",
@@ -47637,33 +47599,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "キクタマチオロシ",
     "alternates": []
   },
-  "9638575": {
-    "jis": "07203",
-    "kana": "トウホクデンリヨク カブシキガイシヤ コオリヤマエイギヨウシヨ",
-    "name": "東北電力　株式会社　郡山営業所",
-    "prefecture": "福島県",
-    "city": "郡山市",
-    "neighborhood": "細沼町",
-    "banchi": "1-5",
-    "postal_code": "9638575",
-    "old_code": "963  ",
-    "post_office": "郡山",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクシマケン",
-    "city_kana": "コオリヤマシ",
-    "neighborhood_kana": "ホソヌママチ",
-    "alternates": []
-  },
   "9638551": {
     "jis": "07203",
     "kana": "ニツポンホウソウキヨウカイ フクシマホウソウキヨク コオリヤマシキヨク",
     "name": "日本放送協会　福島放送局　郡山支局",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "麓山",
@@ -47682,21 +47625,21 @@
   "9638637": {
     "jis": "07203",
     "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ",
     "name": "ニデックプレシジョン　株式会社　郡山事業所",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "富田町",
-    "banchi": "字諏訪内37(郡山郵便局私書箱第37号)",
+    "banchi": "字諏訪内37",
     "postal_code": "9638637",
     "old_code": "963  ",
     "post_office": "郡山",
-    "type": "box",
+    "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "トミタマチ",
     "alternates": []
   },
   "9638580": {
     "jis": "07203",
@@ -48360,33 +48303,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクシマケン",
     "city_kana": "コオリヤマシ",
     "neighborhood_kana": "トラマルマチ",
     "alternates": []
   },
-  "9638611": {
-    "jis": "07203",
-    "kana": "ガツコウホウジン セイセンガクシヤ オウウダイガク",
-    "name": "学校法人　晴川学舎　奥羽大学",
-    "prefecture": "福島県",
-    "city": "郡山市",
-    "neighborhood": "富田町",
-    "banchi": "字三角堂31-1(郡山郵便局私書箱第3号)",
-    "postal_code": "9638611",
-    "old_code": "96391",
-    "post_office": "郡山",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "フクシマケン",
-    "city_kana": "コオリヤマシ",
-    "neighborhood_kana": "トミタマチ",
-    "alternates": []
-  },
   "9638630": {
     "jis": "07203",
     "kana": "コオリヤマシンヨウキンコ",
     "name": "郡山信用金庫",
     "prefecture": "福島県",
     "city": "郡山市",
     "neighborhood": "清水台",
@@ -55215,15 +55139,15 @@
     "neighborhood": "犬塚",
     "banchi": "1570-1",
     "postal_code": "3000595",
     "old_code": "30005",
     "post_office": "江戸崎",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "イナシキシ",
     "neighborhood_kana": "イヌヅカ",
     "alternates": []
   },
   "3000593": {
     "jis": "08229",
@@ -55253,15 +55177,15 @@
     "neighborhood": "須賀津",
     "banchi": "208",
     "postal_code": "3000692",
     "old_code": "30006",
     "post_office": "阿波",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "イナシキシ",
     "neighborhood_kana": "スカヅ",
     "alternates": []
   },
   "3000792": {
     "jis": "08229",
@@ -55272,15 +55196,15 @@
     "neighborhood": "結佐",
     "banchi": "1545",
     "postal_code": "3000792",
     "old_code": "30007",
     "post_office": "阿波",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "イナシキシ",
     "neighborhood_kana": "ケッサ",
     "alternates": []
   },
   "3001492": {
     "jis": "08229",
@@ -58394,14 +58318,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トチギケン",
     "city_kana": "アシカガシ",
     "neighborhood_kana": "トオリ",
     "alternates": []
   },
+  "3268555": {
+    "jis": "09202",
+    "kana": "トチギケンアンソクドボクジムシヨ",
+    "name": "栃木県安足土木事務所",
+    "prefecture": "栃木県",
+    "city": "足利市",
+    "neighborhood": "伊勢町",
+    "banchi": "4丁目19番地",
+    "postal_code": "3268555",
+    "old_code": "326  ",
+    "post_office": "足利",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トチギケン",
+    "city_kana": "アシカガシ",
+    "neighborhood_kana": "イセチョウ",
+    "alternates": []
+  },
   "3260395": {
     "jis": "09202",
     "kana": "サンワシヤツタ- カブシキガイシヤ",
     "name": "三和シャッター　株式会社",
     "prefecture": "栃木県",
     "city": "足利市",
     "neighborhood": "福富新町",
@@ -62404,14 +62347,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "グンマケン",
     "city_kana": "マエバシシ",
     "neighborhood_kana": "オオテマチ",
     "alternates": []
   },
+  "3792194": {
+    "jis": "10201",
+    "kana": "イツパンシヤダンホウジン グンマケントラツクキヨウカイ",
+    "name": "一般社団法人　群馬県トラック協会",
+    "prefecture": "群馬県",
+    "city": "前橋市",
+    "neighborhood": "野中町",
+    "banchi": "322番地1",
+    "postal_code": "3792194",
+    "old_code": "37921",
+    "post_office": "前橋東",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "グンマケン",
+    "city_kana": "マエバシシ",
+    "neighborhood_kana": "ノナカマチ",
+    "alternates": []
+  },
   "3792180": {
     "jis": "10201",
     "kana": "カブシキガイシヤ チヨダコ-ポレ-シヨン",
     "name": "株式会社　チヨダコーポレーション",
     "prefecture": "群馬県",
     "city": "前橋市",
     "neighborhood": "下阿内町",
@@ -62556,33 +62518,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "グンマケン",
     "city_kana": "マエバシシ",
     "neighborhood_kana": "アマガワオオシママチ",
     "alternates": []
   },
-  "3792194": {
-    "jis": "10201",
-    "kana": "シヤダンホウジン グンマケントラツクキヨウカイ",
-    "name": "社団法人　群馬県トラック協会",
-    "prefecture": "群馬県",
-    "city": "前橋市",
-    "neighborhood": "野中町",
-    "banchi": "595",
-    "postal_code": "3792194",
-    "old_code": "37921",
-    "post_office": "前橋東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "グンマケン",
-    "city_kana": "マエバシシ",
-    "neighborhood_kana": "ノナカマチ",
-    "alternates": []
-  },
   "3792193": {
     "jis": "10201",
     "kana": "ナイス カブシキガイシヤ マエバシイチバ",
     "name": "ナイス　株式会社　前橋市場",
     "prefecture": "群馬県",
     "city": "前橋市",
     "neighborhood": "下大島町",
@@ -64912,14 +64855,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "グンマケン",
     "city_kana": "シブカワシ",
     "neighborhood_kana": "ナカムラ",
     "alternates": []
   },
+  "3778566": {
+    "jis": "10208",
+    "kana": "トネガワスイケイサボウジムシヨ",
+    "name": "利根川水系砂防事務所",
+    "prefecture": "群馬県",
+    "city": "渋川市",
+    "neighborhood": "渋川",
+    "banchi": "121-1",
+    "postal_code": "3778566",
+    "old_code": "377  ",
+    "post_office": "渋川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "グンマケン",
+    "city_kana": "シブカワシ",
+    "neighborhood_kana": "シブカワ",
+    "alternates": []
+  },
   "3778511": {
     "jis": "10208",
     "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ニシグンマビヨウイン",
     "name": "独立行政法人　国立病院機構　西群馬病院",
     "prefecture": "群馬県",
     "city": "渋川市",
     "neighborhood": "金井",
@@ -75047,25 +75009,25 @@
   },
   "3691192": {
     "jis": "11218",
     "kana": "フカヤシ カワモトソウゴウシシヨ",
     "name": "深谷市　川本総合支所",
     "prefecture": "埼玉県",
     "city": "深谷市",
-    "neighborhood": "田中",
-    "banchi": "197",
+    "neighborhood": "菅沼",
+    "banchi": "401",
     "postal_code": "3691192",
     "old_code": "36911",
     "post_office": "川本",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "サイタマケン",
     "city_kana": "フカヤシ",
-    "neighborhood_kana": "タナカ",
+    "neighborhood_kana": "スガヌマ",
     "alternates": []
   },
   "3691195": {
     "jis": "11218",
     "kana": "ヨネキユウデリカ カブシキガイシヤ",
     "name": "米久デリカ　株式会社",
     "prefecture": "埼玉県",
@@ -88742,14 +88704,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "イチハラシ",
     "neighborhood_kana": "ゴイチュウオウニシ",
     "alternates": []
   },
+  "2908531": {
+    "jis": "12219",
+    "kana": "カブシキガイシヤ ミツイイ-アンドエスチバジギヨウバ",
+    "name": "株式会社　三井Ｅ＆Ｓ千葉事業場",
+    "prefecture": "千葉県",
+    "city": "市原市",
+    "neighborhood": "八幡海岸通",
+    "banchi": "1番地",
+    "postal_code": "2908531",
+    "old_code": "290  ",
+    "post_office": "市原",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "チバケン",
+    "city_kana": "イチハラシ",
+    "neighborhood_kana": "ヤワタカイガンドオリ",
+    "alternates": []
+  },
   "2908567": {
     "jis": "12219",
     "kana": "カブシキガイシヤ レゾナツク ゴイジギヨウシヨ",
     "name": "株式会社　レゾナック　五井事業所",
     "prefecture": "千葉県",
     "city": "市原市",
     "neighborhood": "五井南海岸",
@@ -88951,33 +88932,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "イチハラシ",
     "neighborhood_kana": "ゴイミナミカイガン",
     "alternates": []
   },
-  "2908531": {
-    "jis": "12219",
-    "kana": "ミツイゾウセン カブシキガイシヤ チバジギヨウシヨ",
-    "name": "三井造船　株式会社　千葉事業所",
-    "prefecture": "千葉県",
-    "city": "市原市",
-    "neighborhood": "八幡海岸通",
-    "banchi": "1番地",
-    "postal_code": "2908531",
-    "old_code": "290  ",
-    "post_office": "市原",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "チバケン",
-    "city_kana": "イチハラシ",
-    "neighborhood_kana": "ヤワタカイガンドオリ",
-    "alternates": []
-  },
   "2908580": {
     "jis": "12219",
     "kana": "ミヤジエンジニアリング カブシキガイシヤ",
     "name": "宮地エンジニアリング　株式会社",
     "prefecture": "千葉県",
     "city": "市原市",
     "neighborhood": "八幡海岸通",
@@ -89819,15 +89781,15 @@
     "neighborhood": "舞浜",
     "banchi": "1番地1",
     "postal_code": "2798504",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798532": {
     "jis": "12227",
@@ -89933,15 +89895,15 @@
     "neighborhood": "美浜",
     "banchi": "1丁目8番1号OLC新浦安ビル4階",
     "postal_code": "2798525",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "ミハマ",
     "alternates": []
   },
   "2798581": {
     "jis": "12227",
@@ -90028,15 +89990,15 @@
     "neighborhood": "舞浜",
     "banchi": "1番地1",
     "postal_code": "2798527",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798585": {
     "jis": "12227",
@@ -90085,15 +90047,15 @@
     "neighborhood": "舞浜",
     "banchi": "2番地18",
     "postal_code": "2798523",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798553": {
     "jis": "12227",
@@ -90123,15 +90085,15 @@
     "neighborhood": "舞浜",
     "banchi": "2番地18",
     "postal_code": "2798570",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798567": {
     "jis": "12227",
@@ -90218,15 +90180,15 @@
     "neighborhood": "明海",
     "banchi": "7丁目1番地1",
     "postal_code": "2798502",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "アケミ",
     "alternates": []
   },
   "2798503": {
     "jis": "12227",
@@ -90237,15 +90199,15 @@
     "neighborhood": "日の出",
     "banchi": "7丁目1番地1",
     "postal_code": "2798503",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "ヒノデ",
     "alternates": []
   },
   "2798526": {
     "jis": "12227",
@@ -90389,15 +90351,15 @@
     "neighborhood": "舞浜",
     "banchi": "2番地50",
     "postal_code": "2798512",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798550": {
     "jis": "12227",
@@ -94385,15 +94347,15 @@
     "neighborhood": "内幸町",
     "banchi": "二丁目2番2号",
     "postal_code": "1008503",
     "old_code": "100  ",
     "post_office": "銀座",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ウチサイワイチョウ",
     "alternates": []
   },
   "1008980": {
     "jis": "13101",
@@ -96812,21 +96774,21 @@
   "1008310": {
     "jis": "13101",
     "kana": "ミツビシデンキ カブシキガイシヤ",
     "name": "三菱電機　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "丸の内",
-    "banchi": "2丁目2-3",
+    "banchi": "二丁目7番3号",
     "postal_code": "1008310",
     "old_code": "100  ",
     "post_office": "銀座",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "マルノウチ",
     "alternates": []
   },
   "1008335": {
     "jis": "13101",
@@ -97432,14 +97394,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "マルノウチ",
     "alternates": []
   },
+  "1018485": {
+    "jis": "13101",
+    "kana": "ア-ルエムトウセロ カブシキガイシヤ",
+    "name": "アールエム東セロ　株式会社",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "神田美土代町",
+    "banchi": "7",
+    "postal_code": "1018485",
+    "old_code": "101  ",
+    "post_office": "神田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "カンダミトシロチョウ",
+    "alternates": []
+  },
   "1018480": {
     "jis": "13101",
     "kana": "アサヒカセイアミダス カブシキガイシヤ",
     "name": "旭化成アミダス　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田錦町",
@@ -100263,33 +100244,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダジンボウチョウ",
     "alternates": []
   },
-  "1018485": {
-    "jis": "13101",
-    "kana": "ミツイカガクトウセロ カブシキガイシヤ",
-    "name": "三井化学東セロ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田美土代町",
-    "banchi": "7",
-    "postal_code": "1018485",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダミトシロチョウ",
-    "alternates": []
-  },
   "1018011": {
     "jis": "13101",
     "kana": "ミツイスミトモカイジヨウカサイホケン カブシキカイシヤ",
     "name": "三井住友海上火災保険　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -104633,14 +104595,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "フジミ",
     "alternates": []
   },
+  "1028113": {
+    "jis": "13101",
+    "kana": "トウキヨウトシヨクギヨウノウリヨクカイハツキヨウカイ",
+    "name": "東京都職業能力開発協会",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "飯田橋",
+    "banchi": "3-10-3東京しごとセンター7階",
+    "postal_code": "1028113",
+    "old_code": "102  ",
+    "post_office": "麹町",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "イイダバシ",
+    "alternates": []
+  },
   "1028226": {
     "jis": "13101",
     "kana": "トウキヨウホウムキヨク",
     "name": "東京法務局",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "九段南",
@@ -105716,14 +105697,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "クダンミナミ",
     "alternates": []
   },
+  "1028274": {
+    "jis": "13101",
+    "kana": "ユ-エイゼンセン キヨウサイジギヨウキヨク",
+    "name": "ＵＡゼンセン　共済事業局",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "九段南",
+    "banchi": "4-8-19CIRCLES+市ケ谷駅前",
+    "postal_code": "1028274",
+    "old_code": "102  ",
+    "post_office": "麹町",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "クダンミナミ",
+    "alternates": []
+  },
   "1028236": {
     "jis": "13101",
     "kana": "ライトコウギヨウ カブシキガイシヤ",
     "name": "ライト工業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "九段北",
@@ -107732,33 +107732,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシハコザキチョウ",
     "alternates": []
   },
-  "1038520": {
-    "jis": "13102",
-    "kana": "カブシキガイシヤ ロイヤルパ-クホテル",
-    "name": "株式会社　ロイヤルパークホテル",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "日本橋蛎殻町",
-    "banchi": "2丁目1-1",
-    "postal_code": "1038520",
-    "old_code": "103  ",
-    "post_office": "日本橋",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ニホンバシカキガラチョウ",
-    "alternates": []
-  },
   "1038412": {
     "jis": "13102",
     "kana": "カントウカガク (カブ)",
     "name": "関東化学　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "日本橋本町",
@@ -108758,50 +108739,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシトミザワチョウ",
     "alternates": []
   },
-  "1038488": {
+  "1038489": {
     "jis": "13102",
     "kana": "トヨタモビリテイサ-ビス カブシキガイシヤ",
     "name": "トヨタモビリティサービス　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
-    "neighborhood": "日本橋浜町",
-    "banchi": "2-12-4",
-    "postal_code": "1038488",
+    "neighborhood": "日本橋久松町",
+    "banchi": "9-9",
+    "postal_code": "1038489",
     "old_code": "103  ",
     "post_office": "日本橋",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
-    "neighborhood_kana": "ニホンバシハマチョウ",
+    "neighborhood_kana": "ニホンバシヒサマツチョウ",
     "alternates": []
   },
-  "1038489": {
+  "1038488": {
     "jis": "13102",
     "kana": "トヨタモビリテイサ-ビス カブシキガイシヤ",
     "name": "トヨタモビリティサービス　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
-    "neighborhood": "日本橋久松町",
-    "banchi": "9-9",
-    "postal_code": "1038489",
+    "neighborhood": "日本橋浜町",
+    "banchi": "2-12-4",
+    "postal_code": "1038488",
     "old_code": "103  ",
     "post_office": "日本橋",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
-    "neighborhood_kana": "ニホンバシヒサマツチョウ",
+    "neighborhood_kana": "ニホンバシハマチョウ",
     "alternates": []
   },
   "1038439": {
     "jis": "13102",
     "kana": "トリイヤクヒン (カブ)",
     "name": "鳥居薬品　株式会社",
     "prefecture": "東京都",
@@ -109613,33 +109594,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシムロマチ",
     "alternates": []
   },
-  "1038263": {
-    "jis": "13102",
-    "kana": "ミツイゾウセン カブシキガイシヤ",
-    "name": "三井造船　株式会社",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "日本橋",
-    "banchi": "1丁目3-16",
-    "postal_code": "1038263",
-    "old_code": "103  ",
-    "post_office": "日本橋",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ニホンバシ",
-    "alternates": []
-  },
   "1038556": {
     "jis": "13102",
     "kana": "ミツイブツサンフユ-チヤ-ズ カブシキガイシヤ",
     "name": "三井物産フューチャーズ　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "日本橋堀留町",
@@ -109670,14 +109632,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシ",
     "alternates": []
   },
+  "1038520": {
+    "jis": "13102",
+    "kana": "ミツビシジシヨホテルズアンドリゾ-ツ カブシキガイシヤ ロイヤルパ-クホテル トウキヨウ・ニホンバシ",
+    "name": "三菱地所ホテルズ＆リゾーツ　株式会社　ロイヤルパークホテル（東京・日本橋）",
+    "prefecture": "東京都",
+    "city": "中央区",
+    "neighborhood": "日本橋蛎殻町",
+    "banchi": "2丁目1-1",
+    "postal_code": "1038520",
+    "old_code": "103  ",
+    "post_office": "日本橋",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チュウオウク",
+    "neighborhood_kana": "ニホンバシカキガラチョウ",
+    "alternates": []
+  },
   "1038460": {
     "jis": "13102",
     "kana": "ミツワデンキ (カブ)",
     "name": "ミツワ電機　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "東日本橋",
@@ -111431,15 +111412,15 @@
     "neighborhood": "築地",
     "banchi": "五丁目6番4号",
     "postal_code": "1048439",
     "old_code": "104  ",
     "post_office": "晴海",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ツキジ",
     "alternates": []
   },
   "1048442": {
     "jis": "13102",
@@ -114566,15 +114547,15 @@
     "neighborhood": "海岸",
     "banchi": "1-2-20汐留ビルディング9F",
     "postal_code": "1058316",
     "old_code": "105  ",
     "post_office": "銀座",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "カイガン",
     "alternates": []
   },
   "1058670": {
     "jis": "13103",
@@ -117165,45 +117146,25 @@
   "1058433": {
     "jis": "13103",
     "kana": "ピ-エイチシ- カブシキガイシヤ",
     "name": "ＰＨＣ　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "西新橋",
-    "banchi": "2-38-5",
+    "banchi": "3丁目7-1",
     "postal_code": "1058433",
     "old_code": "105  ",
     "post_office": "芝",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ニシシンバシ",
-    "alternates": [
-      {
-        "jis": "13103",
-        "kana": "ピ-エイチシ-ホ-ルデイングス カブシキガイシヤ",
-        "name": "ＰＨＣホールディングス　株式会社",
-        "prefecture": "東京都",
-        "city": "港区",
-        "neighborhood": "西新橋",
-        "banchi": "2-38-5",
-        "postal_code": "1058433",
-        "old_code": "105  ",
-        "post_office": "芝",
-        "type": "office",
-        "multiple": false,
-        "new": false,
-        "prefecture_kana": "トウキョウト",
-        "city_kana": "ミナトク",
-        "neighborhood_kana": "ニシシンバシ",
-        "alternates": []
-      }
-    ]
+    "alternates": []
   },
   "1058668": {
     "jis": "13103",
     "kana": "フジツウエフ・アイ・ピ- カブシキガイシヤ アクテイブオフイス",
     "name": "富士通エフ・アイ・ピー　株式会社　アクティブオフィス",
     "prefecture": "東京都",
     "city": "港区",
@@ -117292,33 +117253,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "シバダイモン",
     "alternates": []
   },
-  "1058466": {
-    "jis": "13103",
-    "kana": "ミツイシヨクヒン カブシキガイシヤ",
-    "name": "三井食品　株式会社",
-    "prefecture": "東京都",
-    "city": "港区",
-    "neighborhood": "西新橋",
-    "banchi": "1丁目1番1号",
-    "postal_code": "1058466",
-    "old_code": "105  ",
-    "post_office": "芝",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ミナトク",
-    "neighborhood_kana": "ニシシンバシ",
-    "alternates": []
-  },
   "1058574": {
     "jis": "13103",
     "kana": "ミツイスミトモシンタクギンコウ カブシキガイシヤ",
     "name": "三井住友信託銀行　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "芝",
@@ -117368,14 +117310,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ニシシンバシ",
     "alternates": []
   },
+  "1058466": {
+    "jis": "13103",
+    "kana": "ミツイブツサンリユウツウグル-プ カブシキガイシヤ",
+    "name": "三井物産流通グループ　株式会社",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "西新橋",
+    "banchi": "1丁目1番1号",
+    "postal_code": "1058466",
+    "old_code": "105  ",
+    "post_office": "芝",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "ニシシンバシ",
+    "alternates": []
+  },
   "1058712": {
     "jis": "13103",
     "kana": "ミツビシエイチシ-キヤピタル カブシキガイシヤ",
     "name": "三菱ＨＣキャピタル　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "西新橋",
@@ -117501,14 +117462,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "シバコウエン",
     "alternates": []
   },
+  "1058309": {
+    "jis": "13103",
+    "kana": "モリナガセイカ カブシキガイシヤ",
+    "name": "森永製菓　株式会社",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "芝浦",
+    "banchi": "1丁目13-16",
+    "postal_code": "1058309",
+    "old_code": "105  ",
+    "post_office": "銀座",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "シバウラ",
+    "alternates": []
+  },
   "1058451": {
     "jis": "13103",
     "kana": "モリムラシヨウジ カブシキガイシヤ",
     "name": "森村商事　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "虎ノ門",
@@ -120773,15 +120753,15 @@
     "city_kana": "ミナトク",
     "neighborhood_kana": "アカサカ",
     "alternates": []
   },
   "1078431": {
     "jis": "13103",
     "kana": "ニホンカンザイセンタ- カブシキガイシヤ",
-    "name": "日本管財センター　株式会社",
+    "name": "日本管材センター　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "赤坂",
     "banchi": "1-1-14",
     "postal_code": "1078431",
     "old_code": "107  ",
     "post_office": "赤坂",
@@ -123335,14 +123315,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "コウナン",
     "alternates": []
   },
+  "1088331": {
+    "jis": "13103",
+    "kana": "テイ-デイ-シネツクス カブシキガイシヤ",
+    "name": "ＴＤ　ＳＹＮＮＥＸ　株式会社",
+    "prefecture": "東京都",
+    "city": "港区",
+    "neighborhood": "芝浦",
+    "banchi": "3-1-1msbTamachiステーションタワーN41F",
+    "postal_code": "1088331",
+    "old_code": "108  ",
+    "post_office": "高輪",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "ミナトク",
+    "neighborhood_kana": "シバウラ",
+    "alternates": []
+  },
   "1088506": {
     "jis": "13103",
     "kana": "テイエチケ- カブシキカイシヤ",
     "name": "ＴＨＫ　株式会社",
     "prefecture": "東京都",
     "city": "港区",
     "neighborhood": "芝浦",
@@ -130268,15 +130267,15 @@
     "neighborhood": "西新宿",
     "banchi": "6丁目5-1新宿アイランドタワー6F",
     "postal_code": "1631349",
     "old_code": "16313",
     "post_office": "新宿",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "ニシシンジュク",
     "alternates": []
   },
   "1638677": {
     "jis": "13104",
@@ -143025,52 +143024,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "キバ",
     "alternates": []
   },
-  "1358570": {
-    "jis": "13108",
-    "kana": "ニツシンセイトウ カブシキガイシヤ トヨスコウジヨウ",
-    "name": "日新製糖　株式会社　豊洲工場",
-    "prefecture": "東京都",
-    "city": "江東区",
-    "neighborhood": "豊洲",
-    "banchi": "4丁目9-11",
-    "postal_code": "1358570",
-    "old_code": "135  ",
-    "post_office": "晴海",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "コウトウク",
-    "neighborhood_kana": "トヨス",
-    "alternates": []
-  },
-  "1358553": {
-    "jis": "13108",
-    "kana": "ニツシンセイトウ カブシキガイシヤ ヨカカイハツホンブ ドウ.スポ-ツプラザハルミ",
-    "name": "日新製糖　株式会社　余暇開発本部　ドゥ・スポーツプラザ晴海",
-    "prefecture": "東京都",
-    "city": "江東区",
-    "neighborhood": "豊洲",
-    "banchi": "5丁目6-41",
-    "postal_code": "1358553",
-    "old_code": "135  ",
-    "post_office": "晴海",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "コウトウク",
-    "neighborhood_kana": "トヨス",
-    "alternates": []
-  },
   "1358477": {
     "jis": "13108",
     "kana": "ニツポンチユウオウケイバカイ デンワトウヒヨウセンタ-",
     "name": "日本中央競馬会　電話投票センター",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "永代",
@@ -143633,14 +143594,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "トウヨウ",
     "alternates": []
   },
+  "1368881": {
+    "jis": "13108",
+    "kana": "(カ) ミキモト",
+    "name": "株式会社　ミキモト",
+    "prefecture": "東京都",
+    "city": "江東区",
+    "neighborhood": "南砂",
+    "banchi": "7-11-24",
+    "postal_code": "1368881",
+    "old_code": "136  ",
+    "post_office": "城東",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "コウトウク",
+    "neighborhood_kana": "ミナミスナ",
+    "alternates": []
+  },
   "1368581": {
     "jis": "13108",
     "kana": "(カブ) シ-ア-ルシ-ソウゴウケンキユウシヨ",
     "name": "（株）　ＣＲＣ総合研究所",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "南砂",
@@ -145072,15 +145052,15 @@
     "neighborhood": "東品川",
     "banchi": "四丁目12番4号品川シーサイドパークタワー",
     "postal_code": "1408586",
     "old_code": "140  ",
     "post_office": "品川",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シナガワク",
     "neighborhood_kana": "ヒガシシナガワ",
     "alternates": []
   },
   "1408688": {
     "jis": "13109",
@@ -160171,33 +160151,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ナカノク",
     "neighborhood_kana": "ヤヨイチョウ",
     "alternates": []
   },
-  "1648512": {
-    "jis": "13114",
-    "kana": "カブシキガイシヤ ナカノサンプラザ",
-    "name": "株式会社　中野サンプラザ",
-    "prefecture": "東京都",
-    "city": "中野区",
-    "neighborhood": "中野",
-    "banchi": "4丁目1-1",
-    "postal_code": "1648512",
-    "old_code": "164  ",
-    "post_office": "中野",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "ナカノク",
-    "neighborhood_kana": "ナカノ",
-    "alternates": []
-  },
   "1648705": {
     "jis": "13114",
     "kana": "カブシキガイシヤ ニホンヴオ-グシヤ",
     "name": "株式会社　日本ヴォーグ社",
     "prefecture": "東京都",
     "city": "中野区",
     "neighborhood": "弥生町",
@@ -160501,21 +160462,21 @@
   "1648501": {
     "jis": "13114",
     "kana": "ナカノクヤクシヨ",
     "name": "中野区役所",
     "prefecture": "東京都",
     "city": "中野区",
     "neighborhood": "中野",
-    "banchi": "4丁目8-1",
+    "banchi": "四丁目11番19号",
     "postal_code": "1648501",
     "old_code": "164  ",
     "post_office": "中野",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ナカノク",
     "neighborhood_kana": "ナカノ",
     "alternates": []
   },
   "1648686": {
     "jis": "13114",
@@ -165789,15 +165750,15 @@
     "neighborhood": "南千住",
     "banchi": "3丁目13番1号",
     "postal_code": "1168522",
     "old_code": "116  ",
     "post_office": "荒川",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "アラカワク",
     "neighborhood_kana": "ミナミセンジュ",
     "alternates": []
   },
   "1168533": {
     "jis": "13118",
@@ -176208,33 +176169,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チョウフシ",
     "neighborhood_kana": "フジミチョウ",
     "alternates": []
   },
-  "1828686": {
-    "jis": "13208",
-    "kana": "カブシキガイシヤ フジカラ-サ-ビス トウキヨウジギヨウシヨ",
-    "name": "株式会社　フジカラーサービス　東京事業所",
-    "prefecture": "東京都",
-    "city": "調布市",
-    "neighborhood": "柴崎",
-    "banchi": "1丁目67-1(調布郵便局私書箱第10号)",
-    "postal_code": "1828686",
-    "old_code": "182  ",
-    "post_office": "調布",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チョウフシ",
-    "neighborhood_kana": "シバサキ",
-    "alternates": []
-  },
   "1828558": {
     "jis": "13208",
     "kana": "キユ-ピ- カブシキガイシヤ センガワコウジヨウ",
     "name": "キユーピー　株式会社　仙川工場",
     "prefecture": "東京都",
     "city": "調布市",
     "neighborhood": "仙川町",
@@ -182136,14 +182078,90 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ヨコハマシニシク",
     "neighborhood_kana": "ミナトミライ",
     "alternates": []
   },
+  "2208562": {
+    "jis": "14103",
+    "kana": "タイヨウニツサン カブシキガイシヤ カントウシシヤ",
+    "name": "大陽日酸　株式会社　関東支社",
+    "prefecture": "神奈川県",
+    "city": "横浜市西区",
+    "neighborhood": "みなとみらい",
+    "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階",
+    "postal_code": "2208562",
+    "old_code": "220  ",
+    "post_office": "神奈川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシニシク",
+    "neighborhood_kana": "ミナトミライ",
+    "alternates": []
+  },
+  "2208561": {
+    "jis": "14103",
+    "kana": "タイヨウニツサン カブシキガイシヤ ミナトミライジギヨウシヨ",
+    "name": "大陽日酸　株式会社　みなとみらい事業所",
+    "prefecture": "神奈川県",
+    "city": "横浜市西区",
+    "neighborhood": "みなとみらい",
+    "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階",
+    "postal_code": "2208561",
+    "old_code": "220  ",
+    "post_office": "神奈川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシニシク",
+    "neighborhood_kana": "ミナトミライ",
+    "alternates": []
+  },
+  "2208563": {
+    "jis": "14103",
+    "kana": "タイヨウニツサンエンジニアリング カブシキガイシヤ",
+    "name": "大陽日酸エンジニアリング　株式会社",
+    "prefecture": "神奈川県",
+    "city": "横浜市西区",
+    "neighborhood": "みなとみらい",
+    "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階",
+    "postal_code": "2208563",
+    "old_code": "220  ",
+    "post_office": "神奈川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシニシク",
+    "neighborhood_kana": "ミナトミライ",
+    "alternates": []
+  },
+  "2208564": {
+    "jis": "14103",
+    "kana": "タイヨウニツサンエンジニアリング カブシキガイシヤ カントウシテン",
+    "name": "大陽日酸エンジニアリング　株式会社　関東支店",
+    "prefecture": "神奈川県",
+    "city": "横浜市西区",
+    "neighborhood": "みなとみらい",
+    "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階",
+    "postal_code": "2208564",
+    "old_code": "220  ",
+    "post_office": "神奈川",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシニシク",
+    "neighborhood_kana": "ミナトミライ",
+    "alternates": []
+  },
   "2208620": {
     "jis": "14103",
     "kana": "ダイワハウスコウギヨウ (カ) ヨコハマシシヤ",
     "name": "大和ハウス工業　株式会社　横浜支社",
     "prefecture": "神奈川県",
     "city": "横浜市西区",
     "neighborhood": "みなとみらい",
@@ -184397,14 +184415,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ヨコハマシカナザワク",
     "neighborhood_kana": "サチウラ",
     "alternates": []
   },
+  "2368609": {
+    "jis": "14108",
+    "kana": "ヨコハマミナミコウキヨウシヨクギヨウアンテイシヨ",
+    "name": "横浜南公共職業安定所",
+    "prefecture": "神奈川県",
+    "city": "横浜市金沢区",
+    "neighborhood": "寺前",
+    "banchi": "1-9-6",
+    "postal_code": "2368609",
+    "old_code": "236  ",
+    "post_office": "横浜金沢",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシカナザワク",
+    "neighborhood_kana": "テラマエ",
+    "alternates": []
+  },
   "2368550": {
     "jis": "14108",
     "kana": "ヨコハマミナミゼイムシヨ",
     "name": "横浜南税務署",
     "prefecture": "神奈川県",
     "city": "横浜市金沢区",
     "neighborhood": "並木",
@@ -195799,33 +195836,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ザマシ",
     "neighborhood_kana": "ミドリガオカ",
     "alternates": []
   },
-  "2528550": {
-    "jis": "14216",
-    "kana": "トウキヨウコスモスデンキ カブシキガイシヤ",
-    "name": "東京コスモス電機　株式会社",
-    "prefecture": "神奈川県",
-    "city": "座間市",
-    "neighborhood": "相武台",
-    "banchi": "2丁目268",
-    "postal_code": "2528550",
-    "old_code": "228  ",
-    "post_office": "座間",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "カナガワケン",
-    "city_kana": "ザマシ",
-    "neighborhood_kana": "ソウブダイ",
-    "alternates": []
-  },
   "2528502": {
     "jis": "14216",
     "kana": "ニツサンジドウシヤ カブシキガイシヤ ザマジギヨウシヨ",
     "name": "日産自動車　株式会社　座間事業所",
     "prefecture": "神奈川県",
     "city": "座間市",
     "neighborhood": "広野台",
@@ -195913,14 +195931,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ザマシ",
     "neighborhood_kana": "ヒロノダイ",
     "alternates": []
   },
+  "2528550": {
+    "jis": "14216",
+    "kana": "トウキヨウコスモスデンキ カブシキガイシヤ",
+    "name": "東京コスモス電機　株式会社",
+    "prefecture": "神奈川県",
+    "city": "座間市",
+    "neighborhood": "相武台",
+    "banchi": "2丁目12番1号",
+    "postal_code": "2528550",
+    "old_code": "252  ",
+    "post_office": "座間",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ザマシ",
+    "neighborhood_kana": "ソウブダイ",
+    "alternates": []
+  },
   "2528560": {
     "jis": "14216",
     "kana": "マガシ-クブツリユウセンタ-マガコ",
     "name": "マガシーク物流センターｍａｇａｃｏ",
     "prefecture": "神奈川県",
     "city": "座間市",
     "neighborhood": "広野台",
@@ -205854,42 +205891,42 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ミョウコウシ",
     "neighborhood_kana": "サカエチョウ",
     "alternates": []
   },
-  "9492194": {
+  "9492193": {
     "jis": "15217",
-    "kana": "ダイイチデンコウ カブシキカイシヤ タグチコウジヨウ",
-    "name": "第一電工　株式会社　田口工場",
+    "kana": "シンニツポンデンコウ カブシキガイシヤ ミヨウコウコウジヨウ",
+    "name": "新日本電工　株式会社　妙高工場",
     "prefecture": "新潟県",
     "city": "妙高市",
-    "neighborhood": "大字関川",
-    "banchi": "70",
-    "postal_code": "9492194",
+    "neighborhood": "大字田口",
+    "banchi": "272",
+    "postal_code": "9492193",
     "old_code": "94921",
     "post_office": "妙高高原",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "9492193": {
+  "9492194": {
     "jis": "15217",
-    "kana": "チユウオウデンキコウギヨウ カブシキカイシヤ タグチコウジヨウ",
-    "name": "中央電気工業　株式会社　田口工場",
+    "kana": "ダイイチデンコウ カブシキカイシヤ タグチコウジヨウ",
+    "name": "第一電工　株式会社　田口工場",
     "prefecture": "新潟県",
     "city": "妙高市",
-    "neighborhood": "大字田口",
-    "banchi": "272",
-    "postal_code": "9492193",
+    "neighborhood": "大字関川",
+    "banchi": "70",
+    "postal_code": "9492194",
     "old_code": "94921",
     "post_office": "妙高高原",
     "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
@@ -216024,14 +216061,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "カナザワシ",
     "neighborhood_kana": "コウリンボウ",
     "alternates": []
   },
+  "9208545": {
+    "jis": "17201",
+    "kana": "カブシキガイシヤ マルビシ",
+    "name": "株式会社　丸菱",
+    "prefecture": "石川県",
+    "city": "金沢市",
+    "neighborhood": "問屋町",
+    "banchi": "2丁目20番地",
+    "postal_code": "9208545",
+    "old_code": "920  ",
+    "post_office": "金沢中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イシカワケン",
+    "city_kana": "カナザワシ",
+    "neighborhood_kana": "トイヤマチ",
+    "alternates": []
+  },
   "9208625": {
     "jis": "17201",
     "kana": "カブシキガイシヤ ミナミシヨウテン",
     "name": "株式会社　南商店",
     "prefecture": "石川県",
     "city": "金沢市",
     "neighborhood": "京町",
@@ -233185,14 +233241,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ナガノケン",
     "city_kana": "ナガノシ",
     "neighborhood_kana": "ニシワダ",
     "alternates": []
   },
+  "3818501": {
+    "jis": "20201",
+    "kana": "エフアイシ-テイ カブシキガイシヤ",
+    "name": "ＦＩＣＴ　株式会社",
+    "prefecture": "長野県",
+    "city": "長野市",
+    "neighborhood": "北尾張部",
+    "banchi": "36",
+    "postal_code": "3818501",
+    "old_code": "381  ",
+    "post_office": "長野東",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ナガノケン",
+    "city_kana": "ナガノシ",
+    "neighborhood_kana": "キタオワリベ",
+    "alternates": []
+  },
   "3818560": {
     "jis": "20201",
     "kana": "オカヤサンソ カブシキガイシヤ ナガノジギヨウブ",
     "name": "岡谷酸素　株式会社　長野事業部",
     "prefecture": "長野県",
     "city": "長野市",
     "neighborhood": "大字中越",
@@ -233527,33 +233602,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "3818501": {
-    "jis": "20201",
-    "kana": "フジツウ カブシキガイシヤ ナガノコウジヨウ",
-    "name": "富士通　株式会社　長野工場",
-    "prefecture": "長野県",
-    "city": "長野市",
-    "neighborhood": "大字北尾張部",
-    "banchi": "36",
-    "postal_code": "3818501",
-    "old_code": "381  ",
-    "post_office": "長野東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "3818539": {
     "jis": "20201",
     "kana": "マツダサンギヨウ カブシキガイシヤ",
     "name": "松田産業　株式会社",
     "prefecture": "長野県",
     "city": "長野市",
     "neighborhood": "大字南長池",
@@ -234363,14 +234419,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
+  "3908704": {
+    "jis": "20202",
+    "kana": "カブシキガイシヤ ハチジユウニギンコウ マツモトエイギヨウブ",
+    "name": "株式会社　八十二銀行　松本営業部",
+    "prefecture": "長野県",
+    "city": "松本市",
+    "neighborhood": "大手",
+    "banchi": "3丁目1番1号(松本郵便局私書箱第30号)",
+    "postal_code": "3908704",
+    "old_code": "390  ",
+    "post_office": "松本",
+    "type": "box",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ナガノケン",
+    "city_kana": "マツモトシ",
+    "neighborhood_kana": "オオテ",
+    "alternates": []
+  },
   "3908623": {
     "jis": "20202",
     "kana": "ガツコウホウジン ガイゴガクエン シナノムツミコウトウガツコウ",
     "name": "学校法人　外語学園　信農むつみ高等学校",
     "prefecture": "長野県",
     "city": "松本市",
     "neighborhood": "南松本",
@@ -238013,33 +238088,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "3828501": {
-    "jis": "20207",
-    "kana": "フジツウ カブシキガイシヤ スザカコウジヨウ",
-    "name": "富士通　株式会社　須坂工場",
-    "prefecture": "長野県",
-    "city": "須坂市",
-    "neighborhood": "大字小山",
-    "banchi": "460",
-    "postal_code": "3828501",
-    "old_code": "382  ",
-    "post_office": "須坂",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "3828585": {
     "jis": "20207",
     "kana": "ホクリクコカ・コ-ラボトリング カブシキガイシヤ",
     "name": "北陸コカ・コーラボトリング　株式会社",
     "prefecture": "長野県",
     "city": "須坂市",
     "neighborhood": "大字井上",
@@ -238925,33 +238981,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "3892298": {
-    "jis": "20213",
-    "kana": "カブシキガイシヤ シナノフジツウ",
-    "name": "株式会社　しなの富士通",
-    "prefecture": "長野県",
-    "city": "飯山市",
-    "neighborhood": "大字野坂田",
-    "banchi": "935",
-    "postal_code": "3892298",
-    "old_code": "38922",
-    "post_office": "飯山",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "3918531": {
     "jis": "20214",
     "kana": "カブシキガイシヤ イ-スタン",
     "name": "株式会社　イースタン",
     "prefecture": "長野県",
     "city": "茅野市",
     "neighborhood": "塚原",
@@ -242649,33 +242686,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
-  "3892392": {
-    "jis": "20562",
-    "kana": "キジマダイラムラヤクバ",
-    "name": "木島平村役場",
-    "prefecture": "長野県",
-    "city": "下高井郡木島平村",
-    "neighborhood": "大字往郷",
-    "banchi": "973-1",
-    "postal_code": "3892392",
-    "old_code": "38923",
-    "post_office": "木島平",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "",
-    "city_kana": "",
-    "neighborhood_kana": "",
-    "alternates": []
-  },
   "3892592": {
     "jis": "20563",
     "kana": "ノザワオンセンムラヤクバ",
     "name": "野沢温泉村役場",
     "prefecture": "長野県",
     "city": "下高井郡野沢温泉村",
     "neighborhood": "大字豊郷",
@@ -255223,15 +255241,15 @@
     "neighborhood": "砂山町",
     "banchi": "1183番地",
     "postal_code": "4308667",
     "old_code": "430  ",
     "post_office": "浜松",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "シズオカケン",
     "city_kana": "ハママツシチュウオウク",
     "neighborhood_kana": "スナヤマチョウ",
     "alternates": []
   },
   "4308587": {
     "jis": "22138",
@@ -257124,15 +257142,15 @@
     "neighborhood": "大岡",
     "banchi": "2068-3",
     "postal_code": "4108510",
     "old_code": "410  ",
     "post_office": "沼津",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "シズオカケン",
     "city_kana": "ヌマヅシ",
     "neighborhood_kana": "オオオカ",
     "alternates": []
   },
   "4108580": {
     "jis": "22203",
@@ -257181,15 +257199,15 @@
     "neighborhood": "日の出町",
     "banchi": "1-40(沼津郵便局私書箱第7号)",
     "postal_code": "4108655",
     "old_code": "410  ",
     "post_office": "沼津",
     "type": "box",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "シズオカケン",
     "city_kana": "ヌマヅシ",
     "neighborhood_kana": "ヒノデチョウ",
     "alternates": []
   },
   "4108602": {
     "jis": "22203",
@@ -268836,33 +268854,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカムラク",
     "neighborhood_kana": "タケバシチョウ",
     "alternates": []
   },
-  "4538702": {
-    "jis": "23105",
-    "kana": "カブシキガイシヤ サポ-テイングチユウキヨウ",
-    "name": "株式会社　サポーティング中京",
-    "prefecture": "愛知県",
-    "city": "名古屋市中村区",
-    "neighborhood": "平池町",
-    "banchi": "4丁目60番地11",
-    "postal_code": "4538702",
-    "old_code": "453  ",
-    "post_office": "中村",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "ナゴヤシナカムラク",
-    "neighborhood_kana": "ヒライケチョウ",
-    "alternates": []
-  },
   "4538512": {
     "jis": "23105",
     "kana": "カブシキガイシヤ ジユニア-",
     "name": "株式会社　ジュニアー",
     "prefecture": "愛知県",
     "city": "名古屋市中村区",
     "neighborhood": "黄金通",
@@ -269077,15 +269076,15 @@
     "neighborhood": "椿町",
     "banchi": "14番8号",
     "postal_code": "4538565",
     "old_code": "453  ",
     "post_office": "中村",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "ナゴヤシナカムラク",
     "neighborhood_kana": "ツバキチョウ",
     "alternates": []
   },
   "4538521": {
     "jis": "23105",
@@ -279365,33 +279364,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "トヨハシシ",
     "neighborhood_kana": "オオイワチョウ",
     "alternates": []
   },
-  "4448564": {
-    "jis": "23202",
-    "kana": "アイシン・エイ・ダブリユ (カブ) オカザキコウジヨウ",
-    "name": "アイシン・エイ・ダブリュ　（株）　岡崎工場",
-    "prefecture": "愛知県",
-    "city": "岡崎市",
-    "neighborhood": "岡町",
-    "banchi": "字原山6-18",
-    "postal_code": "4448564",
-    "old_code": "444  ",
-    "post_office": "岡崎",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "オカザキシ",
-    "neighborhood_kana": "オカチョウ",
-    "alternates": []
-  },
   "4448520": {
     "jis": "23202",
     "kana": "アイチガクセンダイガク",
     "name": "愛知学泉大学",
     "prefecture": "愛知県",
     "city": "岡崎市",
     "neighborhood": "舳越町",
@@ -279536,14 +279516,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "オカザキシ",
     "neighborhood_kana": "イダミナミマチ",
     "alternates": []
   },
+  "4448564": {
+    "jis": "23202",
+    "kana": "カブシキガイシヤ アイシン オカザキコウジヨウ",
+    "name": "株式会社　アイシン　岡崎工場",
+    "prefecture": "愛知県",
+    "city": "岡崎市",
+    "neighborhood": "岡町",
+    "banchi": "字原山6-18",
+    "postal_code": "4448564",
+    "old_code": "444  ",
+    "post_office": "岡崎",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "オカザキシ",
+    "neighborhood_kana": "オカチョウ",
+    "alternates": []
+  },
   "4448530": {
     "jis": "23202",
     "kana": "カブシキガイシヤ カワモトセイサクシヨ オカザキコウジヨウ",
     "name": "株式会社　川本製作所　岡崎工場",
     "prefecture": "愛知県",
     "city": "岡崎市",
     "neighborhood": "橋目町",
@@ -284154,33 +284153,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "カリヤシ",
     "neighborhood_kana": "アイオイチョウ",
     "alternates": []
   },
-  "4488650": {
-    "jis": "23210",
-    "kana": "アイシンセイキ カブシキガイシヤ",
-    "name": "アイシン精機　株式会社",
-    "prefecture": "愛知県",
-    "city": "刈谷市",
-    "neighborhood": "朝日町",
-    "banchi": "2丁目1(刈谷郵便局私書箱第13号)",
-    "postal_code": "4488650",
-    "old_code": "448  ",
-    "post_office": "刈谷",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "カリヤシ",
-    "neighborhood_kana": "アサヒマチ",
-    "alternates": []
-  },
   "4488543": {
     "jis": "23210",
     "kana": "アイチキヨウイクダイガク セイカツキヨウドウクミアイ",
     "name": "愛知教育大学　生活協同組合",
     "prefecture": "愛知県",
     "city": "刈谷市",
     "neighborhood": "井ケ谷町",
@@ -284287,14 +284267,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "カリヤシ",
     "neighborhood_kana": "ナカヤマチョウ",
     "alternates": []
   },
+  "4488650": {
+    "jis": "23210",
+    "kana": "カブシキガイシヤ アイシン",
+    "name": "株式会社　アイシン",
+    "prefecture": "愛知県",
+    "city": "刈谷市",
+    "neighborhood": "朝日町",
+    "banchi": "2丁目1(刈谷郵便局私書箱第13号)",
+    "postal_code": "4488650",
+    "old_code": "448  ",
+    "post_office": "刈谷",
+    "type": "box",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "カリヤシ",
+    "neighborhood_kana": "アサヒマチ",
+    "alternates": []
+  },
   "4488688": {
     "jis": "23210",
     "kana": "カブシキガイシヤ アドヴイツクス",
     "name": "株式会社　アドヴィックス",
     "prefecture": "愛知県",
     "city": "刈谷市",
     "neighborhood": "昭和町",
@@ -285923,26 +285922,26 @@
     "prefecture_kana": "アイチケン",
     "city_kana": "トヨタシ",
     "neighborhood_kana": "ヨシワラチョウ",
     "alternates": []
   },
   "4441192": {
     "jis": "23212",
-    "kana": "アイシン・エイ・ダブリユ カブシキガイシヤ",
-    "name": "アイシン・エイ・ダブリュ　株式会社",
+    "kana": "カブシキガイシヤ アイシン アンジヨウチク",
+    "name": "株式会社　アイシン　安城地区",
     "prefecture": "愛知県",
     "city": "安城市",
     "neighborhood": "藤井町",
     "banchi": "高根10",
     "postal_code": "4441192",
     "old_code": "44411",
     "post_office": "桜井",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "アイチケン",
     "city_kana": "アンジョウシ",
     "neighborhood_kana": "フジイチョウ",
     "alternates": []
   },
   "4441195": {
     "jis": "23212",
@@ -286073,33 +286072,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "アンジョウシ",
     "neighborhood_kana": "イズミチョウ",
     "alternates": []
   },
-  "4468524": {
-    "jis": "23212",
-    "kana": "アイシンセイキ カブシキガイシヤ アンジヨウコウジヨウ",
-    "name": "アイシン精機　株式会社　安城工場",
-    "prefecture": "愛知県",
-    "city": "安城市",
-    "neighborhood": "三河安城町",
-    "banchi": "1丁目11番地2",
-    "postal_code": "4468524",
-    "old_code": "446  ",
-    "post_office": "安城",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "アイチケン",
-    "city_kana": "アンジョウシ",
-    "neighborhood_kana": "ミカワアンジョウチョウ",
-    "alternates": []
-  },
   "4468602": {
     "jis": "23212",
     "kana": "アイチケン コウセイノウギヨウキヨウドウクミアイレンゴウカイ アンジヨウコウセイビヨウイン",
     "name": "愛知県　厚生農業協同組合連合会　安城更生病院",
     "prefecture": "愛知県",
     "city": "安城市",
     "neighborhood": "安城町",
@@ -286301,14 +286281,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "アンジョウシ",
     "neighborhood_kana": "シンメイチョウ",
     "alternates": []
   },
+  "4468524": {
+    "jis": "23212",
+    "kana": "カブシキガイシヤ アイシン アンジヨウコウジヨウ",
+    "name": "株式会社　アイシン　安城工場",
+    "prefecture": "愛知県",
+    "city": "安城市",
+    "neighborhood": "三河安城町",
+    "banchi": "1丁目11番地2",
+    "postal_code": "4468524",
+    "old_code": "446  ",
+    "post_office": "安城",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "アイチケン",
+    "city_kana": "アンジョウシ",
+    "neighborhood_kana": "ミカワアンジョウチョウ",
+    "alternates": []
+  },
   "4468504": {
     "jis": "23212",
     "kana": "カブシキガイシヤ イノアツクコ-ポレ-シヨン アンジヨウジギヨウシヨ",
     "name": "株式会社　イノアックコーポレーション　安城事業所",
     "prefecture": "愛知県",
     "city": "安城市",
     "neighborhood": "今池町",
@@ -287272,26 +287271,26 @@
     "prefecture_kana": "アイチケン",
     "city_kana": "ニシオシ",
     "neighborhood_kana": "シモマチ",
     "alternates": []
   },
   "4438555": {
     "jis": "23214",
-    "kana": "アイシン・エイ・ダブリユ カブシキガイシヤ ガマゴオリコウジヨウ",
-    "name": "アイシン・エイ・ダブリュ　株式会社　蒲郡工場",
+    "kana": "カブシキガイシヤ アイシン ガマゴオリコウジヨウ",
+    "name": "株式会社　アイシン　蒲郡工場",
     "prefecture": "愛知県",
     "city": "蒲郡市",
     "neighborhood": "浜町",
     "banchi": "24番3",
     "postal_code": "4438555",
     "old_code": "443  ",
     "post_office": "蒲郡",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "アイチケン",
     "city_kana": "ガマゴオリシ",
     "neighborhood_kana": "ハマチョウ",
     "alternates": []
   },
   "4438588": {
     "jis": "23214",
@@ -288771,14 +288770,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
+  "4858566": {
+    "jis": "23219",
+    "kana": "ニホンガイシ カブシキガイシヤ コマキジギヨウシヨ",
+    "name": "日本ガイシ　株式会社　小牧事業所",
+    "prefecture": "愛知県",
+    "city": "小牧市",
+    "neighborhood": "大字二重堀",
+    "banchi": "字田神1155",
+    "postal_code": "4858566",
+    "old_code": "485  ",
+    "post_office": "小牧",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "",
+    "city_kana": "",
+    "neighborhood_kana": "",
+    "alternates": []
+  },
   "4858505": {
     "jis": "23219",
     "kana": "マルビシコウギヨウ カブシキガイシヤ",
     "name": "丸菱工業　株式会社",
     "prefecture": "愛知県",
     "city": "小牧市",
     "neighborhood": "大字本庄",
@@ -290000,15 +290018,15 @@
     "neighborhood": "森岡町",
     "banchi": "7丁目426番地",
     "postal_code": "4748710",
     "old_code": "474  ",
     "post_office": "大府",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "アイチケン",
     "city_kana": "オオブシ",
     "neighborhood_kana": "モリオカチョウ",
     "alternates": []
   },
   "4748510": {
     "jis": "23223",
@@ -298724,15 +298742,15 @@
     "neighborhood": "白木町",
     "banchi": "字押之尾60番37",
     "postal_code": "5190194",
     "old_code": "51901",
     "post_office": "亀山",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ミエケン",
     "city_kana": "カメヤマシ",
     "neighborhood_kana": "シラキチョウ",
     "alternates": []
   },
   "5190196": {
     "jis": "24210",
@@ -302104,42 +302122,23 @@
     "name": "野洲市　市民サービスセンター",
     "prefecture": "滋賀県",
     "city": "野洲市",
     "neighborhood": "西河原",
     "banchi": "2400番地",
     "postal_code": "5202492",
     "old_code": "52024",
-    "post_office": "中主",
+    "post_office": "野洲",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "シガケン",
     "city_kana": "ヤスシ",
     "neighborhood_kana": "ニシガワラ",
     "alternates": []
   },
-  "5240292": {
-    "jis": "25210",
-    "kana": "カブシキガイシヤ アユヤ",
-    "name": "株式会社　鮎家",
-    "prefecture": "滋賀県",
-    "city": "野洲市",
-    "neighborhood": "吉川",
-    "banchi": "4187番地",
-    "postal_code": "5240292",
-    "old_code": "52402",
-    "post_office": "幸津川",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "シガケン",
-    "city_kana": "ヤスシ",
-    "neighborhood_kana": "ヨシカワ",
-    "alternates": []
-  },
   "5203182": {
     "jis": "25211",
     "kana": "カブシキガイシヤ エム・エス・コミユニケ-シヨンズ オオサカブツリユウブ ブツリユウセンタ-",
     "name": "株式会社　エム・エス・コミュニケーションズ　大阪物流部　物流センター",
     "prefecture": "滋賀県",
     "city": "湖南市",
     "neighborhood": "石部口",
@@ -302647,26 +302646,26 @@
     "prefecture_kana": "シガケン",
     "city_kana": "ヒガシオウミシ",
     "neighborhood_kana": "ヨウカイチミドリマチ",
     "alternates": []
   },
   "5278555": {
     "jis": "25213",
-    "kana": "キヨウセラ カブシキガイシヤ シガヨウカイチコウジヨウ",
-    "name": "京セラ　株式会社　滋賀八日市工場",
+    "kana": "キヨウセラ カブシキガイシヤ シガヒガシオウミコウジヨウ ダイイチブロツク",
+    "name": "京セラ　株式会社　滋賀東近江工場　第１ブロック",
     "prefecture": "滋賀県",
     "city": "東近江市",
     "neighborhood": "蛇溝町",
-    "banchi": "長谷野1166番地の6",
+    "banchi": "1166-6",
     "postal_code": "5278555",
     "old_code": "527  ",
     "post_office": "八日市",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "シガケン",
     "city_kana": "ヒガシオウミシ",
     "neighborhood_kana": "ヘビミゾチョウ",
     "alternates": []
   },
   "5278542": {
     "jis": "25213",
@@ -303008,26 +303007,26 @@
     "prefecture_kana": "シガケン",
     "city_kana": "ヒガシオウミシ",
     "neighborhood_kana": "イシドウチョウ",
     "alternates": []
   },
   "5291595": {
     "jis": "25213",
-    "kana": "キヨウセラ カブシキガイシヤ シガガモウコウジヨウ",
-    "name": "京セラ　株式会社　滋賀蒲生工場",
+    "kana": "キヨウセラ カブシキガイシヤ シガヒガシオウミコウジヨウ ダイニブロツク",
+    "name": "京セラ　株式会社　滋賀東近江工場　第２ブロック",
     "prefecture": "滋賀県",
     "city": "東近江市",
     "neighborhood": "川合町",
     "banchi": "10-1",
     "postal_code": "5291595",
     "old_code": "52915",
     "post_office": "八日市",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "シガケン",
     "city_kana": "ヒガシオウミシ",
     "neighborhood_kana": "カワイチョウ",
     "alternates": []
   },
   "5291592": {
     "jis": "25213",
@@ -315344,14 +315343,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "シロミ",
     "alternates": []
   },
+  "5408519": {
+    "jis": "27128",
+    "kana": "テレビオオサカ カブシキガイシヤ",
+    "name": "テレビ大阪　株式会社",
+    "prefecture": "大阪府",
+    "city": "大阪市中央区",
+    "neighborhood": "大手前",
+    "banchi": "1丁目1番7号",
+    "postal_code": "5408519",
+    "old_code": "540  ",
+    "post_office": "大阪東",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "オオサカフ",
+    "city_kana": "オオサカシチュウオウク",
+    "neighborhood_kana": "オオテマエ",
+    "alternates": []
+  },
   "5408505": {
     "jis": "27128",
     "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ",
     "name": "東京海上日動火災保険　株式会社",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
     "neighborhood": "城見",
@@ -315610,33 +315628,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "オオサカシチュウオウク",
     "neighborhood_kana": "タニマチ",
     "alternates": []
   },
-  "5408519": {
-    "jis": "27128",
-    "kana": "テレビオオサカ カブシキガイシヤ",
-    "name": "テレビ大阪　株式会社",
-    "prefecture": "大阪府",
-    "city": "大阪市中央区",
-    "neighborhood": "大手前",
-    "banchi": "1丁目2-18",
-    "postal_code": "5408519",
-    "old_code": "54019",
-    "post_office": "大阪東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "オオサカフ",
-    "city_kana": "オオサカシチュウオウク",
-    "neighborhood_kana": "オオテマエ",
-    "alternates": []
-  },
   "5408570": {
     "jis": "27128",
     "kana": "オオサカフチヨウ",
     "name": "大阪府庁",
     "prefecture": "大阪府",
     "city": "大阪市中央区",
     "neighborhood": "大手前",
@@ -320147,15 +320146,15 @@
     "neighborhood": "畠中",
     "banchi": "1丁目17-2",
     "postal_code": "5978577",
     "old_code": "597  ",
     "post_office": "貝塚",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "カイヅカシ",
     "neighborhood_kana": "ハタケナカ",
     "alternates": []
   },
   "5978515": {
     "jis": "27208",
@@ -349567,26 +349566,26 @@
     "prefecture_kana": "オカヤマケン",
     "city_kana": "タマノシ",
     "neighborhood_kana": "チッコウ",
     "alternates": []
   },
   "7068651": {
     "jis": "33204",
-    "kana": "カブシキガイシヤ ミツイイ-アンドエスホ-ルデイングスタマノソウゴウジムシヨ",
-    "name": "株式会社　三井Ｅ＆Ｓホールディングス玉野総合事務所",
+    "kana": "カブシキガイシヤ ミツイイ-アンドエスタマノソウゴウジムシヨ",
+    "name": "株式会社　三井Ｅ＆Ｓ玉野総合事務所",
     "prefecture": "岡山県",
     "city": "玉野市",
     "neighborhood": "玉",
     "banchi": "3丁目1番1号(玉野郵便局私書箱第1号)",
     "postal_code": "7068651",
     "old_code": "706  ",
     "post_office": "玉野",
     "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "タマノシ",
     "neighborhood_kana": "タマ",
     "alternates": []
   },
   "7068510": {
     "jis": "33204",
@@ -350104,21 +350103,21 @@
   "7160295": {
     "jis": "33209",
     "kana": "タカハシシカワカミチイキキヨク",
     "name": "高梁市川上地域局",
     "prefecture": "岡山県",
     "city": "高梁市",
     "neighborhood": "川上町地頭",
-    "banchi": "1819-1",
+    "banchi": "1822番地",
     "postal_code": "7160295",
     "old_code": "71602",
     "post_office": "吉備川上",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "タカハシシ",
     "neighborhood_kana": "カワカミチョウジトウ",
     "alternates": []
   },
   "7160396": {
     "jis": "33209",
@@ -360716,15 +360715,15 @@
     "neighborhood": "大須",
     "banchi": "2丁目1-1",
     "postal_code": "7358588",
     "old_code": "735  ",
     "post_office": "安芸府中",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヒロシマケン",
     "city_kana": "アキグンフチュウチョウ",
     "neighborhood_kana": "オオス",
     "alternates": []
   },
   "7358511": {
     "jis": "34302",
@@ -369585,25 +369584,25 @@
   },
   "7608545": {
     "jis": "37201",
     "kana": "カブシキガイシヤ タカマツリビングシンブンシヤ",
     "name": "株式会社　高松リビング新聞社",
     "prefecture": "香川県",
     "city": "高松市",
-    "neighborhood": "丸亀町",
-    "banchi": "8-23丸亀町グリーン東館3階",
+    "neighborhood": "古新町",
+    "banchi": "8-1高松スクエアビル2階",
     "postal_code": "7608545",
     "old_code": "760  ",
     "post_office": "高松中央",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "カガワケン",
     "city_kana": "タカマツシ",
-    "neighborhood_kana": "マルガメマチ",
+    "neighborhood_kana": "フルジンマチ",
     "alternates": []
   },
   "7608667": {
     "jis": "37201",
     "kana": "カブシキガイシヤ チユウゴクギンコウ タカマツシテン",
     "name": "株式会社　中国銀行　高松支店",
     "prefecture": "香川県",
@@ -377789,33 +377788,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "エヒメケン",
     "city_kana": "ニイハマシ",
     "neighborhood_kana": "オウジチョウ",
     "alternates": []
   },
-  "7928501": {
-    "jis": "38205",
-    "kana": "ダイワシヨウケン カブシキガイシヤ ニイハマシテン",
-    "name": "大和証券　株式会社　新居浜支店",
-    "prefecture": "愛媛県",
-    "city": "新居浜市",
-    "neighborhood": "港町",
-    "banchi": "2-10",
-    "postal_code": "7928501",
-    "old_code": "792  ",
-    "post_office": "新居浜",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "エヒメケン",
-    "city_kana": "ニイハマシ",
-    "neighborhood_kana": "ミナトマチ",
-    "alternates": []
-  },
   "7928670": {
     "jis": "38205",
     "kana": "トウヨシンヨウキンコ",
     "name": "東予信用金庫",
     "prefecture": "愛媛県",
     "city": "新居浜市",
     "neighborhood": "中須賀町",
@@ -388710,15 +388690,15 @@
     "neighborhood": "博多駅東",
     "banchi": "1丁目17番1号(コネクトスクエア博多内)",
     "postal_code": "8128542",
     "old_code": "812  ",
     "post_office": "博多北",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "フクオカシハカタク",
     "neighborhood_kana": "ハカタエキヒガシ",
     "alternates": []
   },
   "8128547": {
     "jis": "40132",
@@ -400239,21 +400219,21 @@
   "8430393": {
     "jis": "41209",
     "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ウレシノイリヨウセンタ-",
     "name": "独立行政法人　国立病院機構　嬉野医療センター",
     "prefecture": "佐賀県",
     "city": "嬉野市",
     "neighborhood": "嬉野町大字下宿",
-    "banchi": "甲4279-3",
+    "banchi": "甲4760-1",
     "postal_code": "8430393",
     "old_code": "84303",
     "post_office": "嬉野",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "8491492": {
     "jis": "41209",
@@ -400929,15 +400909,15 @@
     "neighborhood": "栄町",
     "banchi": "5-5FM長崎ビル3F",
     "postal_code": "8508505",
     "old_code": "850  ",
     "post_office": "長崎中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ナガサキケン",
     "city_kana": "ナガサキシ",
     "neighborhood_kana": "サカエマチ",
     "alternates": []
   },
   "8508545": {
     "jis": "42201",
@@ -405857,14 +405837,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "ハナバタチョウ",
     "alternates": []
   },
+  "8608688": {
+    "jis": "43101",
+    "kana": "ダイワシヨウケン カブシキガイシヤ クマモトシテン",
+    "name": "大和証券　株式会社　熊本支店",
+    "prefecture": "熊本県",
+    "city": "熊本市中央区",
+    "neighborhood": "辛島町",
+    "banchi": "5-1(熊本中央郵便局私書箱第120号)",
+    "postal_code": "8608688",
+    "old_code": "860  ",
+    "post_office": "熊本中央",
+    "type": "box",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "クマモトケン",
+    "city_kana": "クマモトシチュウオウク",
+    "neighborhood_kana": "カラシマチョウ",
+    "alternates": []
+  },
   "8608618": {
     "jis": "43101",
     "kana": "チユオウクヤクシヨ",
     "name": "中央区役所",
     "prefecture": "熊本県",
     "city": "熊本市中央区",
     "neighborhood": "手取本町",
@@ -406199,33 +406198,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "ジョウトウマチ",
     "alternates": []
   },
-  "8608688": {
-    "jis": "43101",
-    "kana": "ダイワシヨウケン カブシキガイシヤ クマモトシテン",
-    "name": "大和証券　株式会社　熊本支店",
-    "prefecture": "熊本県",
-    "city": "熊本市中央区",
-    "neighborhood": "花畑町",
-    "banchi": "12-28(熊本中央郵便局私書箱第120号)",
-    "postal_code": "8608688",
-    "old_code": "86091",
-    "post_office": "熊本中央",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "クマモトケン",
-    "city_kana": "クマモトシチュウオウク",
-    "neighborhood_kana": "ハナバタチョウ",
-    "alternates": []
-  },
   "8608605": {
     "jis": "43101",
     "kana": "ニホンセイメイホケン ソウゴガイシヤ クマモトシシヤ",
     "name": "日本生命保険　相互会社　熊本支社",
     "prefecture": "熊本県",
     "city": "熊本市中央区",
     "neighborhood": "中央街",
@@ -411143,26 +411123,26 @@
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "8700395": {
     "jis": "44201",
-    "kana": "カブシキガイシヤ ミツイイ-アンドエスマシナリ- オオイタコウジヨウ",
-    "name": "株式会社　三井Ｅ＆Ｓマシナリー　大分工場",
+    "kana": "カブシキガイシヤ ミツイイ-アンドエス オオイタジギヨウバ",
+    "name": "株式会社　三井Ｅ＆Ｓ　大分事業場",
     "prefecture": "大分県",
     "city": "大分市",
     "neighborhood": "大字日吉原",
     "banchi": "3番地",
     "postal_code": "8700395",
     "old_code": "87003",
     "post_office": "大分東",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "8700397": {
     "jis": "44201",
@@ -413231,33 +413211,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ミヤザキケン",
     "city_kana": "ミヤザキシ",
     "neighborhood_kana": "タチバナドオリニシ",
     "alternates": []
   },
-  "8808583": {
-    "jis": "45201",
-    "kana": "カブシキガイシヤ エフエムミヤザキ",
-    "name": "株式会社　エフエム宮崎",
-    "prefecture": "宮崎県",
-    "city": "宮崎市",
-    "neighborhood": "祇園",
-    "banchi": "2丁目78",
-    "postal_code": "8808583",
-    "old_code": "880  ",
-    "post_office": "宮崎中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "ミヤザキケン",
-    "city_kana": "ミヤザキシ",
-    "neighborhood_kana": "ギオン",
-    "alternates": []
-  },
   "8808550": {
     "jis": "45201",
     "kana": "カブシキガイシヤ シダグミ",
     "name": "株式会社　志多組",
     "prefecture": "宮崎県",
     "city": "宮崎市",
     "neighborhood": "高千穂通",
@@ -421118,26 +421079,26 @@
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "8919292": {
     "jis": "46534",
-    "kana": "コウクウジエイタイダイ55ケイカイグン",
-    "name": "航空自衛隊第５５警戒群",
+    "kana": "コウクウジエイタイダイ55ケイカイタイ",
+    "name": "航空自衛隊第５５警戒隊",
     "prefecture": "鹿児島県",
     "city": "大島郡知名町",
-    "neighborhood": "大字上平川",
-    "banchi": "2081-1",
+    "neighborhood": "大字瀬利覚",
+    "banchi": "3196-1",
     "postal_code": "8919292",
     "old_code": "89192",
     "post_office": "知名",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "8919295": {
     "jis": "46534",
```

### Comparing `posuto-2024.4.0/posuto/postaldata.db` & `posuto-2024.5.0/posuto/postaldata.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -20237,14 +20237,15 @@
 INSERT INTO postal_data VALUES('9660932','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660932", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "カミサンミヤマチヨシカワ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "上三宮町吉川", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','上三宮町吉川');
 INSERT INTO postal_data VALUES('9660842','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660842", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "カワシモ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "川下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','川下');
 INSERT INTO postal_data VALUES('9660851','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660851", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "キタハラ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "北原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','北原');
 INSERT INTO postal_data VALUES('9660072','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660072", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "キタマチ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "北町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','北町');
 INSERT INTO postal_data VALUES('9660006','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660006", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "キタマチカミ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "北町上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','北町上');
 INSERT INTO postal_data VALUES('9660835','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660835", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ギョウサク", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "行作", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','行作');
 INSERT INTO postal_data VALUES('9660892','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660892", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "キョウダン", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "経壇", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','経壇');
+INSERT INTO postal_data VALUES('9660897','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660897", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "キョウダンヒガシ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "経壇東", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','経壇東');
 INSERT INTO postal_data VALUES('9660874','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660874", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "クボヤシキ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "窪屋敷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','窪屋敷');
 INSERT INTO postal_data VALUES('9660022','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660022", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "クマグラマチオグニ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "熊倉町雄国", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','熊倉町雄国');
 INSERT INTO postal_data VALUES('9660024','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660024", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "クマグラマチクマグラ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "熊倉町熊倉", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','熊倉町熊倉');
 INSERT INTO postal_data VALUES('9660023','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660023", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "クマグラマチシンゴウ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "熊倉町新合", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','熊倉町新合');
 INSERT INTO postal_data VALUES('9660021','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660021", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "クマグラマチミヤコ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "熊倉町都", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','熊倉町都');
 INSERT INTO postal_data VALUES('9660923','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660923", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ケイトクマチシングウ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "慶徳町新宮", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','慶徳町新宮');
 INSERT INTO postal_data VALUES('9660922','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660922", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ケイトクマチトヨオカ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "慶徳町豊岡", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','慶徳町豊岡');
@@ -20301,15 +20302,17 @@
 INSERT INTO postal_data VALUES('9660011','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660011", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "セキシバマチセキシバ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "関柴町関柴", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','関柴町関柴');
 INSERT INTO postal_data VALUES('9660013','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660013", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "セキシバマチトヨアシ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "関柴町豊芦", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','関柴町豊芦');
 INSERT INTO postal_data VALUES('9660016','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660016", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "セキシバマチヒラバヤシ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "関柴町平林", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','関柴町平林');
 INSERT INTO postal_data VALUES('9660017','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660017", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "セキシバマチミツイ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "関柴町三津井", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','関柴町三津井');
 INSERT INTO postal_data VALUES('9660033','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660033", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "セト", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "瀬戸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','瀬戸');
 INSERT INTO postal_data VALUES('9660047','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660047", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ゼニタ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "銭田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','銭田');
 INSERT INTO postal_data VALUES('9660853','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660853", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "センガリ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "千苅", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','千苅');
+INSERT INTO postal_data VALUES('9660917','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660917", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "センガリナカミチウエ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "千苅中道上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','千苅中道上');
 INSERT INTO postal_data VALUES('9660854','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660854", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "センガリミチウエ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "千苅道上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','千苅道上');
+INSERT INTO postal_data VALUES('9660916','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660916", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "センガリミチシタ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "千苅道下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','千苅道下');
 INSERT INTO postal_data VALUES('9660064','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660064", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ソウザノミヤ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "惣座宮", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','惣座宮');
 INSERT INTO postal_data VALUES('9660055','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660055", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "ダイ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','台');
 INSERT INTO postal_data VALUES('9660855','{"jisx0402": "07208", "old_code": "966  ", "postal_code": "9660855", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "タイシドウ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "太子堂", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','太子堂');
 INSERT INTO postal_data VALUES('9694303','{"jisx0402": "07208", "old_code": "96943", "postal_code": "9694303", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "タカサトマチアガツ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "高郷町揚津", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','高郷町揚津');
 INSERT INTO postal_data VALUES('9694312','{"jisx0402": "07208", "old_code": "96943", "postal_code": "9694312", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "タカサトマチイケノハラ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "高郷町池ノ原", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','高郷町池ノ原');
 INSERT INTO postal_data VALUES('9694304','{"jisx0402": "07208", "old_code": "96943", "postal_code": "9694304", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "タカサトマチイワミ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "高郷町磐見", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','高郷町磐見');
 INSERT INTO postal_data VALUES('9694316','{"jisx0402": "07208", "old_code": "96943", "postal_code": "9694316", "prefecture_kana": "フクシマケン", "city_kana": "キタカタシ", "neighborhood_kana": "タカサトマチオオタガ", "prefecture": "福島県", "city": "喜多方市", "neighborhood": "高郷町大田賀", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福島県','喜多方市','高郷町大田賀');
@@ -24522,15 +24525,15 @@
 INSERT INTO postal_data VALUES('3000604','{"jisx0402": "08229", "old_code": "30006", "postal_code": "3000604", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カマイ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "釜井", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','釜井');
 INSERT INTO postal_data VALUES('3000522','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000522", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カマガヤマ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "蒲ケ山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','蒲ケ山');
 INSERT INTO postal_data VALUES('3000528','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000528", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カミキミヤマ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "上君山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','上君山');
 INSERT INTO postal_data VALUES('3000737','{"jisx0402": "08229", "old_code": "30007", "postal_code": "3000737", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カミスダ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "上須田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','上須田');
 INSERT INTO postal_data VALUES('3010902','{"jisx0402": "08229", "old_code": "301  ", "postal_code": "3010902", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カミネモト", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "上根本", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','上根本');
 INSERT INTO postal_data VALUES('3000732','{"jisx0402": "08229", "old_code": "30007", "postal_code": "3000732", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カミノシマ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "上之島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','上之島');
 INSERT INTO postal_data VALUES('3000643','{"jisx0402": "08229", "old_code": "30006", "postal_code": "3000643", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "カミマワタシ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "上馬渡", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','上馬渡');
-INSERT INTO postal_data VALUES('3000520','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000520", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "キミガノモリ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "君賀の森", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','君賀の森');
+INSERT INTO postal_data VALUES('3000520','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000520", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "キミガノモリ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "君賀の森", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','君賀の森');
 INSERT INTO postal_data VALUES('3000513','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000513", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "クワヤマ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "桑山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','桑山');
 INSERT INTO postal_data VALUES('3000734','{"jisx0402": "08229", "old_code": "30007", "postal_code": "3000734", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "ケッサ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "結佐", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','結佐');
 INSERT INTO postal_data VALUES('3000746','{"jisx0402": "08229", "old_code": "30007", "postal_code": "3000746", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "コウザキホンジュク", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "神崎本宿", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','神崎本宿');
 INSERT INTO postal_data VALUES('3000605','{"jisx0402": "08229", "old_code": "30006", "postal_code": "3000605", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "コウダ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "幸田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','幸田');
 INSERT INTO postal_data VALUES('3000733','{"jisx0402": "08229", "old_code": "30007", "postal_code": "3000733", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "コクノウ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "石納", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','石納');
 INSERT INTO postal_data VALUES('3000524','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000524", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "コハガ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "小羽賀", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','小羽賀');
 INSERT INTO postal_data VALUES('3000514','{"jisx0402": "08229", "old_code": "30005", "postal_code": "3000514", "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "コマツカ", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "駒塚", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','茨城県','稲敷市','駒塚');
@@ -25593,26 +25596,26 @@
 INSERT INTO postal_data VALUES('3210916','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210916", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシキノシロマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東木代町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東木代町');
 INSERT INTO postal_data VALUES('3210953','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210953", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシシュクゴウ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東宿郷", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東宿郷');
 INSERT INTO postal_data VALUES('3200062','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200062", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシタカラギチョウ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東宝木町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東宝木町');
 INSERT INTO postal_data VALUES('3200054','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200054", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシトマツリ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東戸祭", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東戸祭');
 INSERT INTO postal_data VALUES('3200021','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200021", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシハナワダ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東塙田", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東塙田');
 INSERT INTO postal_data VALUES('3210168','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210168", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシハラマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東原町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東原町');
 INSERT INTO postal_data VALUES('3210985','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210985", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東町');
-INSERT INTO postal_data VALUES('3210946','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210946", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシミネ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東峰", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東峰');
+INSERT INTO postal_data VALUES('3210946','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210946", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシミネ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東峰", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東峰');
 INSERT INTO postal_data VALUES('3210944','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210944", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシミネマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東峰町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東峰町');
 INSERT INTO postal_data VALUES('3210925','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210925", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシヤナゼ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東簗瀬", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東簗瀬');
 INSERT INTO postal_data VALUES('3210116','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210116", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒガシヨコタマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "東横田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','東横田町');
 INSERT INTO postal_data VALUES('3200832','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200832", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒノデ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "日の出", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','日の出');
 INSERT INTO postal_data VALUES('3213232','{"jisx0402": "09201", "old_code": "32132", "postal_code": "3213232", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒムロマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "氷室町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','氷室町');
 INSERT INTO postal_data VALUES('3210138','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210138", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒョウゴツカ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "兵庫塚", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','兵庫塚');
 INSERT INTO postal_data VALUES('3210156','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210156", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒョウゴツカマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "兵庫塚町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','兵庫塚町');
 INSERT INTO postal_data VALUES('3210905','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210905", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒライデコウギョウダンチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平出工業団地", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平出工業団地');
 INSERT INTO postal_data VALUES('3210901','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210901", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒライデマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平出町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平出町');
 INSERT INTO postal_data VALUES('3210918','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210918", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒラツカマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平塚町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平塚町');
-INSERT INTO postal_data VALUES('3210936','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210936", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒラマツ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平松", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平松');
+INSERT INTO postal_data VALUES('3210936','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210936", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒラマツ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平松", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平松');
 INSERT INTO postal_data VALUES('3210931','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210931", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒラマツチョウ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平松町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平松町');
 INSERT INTO postal_data VALUES('3210932','{"jisx0402": "09201", "old_code": "321  ", "postal_code": "3210932", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "ヒラマツホンチョウ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "平松本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','平松本町');
 INSERT INTO postal_data VALUES('3210342','{"jisx0402": "09201", "old_code": "32103", "postal_code": "3210342", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "フクオカマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "福岡町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','福岡町');
 INSERT INTO postal_data VALUES('3200011','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200011", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "フジミガオカ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "富士見が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','富士見が丘');
 INSERT INTO postal_data VALUES('3210146','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210146", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "フジミチョウ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "富士見町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','富士見町');
 INSERT INTO postal_data VALUES('3200804','{"jisx0402": "09201", "old_code": "320  ", "postal_code": "3200804", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "フタアラマチ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "二荒町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','二荒町');
 INSERT INTO postal_data VALUES('3210164','{"jisx0402": "09201", "old_code": "32101", "postal_code": "3210164", "prefecture_kana": "トチギケン", "city_kana": "ウツノミヤシ", "neighborhood_kana": "フタバ", "prefecture": "栃木県", "city": "宇都宮市", "neighborhood": "双葉", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','栃木県','宇都宮市','双葉');
@@ -31285,15 +31288,15 @@
 INSERT INTO postal_data VALUES('3500451','{"jisx0402": "11326", "old_code": "35004", "postal_code": "3500451", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンモロヤママチ", "neighborhood_kana": "モロホンゴウ", "prefecture": "埼玉県", "city": "入間郡毛呂山町", "neighborhood": "毛呂本郷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡毛呂山町','毛呂本郷');
 INSERT INTO postal_data VALUES('3500462','{"jisx0402": "11326", "old_code": "35004", "postal_code": "3500462", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンモロヤママチ", "neighborhood_kana": "ワカヤマ", "prefecture": "埼玉県", "city": "入間郡毛呂山町", "neighborhood": "若山", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡毛呂山町','若山');
 INSERT INTO postal_data VALUES('3500415','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500415", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "ウエノ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "上野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','上野');
 INSERT INTO postal_data VALUES('3500417','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500417", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "ウエノヒガシ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "上野東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','上野東');
 INSERT INTO postal_data VALUES('3500403','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500403", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "オオヤ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "大谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','大谷');
 INSERT INTO postal_data VALUES('3500416','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500416", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "オゴセ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "越生", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','越生');
 INSERT INTO postal_data VALUES('3500414','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500414", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "オゴセヒガシ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "越生東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','越生東');
-INSERT INTO postal_data VALUES('3500418','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500418", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "カスガ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "春日", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','春日');
+INSERT INTO postal_data VALUES('3500418','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500418", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "カスガ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "春日", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','春日');
 INSERT INTO postal_data VALUES('3500402','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500402", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "カノシタ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "鹿下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','鹿下');
 INSERT INTO postal_data VALUES('3500407','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500407", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "カミヤツ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "上谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','上谷');
 INSERT INTO postal_data VALUES('3500411','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500411", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "クロイワ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "黒岩", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','黒岩');
 INSERT INTO postal_data VALUES('3500424','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500424", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "クロヤマ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "黒山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','黒山');
 INSERT INTO postal_data VALUES('3500422','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500422", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "コスギ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "小杉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','小杉');
 INSERT INTO postal_data VALUES('3500423','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500423", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "ダイマ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "大満", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','大満');
 INSERT INTO postal_data VALUES('3500425','{"jisx0402": "11327", "old_code": "35004", "postal_code": "3500425", "prefecture_kana": "サイタマケン", "city_kana": "イルマグンオゴセマチ", "neighborhood_kana": "タツガヤ", "prefecture": "埼玉県", "city": "入間郡越生町", "neighborhood": "龍ケ谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','入間郡越生町','龍ケ谷');
@@ -50817,15 +50820,15 @@
 INSERT INTO postal_data VALUES('9230946','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230946", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アイオイマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "相生町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','相生町');
 INSERT INTO postal_data VALUES('9230967','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230967", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アオジチョウ", "prefecture": "石川県", "city": "小松市", "neighborhood": "青路町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','青路町');
 INSERT INTO postal_data VALUES('9230185','{"jisx0402": "17203", "old_code": "92301", "postal_code": "9230185", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アカゼマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "赤瀬町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','赤瀬町');
 INSERT INTO postal_data VALUES('9230187','{"jisx0402": "17203", "old_code": "92301", "postal_code": "9230187", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アガリエマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "上リ江町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','上リ江町');
 INSERT INTO postal_data VALUES('9230035','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230035", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アケボノマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "あけぼの町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','あけぼの町');
 INSERT INTO postal_data VALUES('9230953','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230953", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アサヒマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "旭町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','旭町');
 INSERT INTO postal_data VALUES('9230938','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230938", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アシダマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "芦田町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','芦田町');
-INSERT INTO postal_data VALUES('9230995','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230995", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アタカシンマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "安宅新町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','安宅新町');
+INSERT INTO postal_data VALUES('9230995','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230995", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アタカシンマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "安宅新町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','石川県','小松市','安宅新町');
 INSERT INTO postal_data VALUES('9230003','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230003", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アタカマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "安宅町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','安宅町');
 INSERT INTO postal_data VALUES('9230922','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230922", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アメヤマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "飴屋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','飴屋町');
 INSERT INTO postal_data VALUES('9230823','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230823", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アラキダマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "荒木田町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','荒木田町');
 INSERT INTO postal_data VALUES('9230078','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230078", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アラシマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "嵐町", "partial": false, "koazabanchi": true, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230078", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ナカノトウゲマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "中ノ峠町", "partial": false, "koazabanchi": true, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','石川県','小松市','嵐町');
 INSERT INTO postal_data VALUES('9230032','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230032", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アラヤマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "荒屋町", "partial": false, "koazabanchi": true, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','荒屋町');
 INSERT INTO postal_data VALUES('9230864','{"jisx0402": "17203", "old_code": "923  ", "postal_code": "9230864", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アリアケマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "有明町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','石川県','小松市','有明町');
 INSERT INTO postal_data VALUES('9230326','{"jisx0402": "17203", "old_code": "92303", "postal_code": "9230326", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アワヅオンセン", "prefecture": "石川県", "city": "小松市", "neighborhood": "粟津温泉", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "17203", "old_code": "92303", "postal_code": "9230326", "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アワヅマチ", "prefecture": "石川県", "city": "小松市", "neighborhood": "粟津町", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','石川県','小松市','粟津温泉');
@@ -83520,15 +83523,15 @@
 INSERT INTO postal_data VALUES('5700075','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700075", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ベニヤチョウ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "紅屋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','紅屋町');
 INSERT INTO postal_data VALUES('5700091','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700091", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ホクトチョウ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "北斗町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','北斗町');
 INSERT INTO postal_data VALUES('5700028','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700028", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ホンマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "本町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','本町');
 INSERT INTO postal_data VALUES('5700052','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700052", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "マツシタチョウ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "松下町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','松下町');
 INSERT INTO postal_data VALUES('5700085','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700085", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "マツマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "松町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','松町');
 INSERT INTO postal_data VALUES('5700084','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700084", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミドリマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "緑町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','緑町');
 INSERT INTO postal_data VALUES('5700045','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700045", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミナミテラカタナカドオリ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "南寺方中通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','南寺方中通');
-INSERT INTO postal_data VALUES('5700043','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700043", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミナミテラカタヒガシドオリ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "南寺方東通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','南寺方東通');
+INSERT INTO postal_data VALUES('5700043','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700043", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミナミテラカタヒガシドオリ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "南寺方東通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','南寺方東通');
 INSERT INTO postal_data VALUES('5700044','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700044", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミナミテラカタミナミドオリ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "南寺方南通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','南寺方南通');
 INSERT INTO postal_data VALUES('5700046','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700046", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ミナミテラカタキタドオリ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "南寺方北通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','南寺方北通');
 INSERT INTO postal_data VALUES('5700097','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700097", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "モモマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "桃町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','桃町');
 INSERT INTO postal_data VALUES('5700005','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700005", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヤグモナカマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "八雲中町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','八雲中町');
 INSERT INTO postal_data VALUES('5700021','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700021", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヤグモヒガシマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "八雲東町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','八雲東町');
 INSERT INTO postal_data VALUES('5700006','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700006", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヤグモニシマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "八雲西町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','八雲西町');
 INSERT INTO postal_data VALUES('5700008','{"jisx0402": "27209", "old_code": "570  ", "postal_code": "5700008", "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヤグモキタマチ", "prefecture": "大阪府", "city": "守口市", "neighborhood": "八雲北町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','大阪府','守口市','八雲北町');
@@ -92726,14 +92729,15 @@
 INSERT INTO postal_data VALUES('6408268','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408268", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "ヒロミチ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "広道", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','広道');
 INSERT INTO postal_data VALUES('6496339','{"jisx0402": "30201", "old_code": "64963", "postal_code": "6496339", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "ヒロニシ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "弘西", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','弘西');
 INSERT INTO postal_data VALUES('6408137','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408137", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フキアゲ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "吹上", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','吹上');
 INSERT INTO postal_data VALUES('6408324','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408324", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フキヤチョウ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "吹屋町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','吹屋町');
 INSERT INTO postal_data VALUES('6408401','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408401", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フクシマ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "福島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','福島');
 INSERT INTO postal_data VALUES('6408043','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408043", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フクマチ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "福町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','福町');
 INSERT INTO postal_data VALUES('6496318','{"jisx0402": "30201", "old_code": "64963", "postal_code": "6496318", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フジタ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "藤田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','藤田');
+INSERT INTO postal_data VALUES('6408454','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408454", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フジトダイ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "ふじと台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','ふじと台');
 INSERT INTO postal_data VALUES('6408068','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408068", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フタスジメ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "二筋目", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','二筋目');
 INSERT INTO postal_data VALUES('6496338','{"jisx0402": "30201", "old_code": "64963", "postal_code": "6496338", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フチュウ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "府中", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','府中');
 INSERT INTO postal_data VALUES('6408213','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408213", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フナダイクマチ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "舟大工町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','舟大工町');
 INSERT INTO postal_data VALUES('6408255','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408255", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フナヅチョウ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "舟津町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','舟津町');
 INSERT INTO postal_data VALUES('6408461','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408461", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フナドコロ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "船所", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','船所');
 INSERT INTO postal_data VALUES('6400332','{"jisx0402": "30201", "old_code": "64003", "postal_code": "6400332", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "フユノ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "冬野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','冬野');
 INSERT INTO postal_data VALUES('6408131','{"jisx0402": "30201", "old_code": "640  ", "postal_code": "6408131", "prefecture_kana": "ワカヤマケン", "city_kana": "ワカヤマシ", "neighborhood_kana": "ベザイテンチョウ", "prefecture": "和歌山県", "city": "和歌山市", "neighborhood": "弁財天丁", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','和歌山県','和歌山市','弁財天丁');
@@ -94492,14 +94496,15 @@
 INSERT INTO postal_data VALUES('6893523','{"jisx0402": "31202", "old_code": "68935", "postal_code": "6893523", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "フクマン", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "福万", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','福万');
 INSERT INTO postal_data VALUES('6830055','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830055", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "フジミチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "冨士見町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','冨士見町');
 INSERT INTO postal_data VALUES('6830025','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830025", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "フルイチ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "古市", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','古市');
 INSERT INTO postal_data VALUES('6830254','{"jisx0402": "31202", "old_code": "68302", "postal_code": "6830254", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ベッショ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "別所", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','別所');
 INSERT INTO postal_data VALUES('6830063','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830063", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ホツショウジマチ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "法勝寺町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','法勝寺町');
 INSERT INTO postal_data VALUES('6830065','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830065", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "マンノウチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "万能町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','万能町');
 INSERT INTO postal_data VALUES('6893534','{"jisx0402": "31202", "old_code": "68935", "postal_code": "6893534", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ミズハマ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "水浜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','水浜');
+INSERT INTO postal_data VALUES('6893516','{"jisx0402": "31202", "old_code": "68935", "postal_code": "6893516", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ミノリチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "みのり町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','みのり町');
 INSERT INTO postal_data VALUES('6830843','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830843", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ミハタチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "三旗町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','三旗町');
 INSERT INTO postal_data VALUES('6830034','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830034", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ミヨシ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "美吉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','美吉');
 INSERT INTO postal_data VALUES('6830017','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830017", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ムナカタ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "宗像", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','宗像');
 INSERT INTO postal_data VALUES('6830053','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830053", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "メイジチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "明治町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','明治町');
 INSERT INTO postal_data VALUES('6830035','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830035", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "メグミチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "目久美町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','目久美町');
 INSERT INTO postal_data VALUES('6830036','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830036", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ヤヨイチョウ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "弥生町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','弥生町');
 INSERT INTO postal_data VALUES('6830012','{"jisx0402": "31202", "old_code": "683  ", "postal_code": "6830012", "prefecture_kana": "トットリケン", "city_kana": "ヨナゴシ", "neighborhood_kana": "ヤワタ", "prefecture": "鳥取県", "city": "米子市", "neighborhood": "八幡", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鳥取県','米子市','八幡');
@@ -99139,16 +99144,14 @@
 INSERT INTO postal_data VALUES('7315128','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315128", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチュウオウ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市中央", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市中央');
 INSERT INTO postal_data VALUES('7315102','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315102", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウイシウチ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町石内", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町石内');
 INSERT INTO postal_data VALUES('7315104','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315104", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウカミコブカワ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町上小深川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町上小深川');
 INSERT INTO postal_data VALUES('7315105','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315105", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウシモコブカワ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町下小深川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町下小深川');
 INSERT INTO postal_data VALUES('7315151','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315151", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウカミゴウチ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町上河内", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町上河内');
 INSERT INTO postal_data VALUES('7315152','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315152", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウシモゴウチ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町下河内", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町下河内');
 INSERT INTO postal_data VALUES('7315123','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315123", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウショウワダイ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町昭和台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町昭和台');
-INSERT INTO postal_data VALUES('7315116','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315116", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウテラダ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町寺田", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315116", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤハタ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "八幡", "partial": false, "koazabanchi": false, "chome": true, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','広島県','広島市佐伯区','五日市町寺田');
-INSERT INTO postal_data VALUES('7315115','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315115", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウナカジ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町中地", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315115", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤハタヒガシ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "八幡東", "partial": false, "koazabanchi": false, "chome": true, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','広島県','広島市佐伯区','五日市町中地');
 INSERT INTO postal_data VALUES('7315121','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315121", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウミスズエン", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町美鈴園", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町美鈴園');
 INSERT INTO postal_data VALUES('7315122','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315122", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "イツカイチチョウミナガ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "五日市町皆賀", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','五日市町皆賀');
 INSERT INTO postal_data VALUES('7315135','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315135", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "カイロウエン", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "海老園", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','海老園');
 INSERT INTO postal_data VALUES('7315134','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315134", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "カイロウヤマチョウ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "海老山町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','海老山町');
 INSERT INTO postal_data VALUES('7315138','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315138", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "カイロウヤマミナミ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "海老山南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','海老山南');
 INSERT INTO postal_data VALUES('7315157','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315157", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "カンノンダイ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "観音台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','観音台');
 INSERT INTO postal_data VALUES('7315156','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315156", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "クラシゲ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "倉重", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','倉重');
@@ -99170,15 +99173,17 @@
 INSERT INTO postal_data VALUES('7315112','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315112", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ミスズガオカミナミ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "美鈴が丘南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','美鈴が丘南');
 INSERT INTO postal_data VALUES('7315124','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315124", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ミナガ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "皆賀", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','皆賀');
 INSERT INTO postal_data VALUES('7315137','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315137", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ミノリ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "美の里", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','美の里');
 INSERT INTO postal_data VALUES('7315143','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315143", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ミヤケ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "三宅", "partial": false, "koazabanchi": false, "chome": true, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315143", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ミヤケチョウ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "三宅町", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": null}','広島県','広島市佐伯区','三宅');
 INSERT INTO postal_data VALUES('7315154','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315154", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤクシガオカ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "薬師が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','薬師が丘');
 INSERT INTO postal_data VALUES('7315146','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315146", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤシロ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "屋代", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','屋代');
 INSERT INTO postal_data VALUES('7315147','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315147", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤシロチョウ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "屋代町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','屋代町');
+INSERT INTO postal_data VALUES('7315116','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315116", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤハタ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "八幡", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','八幡');
 INSERT INTO postal_data VALUES('7315117','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315117", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤハタガオカ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "八幡が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','八幡が丘');
+INSERT INTO postal_data VALUES('7315115','{"jisx0402": "34108", "old_code": "73151", "postal_code": "7315115", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ヤハタヒガシ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "八幡東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','八幡東');
 INSERT INTO postal_data VALUES('7380603','{"jisx0402": "34108", "old_code": "73806", "postal_code": "7380603", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウシモ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','湯来町下');
 INSERT INTO postal_data VALUES('7380512','{"jisx0402": "34108", "old_code": "73805", "postal_code": "7380512", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウシラサゴ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町白砂", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','湯来町白砂');
 INSERT INTO postal_data VALUES('7380513','{"jisx0402": "34108", "old_code": "73805", "postal_code": "7380513", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウスガサワ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町菅沢", "partial": true, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [{"jisx0402": "34108", "old_code": "73805", "postal_code": "7380513", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウフシダニ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町伏谷", "partial": false, "koazabanchi": false, "chome": false, "multi": true, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}], "note": "黒谷"}','広島県','広島市佐伯区','湯来町菅沢');
 INSERT INTO postal_data VALUES('7380722','{"jisx0402": "34108", "old_code": "73807", "postal_code": "7380722", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウスガサワ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町菅沢", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "その他"}','広島県','広島市佐伯区','湯来町菅沢');
 INSERT INTO postal_data VALUES('7380721','{"jisx0402": "34108", "old_code": "73807", "postal_code": "7380721", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウタダ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町多田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','湯来町多田');
 INSERT INTO postal_data VALUES('7380511','{"jisx0402": "34108", "old_code": "73805", "postal_code": "7380511", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウツヅラハラ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町葛原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','湯来町葛原');
 INSERT INTO postal_data VALUES('7380602','{"jisx0402": "34108", "old_code": "73806", "postal_code": "7380602", "prefecture_kana": "ヒロシマケン", "city_kana": "ヒロシマシサエキク", "neighborhood_kana": "ユキチョウムギタニ", "prefecture": "広島県", "city": "広島市佐伯区", "neighborhood": "湯来町麦谷", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','広島県','広島市佐伯区','湯来町麦谷');
@@ -118821,14 +118826,15 @@
 INSERT INTO postal_data VALUES('8951504','{"jisx0402": "46215", "old_code": "89515", "postal_code": "8951504", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "ケドウインチョウクロキ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "祁答院町黒木", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','祁答院町黒木');
 INSERT INTO postal_data VALUES('8951501','{"jisx0402": "46215", "old_code": "89515", "postal_code": "8951501", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "ケドウインチョウシモデ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "祁答院町下手", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','祁答院町下手');
 INSERT INTO postal_data VALUES('8950073','{"jisx0402": "46215", "old_code": "895  ", "postal_code": "8950073", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "コクブンジチョウ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "国分寺町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','国分寺町');
 INSERT INTO postal_data VALUES('8991922','{"jisx0402": "46215", "old_code": "89919", "postal_code": "8991922", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "コクラチョウ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "小倉町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','小倉町');
 INSERT INTO postal_data VALUES('8950066','{"jisx0402": "46215", "old_code": "895  ", "postal_code": "8950066", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "ゴダイチョウ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "五代町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','五代町');
 INSERT INTO postal_data VALUES('8950034','{"jisx0402": "46215", "old_code": "895  ", "postal_code": "8950034", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "コバンチャヤチョウ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "木場茶屋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','木場茶屋町');
 INSERT INTO postal_data VALUES('8950061','{"jisx0402": "46215", "old_code": "895  ", "postal_code": "8950061", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "ゴリョウシタチョウ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "御陵下町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','御陵下町');
+INSERT INTO postal_data VALUES('8991926','{"jisx0402": "46215", "old_code": "89919", "postal_code": "8991926", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "サーキュラーパーク", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "サーキュラーパーク", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','サーキュラーパーク');
 INSERT INTO postal_data VALUES('8961101','{"jisx0402": "46215", "old_code": "89611", "postal_code": "8961101", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "サトチョウサト", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "里町里", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','里町里');
 INSERT INTO postal_data VALUES('8961521','{"jisx0402": "46215", "old_code": "89615", "postal_code": "8961521", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウアオセ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町青瀬", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','下甑町青瀬');
 INSERT INTO postal_data VALUES('8961602','{"jisx0402": "46215", "old_code": "89616", "postal_code": "8961602", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウカタノウラ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町片野浦", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','下甑町片野浦');
 INSERT INTO postal_data VALUES('8961412','{"jisx0402": "46215", "old_code": "89614", "postal_code": "8961412", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウセセノウラ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町瀬々野浦", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "1700番地〜、内川内"}','鹿児島県','薩摩川内市','下甑町瀬々野浦');
 INSERT INTO postal_data VALUES('8961512','{"jisx0402": "46215", "old_code": "89615", "postal_code": "8961512", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウセセノウラ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町瀬々野浦", "partial": true, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "その他"}','鹿児島県','薩摩川内市','下甑町瀬々野浦');
 INSERT INTO postal_data VALUES('8961601','{"jisx0402": "46215", "old_code": "89616", "postal_code": "8961601", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウテウチ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町手打", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','下甑町手打');
 INSERT INTO postal_data VALUES('8961411','{"jisx0402": "46215", "old_code": "89614", "postal_code": "8961411", "prefecture_kana": "カゴシマケン", "city_kana": "サツマセンダイシ", "neighborhood_kana": "シモコシキチョウナガハマ", "prefecture": "鹿児島県", "city": "薩摩川内市", "neighborhood": "下甑町長浜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','薩摩川内市','下甑町長浜');
@@ -120651,34 +120657,33 @@
 INSERT INTO office_data VALUES('0608644','{"jis": "01101", "kana": "ホツカイドウリヨキヤクテツドウ カブシキガイシヤ", "name": "北海道旅客鉄道　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北十一条西", "banchi": "15丁目", "postal_code": "0608644", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608632','{"jis": "01101", "kana": "マエダケンセツコウギヨウ カブシキガイシヤ ホツカイドウシテン", "name": "前田建設工業　株式会社　北海道支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "7丁目1番1号井門札幌パークフロントビル8階", "postal_code": "0608632", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608505','{"jis": "01101", "kana": "マルスイサツポロチユウオウスイサン カブシキガイシヤ", "name": "丸水札幌中央水産　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北十二条西", "banchi": "20丁目2番1号", "postal_code": "0608505", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608636','{"jis": "01101", "kana": "マルベニ カブシキガイシヤ ホツカイドウシシヤ", "name": "丸紅　（株）　北海道支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条東", "banchi": "1丁目5番大通バスセンタービル1号館", "postal_code": "0608636", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608609','{"jis": "01101", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキガイシヤ", "name": "三井住友海上火災保険　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "7丁目1", "postal_code": "0608609", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608631','{"jis": "01101", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキガイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "2丁目札幌MTビル", "postal_code": "0608631", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608548','{"jis": "01101", "kana": "ミツイフドウサンリアルテイサツポロ カブシキカイシヤ", "name": "三井不動産リアルティ札幌　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北二条西", "banchi": "4丁目1番地札幌三井JPビルディング17階", "postal_code": "0608548", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ２ジョウニシ", "alternates": []}');
+INSERT INTO office_data VALUES('0608654','{"jis": "01101", "kana": "ミツビシシヨウジ カブシキガイシヤ ホツカイドウシシヤ", "name": "三菱商事　株式会社　北海道支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北二条西", "banchi": "4丁目", "postal_code": "0608654", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608503','{"jis": "01101", "kana": "メデイカルプラザサツポロ", "name": "メディカルプラザ札幌", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北五条西", "banchi": "2丁目JRタワーオフィスプラザさっぽろ8F", "postal_code": "0608503", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ５ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608625','{"jis": "01101", "kana": "ユ-エフジエイニコス カブシキガイシヤ", "name": "ＵＦＪニコス　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "4丁目1-1日本生命札幌ビル", "postal_code": "0608625", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608501','{"jis": "01101", "kana": "ホツカイドウホウソウ カブシキガイシヤ (エイチビ-シ-)", "name": "北海道放送　株式会社　（ＨＢＣ）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "5丁目", "postal_code": "0608501", "old_code": "06001", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608517','{"jis": "01101", "kana": "カブシキガイシヤ テレビホツカイドウ (テイブイエイチ)", "name": "株式会社　テレビ北海道　（ＴＶｈ）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通東", "banchi": "6丁目12", "postal_code": "0608517", "old_code": "06017", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608527','{"jis": "01101", "kana": "ホツカイドウブンカホウソウ カブシキガイシヤ (ユ-エイチビ-)", "name": "北海道文化放送　株式会社　（ＵＨＢ）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "14丁目", "postal_code": "0608527", "old_code": "06027", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608588','{"jis": "01101", "kana": "ホツカイドウチヨウ", "name": "北海道庁", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "6丁目", "postal_code": "0608588", "old_code": "06088", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608658','{"jis": "01101", "kana": "(カ) ホツカイドウケンセツシンブンシヤ", "name": "株式会社　北海道建設新聞社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北四条西", "banchi": "19丁目(札幌中央郵便局私書箱第188号)", "postal_code": "0608658", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ４ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608676','{"jis": "01101", "kana": "カブシキガイシヤ ホツカイドウギンコウ", "name": "株式会社　北海道銀行", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "4丁目1(札幌中央郵便局私書箱第76号)", "postal_code": "0608676", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608711','{"jis": "01101", "kana": "カブシキガイシヤ ホツカイドウシンブンシヤ", "name": "株式会社　北海道新聞社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "3丁目6(札幌中央郵便局私書箱第3号)", "postal_code": "0608711", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608668','{"jis": "01101", "kana": "カブシキガイシヤ マルヨイケウチ", "name": "株式会社　丸ヨ池内", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "2丁目18(札幌中央郵便局私書箱第246号)", "postal_code": "0608668", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608705','{"jis": "01101", "kana": "サツポロテレビホウソウ カブシキガイシヤ (エステイ-ブイ)", "name": "札幌テレビ放送　株式会社　（ＳＴＶ）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "8丁目1-1(札幌中央郵便局私書箱第198号)", "postal_code": "0608705", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608706','{"jis": "01101", "kana": "サツポロテレビホウソウ カブシキガイシヤ (エステイブイ)", "name": "札幌テレビ放送　株式会社　（ＳＴＶ）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "8丁目1-1(札幌中央郵便局私書箱第222号)", "postal_code": "0608706", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608707','{"jis": "01101", "kana": "サツポロテレビホウソウ カブシキガイシヤ (エステイブイ) ドサンコワイド212", "name": "札幌テレビ放送　株式会社　（ＳＴＶ）　どさんこワイド２１２", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "8丁目1-1(札幌中央郵便局私書箱第212号)", "postal_code": "0608707", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608671','{"jis": "01101", "kana": "タカハシスイサン カブシキガイシヤ", "name": "高橋水産　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北十二条西", "banchi": "20丁目1-10(札幌中央郵便局私書箱第94号)", "postal_code": "0608671", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１２ジョウニシ", "alternates": []}');
-INSERT INTO office_data VALUES('0608720','{"jis": "01101", "kana": "ノムラシヨウケン カブシキガイシヤ サツポロシテン", "name": "野村證券　株式会社　札幌支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "4丁目(札幌中央郵便局私書箱第23号)", "postal_code": "0608720", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608651','{"jis": "01101", "kana": "ホクレン ノウギヨウキヨウドウクミアイレンゴウカイ", "name": "ホクレン　農業協同組合連合会", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北四条西", "banchi": "1丁目3(札幌中央郵便局私書箱第167号)", "postal_code": "0608651", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ４ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608670','{"jis": "01101", "kana": "ホツカイドウシンヨウホシヨウキヨウカイ", "name": "北海道信用保証協会", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "14丁目1(札幌中央郵便局私書箱第21号)", "postal_code": "0608670", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608677','{"jis": "01101", "kana": "ホツカイドウデンリヨク カブシキガイシヤ", "name": "北海道電力　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通東", "banchi": "1丁目2(札幌中央郵便局私書箱第4号)", "postal_code": "0608677", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608725','{"jis": "01101", "kana": "ホツカイドウロウドウキンコ ホンブ", "name": "北海道労働金庫　本部", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "5丁目3-10(札幌中央郵便局私書箱第225号)", "postal_code": "0608725", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
-INSERT INTO office_data VALUES('0608654','{"jis": "01101", "kana": "ミツビシシヨウジ カブシキガイシヤ ホツカイドウシシヤ", "name": "三菱商事　株式会社　北海道支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北二条西", "banchi": "4丁目(札幌中央郵便局私書箱第45号)", "postal_code": "0608654", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0648503','{"jis": "01101", "kana": "アツミコウギヨウ カブシキガイシヤ", "name": "渥美工業　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南六条西", "banchi": "17丁目1番1号", "postal_code": "0648503", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ６ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0648557','{"jis": "01101", "kana": "イリヨウホウジン ケイジンカイ サツポロニシマルヤマビヨウイン", "name": "医療法人　渓仁会　札幌西円山病院", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "円山西町", "banchi": "4丁目7番25号", "postal_code": "0648557", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "マルヤマニシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('0648570','{"jis": "01101", "kana": "イリヨウホウジン サンセイカイ ミヤノモリキネンビヨウイン", "name": "医療法人　讃生会　宮の森記念病院", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "宮の森三条", "banchi": "7丁目5番25号", "postal_code": "0648570", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミヤノモリ３ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0648567','{"jis": "01101", "kana": "イリヨウホウジン シオン", "name": "医療法人　シオン", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南十四条西", "banchi": "15丁目3-1", "postal_code": "0648567", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１４ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0648536','{"jis": "01101", "kana": "イリヨウホウジンシヤダン ジソウカイ ヒラマツビヨウイン", "name": "医療法人社団　慈藻会　平松病院", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南二十二条西", "banchi": "14丁目", "postal_code": "0648536", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ２２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0648519','{"jis": "01101", "kana": "エヌテイ-テイ-テレワイズワイドサ-ビスセンタ-", "name": "ＮＴＴテレワイズ・ワイドサービスセンター", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南十四条西", "banchi": "13丁目NTT南ビル", "postal_code": "0648519", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１４ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0648610','{"jis": "01101", "kana": "カブシキカイシヤ ア-クス", "name": "株式会社　アークス", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南十三条西", "banchi": "11丁目2番32号", "postal_code": "0648610", "old_code": "064  ", "post_office": "山鼻", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１３ジョウニシ", "alternates": []}');
@@ -121849,15 +121854,14 @@
 INSERT INTO office_data VALUES('0368501','{"jis": "02202", "kana": "カブシキガイシヤ サイキ", "name": "株式会社　サイキ", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字城東中央", "banchi": "3丁目6-6", "postal_code": "0368501", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368588','{"jis": "02202", "kana": "シヤダンホウジン ヒロサキカンコウコンベンシヨンキヨウカイ", "name": "社団法人　弘前観光コンベンション協会", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字下白銀町", "banchi": "2-1", "postal_code": "0368588", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368522','{"jis": "02202", "kana": "ツガルヒロサキノウギヨウキヨウドウクミアイ", "name": "つがる弘前農業協同組合", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字城東北", "banchi": "四丁目1の1", "postal_code": "0368522", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368511','{"jis": "02202", "kana": "ツガルホケンセイカツキヨウドウクミアイ ケンセイビヨウイン", "name": "津軽保険生活協同組合　健生病院", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字扇町", "banchi": "2丁目2番2", "postal_code": "0368511", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368655','{"jis": "02202", "kana": "トウホクカガクヤクヒン カブシキガイシヤ", "name": "東北化学薬品　株式会社", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字神田", "banchi": "1丁目3-1", "postal_code": "0368655", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368503','{"jis": "02202", "kana": "トウホクジヨシタンキダイガク", "name": "東北女子短期大学", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字上瓦ケ町", "banchi": "25", "postal_code": "0368503", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368530','{"jis": "02202", "kana": "トウホクジヨシダイガク", "name": "東北女子大学", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字清原", "banchi": "1丁目1番地16", "postal_code": "0368530", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('0368555','{"jis": "02202", "kana": "トウホクデンリヨク カブシキガイシヤ ヒロサキエイギヨウシヨ", "name": "東北電力　株式会社　弘前営業所", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字本町", "banchi": "1", "postal_code": "0368555", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368777','{"jis": "02202", "kana": "トウホクデンリヨクネツトワ-ク カブシキガイシヤ ヒロサキデンリヨクセンタ-", "name": "東北電力ネットワーク　株式会社　弘前電力センター", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字本町", "banchi": "1番地", "postal_code": "0368777", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368545','{"jis": "02202", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ヒロサキビヨウイン", "name": "独立行政法人　国立病院機構　弘前病院", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字富野町", "banchi": "1番地", "postal_code": "0368545", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368538','{"jis": "02202", "kana": "ニツポンネンキンキコウ ヒロサキネンキンジムシヨ", "name": "日本年金機構　弘前年金事務所", "prefecture": "青森県", "city": "弘前市", "neighborhood": "外崎", "banchi": "5-2-6", "postal_code": "0368538", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ヒロサキシ", "neighborhood_kana": "トノサキ", "alternates": []}');
 INSERT INTO office_data VALUES('0368502','{"jis": "02202", "kana": "ハロ-ワ-クヒロサキ.ヒロサキコウキヨウシヨクギヨウアンテイシヨ", "name": "ハローワーク弘前・弘前公共職業安定所", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字南富田町", "banchi": "5-1", "postal_code": "0368502", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368689','{"jis": "02202", "kana": "ヒロサキ ゼイムシヨ", "name": "弘前　税務署", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字本町", "banchi": "2-2", "postal_code": "0368689", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368577','{"jis": "02202", "kana": "ヒロサキガクインダイガク", "name": "弘前学院大学", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字稔町", "banchi": "13-1", "postal_code": "0368577", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0368585','{"jis": "02202", "kana": "ヒロサキコウギヨウコウトウガツコウ", "name": "弘前工業高等学校", "prefecture": "青森県", "city": "弘前市", "neighborhood": "大字馬屋町", "banchi": "6-2", "postal_code": "0368585", "old_code": "036  ", "post_office": "弘前", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -121885,15 +121889,14 @@
 INSERT INTO office_data VALUES('0318570','{"jis": "02203", "kana": "カブシキガイシヤ ハチノヘパ-クホテル", "name": "株式会社　八戸パークホテル", "prefecture": "青森県", "city": "八戸市", "neighborhood": "吹上", "banchi": "1丁目15-90", "postal_code": "0318570", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "フキアゲ", "alternates": []}');
 INSERT INTO office_data VALUES('0318558','{"jis": "02203", "kana": "カブシキガイシヤ ヒグチ", "name": "株式会社　ヒグチ", "prefecture": "青森県", "city": "八戸市", "neighborhood": "城下", "banchi": "3丁目13-14", "postal_code": "0318558", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "シロシタ", "alternates": []}');
 INSERT INTO office_data VALUES('0318533','{"jis": "02203", "kana": "カブシキガイシヤ ミハルヤ", "name": "株式会社　三春屋", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字十三日町", "banchi": "13", "postal_code": "0318533", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318577','{"jis": "02203", "kana": "カブシキガイシヤ ヤマヨ", "name": "株式会社　ヤマヨ", "prefecture": "青森県", "city": "八戸市", "neighborhood": "江陽", "banchi": "4丁目10-24", "postal_code": "0318577", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "コウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('0318655','{"jis": "02203", "kana": "カブシキガイシヤ ヨシダサンギヨウ", "name": "株式会社　吉田産業", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字廿三日町", "banchi": "2", "postal_code": "0318655", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318544','{"jis": "02203", "kana": "ガツコウホウジン コウセイガクイン ホンブジムキヨク", "name": "学校法人　光星学院　本部事務局", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字美保野", "banchi": "13番地98", "postal_code": "0318544", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318507','{"jis": "02203", "kana": "コウセイガクインコウトウガツコウ", "name": "光星学院高等学校", "prefecture": "青森県", "city": "八戸市", "neighborhood": "湊高台", "banchi": "6丁目14-5", "postal_code": "0318507", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "ミナトタカダイ", "alternates": []}');
-INSERT INTO office_data VALUES('0318550','{"jis": "02203", "kana": "トウホクデンリヨク カブシキガイシヤ ハチノヘエイギヨウシヨ", "name": "東北電力　株式会社　八戸営業所", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字堤町", "banchi": "11-2", "postal_code": "0318550", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318538','{"jis": "02203", "kana": "ナガサキヤ ハチノヘテン", "name": "長崎屋　八戸店", "prefecture": "青森県", "city": "八戸市", "neighborhood": "江陽", "banchi": "2丁目14-1", "postal_code": "0318538", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "コウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('0318510','{"jis": "02203", "kana": "ハチノヘケイサツシヨ", "name": "八戸警察署", "prefecture": "青森県", "city": "八戸市", "neighborhood": "城下", "banchi": "1丁目16-25", "postal_code": "0318510", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "シロシタ", "alternates": []}');
 INSERT INTO office_data VALUES('0318501','{"jis": "02203", "kana": "ハチノヘコウギヨウダイガク", "name": "八戸工業大学", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字妙", "banchi": "字大開88-1", "postal_code": "0318501", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318505','{"jis": "02203", "kana": "ハチノヘコウギヨウダイガクダイニコウトウガツコウ", "name": "八戸工業大学第二高等学校", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字妙", "banchi": "字大開67", "postal_code": "0318505", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318686','{"jis": "02203", "kana": "ハチノヘシヤクシヨ", "name": "八戸市役所", "prefecture": "青森県", "city": "八戸市", "neighborhood": "内丸", "banchi": "1丁目1-1", "postal_code": "0318686", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アオモリケン", "city_kana": "ハチノヘシ", "neighborhood_kana": "ウチマル", "alternates": []}');
 INSERT INTO office_data VALUES('0318511','{"jis": "02203", "kana": "ハチノヘシヨウコウカイギシヨ", "name": "八戸商工会議所", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字堀端町", "banchi": "2-3", "postal_code": "0318511", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0318555','{"jis": "02203", "kana": "ハチノヘシリツ シミンビヨウイン", "name": "八戸市立　市民病院", "prefecture": "青森県", "city": "八戸市", "neighborhood": "大字田向", "banchi": "字毘沙門平1", "postal_code": "0318555", "old_code": "031  ", "post_office": "八戸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -122870,14 +122873,15 @@
 INSERT INTO office_data VALUES('9920892','{"jis": "06402", "kana": "シラタカマチヤクバ", "name": "白鷹町役場", "prefecture": "山形県", "city": "西置賜郡白鷹町", "neighborhood": "大字荒砥甲", "banchi": "833(荒砥郵便局私書箱第8号)", "postal_code": "9920892", "old_code": "99208", "post_office": "荒砥", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9990696','{"jis": "06403", "kana": "イイデマチヤクバ", "name": "飯豊町役場", "prefecture": "山形県", "city": "西置賜郡飯豊町", "neighborhood": "大字椿", "banchi": "2888", "postal_code": "9990696", "old_code": "999  ", "post_office": "萩生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9971392','{"jis": "06426", "kana": "ヤマガタケン シヨウナイソウゴウシチヨウ", "name": "山形県　庄内総合支庁", "prefecture": "山形県", "city": "東田川郡三川町", "neighborhood": "大字横山", "banchi": "字袖東19-1", "postal_code": "9971392", "old_code": "99713", "post_office": "三川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9608611','{"jis": "07201", "kana": "イツパンザイダンホウジン オオハラキネンザイダン オオハラソウゴウビヨウイン", "name": "一般財団法人　大原記念財団　大原綜合病院", "prefecture": "福島県", "city": "福島市", "neighborhood": "上町", "banchi": "6番1号(福島中央郵便局私書箱第55号)", "postal_code": "9608611", "old_code": "960  ", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ウワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608511','{"jis": "07201", "kana": "エヌイ-シ-ネツトワ-クプロダクツ カブシキガイシヤ", "name": "ＮＥＣネットワークプロダクツ　株式会社", "prefecture": "福島県", "city": "福島市", "neighborhood": "清水町", "banchi": "字一本松1-1", "postal_code": "9608511", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "シミズマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608518','{"jis": "07201", "kana": "カブシキガイシヤ テイコクデ-タバンク フクシマシテン", "name": "株式会社　帝国データバンク　福島支店", "prefecture": "福島県", "city": "福島市", "neighborhood": "大町", "banchi": "7-11明治安田生命福島ビル3階", "postal_code": "9608518", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608501','{"jis": "07201", "kana": "カブシキガイシヤ ナカゴウ", "name": "株式会社　中合", "prefecture": "福島県", "city": "福島市", "neighborhood": "栄町", "banchi": "5-1", "postal_code": "9608501", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9608603','{"jis": "07201", "kana": "カブシキガイシヤ ミズホギンコウ フクシマシテン", "name": "株式会社　みずほ銀行　福島支店", "prefecture": "福島県", "city": "福島市", "neighborhood": "置賜町", "banchi": "6番20号", "postal_code": "9608603", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オキタマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608520','{"jis": "07201", "kana": "カブシキガイシヤ ヤクルトホンシヤ フクシマコウジヨウ", "name": "株式会社　ヤクルト本社　福島工場", "prefecture": "福島県", "city": "福島市", "neighborhood": "黒岩", "banchi": "字遠沖10-1", "postal_code": "9608520", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "クロイワ", "alternates": []}');
 INSERT INTO office_data VALUES('9608580','{"jis": "07201", "kana": "カブシキガイシヤ ユアテツク フクシマシシヤ", "name": "株式会社　ユアテック　福島支社", "prefecture": "福島県", "city": "福島市", "neighborhood": "伏拝", "banchi": "字沖35-1", "postal_code": "9608580", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "フシオガミ", "alternates": []}');
 INSERT INTO office_data VALUES('9608655','{"jis": "07201", "kana": "カブシキガイシヤ ラジオフクシマ", "name": "株式会社　ラジオ福島", "prefecture": "福島県", "city": "福島市", "neighborhood": "太田町", "banchi": "13-17", "postal_code": "9608655", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オオタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608584','{"jis": "07201", "kana": "コクドコウツウシヨウ トウホクチホウセイビキヨク フクシマカセンコクドウジムシヨ", "name": "国土交通省　東北地方整備局　福島河川国道事務所", "prefecture": "福島県", "city": "福島市", "neighborhood": "黒岩", "banchi": "字榎平36", "postal_code": "9608584", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "クロイワ", "alternates": []}');
 INSERT INTO office_data VALUES('9608585','{"jis": "07201", "kana": "サクラノセイボタンキダイガク", "name": "桜の聖母短期大学", "prefecture": "福島県", "city": "福島市", "neighborhood": "花園町", "banchi": "3-6", "postal_code": "9608585", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ハナゾノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608521','{"jis": "07201", "kana": "ザイダンホウジン デンキツウシンキヨウサイカイ フクシマエイギヨウシヨ", "name": "財団法人　電気通信共済会　福島営業所", "prefecture": "福島県", "city": "福島市", "neighborhood": "北町", "banchi": "1-15", "postal_code": "9608521", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "キタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608550','{"jis": "07201", "kana": "ザイダンホウジン フクシマケン ホケンエイセイキヨウカイ", "name": "財団法人　福島県　保健衛生協会", "prefecture": "福島県", "city": "福島市", "neighborhood": "方木田", "banchi": "字水戸内19-6", "postal_code": "9608550", "old_code": "960  ", "post_office": "福島中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ホウキダ", "alternates": []}');
@@ -122946,15 +122950,14 @@
 INSERT INTO office_data VALUES('9602292','{"jis": "07201", "kana": "フクシマケンケイサツ フクシマウンテンメンキヨセンタ-", "name": "福島県警察　福島運転免許センター", "prefecture": "福島県", "city": "福島市", "neighborhood": "町庭坂", "banchi": "字大原1-1", "postal_code": "9602292", "old_code": "96022", "post_office": "庭坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "マチニワサカ", "alternates": []}');
 INSERT INTO office_data VALUES('9608670','{"jis": "07201", "kana": "フクシマケンチヨウ", "name": "福島県庁", "prefecture": "福島県", "city": "福島市", "neighborhood": "杉妻町", "banchi": "2-16(福島県庁内郵便局私書箱第1号)", "postal_code": "9608670", "old_code": "96070", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スギツマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608605','{"jis": "07201", "kana": "カブシキガイシヤ イワセシヨテン", "name": "株式会社　岩瀬書店", "prefecture": "福島県", "city": "福島市", "neighborhood": "御山", "banchi": "字中川原80-1(福島中央郵便局私書箱第84号)", "postal_code": "9608605", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('9608633','{"jis": "07201", "kana": "カブシキガイシヤ トウホウギンコウ ホンテン", "name": "株式会社　東邦銀行　本店", "prefecture": "福島県", "city": "福島市", "neighborhood": "大町", "banchi": "3-25(福島中央郵便局私書箱第33号)", "postal_code": "9608633", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608626','{"jis": "07201", "kana": "カブシキガイシヤ トウホウギンコウジムセンタ-", "name": "（株）　東邦銀行事務センター", "prefecture": "福島県", "city": "福島市", "neighborhood": "飯坂町平野", "banchi": "字桜田3-4(福島中央郵便局私書箱第26号)", "postal_code": "9608626", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "イイザカマチヒラノ", "alternates": []}');
 INSERT INTO office_data VALUES('9608625','{"jis": "07201", "kana": "カブシキガイシヤ フクシマギンコウ", "name": "株式会社　福島銀行", "prefecture": "福島県", "city": "福島市", "neighborhood": "万世町", "banchi": "2-5(福島中央郵便局私書箱第57号)", "postal_code": "9608625", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "バンセイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608602','{"jis": "07201", "kana": "カブシキガイシヤ フクシマミンポウシヤ", "name": "株式会社　福島民報社", "prefecture": "福島県", "city": "福島市", "neighborhood": "太田町", "banchi": "13-17(福島中央郵便局私書箱第1号)", "postal_code": "9608602", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オオタマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9608603','{"jis": "07201", "kana": "カブシキガイシヤ ミズホギンコウ フクシマシテン", "name": "株式会社　みずほ銀行　福島支店", "prefecture": "福島県", "city": "福島市", "neighborhood": "置賜町", "banchi": "6番20号(福島中央郵便局私書箱第41号)", "postal_code": "9608603", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "オキタマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608610','{"jis": "07201", "kana": "サトウコウギヨウ カブシキガイシヤ", "name": "佐藤工業　株式会社", "prefecture": "福島県", "city": "福島市", "neighborhood": "泉", "banchi": "字清水内1(福島中央郵便局私書箱第38号)", "postal_code": "9608610", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "イズミ", "alternates": []}');
 INSERT INTO office_data VALUES('9608651','{"jis": "07201", "kana": "ダイワシヨウケン カブシキカイシヤ フクシマシテン", "name": "大和証券　株式会社　福島支店", "prefecture": "福島県", "city": "福島市", "neighborhood": "栄町", "banchi": "11-25(福島中央郵便局私書箱第4号)", "postal_code": "9608651", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608607','{"jis": "07201", "kana": "トウホクロウドウキンコ フクシマケンホンブ", "name": "東北労働金庫　福島県本部", "prefecture": "福島県", "city": "福島市", "neighborhood": "宮町", "banchi": "3-16(福島中央郵便局私書箱第67号)", "postal_code": "9608607", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "ミヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608614','{"jis": "07201", "kana": "ニツポンギンコウ フクシマシテン", "name": "日本銀行　福島支店", "prefecture": "福島県", "city": "福島市", "neighborhood": "本町", "banchi": "6-24(福島中央郵便局私書箱第46号)", "postal_code": "9608614", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "モトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9608668','{"jis": "07201", "kana": "フクシマケン ケンポクケンセツジムシヨ", "name": "福島県　県北建設事務所", "prefecture": "福島県", "city": "福島市", "neighborhood": "杉妻町", "banchi": "5-75(福島県庁内郵便局私書箱第17号)", "postal_code": "9608668", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スギツマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608677','{"jis": "07201", "kana": "フクシマケン ケンポクチホウシンコウキヨク ケンゼイブ", "name": "福島県　県北地方振興局　県税部", "prefecture": "福島県", "city": "福島市", "neighborhood": "杉妻町", "banchi": "5-75(福島県庁内郵便局私書箱第3号)", "postal_code": "9608677", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スギツマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9608666','{"jis": "07201", "kana": "フクシマケン ジドウシヤケンゼイジムシヨ", "name": "福島県　自動車県税事務所", "prefecture": "福島県", "city": "福島市", "neighborhood": "杉妻町", "banchi": "2-16(福島県庁内郵便局私書箱第34号)", "postal_code": "9608666", "old_code": "96091", "post_office": "福島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "フクシマシ", "neighborhood_kana": "スギツマチョウ", "alternates": []}');
@@ -123005,31 +123008,31 @@
 INSERT INTO office_data VALUES('9638510','{"jis": "07203", "kana": "カブシキガイシヤ ヒタチセイサクシヨ ツウシンネツトワ-クジギヨウブ", "name": "株式会社　日立製作所　通信ネットワーク事業部", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字船場向", "banchi": "94", "postal_code": "9638510", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638660','{"jis": "07203", "kana": "カブシキガイシヤ フクシマギンコウ コオリヤマシテン", "name": "株式会社　福島銀行　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "堤下町", "banchi": "11-10(郡山中町郵便局私書箱第640号)", "postal_code": "9638660", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ツツミシタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638533','{"jis": "07203", "kana": "カブシキガイシヤ フクシマチユウオウテレビ", "name": "株式会社　福島中央テレビ", "prefecture": "福島県", "city": "郡山市", "neighborhood": "池ノ台", "banchi": "13-23", "postal_code": "9638533", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "イケノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9638535','{"jis": "07203", "kana": "カブシキガイシヤ フクシマホウソウ", "name": "株式会社　福島放送", "prefecture": "福島県", "city": "郡山市", "neighborhood": "桑野", "banchi": "4丁目3-6", "postal_code": "9638535", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "クワノ", "alternates": []}');
 INSERT INTO office_data VALUES('9638567','{"jis": "07203", "kana": "カブシキガイシヤ ミヤカワカミテン", "name": "株式会社　宮川紙店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字下亀田", "banchi": "13-2", "postal_code": "9638567", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638543','{"jis": "07203", "kana": "カブシキガイシヤ ヨ-クベニマル", "name": "株式会社　ヨークベニマル", "prefecture": "福島県", "city": "郡山市", "neighborhood": "谷島町", "banchi": "5番42号", "postal_code": "9638543", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ヤシママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638503','{"jis": "07203", "kana": "ガツコウホウジン コオリヤマカイセイガクエン コオリヤマジヨシダイガク コオリヤマジヨシダイガクタンキダイガクブ コオリヤマジヨシダイガクフゾクコウトウガツコウ コオ", "name": "学校法人　郡山開成学園　郡山女子大学　郡山女子大学短期大学部　郡山女子大学附属高等学校　郡山女子大学附属幼稚園", "prefecture": "福島県", "city": "郡山市", "neighborhood": "開成", "banchi": "3丁目25-2", "postal_code": "9638503", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "カイセイ", "alternates": []}');
+INSERT INTO office_data VALUES('9638611','{"jis": "07203", "kana": "ガツコウホウジン セイセンガクシヤ オウウダイガク", "name": "学校法人　晴川学舎　奥羽大学", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字三角堂31-1", "postal_code": "9638611", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638501','{"jis": "07203", "kana": "コウエキザイダンホウジン ホシソウゴウビヨウイン", "name": "公益財団法人　星総合病院", "prefecture": "福島県", "city": "郡山市", "neighborhood": "向河原町", "banchi": "159番1号", "postal_code": "9638501", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ムカイガワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638585','{"jis": "07203", "kana": "コウエキザイダンホウジン ユアサホウオンカイ ジユセンドウソウゴウビヨウイン", "name": "公益財団法人　湯浅報恩会　寿泉堂綜合病院", "prefecture": "福島県", "city": "郡山市", "neighborhood": "駅前", "banchi": "1丁目1-17", "postal_code": "9638585", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9638655','{"jis": "07203", "kana": "コオリヤマ ゼイムシヨ", "name": "郡山　税務署", "prefecture": "福島県", "city": "郡山市", "neighborhood": "堂前町", "banchi": "20-11", "postal_code": "9638655", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ドウマエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638610','{"jis": "07203", "kana": "コオリヤマケイサツシヨ", "name": "郡山警察署", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字城清水", "banchi": "23", "postal_code": "9638610", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638609','{"jis": "07203", "kana": "コオリヤマコウキヨウシヨクギヨウアンテイシヨ", "name": "郡山公共職業安定所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "方八町", "banchi": "2丁目1-26(郡山中町郵便局私書箱第618号)", "postal_code": "9638609", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ホウハッチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9638601','{"jis": "07203", "kana": "コオリヤマシヤクシヨ", "name": "郡山市役所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "朝日", "banchi": "1丁目23-7", "postal_code": "9638601", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アサヒ", "alternates": []}');
 INSERT INTO office_data VALUES('9638666','{"jis": "07203", "kana": "サトウ カブシキガイシヤ", "name": "佐藤　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "2-7(郡山中町郵便局私書箱第655号)", "postal_code": "9638666", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638513','{"jis": "07203", "kana": "スミトモセイメイホケン ソウゴガイシヤ フクシマシシヤ", "name": "住友生命保険　相互会社　福島支社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "清水台", "banchi": "1丁目4-7住友生命郡山清水台ビル4階", "postal_code": "9638513", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シミズダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9638560','{"jis": "07203", "kana": "セキスイハイムトウホク カブシキガイシヤ フクシマシシヤ", "name": "セキスイハイム東北　株式会社　福島支社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "島", "banchi": "2丁目50-15", "postal_code": "9638560", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シマ", "alternates": []}');
 INSERT INTO office_data VALUES('9638670','{"jis": "07203", "kana": "タカラカセイキキ カブシキガイシヤ", "name": "宝化成機器　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目62-1(郡山卸町郵便局私書箱第355号)", "postal_code": "9638670", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
 INSERT INTO office_data VALUES('9638661','{"jis": "07203", "kana": "ダイワシヨウケン カブシキガイシヤ コオリヤマシテン", "name": "大和証券　株式会社　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "10-10(郡山中町郵便局私書箱第603号)", "postal_code": "9638661", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638570','{"jis": "07203", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ フクシマシテン", "name": "東京海上日動火災保険　株式会社　福島支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "長者", "banchi": "1丁目7-20", "postal_code": "9638570", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "チョウジャ", "alternates": []}');
 INSERT INTO office_data VALUES('9638506','{"jis": "07203", "kana": "トウジルシコオリヤマセイカ カブシキガイシヤ", "name": "東印郡山青果　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富久山町久保田", "banchi": "字太郎殿前193", "postal_code": "9638506", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "フクヤママチクボタ", "alternates": []}');
 INSERT INTO office_data VALUES('9638676','{"jis": "07203", "kana": "トウホクアルフレツサ カブシキガイシヤ", "name": "東北アルフレッサ　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "喜久田町卸", "banchi": "1丁目46-1(郡山卸町郵便局私書箱第357号)", "postal_code": "9638676", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "キクタマチオロシ", "alternates": []}');
-INSERT INTO office_data VALUES('9638575','{"jis": "07203", "kana": "トウホクデンリヨク カブシキガイシヤ コオリヤマエイギヨウシヨ", "name": "東北電力　株式会社　郡山営業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "細沼町", "banchi": "1-5", "postal_code": "9638575", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ホソヌママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638551','{"jis": "07203", "kana": "ニツポンホウソウキヨウカイ フクシマホウソウキヨク コオリヤマシキヨク", "name": "日本放送協会　福島放送局　郡山支局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目5-21", "postal_code": "9638551", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}');
-INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "ニデックプレシジョン　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37(郡山郵便局私書箱第37号)", "postal_code": "9638637", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9638637','{"jis": "07203", "kana": "ニデツクプレシジヨン カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "ニデックプレシジョン　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字諏訪内37", "postal_code": "9638637", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638580','{"jis": "07203", "kana": "ニホンセイメイホケン ソウゴガイシヤ コオリヤマシシヤ", "name": "日本生命保険　相互会社　郡山支社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "駅前", "banchi": "2丁目12-2", "postal_code": "9638580", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "エキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('9638508','{"jis": "07203", "kana": "ニホンタバコサンギヨウ カブシキガイシヤ コオリヤマコウジヨウ", "name": "日本たばこ産業　株式会社　郡山工場", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字外河原", "banchi": "8-1", "postal_code": "9638508", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638556','{"jis": "07203", "kana": "パナソニツク インダストリ- カブシキガイシヤ コオリヤマジギヨウシヨ", "name": "パナソニック　インダストリー　株式会社　郡山事業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "字石塚", "banchi": "111番地", "postal_code": "9638556", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9638540','{"jis": "07203", "kana": "フクシマケンキヨウイクチヨウケンチユウキヨウイクジムシヨ", "name": "福島県教育庁県中教育事務所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": [{"jis": "07203", "kana": "フクシマケンケンチユウチホウシンコウキヨク", "name": "福島県県中地方振興局", "prefecture": "福島県", "city": "郡山市", "neighborhood": "麓山", "banchi": "1丁目1番1号", "postal_code": "9638540", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ハヤマ", "alternates": []}]}');
 INSERT INTO office_data VALUES('9638668','{"jis": "07203", "kana": "フクシマケンシヨウコウシンヨウクミアイ", "name": "福島県商工信用組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "堂前町", "banchi": "7-7(郡山中町郵便局私書箱第616号)", "postal_code": "9638668", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ドウマエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638502','{"jis": "07203", "kana": "フクシマサクラノウギヨウキヨウドウクミアイ", "name": "福島さくら農業協同組合", "prefecture": "福島県", "city": "郡山市", "neighborhood": "朝日", "banchi": "2丁目14-7", "postal_code": "9638502", "old_code": "963  ", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アサヒ", "alternates": []}');
 INSERT INTO office_data VALUES('9638664','{"jis": "07203", "kana": "フクシマシンヨウハンバイ カブシキガイシヤ", "name": "福島信用販売　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "14-26(郡山中町郵便局私書箱第628号)", "postal_code": "9638664", "old_code": "963  ", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
@@ -123056,15 +123059,14 @@
 INSERT INTO office_data VALUES('9638642','{"jis": "07203", "kana": "ニホンダイガク コウガクブ", "name": "日本大学　工学部", "prefecture": "福島県", "city": "郡山市", "neighborhood": "田村町徳定", "banchi": "字中河原1(郡山郵便局私書箱第12号)", "postal_code": "9638642", "old_code": "96311", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "タムラマチトクサダ", "alternates": []}');
 INSERT INTO office_data VALUES('9631380','{"jis": "07203", "kana": "カンポノヤドコオリヤマ", "name": "かんぽの宿郡山", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町熱海", "banchi": "3丁目198", "postal_code": "9631380", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアタミ", "alternates": []}');
 INSERT INTO office_data VALUES('9631388','{"jis": "07203", "kana": "トウホクカザイ カブシキガイシヤ", "name": "東北花材　株式会社", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町安子島", "banchi": "字薬師堂125", "postal_code": "9631388", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアコガシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9631386','{"jis": "07203", "kana": "ナカヤマシヨウジ カブシキガイシヤ コオリヤマエイギヨウシヨ", "name": "中山商事　株式会社　郡山営業所", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町安子島", "banchi": "字南原13-1", "postal_code": "9631386", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアコガシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9631387','{"jis": "07203", "kana": "ホテルハナノユ", "name": "ホテル華の湯", "prefecture": "福島県", "city": "郡山市", "neighborhood": "熱海町熱海", "banchi": "5丁目8-60", "postal_code": "9631387", "old_code": "96313", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "アタミマチアタミ", "alternates": []}');
 INSERT INTO office_data VALUES('9638622','{"jis": "07203", "kana": "カブシキガイシヤ ダイトウギンコウ", "name": "株式会社　大東銀行", "prefecture": "福島県", "city": "郡山市", "neighborhood": "中町", "banchi": "19-1(郡山郵便局私書箱第8号)", "postal_code": "9638622", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638602','{"jis": "07203", "kana": "カブシキガイシヤ トウホウギンコウ コオリヤマシテン", "name": "株式会社　東邦銀行　郡山支店", "prefecture": "福島県", "city": "郡山市", "neighborhood": "虎丸町", "banchi": "20-58(郡山郵便局私書箱第20号)", "postal_code": "9638602", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トラマルマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9638611','{"jis": "07203", "kana": "ガツコウホウジン セイセンガクシヤ オウウダイガク", "name": "学校法人　晴川学舎　奥羽大学", "prefecture": "福島県", "city": "郡山市", "neighborhood": "富田町", "banchi": "字三角堂31-1(郡山郵便局私書箱第3号)", "postal_code": "9638611", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "トミタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9638630','{"jis": "07203", "kana": "コオリヤマシンヨウキンコ", "name": "郡山信用金庫", "prefecture": "福島県", "city": "郡山市", "neighborhood": "清水台", "banchi": "2丁目13-26(郡山郵便局私書箱第6号)", "postal_code": "9638630", "old_code": "96391", "post_office": "郡山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シミズダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9638794','{"jis": "07203", "kana": "コオリヤマテン ホウジンサ-ビスブ", "name": "郡山店　法人サービス部", "prefecture": "福島県", "city": "郡山市", "neighborhood": "清水台", "banchi": "2丁目13-21", "postal_code": "9638794", "old_code": "96399", "post_office": "郡山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "コオリヤマシ", "neighborhood_kana": "シミズダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9708611','{"jis": "07204", "kana": "イワキゼイムシヨ", "name": "いわき税務署", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字菱川町6-3", "postal_code": "9708611", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708551','{"jis": "07204", "kana": "イワキメイセイダイガク", "name": "いわき明星大学", "prefecture": "福島県", "city": "いわき市", "neighborhood": "中央台飯野", "banchi": "5丁目5-1", "postal_code": "9708551", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "チュウオウダイイイノ", "alternates": []}');
 INSERT INTO office_data VALUES('9708703','{"jis": "07204", "kana": "イワキロウドウキジユンカントクシヨ", "name": "いわき労働基準監督署", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町4-11", "postal_code": "9708703", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
 INSERT INTO office_data VALUES('9708625','{"jis": "07204", "kana": "オカダデンキサンギヨウ カブシキガイシヤ", "name": "岡田電気産業　株式会社", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平谷川瀬", "banchi": "一丁目6-1(いわき郵便局私書箱第25号)", "postal_code": "9708625", "old_code": "970  ", "post_office": "いわき", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラヤガワセ", "alternates": []}');
 INSERT INTO office_data VALUES('9708511','{"jis": "07204", "kana": "カブシキカイシヤエヌテイテイヒガシニホンフクシマ イワキシテン", "name": "株式会社　ＮＴＴ東日本－福島　いわき支店", "prefecture": "福島県", "city": "いわき市", "neighborhood": "平", "banchi": "字堂根町3-2", "postal_code": "9708511", "old_code": "970  ", "post_office": "いわき", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクシマケン", "city_kana": "イワキシ", "neighborhood_kana": "タイラ", "alternates": []}');
@@ -123406,18 +123408,18 @@
 INSERT INTO office_data VALUES('3080193','{"jis": "08227", "kana": "フレクストロニクス・インタ-ナシヨナル カブシキガイシヤ", "name": "フレクストロニクス・インターナショナル　株式会社", "prefecture": "茨城県", "city": "筑西市", "neighborhood": "関舘", "banchi": "367-2", "postal_code": "3080193", "old_code": "30801", "post_office": "関城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "チクセイシ", "neighborhood_kana": "セキタテ", "alternates": []}');
 INSERT INTO office_data VALUES('3088638','{"jis": "08227", "kana": "カブシキガイシヤ エムシ-シ-", "name": "株式会社　ＭＣＣ", "prefecture": "茨城県", "city": "筑西市", "neighborhood": "乙", "banchi": "589(下館郵便局私書箱第26号)", "postal_code": "3088638", "old_code": "30891", "post_office": "下館", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "チクセイシ", "neighborhood_kana": "オツ", "alternates": []}');
 INSERT INTO office_data VALUES('3088616','{"jis": "08227", "kana": "チクセイシヤクシヨ", "name": "筑西市役所", "prefecture": "茨城県", "city": "筑西市", "neighborhood": "下中山", "banchi": "732-1(下館郵便局私書箱第16号)", "postal_code": "3088616", "old_code": "30891", "post_office": "下館", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "チクセイシ", "neighborhood_kana": "シモナカヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('3091195','{"jis": "08227", "kana": "キヨウワチユウオウビヨウイン", "name": "協和中央病院", "prefecture": "茨城県", "city": "筑西市", "neighborhood": "門井", "banchi": "1676-1", "postal_code": "3091195", "old_code": "30911", "post_office": "協和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "チクセイシ", "neighborhood_kana": "カドイ", "alternates": []}');
 INSERT INTO office_data VALUES('3091192','{"jis": "08227", "kana": "チクセイシヤクシヨ キヨウワシシヨ", "name": "筑西市役所　協和支所", "prefecture": "茨城県", "city": "筑西市", "neighborhood": "門井", "banchi": "1962-2", "postal_code": "3091192", "old_code": "30911", "post_office": "協和", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "チクセイシ", "neighborhood_kana": "カドイ", "alternates": []}');
 INSERT INTO office_data VALUES('3060595','{"jis": "08228", "kana": "バンドウシヤクシヨ サシマチヨウシヤ", "name": "坂東市役所　猿島庁舎", "prefecture": "茨城県", "city": "坂東市", "neighborhood": "山", "banchi": "2730", "postal_code": "3060595", "old_code": "30605", "post_office": "岩井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "バンドウシ", "neighborhood_kana": "ヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('3060692','{"jis": "08228", "kana": "バンドウシヤクシヨ イワイチヨウシヤ", "name": "坂東市役所　岩井庁舎", "prefecture": "茨城県", "city": "坂東市", "neighborhood": "岩井", "banchi": "4365", "postal_code": "3060692", "old_code": "30606", "post_office": "岩井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "バンドウシ", "neighborhood_kana": "イワイ", "alternates": []}');
-INSERT INTO office_data VALUES('3000595','{"jis": "08229", "kana": "イナシキシヤクシヨ", "name": "稲敷市役所", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "犬塚", "banchi": "1570-1", "postal_code": "3000595", "old_code": "30005", "post_office": "江戸崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "イヌヅカ", "alternates": []}');
+INSERT INTO office_data VALUES('3000595','{"jis": "08229", "kana": "イナシキシヤクシヨ", "name": "稲敷市役所", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "犬塚", "banchi": "1570-1", "postal_code": "3000595", "old_code": "30005", "post_office": "江戸崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "イヌヅカ", "alternates": []}');
 INSERT INTO office_data VALUES('3000593','{"jis": "08229", "kana": "イバラキケンツチウラケンゼイジムシヨ イナシキシシヨ", "name": "茨城県土浦県税事務所　稲敷支所", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "江戸崎", "banchi": "甲541", "postal_code": "3000593", "old_code": "30005", "post_office": "江戸崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3000692','{"jis": "08229", "kana": "イナシキシサクラガワコウミンカン(サクラガワチクセンタ-)", "name": "稲敷市桜川公民館（桜川地区センター）", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "須賀津", "banchi": "208", "postal_code": "3000692", "old_code": "30006", "post_office": "阿波", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "スカヅ", "alternates": []}');
-INSERT INTO office_data VALUES('3000792','{"jis": "08229", "kana": "イナシキシヤクシヨ アズマシシヨ", "name": "稲敷市役所　東支所", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "結佐", "banchi": "1545", "postal_code": "3000792", "old_code": "30007", "post_office": "阿波", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "ケッサ", "alternates": []}');
+INSERT INTO office_data VALUES('3000692','{"jis": "08229", "kana": "イナシキシサクラガワコウミンカン(サクラガワチクセンタ-)", "name": "稲敷市桜川公民館（桜川地区センター）", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "須賀津", "banchi": "208", "postal_code": "3000692", "old_code": "30006", "post_office": "阿波", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "スカヅ", "alternates": []}');
+INSERT INTO office_data VALUES('3000792','{"jis": "08229", "kana": "イナシキシヤクシヨ アズマシシヨ", "name": "稲敷市役所　東支所", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "結佐", "banchi": "1545", "postal_code": "3000792", "old_code": "30007", "post_office": "阿波", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "ケッサ", "alternates": []}');
 INSERT INTO office_data VALUES('3001492','{"jis": "08229", "kana": "イナシキシシントネコウミンカンシントネチクセンタ-", "name": "稲敷市新利根公民館（新利根地区センター）", "prefecture": "茨城県", "city": "稲敷市", "neighborhood": "伊佐津", "banchi": "3239-1", "postal_code": "3001492", "old_code": "30014", "post_office": "龍ケ崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "イナシキシ", "neighborhood_kana": "イサツ", "alternates": []}');
 INSERT INTO office_data VALUES('3000192','{"jis": "08230", "kana": "カスミガウラシソウムブカスミガウラチヨウシヤ", "name": "かすみがうら市総務部霞ケ浦庁舎", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "大和田", "banchi": "828-5", "postal_code": "3000192", "old_code": "30001", "post_office": "出島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "オオワダ", "alternates": []}');
 INSERT INTO office_data VALUES('3000193','{"jis": "08230", "kana": "カブシキガイシヤ サンキツクバリユウツウセンタ-", "name": "株式会社　三喜つくば流通センター", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "深谷", "banchi": "24-10", "postal_code": "3000193", "old_code": "30001", "post_office": "出島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "フカヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3000195','{"jis": "08230", "kana": "トウキヨウセイコウ カブシキガイシヤ ツチウラコウジヨウ", "name": "東京製綱　株式会社　土浦工場", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "宍倉", "banchi": "5707", "postal_code": "3000195", "old_code": "30001", "post_office": "出島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "シシクラ", "alternates": []}');
 INSERT INTO office_data VALUES('3158516','{"jis": "08230", "kana": "イリエコウエイ カブシキガイシヤ", "name": "入江工営　株式会社", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "上稲吉", "banchi": "字東清水2045番地3", "postal_code": "3158516", "old_code": "315  ", "post_office": "石岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "カミイナヨシ", "alternates": []}');
 INSERT INTO office_data VALUES('3158512','{"jis": "08230", "kana": "カスミガウラシヤクシヨ チヨダチヨウシヤ", "name": "かすみがうら市役所　千代田庁舎", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "上土田", "banchi": "461", "postal_code": "3158512", "old_code": "315  ", "post_office": "石岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "カミツチダ", "alternates": []}');
 INSERT INTO office_data VALUES('3158513','{"jis": "08230", "kana": "トウヨウヘイセイポリマ- カブシキガイシヤ", "name": "東洋平成ポリマー　株式会社", "prefecture": "茨城県", "city": "かすみがうら市", "neighborhood": "下稲吉", "banchi": "2591番地", "postal_code": "3158513", "old_code": "315  ", "post_office": "石岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "カスミガウラシ", "neighborhood_kana": "シモイナヨシ", "alternates": []}');
@@ -123574,14 +123576,15 @@
 INSERT INTO office_data VALUES('3268550','{"jis": "09202", "kana": "カブシキガイシヤ アシカガモ-ル", "name": "株式会社　足利モール", "prefecture": "栃木県", "city": "足利市", "neighborhood": "朝倉町", "banchi": "245-5", "postal_code": "3268550", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "アサクラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3268505','{"jis": "09202", "kana": "カブシキガイシヤ カイリンジユク", "name": "株式会社　開倫塾", "prefecture": "栃木県", "city": "足利市", "neighborhood": "堀込町", "banchi": "145", "postal_code": "3268505", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "ホリゴメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3268520','{"jis": "09202", "kana": "カブシキガイシヤ コスミツクシユツパン", "name": "株式会社　コスミック出版", "prefecture": "栃木県", "city": "足利市", "neighborhood": "葉鹿町", "banchi": "1218", "postal_code": "3268520", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "ハジカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3268585','{"jis": "09202", "kana": "カブシキガイシヤ シンエイ", "name": "株式会社　信栄", "prefecture": "栃木県", "city": "足利市", "neighborhood": "通", "banchi": "4丁目2790", "postal_code": "3268585", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "トオリ", "alternates": []}');
 INSERT INTO office_data VALUES('3268521','{"jis": "09202", "kana": "カブシキガイシヤ デンパジツケンシヤ", "name": "株式会社　電波実験社", "prefecture": "栃木県", "city": "足利市", "neighborhood": "葉鹿町", "banchi": "1218", "postal_code": "3268521", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "ハジカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3268501','{"jis": "09202", "kana": "カブシキガイシヤ レンタルノニツケン", "name": "株式会社　レンタルのニッケン", "prefecture": "栃木県", "city": "足利市", "neighborhood": "大久保町", "banchi": "282-1", "postal_code": "3268501", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "オオクボチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3268686','{"jis": "09202", "kana": "シヨウコウクミアイ チユウオウキンコ アシカガシテン", "name": "商工組合　中央金庫　足利支店", "prefecture": "栃木県", "city": "足利市", "neighborhood": "通", "banchi": "2丁目2751(足利郵便局私書箱第54号)", "postal_code": "3268686", "old_code": "326  ", "post_office": "足利", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "トオリ", "alternates": []}');
+INSERT INTO office_data VALUES('3268555','{"jis": "09202", "kana": "トチギケンアンソクドボクジムシヨ", "name": "栃木県安足土木事務所", "prefecture": "栃木県", "city": "足利市", "neighborhood": "伊勢町", "banchi": "4丁目19番地", "postal_code": "3268555", "old_code": "326  ", "post_office": "足利", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "イセチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3260395','{"jis": "09202", "kana": "サンワシヤツタ- カブシキガイシヤ", "name": "三和シャッター　株式会社", "prefecture": "栃木県", "city": "足利市", "neighborhood": "福富新町", "banchi": "768", "postal_code": "3260395", "old_code": "32603", "post_office": "福居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "フクトミシンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3260392','{"jis": "09202", "kana": "リヨウモウマルゼン カブシキガイシヤ", "name": "両毛丸善　株式会社", "prefecture": "栃木県", "city": "足利市", "neighborhood": "問屋町", "banchi": "1535-2", "postal_code": "3260392", "old_code": "32603", "post_office": "福居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "アシカガシ", "neighborhood_kana": "トンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3220692','{"jis": "09203", "kana": "トチギシヤクシヨ ニシカタソウゴウシシヨ", "name": "栃木市役所　西方総合支所", "prefecture": "栃木県", "city": "栃木市", "neighborhood": "西方町本城", "banchi": "1番地", "postal_code": "3220692", "old_code": "32206", "post_office": "楡木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "トチギシ", "neighborhood_kana": "ニシカタマチホンジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3231192','{"jis": "09203", "kana": "トチギシヤクシヨ フジオカソウゴウシシヨ", "name": "栃木市役所　藤岡総合支所", "prefecture": "栃木県", "city": "栃木市", "neighborhood": "大字藤岡町藤岡", "banchi": "1022-5", "postal_code": "3231192", "old_code": "32311", "post_office": "藤岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3288501','{"jis": "09203", "kana": "イオン カブシキガイシヤ ジヤスコ トチギテン", "name": "イオン　（株）　ジャスコ栃木店", "prefecture": "栃木県", "city": "栃木市", "neighborhood": "箱森町", "banchi": "37-9", "postal_code": "3288501", "old_code": "328  ", "post_office": "栃木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "トチギシ", "neighborhood_kana": "ハコノモリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3288555','{"jis": "09203", "kana": "イワシタシヨクヒン カブシキガイシヤ", "name": "岩下食品　株式会社", "prefecture": "栃木県", "city": "栃木市", "neighborhood": "沼和田町", "banchi": "23-5", "postal_code": "3288555", "old_code": "328  ", "post_office": "栃木", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "トチギシ", "neighborhood_kana": "ヌマワダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3288668','{"jis": "09203", "kana": "カブシキガイシヤ アシカガギンコウ トチギシテン", "name": "株式会社　足利銀行　栃木支店", "prefecture": "栃木県", "city": "栃木市", "neighborhood": "倭町", "banchi": "11-1(栃木郵便局私書箱第5号)", "postal_code": "3288668", "old_code": "328  ", "post_office": "栃木", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トチギケン", "city_kana": "トチギシ", "neighborhood_kana": "ヤマトチョウ", "alternates": []}');
@@ -123784,23 +123787,23 @@
 INSERT INTO office_data VALUES('3710292','{"jis": "10201", "kana": "マエバシシ オオゴシシヨ", "name": "前橋市　大胡支所", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "堀越町", "banchi": "1115", "postal_code": "3710292", "old_code": "37102", "post_office": "大胡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "ホリコシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3710293','{"jis": "10201", "kana": "マエバシシ カスカワシシヨ", "name": "前橋市　粕川支所", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "粕川町西田面", "banchi": "216-1", "postal_code": "3710293", "old_code": "37102", "post_office": "大胡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "カスカワマチニシタナボ", "alternates": []}');
 INSERT INTO office_data VALUES('3710294','{"jis": "10201", "kana": "マエバシシ ミヤギシシヨ", "name": "前橋市　宮城支所", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "鼻毛石町", "banchi": "1426-3", "postal_code": "3710294", "old_code": "37102", "post_office": "大胡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "ハナゲイシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3718503','{"jis": "10201", "kana": "カネコシユビヨウ カブシキガイシヤ", "name": "カネコ種苗　株式会社", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "古市町", "banchi": "1丁目50-12", "postal_code": "3718503", "old_code": "37108", "post_office": "前橋中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "フルイチマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3718611','{"jis": "10201", "kana": "カブシキガイシヤ グンマギンコウ", "name": "株式会社　群馬銀行", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "元総社町", "banchi": "194(前橋中央郵便局私書箱第12号)", "postal_code": "3718611", "old_code": "37191", "post_office": "前橋中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "モトソウジャマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3718666','{"jis": "10201", "kana": "カブシキガイシヤ ジヨウモウシンブンシヤ", "name": "株式会社　上毛新聞社", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "古市町", "banchi": "1丁目50-21(前橋中央郵便局私書箱第4号)", "postal_code": "3718666", "old_code": "37191", "post_office": "前橋中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "フルイチマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3718686','{"jis": "10201", "kana": "マエバシ ゼイムシヨ", "name": "前橋　税務署", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "大手町", "banchi": "2丁目3番地1号前橋地方合同庁舎(前橋中央郵便局私書箱第11号)", "postal_code": "3718686", "old_code": "37191", "post_office": "前橋中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "オオテマチ", "alternates": []}');
+INSERT INTO office_data VALUES('3792194','{"jis": "10201", "kana": "イツパンシヤダンホウジン グンマケントラツクキヨウカイ", "name": "一般社団法人　群馬県トラック協会", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "野中町", "banchi": "322番地1", "postal_code": "3792194", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "ノナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792180','{"jis": "10201", "kana": "カブシキガイシヤ チヨダコ-ポレ-シヨン", "name": "株式会社　チヨダコーポレーション", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "下阿内町", "banchi": "377-11", "postal_code": "3792180", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "シモアウチマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792198','{"jis": "10201", "kana": "カブシキガイシヤ フレツセイ", "name": "株式会社　フレッセイ", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "力丸町", "banchi": "491番地1", "postal_code": "3792198", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "リキマルマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792187','{"jis": "10201", "kana": "カブシキガイシヤ ベイシア", "name": "株式会社　ベイシア", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "亀里町", "banchi": "900", "postal_code": "3792187", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "カメサトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792184','{"jis": "10201", "kana": "ガツコウホウジン ヤマザキガクエン", "name": "学校法人　山崎学園", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "小屋原町", "banchi": "1145-1", "postal_code": "3792184", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "コヤハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792186','{"jis": "10201", "kana": "キヨウアイガクエンシヨウガツコウ", "name": "共愛学園小学校", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "小屋原町", "banchi": "1097-2", "postal_code": "3792186", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "コヤハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792185','{"jis": "10201", "kana": "キヨウアイガクエンチユウガクコウトウガツコウ", "name": "共愛学園中学高等学校", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "小屋原町", "banchi": "1115-3", "postal_code": "3792185", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "コヤハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792192','{"jis": "10201", "kana": "キヨウアイガクエンマエバシコクサイダイガク", "name": "共愛学園前橋国際大学", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "小屋原町", "banchi": "1154-4", "postal_code": "3792192", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "コヤハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792181','{"jis": "10201", "kana": "グンマケンセキジユウジケツエキセンタ-", "name": "群馬県赤十字血液センター", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "天川大島町", "banchi": "2丁目31-13", "postal_code": "3792181", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "アマガワオオシママチ", "alternates": []}');
-INSERT INTO office_data VALUES('3792194','{"jis": "10201", "kana": "シヤダンホウジン グンマケントラツクキヨウカイ", "name": "社団法人　群馬県トラック協会", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "野中町", "banchi": "595", "postal_code": "3792194", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "ノナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792193','{"jis": "10201", "kana": "ナイス カブシキガイシヤ マエバシイチバ", "name": "ナイス　株式会社　前橋市場", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "下大島町", "banchi": "568", "postal_code": "3792193", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "シモオオシママチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792197','{"jis": "10201", "kana": "マチダコ-ポレ-シヨン カブシキガイシヤ", "name": "マチダコーポレーション　株式会社", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "駒形町", "banchi": "618", "postal_code": "3792197", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "コマガタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3792195','{"jis": "10201", "kana": "マツクシヨクヒン カブシキガイシヤ", "name": "マック食品　株式会社", "prefecture": "群馬県", "city": "前橋市", "neighborhood": "力丸町", "banchi": "488-1", "postal_code": "3792195", "old_code": "37921", "post_office": "前橋東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "マエバシシ", "neighborhood_kana": "リキマルマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3708585','{"jis": "10202", "kana": "オキデンキコウギヨウ カブシキガイシヤ タカサキチク", "name": "沖電気工業　株式会社　高崎地区", "prefecture": "群馬県", "city": "高崎市", "neighborhood": "双葉町", "banchi": "3-1", "postal_code": "3708585", "old_code": "370  ", "post_office": "高崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "タカサキシ", "neighborhood_kana": "フタバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3708622','{"jis": "10202", "kana": "カブシキガイシヤ グンマギンコウ タカサキシテン", "name": "株式会社　群馬銀行　高崎支店", "prefecture": "群馬県", "city": "高崎市", "neighborhood": "問屋町", "banchi": "3丁目10-3(高崎郵便局私書箱第12号)", "postal_code": "3708622", "old_code": "370  ", "post_office": "高崎", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "タカサキシ", "neighborhood_kana": "トンヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3708555','{"jis": "10202", "kana": "カブシキガイシヤ スズランタカサキテン", "name": "株式会社　スズラン高崎店", "prefecture": "群馬県", "city": "高崎市", "neighborhood": "鞘町", "banchi": "1-1", "postal_code": "3708555", "old_code": "370  ", "post_office": "高崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "タカサキシ", "neighborhood_kana": "サヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3708565','{"jis": "10202", "kana": "カブシキガイシヤ タカサキタカシマヤ", "name": "株式会社　高崎高島屋", "prefecture": "群馬県", "city": "高崎市", "neighborhood": "旭町", "banchi": "45", "postal_code": "3708565", "old_code": "370  ", "post_office": "高崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "タカサキシ", "neighborhood_kana": "アサヒチョウ", "alternates": []}');
@@ -123916,14 +123919,15 @@
 INSERT INTO office_data VALUES('3778616','{"jis": "10208", "kana": "キタグンマシンヨウキンコ", "name": "北群馬信用金庫", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "石原", "banchi": "203-3(渋川郵便局私書箱第16号)", "postal_code": "3778616", "old_code": "377  ", "post_office": "渋川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イシハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3778577','{"jis": "10208", "kana": "グンマケンリツ シヨウニイリヨウセンタ-", "name": "群馬県立　小児医療センター", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "北橘町下箱田", "banchi": "779", "postal_code": "3778577", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "ホッキツマチシモハコダ", "alternates": []}');
 INSERT INTO office_data VALUES('3778555','{"jis": "10208", "kana": "ザイダンホウジン グンマケンマイゾウブンカザイチヨウサジギヨウダン", "name": "財団法人　群馬県埋蔵文化財調査事業団", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "北橘町下箱田", "banchi": "784-2", "postal_code": "3778555", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "ホッキツマチシモハコダ", "alternates": []}');
 INSERT INTO office_data VALUES('3778502','{"jis": "10208", "kana": "シブカワシ ホツキツソウゴウシシヨ", "name": "渋川市　北橘総合支所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "北橘町真壁", "banchi": "2372-1", "postal_code": "3778502", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "ホッキツマチマカベ", "alternates": []}');
 INSERT INTO office_data VALUES('3778501','{"jis": "10208", "kana": "シブカワシヤクシヨ", "name": "渋川市役所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "石原", "banchi": "80", "postal_code": "3778501", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イシハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3778567','{"jis": "10208", "kana": "シヤカイフクシホウジン メグミノソノ", "name": "社会福祉法人　恵の園", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "渋川", "banchi": "4418", "postal_code": "3778567", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "シブカワ", "alternates": []}');
 INSERT INTO office_data VALUES('3778520','{"jis": "10208", "kana": "デンキカガクコウギヨウ カブシキガイシヤ シブカワコウジヨウ", "name": "電気化学工業　株式会社　渋川工場", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "中村", "banchi": "1135", "postal_code": "3778520", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "ナカムラ", "alternates": []}');
+INSERT INTO office_data VALUES('3778566','{"jis": "10208", "kana": "トネガワスイケイサボウジムシヨ", "name": "利根川水系砂防事務所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "渋川", "banchi": "121-1", "postal_code": "3778566", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "シブカワ", "alternates": []}');
 INSERT INTO office_data VALUES('3778511','{"jis": "10208", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ニシグンマビヨウイン", "name": "独立行政法人　国立病院機構　西群馬病院", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "金井", "banchi": "2854", "postal_code": "3778511", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "カナイ", "alternates": []}');
 INSERT INTO office_data VALUES('3778588','{"jis": "10208", "kana": "ニツポンネンキンキコウ シブカワネンキンジムシヨ", "name": "日本年金機構　渋川年金事務所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "石原", "banchi": "143-7", "postal_code": "3778588", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イシハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3778585','{"jis": "10208", "kana": "ミナミサワケンセツ カブシキカイシヤ", "name": "南澤建設　株式会社", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "渋川", "banchi": "2070-21", "postal_code": "3778585", "old_code": "377  ", "post_office": "渋川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "シブカワ", "alternates": []}');
 INSERT INTO office_data VALUES('3770195','{"jis": "10208", "kana": "カブシキガイシヤ テンボウ", "name": "株式会社　天坊", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "伊香保町伊香保", "banchi": "396-20", "postal_code": "3770195", "old_code": "37701", "post_office": "伊香保", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イカホマチイカホ", "alternates": []}');
 INSERT INTO office_data VALUES('3770193','{"jis": "10208", "kana": "カブシキガイシヤ フクイチ", "name": "株式会社　福一", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "伊香保町伊香保", "banchi": "甲8", "postal_code": "3770193", "old_code": "37701", "post_office": "伊香保", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イカホマチイカホ", "alternates": []}');
 INSERT INTO office_data VALUES('3770192','{"jis": "10208", "kana": "シブカワシ イカホソウゴウシシヨ", "name": "渋川市　伊香保総合支所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "伊香保町伊香保", "banchi": "116-1", "postal_code": "3770192", "old_code": "37701", "post_office": "伊香保", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "イカホマチイカホ", "alternates": []}');
 INSERT INTO office_data VALUES('3770292','{"jis": "10208", "kana": "シブカワシ コモチソウゴウシシヨ", "name": "渋川市　子持総合支所", "prefecture": "群馬県", "city": "渋川市", "neighborhood": "吹屋", "banchi": "384", "postal_code": "3770292", "old_code": "37702", "post_office": "子持", "type": "office", "multiple": false, "new": false, "prefecture_kana": "グンマケン", "city_kana": "シブカワシ", "neighborhood_kana": "フキヤ", "alternates": []}');
@@ -124446,15 +124450,15 @@
 INSERT INTO office_data VALUES('3668501','{"jis": "11218", "kana": "フカヤシヤクシヨ", "name": "深谷市役所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "仲町", "banchi": "11-1(深谷郵便局私書箱第4号)", "postal_code": "3668501", "old_code": "366  ", "post_office": "深谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "ナカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3668581','{"jis": "11218", "kana": "ミツヤセイコウ カブシキガイシヤ", "name": "三矢精工　株式会社", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "大字上野台", "banchi": "割塚1400-10", "postal_code": "3668581", "old_code": "366  ", "post_office": "深谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3690293','{"jis": "11218", "kana": "サイタマコウギヨウダイガク", "name": "埼玉工業大学", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "普済寺", "banchi": "1690", "postal_code": "3690293", "old_code": "36902", "post_office": "岡部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "フサイジ", "alternates": []}');
 INSERT INTO office_data VALUES('3690297','{"jis": "11218", "kana": "ヒタチカセイ カブシキガイシヤ サイタマジギヨウシヨ", "name": "日立化成　株式会社　埼玉事業所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "岡", "banchi": "2200", "postal_code": "3690297", "old_code": "36902", "post_office": "深谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "オカ", "alternates": []}');
 INSERT INTO office_data VALUES('3690292','{"jis": "11218", "kana": "フカヤシ オカベソウゴウシシヨ", "name": "深谷市　岡部総合支所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "岡", "banchi": "2381-1", "postal_code": "3690292", "old_code": "36902", "post_office": "岡部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "オカ", "alternates": []}');
 INSERT INTO office_data VALUES('3690295','{"jis": "11218", "kana": "リケンテクノス カブシキガイシヤ", "name": "リケンテクノス　株式会社", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "岡", "banchi": "2058", "postal_code": "3690295", "old_code": "36902", "post_office": "岡部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "オカ", "alternates": []}');
 INSERT INTO office_data VALUES('3691193','{"jis": "11218", "kana": "ケ-ワイビ- カブシキガイシヤ クマガヤコウジヨウ", "name": "ＫＹＢ　株式会社　熊谷工場", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "長在家", "banchi": "2050", "postal_code": "3691193", "old_code": "36911", "post_office": "川本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "ナガザイケ", "alternates": []}');
-INSERT INTO office_data VALUES('3691192','{"jis": "11218", "kana": "フカヤシ カワモトソウゴウシシヨ", "name": "深谷市　川本総合支所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "田中", "banchi": "197", "postal_code": "3691192", "old_code": "36911", "post_office": "川本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "タナカ", "alternates": []}');
+INSERT INTO office_data VALUES('3691192','{"jis": "11218", "kana": "フカヤシ カワモトソウゴウシシヨ", "name": "深谷市　川本総合支所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "菅沼", "banchi": "401", "postal_code": "3691192", "old_code": "36911", "post_office": "川本", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "スガヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3691195','{"jis": "11218", "kana": "ヨネキユウデリカ カブシキガイシヤ", "name": "米久デリカ　株式会社", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "白草台", "banchi": "1565-15", "postal_code": "3691195", "old_code": "36911", "post_office": "川本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "シラクサダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3691293','{"jis": "11218", "kana": "フカヤシ ハナゾノソウゴウシシヨ", "name": "深谷市　花園総合支所", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "小前田", "banchi": "2345", "postal_code": "3691293", "old_code": "36912", "post_office": "寄居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "オマエダ", "alternates": []}');
 INSERT INTO office_data VALUES('3691295','{"jis": "11218", "kana": "ミツビシデンキホ-ムキキ (カブ)", "name": "三菱電機ホーム機器　（株）", "prefecture": "埼玉県", "city": "深谷市", "neighborhood": "小前田", "banchi": "1728-1", "postal_code": "3691295", "old_code": "36912", "post_office": "寄居", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "フカヤシ", "neighborhood_kana": "オマエダ", "alternates": []}');
 INSERT INTO office_data VALUES('3628501','{"jis": "11219", "kana": "アゲオシヤクシヨ", "name": "上尾市役所", "prefecture": "埼玉県", "city": "上尾市", "neighborhood": "本町", "banchi": "3丁目1-1", "postal_code": "3628501", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "アゲオシ", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3628504','{"jis": "11219", "kana": "アゲオゼイムシヨ", "name": "上尾税務署", "prefecture": "埼玉県", "city": "上尾市", "neighborhood": "大字西門前", "banchi": "577", "postal_code": "3628504", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628508','{"jis": "11219", "kana": "アマゾンアゲオエフシ-", "name": "アマゾン上尾ＦＣ", "prefecture": "埼玉県", "city": "上尾市", "neighborhood": "大字中新井", "banchi": "字前826番地5(MCUD上尾)", "postal_code": "3628508", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3628588','{"jis": "11219", "kana": "イリヨウホウジンシヤダン アイユウカイ アゲオチユウオウソウゴウビヨウイン", "name": "医療法人社団　愛友会　上尾中央総合病院", "prefecture": "埼玉県", "city": "上尾市", "neighborhood": "柏座", "banchi": "1丁目10-10", "postal_code": "3628588", "old_code": "362  ", "post_office": "上尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "アゲオシ", "neighborhood_kana": "カシワザ", "alternates": []}');
@@ -125161,26 +125165,26 @@
 INSERT INTO office_data VALUES('2995292','{"jis": "12218", "kana": "カツウラシヤクシヨ", "name": "勝浦市役所", "prefecture": "千葉県", "city": "勝浦市", "neighborhood": "新官", "banchi": "1343-1", "postal_code": "2995292", "old_code": "29952", "post_office": "勝浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カツウラシ", "neighborhood_kana": "シンカン", "alternates": []}');
 INSERT INTO office_data VALUES('2995295','{"jis": "12218", "kana": "コクサイブドウダイガク", "name": "国際武道大学", "prefecture": "千葉県", "city": "勝浦市", "neighborhood": "新官", "banchi": "841", "postal_code": "2995295", "old_code": "29952", "post_office": "勝浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カツウラシ", "neighborhood_kana": "シンカン", "alternates": []}');
 INSERT INTO office_data VALUES('2908566','{"jis": "12219", "kana": "アサヒガラス カブシキガイシヤ チバコウジヨウ", "name": "旭硝子　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "10", "postal_code": "2908566", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908510','{"jis": "12219", "kana": "アサヒガラスエンジニアリング カブシキガイシヤ", "name": "旭硝子エンジニアリング　株式会社", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "38", "postal_code": "2908510", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908501','{"jis": "12219", "kana": "イチハラシヤクシヨ", "name": "市原市役所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "国分寺台中央", "banchi": "1丁目1-1", "postal_code": "2908501", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "コクブンジダイチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('2908540','{"jis": "12219", "kana": "ウエルシアヤツキヨク カブシキガイシヤ ネツトジギヨウブ", "name": "ウエルシア薬局　株式会社　ネット事業部", "prefecture": "千葉県", "city": "市原市", "neighborhood": "南国分寺台", "banchi": "4-1-1-2F", "postal_code": "2908540", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ミナミコクブンジダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2908577','{"jis": "12219", "kana": "カブシキガイシヤ ヒノツクス", "name": "株式会社　ヒノックス", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井中央西", "banchi": "1丁目2-2", "postal_code": "2908577", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイチュウオウニシ", "alternates": []}');
+INSERT INTO office_data VALUES('2908531','{"jis": "12219", "kana": "カブシキガイシヤ ミツイイ-アンドエスチバジギヨウバ", "name": "株式会社　三井Ｅ＆Ｓ千葉事業場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "1番地", "postal_code": "2908531", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908567','{"jis": "12219", "kana": "カブシキガイシヤ レゾナツク ゴイジギヨウシヨ", "name": "株式会社　レゾナック　五井事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "14", "postal_code": "2908567", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908560','{"jis": "12219", "kana": "ケイエイチネオケム カブシキカイシヤ チバコウジヨウ", "name": "ＫＨネオケム　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "11番地1", "postal_code": "2908560", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908558','{"jis": "12219", "kana": "コスモセキユ カブシキガイシヤ チバセイユジヨ", "name": "コスモ石油　株式会社　千葉製油所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "2", "postal_code": "2908558", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908551','{"jis": "12219", "kana": "ジエイエヌシ-セキユカガク カブシキガイシヤ イチハラセイゾウシヨ", "name": "ＪＮＣ石油化学　株式会社　市原製造所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井海岸", "banchi": "5番地の1", "postal_code": "2908551", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908585','{"jis": "12219", "kana": "デイ-アイシ- カブシキガイシヤ チバコウジヨウ", "name": "ＤＩＣ　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "12", "postal_code": "2908585", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908588','{"jis": "12219", "kana": "デンキカガクコウギヨウ カブシキガイシヤ チバコウジヨウ", "name": "電気化学工業　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "6", "postal_code": "2908588", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908530','{"jis": "12219", "kana": "ニホンソウダ カブシキガイシヤ チバコウジヨウ", "name": "日本曹達　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "12-8", "postal_code": "2908530", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2908610','{"jis": "12219", "kana": "フジサツシ カブシキガイシヤ チバコウジヨウ", "name": "不二サッシ　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "13", "postal_code": "2908610", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908511','{"jis": "12219", "kana": "フジデンキシステムズ カブシキガイシヤ チバコウジヨウ", "name": "富士電機システムズ　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "7", "postal_code": "2908511", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908555','{"jis": "12219", "kana": "フルカワデンキコウギヨウ カブシキガイシヤ チバジギヨウシヨ", "name": "古河電気工業　株式会社　千葉事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "6", "postal_code": "2908555", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908503','{"jis": "12219", "kana": "マルゼンセキユカガク カブシキガイシヤ チバコウジヨウ", "name": "丸善石油化学　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "3", "postal_code": "2908503", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
-INSERT INTO office_data VALUES('2908531','{"jis": "12219", "kana": "ミツイゾウセン カブシキガイシヤ チバジギヨウシヨ", "name": "三井造船　株式会社　千葉事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "1番地", "postal_code": "2908531", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908580','{"jis": "12219", "kana": "ミヤジエンジニアリング カブシキガイシヤ", "name": "宮地エンジニアリング　株式会社", "prefecture": "千葉県", "city": "市原市", "neighborhood": "八幡海岸通", "banchi": "3番地", "postal_code": "2908580", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ヤワタカイガンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2908550','{"jis": "12219", "kana": "ユ-ビ-イ-エラストマ- カブシキガイシヤ チバコウジヨウ", "name": "ＵＢＥエラストマー　株式会社　千葉工場", "prefecture": "千葉県", "city": "市原市", "neighborhood": "五井南海岸", "banchi": "8-1", "postal_code": "2908550", "old_code": "290  ", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ゴイミナミカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2900192','{"jis": "12219", "kana": "テイキヨウヘイセイタンキダイガク", "name": "帝京平成短期大学", "prefecture": "千葉県", "city": "市原市", "neighborhood": "ちはら台西", "banchi": "6丁目19", "postal_code": "2900192", "old_code": "29001", "post_office": "市津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "チハラダイニシ", "alternates": []}');
 INSERT INTO office_data VALUES('2900193','{"jis": "12219", "kana": "テイキヨウヘイセイダイガク", "name": "帝京平成大学", "prefecture": "千葉県", "city": "市原市", "neighborhood": "潤井戸", "banchi": "2289-23", "postal_code": "2900193", "old_code": "29001", "post_office": "市津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "ウルイド", "alternates": []}');
 INSERT INTO office_data VALUES('2900194','{"jis": "12219", "kana": "ユニモチハラダイ", "name": "ｕｎｉｍｏちはら台", "prefecture": "千葉県", "city": "市原市", "neighborhood": "ちはら台西", "banchi": "3丁目4", "postal_code": "2900194", "old_code": "29001", "post_office": "市原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "チハラダイニシ", "alternates": []}');
 INSERT INTO office_data VALUES('2990194','{"jis": "12219", "kana": "イデミツエンジニアリング カブシキガイシヤ チバジギヨウシヨ", "name": "出光エンジニアリング　株式会社　千葉事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "姉崎海岸", "banchi": "2-1", "postal_code": "2990194", "old_code": "29901", "post_office": "姉崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "アネサキカイガン", "alternates": []}');
 INSERT INTO office_data VALUES('2990192','{"jis": "12219", "kana": "イデミツコウサン カブシキガイシヤ チバジギヨウシヨ", "name": "出光興産　株式会社　千葉事業所", "prefecture": "千葉県", "city": "市原市", "neighborhood": "姉崎海岸", "banchi": "2番地1", "postal_code": "2990192", "old_code": "29901", "post_office": "姉崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イチハラシ", "neighborhood_kana": "アネサキカイガン", "alternates": []}');
@@ -125217,45 +125221,45 @@
 INSERT INTO office_data VALUES('2991192','{"jis": "12225", "kana": "キミツシヤクシヨ", "name": "君津市役所", "prefecture": "千葉県", "city": "君津市", "neighborhood": "久保", "banchi": "2丁目13-1", "postal_code": "2991192", "old_code": "29911", "post_office": "君津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "キミツシ", "neighborhood_kana": "クボ", "alternates": []}');
 INSERT INTO office_data VALUES('2991195','{"jis": "12225", "kana": "ミシマコウサン カブシキガイシヤ テツコウジギヨウホンブ", "name": "三島光産　株式会社　鉄鋼事業本部", "prefecture": "千葉県", "city": "君津市", "neighborhood": "人見", "banchi": "1212", "postal_code": "2991195", "old_code": "29911", "post_office": "君津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "キミツシ", "neighborhood_kana": "ヒトミ", "alternates": []}');
 INSERT INTO office_data VALUES('2938511','{"jis": "12226", "kana": "ニツポンセイテツ カブシキガイシヤ ギジユツカイハツホンブ", "name": "日本製鉄　株式会社　技術開発本部", "prefecture": "千葉県", "city": "富津市", "neighborhood": "新富", "banchi": "20-1", "postal_code": "2938511", "old_code": "293  ", "post_office": "富津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "フッツシ", "neighborhood_kana": "シントミ", "alternates": []}');
 INSERT INTO office_data VALUES('2938506','{"jis": "12226", "kana": "フツツシヤクシヨ", "name": "富津市役所", "prefecture": "千葉県", "city": "富津市", "neighborhood": "下飯野", "banchi": "2443", "postal_code": "2938506", "old_code": "293  ", "post_office": "富津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "フッツシ", "neighborhood_kana": "シモイイノ", "alternates": []}');
 INSERT INTO office_data VALUES('2798501','{"jis": "12227", "kana": "ウラヤスシヤクシヨ", "name": "浦安市役所", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "猫実", "banchi": "1丁目1-1", "postal_code": "2798501", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ネコザネ", "alternates": []}');
 INSERT INTO office_data VALUES('2798529','{"jis": "12227", "kana": "カブシキガイシヤ イクスピアリ", "name": "株式会社　イクスピアリ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-4", "postal_code": "2798529", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798686','{"jis": "12227", "kana": "カブシキガイシヤ インシツプ", "name": "株式会社　インシップ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "高洲", "banchi": "2-4-10", "postal_code": "2798686", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "タカス", "alternates": []}');
-INSERT INTO office_data VALUES('2798504','{"jis": "12227", "kana": "カブシキガイシヤ エムテツク", "name": "株式会社　Ｍテック", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798504", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798504','{"jis": "12227", "kana": "カブシキガイシヤ エムテツク", "name": "株式会社　Ｍテック", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798504", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798532','{"jis": "12227", "kana": "カブシキガイシヤ エムビ-エム", "name": "株式会社　ＭＢＭ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1-9-2パシフィックマークス新浦安4階", "postal_code": "2798532", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798531','{"jis": "12227", "kana": "カブシキガイシヤ エムビ-エム", "name": "株式会社　ＭＢＭ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-1", "postal_code": "2798531", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798511','{"jis": "12227", "kana": "カブシキガイシヤ オリエンタルランド", "name": "株式会社　オリエンタルランド", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-1", "postal_code": "2798511", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798580','{"jis": "12227", "kana": "カブシキガイシヤ オリエンタルランド", "name": "株式会社　オリエンタルランド", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "一丁目8番1号OLC新浦安ビル", "postal_code": "2798580", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798516','{"jis": "12227", "kana": "カブシキガイシヤ オリエンタルランド・イノベ-シヨンズ", "name": "株式会社　オリエンタルランド・イノベーションズ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1-8-1OLC新浦安ビル", "postal_code": "2798516", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
-INSERT INTO office_data VALUES('2798525','{"jis": "12227", "kana": "カブシキガイシヤ オリエンタルランド・クリエイシヨンズ", "name": "株式会社　オリエンタルランド・クリエイションズ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1丁目8番1号OLC新浦安ビル4階", "postal_code": "2798525", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798525','{"jis": "12227", "kana": "カブシキガイシヤ オリエンタルランド・クリエイシヨンズ", "name": "株式会社　オリエンタルランド・クリエイションズ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1丁目8番1号OLC新浦安ビル4階", "postal_code": "2798525", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798581','{"jis": "12227", "kana": "カブシキガイシヤ グリ-ンアンドア-ツ", "name": "株式会社　グリーンアンドアーツ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "一丁目8番1号OLC新浦安ビル5階", "postal_code": "2798581", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798583','{"jis": "12227", "kana": "カブシキガイシヤ デザインフアクトリ-", "name": "株式会社　デザインファクトリー", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "一丁目8番1号OLC新浦安ビル4階", "postal_code": "2798583", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798541','{"jis": "12227", "kana": "カブシキガイシヤ パルタツク トウキヨウシシヤ", "name": "株式会社　パルタック　東京支社", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "千鳥", "banchi": "12-15", "postal_code": "2798541", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "チドリ", "alternates": []}');
 INSERT INTO office_data VALUES('2798582','{"jis": "12227", "kana": "カブシキガイシヤ フオトワ-クス", "name": "株式会社　フォトワークス", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "一丁目8番1号OLC新浦安ビル5階", "postal_code": "2798582", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
-INSERT INTO office_data VALUES('2798527','{"jis": "12227", "kana": "カブシキガイシヤ ベイフ-ドサ-ビス", "name": "株式会社　ベイフードサービス", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798527", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798527','{"jis": "12227", "kana": "カブシキガイシヤ ベイフ-ドサ-ビス", "name": "株式会社　ベイフードサービス", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798527", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798585','{"jis": "12227", "kana": "カブシキガイシヤ ホテルオ-クラトウキヨウベイ", "name": "株式会社　ホテルオークラ東京ベイ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-8", "postal_code": "2798585", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798521','{"jis": "12227", "kana": "カブシキガイシヤ マイハマコ-ポレ-シヨン", "name": "株式会社　舞浜コーポレーション", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798521", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
-INSERT INTO office_data VALUES('2798523','{"jis": "12227", "kana": "カブシキガイシヤ マイハマリゾ-トライン", "name": "株式会社　舞浜リゾートライン", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地18", "postal_code": "2798523", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798523','{"jis": "12227", "kana": "カブシキガイシヤ マイハマリゾ-トライン", "name": "株式会社　舞浜リゾートライン", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地18", "postal_code": "2798523", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798553','{"jis": "12227", "kana": "カブシキガイシヤ リ-ガルコ-ポレ-シヨン", "name": "株式会社　リーガルコーポレーション", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "2丁目1-8", "postal_code": "2798553", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
-INSERT INTO office_data VALUES('2798570','{"jis": "12227", "kana": "カブシキガイシヤ リゾ-トコスチユ-ミングサ-ビス", "name": "株式会社　リゾートコスチューミングサービス", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地18", "postal_code": "2798570", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798570','{"jis": "12227", "kana": "カブシキガイシヤ リゾ-トコスチユ-ミングサ-ビス", "name": "株式会社　リゾートコスチューミングサービス", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地18", "postal_code": "2798570", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798567','{"jis": "12227", "kana": "ガツコウホウジン リヨウトクジダイガク", "name": "学校法人　了徳寺大学", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "明海", "banchi": "23", "postal_code": "2798567", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "アケミ", "alternates": []}');
 INSERT INTO office_data VALUES('2798601','{"jis": "12227", "kana": "サラリコウボウ カブシキガイシヤ", "name": "サラリ工房　株式会社", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "今川", "banchi": "1-11-37", "postal_code": "2798601", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "イマガワ", "alternates": []}');
 INSERT INTO office_data VALUES('2798522','{"jis": "12227", "kana": "デイズニ-アンバサダ-ホテル", "name": "ディズニーアンバサダーホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地11", "postal_code": "2798522", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798558','{"jis": "12227", "kana": "トウカイダイガクフゾク ウラヤスコウトウガツコウ", "name": "東海大学付属　浦安高等学校", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "東野", "banchi": "3-11-1", "postal_code": "2798558", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒガシノ", "alternates": []}');
-INSERT INTO office_data VALUES('2798502','{"jis": "12227", "kana": "トウキヨウセレブレ-シヨンホテル(ウイツシユ)", "name": "東京セレブレーションホテル（ウィッシュ）", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "明海", "banchi": "7丁目1番地1", "postal_code": "2798502", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "アケミ", "alternates": []}');
-INSERT INTO office_data VALUES('2798503','{"jis": "12227", "kana": "トウキヨウセレブレ-シヨンホテル(デイスカバ-)", "name": "東京セレブレーションホテル（ディスカバー）", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "7丁目1番地1", "postal_code": "2798503", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
+INSERT INTO office_data VALUES('2798502','{"jis": "12227", "kana": "トウキヨウセレブレ-シヨンホテル(ウイツシユ)", "name": "東京セレブレーションホテル（ウィッシュ）", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "明海", "banchi": "7丁目1番地1", "postal_code": "2798502", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "アケミ", "alternates": []}');
+INSERT INTO office_data VALUES('2798503','{"jis": "12227", "kana": "トウキヨウセレブレ-シヨンホテル(デイスカバ-)", "name": "東京セレブレーションホテル（ディスカバー）", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "7丁目1番地1", "postal_code": "2798503", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
 INSERT INTO office_data VALUES('2798526','{"jis": "12227", "kana": "トウキヨウデイズニ-シ-・フアンタジ-スプリングスホテル", "name": "東京ディズニーシー・ファンタジースプリングスホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地2", "postal_code": "2798526", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798519','{"jis": "12227", "kana": "トウキヨウデイズニ-シ-・ホテルミラコスタ", "name": "東京ディズニーシー・ホテルミラコスタ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-13", "postal_code": "2798519", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798505','{"jis": "12227", "kana": "トウキヨウデイズニ-ランドホテル", "name": "東京ディズニーランドホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "29-1", "postal_code": "2798505", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798506','{"jis": "12227", "kana": "トウキヨウデイズニ-リゾ-ト・トイ・スト-リ-ホテル", "name": "東京ディズニーリゾート・トイ・ストーリーホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-47", "postal_code": "2798506", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798530','{"jis": "12227", "kana": "トウキヨウデンリヨク カブシキガイシヤ イチカワウラヤスエイギヨウシヨ", "name": "東京電力　株式会社　市川浦安営業所", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "1", "postal_code": "2798530", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
 INSERT INTO office_data VALUES('2798555','{"jis": "12227", "kana": "トウレ カブシキガイシヤ ダイニホンシヤ", "name": "東レ　株式会社　第２本社", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1丁目8-1", "postal_code": "2798555", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798588','{"jis": "12227", "kana": "ニホンコ-プキヨウサイセイカツキヨウドウクミアイレンゴウカイ", "name": "日本コープ共済生活協同組合連合会", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "入船", "banchi": "1丁目5-2", "postal_code": "2798588", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "イリフネ", "alternates": []}');
-INSERT INTO office_data VALUES('2798512','{"jis": "12227", "kana": "マイハマアンフイシアタ-", "name": "舞浜アンフィシアター", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地50", "postal_code": "2798512", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798512','{"jis": "12227", "kana": "マイハマアンフイシアタ-", "name": "舞浜アンフィシアター", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地50", "postal_code": "2798512", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798550','{"jis": "12227", "kana": "メイカイダイガク", "name": "明海大学", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "明海", "banchi": "8", "postal_code": "2798550", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "アケミ", "alternates": []}');
 INSERT INTO office_data VALUES('2848555','{"jis": "12228", "kana": "ヨツカイドウシヤクシヨ", "name": "四街道市役所", "prefecture": "千葉県", "city": "四街道市", "neighborhood": "鹿渡", "banchi": "無番地", "postal_code": "2848555", "old_code": "284  ", "post_office": "四街道", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ヨツカイドウシ", "neighborhood_kana": "シカワタシ", "alternates": []}');
 INSERT INTO office_data VALUES('2990297','{"jis": "12229", "kana": "アサヒカセイケミカルズ カブシキガイシヤ カワサキセイゾウシヨ チバコウジヨウ", "name": "旭化成ケミカルズ　株式会社　川崎製造所　千葉工場", "prefecture": "千葉県", "city": "袖ケ浦市", "neighborhood": "中袖", "banchi": "5-1", "postal_code": "2990297", "old_code": "29902", "post_office": "袖ケ浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ソデガウラシ", "neighborhood_kana": "ナカソデ", "alternates": []}');
 INSERT INTO office_data VALUES('2990293','{"jis": "12229", "kana": "イデミツコウサン カブシキガイシヤ センシンギジユツケンキユウジヨ", "name": "出光興産　株式会社　先進技術研究所", "prefecture": "千葉県", "city": "袖ケ浦市", "neighborhood": "上泉", "banchi": "1280", "postal_code": "2990293", "old_code": "29902", "post_office": "袖ケ浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ソデガウラシ", "neighborhood_kana": "カミイズミ", "alternates": []}');
 INSERT INTO office_data VALUES('2990296','{"jis": "12229", "kana": "カブシキガイシヤ エバラセイサクシヨ ソデガウラジギヨウシヨ", "name": "株式会社　荏原製作所　袖ヶ浦事業所", "prefecture": "千葉県", "city": "袖ケ浦市", "neighborhood": "中袖", "banchi": "20-1", "postal_code": "2990296", "old_code": "29902", "post_office": "袖ケ浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ソデガウラシ", "neighborhood_kana": "ナカソデ", "alternates": []}');
 INSERT INTO office_data VALUES('2990298','{"jis": "12229", "kana": "シヤカイフクシホウジン チバケンシヤカイフクシジギヨウダン", "name": "社会福祉法人　千葉県社会福祉事業団", "prefecture": "千葉県", "city": "袖ケ浦市", "neighborhood": "蔵波", "banchi": "3108-1", "postal_code": "2990298", "old_code": "29902", "post_office": "袖ケ浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ソデガウラシ", "neighborhood_kana": "クラナミ", "alternates": []}');
 INSERT INTO office_data VALUES('2990295','{"jis": "12229", "kana": "スミトモカガク カブシキカイシヤ チバコウジヨウ", "name": "住友化学　株式会社　千葉工場", "prefecture": "千葉県", "city": "袖ケ浦市", "neighborhood": "北袖", "banchi": "9-1", "postal_code": "2990295", "old_code": "29902", "post_office": "袖ケ浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ソデガウラシ", "neighborhood_kana": "キタソデ", "alternates": []}');
@@ -125447,15 +125451,15 @@
 INSERT INTO office_data VALUES('1008448','{"jis": "13101", "kana": "ザイダンホウジン キギヨウケイエイツウシンガクイン", "name": "財団法人　企業経営通信学院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "有楽町", "banchi": "2丁目10-1東京交通会館ビル9F", "postal_code": "1008448", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ユウラクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008135','{"jis": "13101", "kana": "ザイダンホウジン コクゴサクブンキヨウイクケンキユウジヨ", "name": "財団法人　国語作文教育研究所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "1-1-1パレスサイドビル", "postal_code": "1008135", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1008917','{"jis": "13101", "kana": "ザイダンホウジン ゼンコクロウジンクラブレンゴウカイ", "name": "財団法人　全国老人クラブ連合会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3丁目3-2新霞が関ビル5階", "postal_code": "1008917", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1008139','{"jis": "13101", "kana": "ザイダンホウジン テイシンキヨウカイ", "name": "財団法人　逓信協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "2丁目3-1", "postal_code": "1008139", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008940','{"jis": "13101", "kana": "ザイムシヨウ", "name": "財務省", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3丁目1-1", "postal_code": "1008940", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1008931','{"jis": "13101", "kana": "シゲンエネルギ-チヨウ", "name": "資源エネルギー庁", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "1丁目3-1", "postal_code": "1008931", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1008132','{"jis": "13101", "kana": "シテイグル-プ・サ-ビス・ジヤパン カブシキガイシヤ", "name": "シティグループ・サービス・ジャパン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号大手町パークビルディング", "postal_code": "1008132", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": [{"jis": "13101", "kana": "シテイグル-プ・ジヤパン・ホ-ルデイングス ゴウドウガイシヤ", "name": "シティグループ・ジャパン・ホールディングス　合同会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号大手町パークビルディング", "postal_code": "1008132", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}, {"jis": "13101", "kana": "シテイグル-プシヨウケン カブシキガイシヤ", "name": "シティグループ証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号大手町パークビルディング", "postal_code": "1008132", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}, {"jis": "13101", "kana": "シテイバンク、エヌ・エイ トウキヨウシテン", "name": "シティバンク、エヌ・エイ　東京支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号大手町パークビルディング", "postal_code": "1008132", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}]}');
-INSERT INTO office_data VALUES('1008503','{"jis": "13101", "kana": "シバウラキカイ カブシキガイシヤ", "name": "芝浦機械　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内幸町", "banchi": "二丁目2番2号", "postal_code": "1008503", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチサイワイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1008503','{"jis": "13101", "kana": "シバウラキカイ カブシキガイシヤ", "name": "芝浦機械　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内幸町", "banchi": "二丁目2番2号", "postal_code": "1008503", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチサイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008980','{"jis": "13101", "kana": "シヤカイフクシホウジン ゼンコクシヤカイフクシキヨウギカイ", "name": "社会福祉法人　全国社会福祉協議会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3丁目3-2", "postal_code": "1008980", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1008945','{"jis": "13101", "kana": "シヤカイホケンチヨウ", "name": "社会保険庁", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "1丁目2-2", "postal_code": "1008945", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1008909','{"jis": "13101", "kana": "シヤカイミンシユトウゼンコクレンゴウ", "name": "社会民主党全国連合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "永田町", "banchi": "1丁目8-1", "postal_code": "1008909", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ナガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008188','{"jis": "13101", "kana": "シヤダンホウジン ニホンケイザイダンタイレンゴウカイ", "name": "社団法人　日本経済団体連合会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目3-2", "postal_code": "1008188", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008543','{"jis": "13101", "kana": "シヤダンホウジン ニホンシンブンキヨウカイ", "name": "社団法人　日本新聞協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内幸町", "banchi": "2丁目2-1", "postal_code": "1008543", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチサイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008283','{"jis": "13101", "kana": "シヤングリ・ラホテルトウキヨウ", "name": "シャングリ・ラホテル東京", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1丁目8-3丸の内トラストタワー本館", "postal_code": "1008283", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008960','{"jis": "13101", "kana": "シユウギイン", "name": "衆議院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "永田町", "banchi": "1丁目7-1", "postal_code": "1008960", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ナガタチョウ", "alternates": []}');
@@ -125566,15 +125570,15 @@
 INSERT INTO office_data VALUES('1008324','{"jis": "13101", "kana": "ミツビシガスカガク カブシキガイシヤ", "name": "三菱ガス化学　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2丁目5-2", "postal_code": "1008324", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008251','{"jis": "13101", "kana": "ミツビシケミカル カブシキガイシヤ", "name": "三菱ケミカル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1-1-1パレスビル", "postal_code": "1008251", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008350','{"jis": "13101", "kana": "ミツビシシヨウジプラスチツク カブシキガイシヤ", "name": "三菱商事プラスチック　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1-8-3", "postal_code": "1008350", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008133','{"jis": "13101", "kana": "ミツビシジシヨ カブシキガイシヤ", "name": "三菱地所　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目1番1号", "postal_code": "1008133", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008113','{"jis": "13101", "kana": "ミツビシジシヨリアルエステ-トサ-ビス カブシキガイシヤ", "name": "三菱地所リアルエステートサービス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "2丁目2-1", "postal_code": "1008113", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008189','{"jis": "13101", "kana": "ミツビシジシヨレジデンス カブシキカイシヤ", "name": "三菱地所レジデンス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目9番2号大手町フィナンシャルシティグランキューブ", "postal_code": "1008189", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008332','{"jis": "13101", "kana": "ミツビシジユウコウギヨウ カブシキカイシヤ", "name": "三菱重工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目2番3号丸の内二重橋ビル", "postal_code": "1008332", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
-INSERT INTO office_data VALUES('1008310','{"jis": "13101", "kana": "ミツビシデンキ カブシキガイシヤ", "name": "三菱電機　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2丁目2-3", "postal_code": "1008310", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
+INSERT INTO office_data VALUES('1008310','{"jis": "13101", "kana": "ミツビシデンキ カブシキガイシヤ", "name": "三菱電機　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "二丁目7番3号", "postal_code": "1008310", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008335','{"jis": "13101", "kana": "ミツビシデンキビルソリユ-シヨンズ カブシキガイシヤ", "name": "三菱電機ビルソリューションズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2-7-3", "postal_code": "1008335", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008303','{"jis": "13101", "kana": "ミツビシデンセンコウギヨウ カブシキガイシヤ", "name": "三菱電線工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目4-1", "postal_code": "1008303", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008338','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目3-1", "postal_code": "1008338", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008117','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目2番3号丸の内二重橋ビル22階", "postal_code": "1008117", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008127','{"jis": "13101", "kana": "ミツビシユ-エフジエイモルガン・スタンレ-シヨウケン カブシキガイシヤ", "name": "三菱ＵＦＪモルガン・スタンレー証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目9番2号大手町フィナンシャルシティグランキューブ", "postal_code": "1008127", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1006262','{"jis": "13101", "kana": "メ-ルボツクス・エトセトラ トウキヨウエキテン", "name": "メールボックス・エトセトラ　東京駅店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "1丁目11-1パシフィックセンチュリープレイス丸の内地下1階", "postal_code": "1006262", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008311','{"jis": "13101", "kana": "メイワサンギヨウ カブシキガイシヤ", "name": "明和産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "3丁目3-1", "postal_code": "1008311", "old_code": "100  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
@@ -125599,14 +125603,15 @@
 INSERT INTO office_data VALUES('1008051','{"jis": "13101", "kana": "カブシキガイシヤ マイニチシンブンシヤ トウキヨウホンシヤ", "name": "株式会社　毎日新聞社　東京本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "1丁目1-1", "postal_code": "1008051", "old_code": "10051", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1006051','{"jis": "13101", "kana": "カブシキガイシヤ ジエイテイ-ビ-ホウジントウキヨウ カスミガセキエイギヨウブ", "name": "株式会社　ＪＴＢ法人東京　霞が関営業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "霞が関", "banchi": "3-2-5霞が関ビル23階", "postal_code": "1006051", "old_code": "10060", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カスミガセキ", "alternates": []}');
 INSERT INTO office_data VALUES('1006162','{"jis": "13101", "kana": "デイ・エグゼクテイブ・センタ-・ジヤパン カブシキガイシヤ", "name": "ディ・エグゼクティブ・センター・ジャパン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "永田町", "banchi": "2-11-1山王パークタワー3階", "postal_code": "1006162", "old_code": "10061", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ナガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1008077','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008077", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008078','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008078", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008079','{"jis": "13101", "kana": "カブシキガイシヤ サンギヨウケイザイシンブンシヤ", "name": "株式会社　産業経済新聞社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "大手町", "banchi": "1丁目7-2", "postal_code": "1008079", "old_code": "10077", "post_office": "銀座", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1008086','{"jis": "13101", "kana": "ミツビシシヨウジ カブシキガイシヤ", "name": "三菱商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "丸の内", "banchi": "2丁目3-1", "postal_code": "1008086", "old_code": "10086", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "マルノウチ", "alternates": []}');
+INSERT INTO office_data VALUES('1018485','{"jis": "13101", "kana": "ア-ルエムトウセロ カブシキガイシヤ", "name": "アールエム東セロ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7", "postal_code": "1018485", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018480','{"jis": "13101", "kana": "アサヒカセイアミダス カブシキガイシヤ", "name": "旭化成アミダス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目22番地", "postal_code": "1018480", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018101','{"jis": "13101", "kana": "アサヒカセイホ-ムズ カブシキガイシヤ", "name": "旭化成ホームズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "1丁目105番地神保町三井ビルディング", "postal_code": "1018101", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018318','{"jis": "13101", "kana": "アデカクリ-ンエイド カブシキガイシヤ", "name": "ＡＤＥＫＡクリーンエイド　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2-5-12NMF駿河台ビル2階", "postal_code": "1018318", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018512','{"jis": "13101", "kana": "アルフレツサ カブシキガイシヤ", "name": "アルフレッサ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7番地住友不動産神田ビル13F", "postal_code": "1018512", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018445','{"jis": "13101", "kana": "イオンクレジツトサ-ビス", "name": "イオンクレジットサービス　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目1", "postal_code": "1018445", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018333','{"jis": "13101", "kana": "イツパンザイダンホウジン サンギヨウケイリキヨウカイ", "name": "一般財団法人　産業経理協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "1丁目15-6", "postal_code": "1018333", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018986','{"jis": "13101", "kana": "イツパンザイダンホウジン ニホンケンチクセンタ-", "name": "一般財団法人　日本建築センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1-9東京天理ビル", "postal_code": "1018986", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
@@ -125748,15 +125753,14 @@
 INSERT INTO office_data VALUES('1018528','{"jis": "13101", "kana": "ピツプ カブシキガイシヤ", "name": "ピップ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3-3-7", "postal_code": "1018528", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018542','{"jis": "13101", "kana": "フジパン カブシキガイシヤ カントウジギヨウブ", "name": "フジパン　（株）　関東事業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "10-1", "postal_code": "1018542", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018606','{"jis": "13101", "kana": "フマキラ- カブシキガイシヤ", "name": "フマキラー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美倉町", "banchi": "11", "postal_code": "1018606", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミクラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018477','{"jis": "13101", "kana": "ミズノ カブシキガイシヤ", "name": "ミズノ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "3丁目22", "postal_code": "1018477", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018219','{"jis": "13101", "kana": "ミズホシヨウケン カブシキガイシヤ", "name": "みずほ証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018219", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018443','{"jis": "13101", "kana": "ミズホリサ-チアンドテクノロジ-ズ カブシキガイシヤ", "name": "みずほリサーチ＆テクノロジーズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目3", "postal_code": "1018443", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018429','{"jis": "13101", "kana": "ミタニサンギヨウ カブシキガイシヤ", "name": "三谷産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-36-1千代田ファーストウイング", "postal_code": "1018429", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018485','{"jis": "13101", "kana": "ミツイカガクトウセロ カブシキガイシヤ", "name": "三井化学東セロ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7", "postal_code": "1018485", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018011','{"jis": "13101", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキカイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目9(神田郵便局私書箱第23号)", "postal_code": "1018011", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018338','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-11内神田渋谷ビル9階", "postal_code": "1018338", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018637','{"jis": "13101", "kana": "ミツビシユ-エフジエ-フアクタ- カブシキガイシヤ", "name": "三菱ＵＦＪファクター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番ワテラスタワー", "postal_code": "1018637", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018676','{"jis": "13101", "kana": "ムサシノギンコウ トウキヨウシテン", "name": "（株）　武蔵野銀行　東京支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目15-9(神田郵便局私書箱第45号)", "postal_code": "1018676", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018554','{"jis": "13101", "kana": "メタウオ-タ- カブシキガイシヤ", "name": "メタウォーター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目25番", "postal_code": "1018554", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018626','{"jis": "13101", "kana": "ヤマキ カブシキガイシヤ", "name": "ヤマキ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-8-2", "postal_code": "1018626", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018585','{"jis": "13101", "kana": "ヤマザキセイパン カブシキガイシヤ", "name": "山崎製パン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "3丁目10-1", "postal_code": "1018585", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
@@ -125978,14 +125982,15 @@
 INSERT INTO office_data VALUES('1028451','{"jis": "13101", "kana": "トウアケンセツコウギヨウ カブシキガイシヤ", "name": "東亜建設工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "四番町", "banchi": "5", "postal_code": "1028451", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヨンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028122','{"jis": "13101", "kana": "トウアハンバイ カブシキガイシヤ", "name": "東亜販売　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "2丁目16-9", "postal_code": "1028122", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028382','{"jis": "13101", "kana": "トウキヨウガラス カブシキガイシヤ", "name": "東京硝子　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一番町", "banchi": "6-6", "postal_code": "1028382", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イチバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028161','{"jis": "13101", "kana": "トウキヨウケイサツビヨウイン", "name": "東京警察病院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目10-41", "postal_code": "1028161", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028322','{"jis": "13101", "kana": "トウキヨウコクリツキンダイビジユツカン", "name": "東京国立近代美術館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "北の丸公園", "banchi": "3", "postal_code": "1028322", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キタノマルコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1028265','{"jis": "13101", "kana": "トウキヨウジヨウヨウリヨキヤクジドウシヤコウセイネンキンキキン", "name": "東京乗用旅客自動車厚生年金基金", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4丁目8-13", "postal_code": "1028265", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028798','{"jis": "13101", "kana": "トウキヨウテイシンビヨウイン", "name": "東京逓信病院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目14-23", "postal_code": "1028798", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028113','{"jis": "13101", "kana": "トウキヨウトシヨクギヨウノウリヨクカイハツキヨウカイ", "name": "東京都職業能力開発協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "3-10-3東京しごとセンター7階", "postal_code": "1028113", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028226','{"jis": "13101", "kana": "トウキヨウホウムキヨク", "name": "東京法務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "1丁目1-15", "postal_code": "1028226", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028225','{"jis": "13101", "kana": "トウキヨウホウムキヨク", "name": "東京法務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "1丁目1-15九段第2合同庁舎", "postal_code": "1028225", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028362','{"jis": "13101", "kana": "トウコウコ-セン カブシキガイシヤ", "name": "東工コーセン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "四番町", "banchi": "4-2", "postal_code": "1028362", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヨンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028182','{"jis": "13101", "kana": "トキワコウギヨウ カブシキガイシヤ", "name": "常盤工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4丁目2-38", "postal_code": "1028182", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028131','{"jis": "13101", "kana": "トツパン.フオ-ムズ カブシキガイシヤ", "name": "トッパン・フォームズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目1-8", "postal_code": "1028131", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028332','{"jis": "13101", "kana": "トビシマケンセツ カブシキガイシヤ", "name": "飛島建設　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "2番地", "postal_code": "1028332", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028484','{"jis": "13101", "kana": "トラベラ- カブシキガイシヤ", "name": "トラベラー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目10麹町広洋ビル", "postal_code": "1028484", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
@@ -126035,14 +126040,15 @@
 INSERT INTO office_data VALUES('1028250','{"jis": "13101", "kana": "マルベニメタル カブシキガイシヤ", "name": "丸紅メタル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4丁目1番7号", "postal_code": "1028250", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028176','{"jis": "13101", "kana": "ミシユランタイヤグル-プ", "name": "ミシュランタイヤグループ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "1丁目6-1富士見ビル", "postal_code": "1028176", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028404','{"jis": "13101", "kana": "ミツビシデンキエンジニアリング カブシキガイシヤ", "name": "三菱電機エンジニアリング　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "1丁目13番5号", "postal_code": "1028404", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028525','{"jis": "13101", "kana": "メツトライフセイメイホケン カブシキガイシヤ", "name": "メットライフ生命保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1-3東京ガーデンテラス紀尾井町紀尾井タワー", "postal_code": "1028525", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028557','{"jis": "13101", "kana": "メムビ-イ- キオイチヨウテン", "name": "ＭＢＥ　紀尾井町店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-28", "postal_code": "1028557", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028246','{"jis": "13101", "kana": "ヤスクニジンジヤ", "name": "靖国神社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "3-1-1", "postal_code": "1028246", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028273','{"jis": "13101", "kana": "ユ-エイゼンセン", "name": "ＵＡゼンセン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4-8-16ゼンセン同盟会館内", "postal_code": "1028273", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
+INSERT INTO office_data VALUES('1028274','{"jis": "13101", "kana": "ユ-エイゼンセン キヨウサイジギヨウキヨク", "name": "ＵＡゼンセン　共済事業局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "4-8-19CIRCLES+市ケ谷駅前", "postal_code": "1028274", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028236','{"jis": "13101", "kana": "ライトコウギヨウ カブシキガイシヤ", "name": "ライト工業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-35", "postal_code": "1028236", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028282','{"jis": "13101", "kana": "ラインヤフ- カブシキガイシヤ", "name": "ＬＩＮＥヤフー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1-3東京ガーデンテラス紀尾井町紀尾井タワー", "postal_code": "1028282", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028563','{"jis": "13101", "kana": "リコ-リ-ス カブシキガイシヤ", "name": "リコーリース　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "4-1ニューオータニガーデンコート14F", "postal_code": "1028563", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028223','{"jis": "13101", "kana": "ワイジエイエフエツクス カブシキガイシヤ", "name": "ワイジェイＦＸ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1-3東京ガーデンテラス紀尾井町紀尾井タワー23階", "postal_code": "1028223", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028224','{"jis": "13101", "kana": "ワイズ・インシユアランス カブシキガイシヤ", "name": "ワイズ・インシュアランス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1-3東京ガーデンテラス紀尾井町紀尾井タワー24階", "postal_code": "1028224", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028012','{"jis": "13101", "kana": "ドクリツギヨウセイホウジン コクサイキヨウリヨクキコウ", "name": "独立行政法人　国際協力機構", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "5-25二番町センタービル1F~6F", "postal_code": "1028012", "old_code": "10200", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028008','{"jis": "13101", "kana": "カブシキカイシヤ ブンゲイシユンジユウ", "name": "株式会社　文藝春秋", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23", "postal_code": "1028008", "old_code": "10208", "post_office": "麹町", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
@@ -126133,15 +126139,14 @@
 INSERT INTO office_data VALUES('1038231','{"jis": "13102", "kana": "カブシキガイシヤ マイニチイ-ブイア-ルシステム", "name": "株式会社　毎日ＥＶＲシステム", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "3丁目3-9", "postal_code": "1038231", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038248','{"jis": "13102", "kana": "カブシキガイシヤ マブチシヨウジ", "name": "株式会社　馬渕商事", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "1-15-1パーカービル", "postal_code": "1038248", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038677','{"jis": "13102", "kana": "カブシキガイシヤ ミズホコ-ポレ-トギンコウ", "name": "株式会社　みずほコーポレート銀行", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "1丁目2-16(日本橋郵便局私書箱第147号)", "postal_code": "1038677", "old_code": "103  ", "post_office": "日本橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1038684','{"jis": "13102", "kana": "カブシキガイシヤ ミツビシユ-エフジエイギンコウ", "name": "株式会社　三菱ＵＦＪ銀行", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本石町", "banchi": "1-3-2(日本橋郵便局私書箱第191号)", "postal_code": "1038684", "old_code": "103  ", "post_office": "日本橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンゴクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038522','{"jis": "13102", "kana": "カブシキガイシヤ モモヤ", "name": "株式会社　桃屋", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "2丁目16-2", "postal_code": "1038522", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038542','{"jis": "13102", "kana": "カブシキガイシヤ ヤマシタセツケイ", "name": "株式会社　山下設計", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋小網町", "banchi": "6-1山万ビル", "postal_code": "1038542", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシコアミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038517','{"jis": "13102", "kana": "カブシキガイシヤ ヨシノヤ", "name": "株式会社　吉野家", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "36番2号リバーゲート18階", "postal_code": "1038517", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1038520','{"jis": "13102", "kana": "カブシキガイシヤ ロイヤルパ-クホテル", "name": "株式会社　ロイヤルパークホテル", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "2丁目1-1", "postal_code": "1038520", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038412','{"jis": "13102", "kana": "カントウカガク (カブ)", "name": "関東化学　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "3丁目2-8", "postal_code": "1038412", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038410','{"jis": "13102", "kana": "キスコ カブシキガイシヤ", "name": "ＫＩＳＣＯ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "4丁目11番2号", "postal_code": "1038410", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038503','{"jis": "13102", "kana": "キヨウワハツコウキリン カブシキガイシヤ トウキヨウシテン", "name": "協和発酵キリン　株式会社　東京支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "36-2リバーゲート13階", "postal_code": "1038503", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038433','{"jis": "13102", "kana": "コ-ワ (カブ) トウキヨウシテン", "name": "興和　株式会社　東京支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "3丁目4-14", "postal_code": "1038433", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038241','{"jis": "13102", "kana": "コクブグル-プホンシヤ カブシキガイシヤ", "name": "国分グループ本社　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "1-1-1", "postal_code": "1038241", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038313','{"jis": "13102", "kana": "コサカイカガクコウギヨウ (カブ)", "name": "小堺化学工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋富沢町", "banchi": "11-7", "postal_code": "1038313", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシトミザワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038471','{"jis": "13102", "kana": "サイチヨウブツサン (カブ)", "name": "斎長物産　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋富沢町", "banchi": "8-6小川源ビル2F", "postal_code": "1038471", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシトミザワチョウ", "alternates": []}');
@@ -126187,16 +126192,16 @@
 INSERT INTO office_data VALUES('1038554','{"jis": "13102", "kana": "トウキヨウオリモノケンコウホケンクミアイ", "name": "東京織物健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "1丁目9-6", "postal_code": "1038554", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038465','{"jis": "13102", "kana": "トウキヨウジツギヨウケンコウホケンクミアイ", "name": "東京実業健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "東日本橋", "banchi": "3丁目10-4", "postal_code": "1038465", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヒガシニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038285','{"jis": "13102", "kana": "トウキヨウタテモノ カブシキガイシヤ", "name": "東京建物　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "1丁目4番16号", "postal_code": "1038285", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1038360','{"jis": "13102", "kana": "トウキヨウトニホンバシトクベツシユツチヨウジヨ", "name": "東京都中央区日本橋特別出張所", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "1丁目31-1", "postal_code": "1038360", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038407','{"jis": "13102", "kana": "トウヨウケミカルズ (カブ)", "name": "東洋ケミカルズ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "4丁目5-16", "postal_code": "1038407", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038584','{"jis": "13102", "kana": "トスコ (カブ)", "name": "トスコ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋人形町", "banchi": "1丁目1-10", "postal_code": "1038584", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシニンギョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038472','{"jis": "13102", "kana": "トヨシマ (カブ) トウキヨウホンシヤ", "name": "豊島　株式会社　東京本社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋富沢町", "banchi": "9-10", "postal_code": "1038472", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシトミザワチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1038489','{"jis": "13102", "kana": "トヨタモビリテイサ-ビス カブシキガイシヤ", "name": "トヨタモビリティサービス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋久松町", "banchi": "9-9", "postal_code": "1038489", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシヒサマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038488','{"jis": "13102", "kana": "トヨタモビリテイサ-ビス カブシキガイシヤ", "name": "トヨタモビリティサービス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋浜町", "banchi": "2-12-4", "postal_code": "1038488", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1038489','{"jis": "13102", "kana": "トヨタモビリテイサ-ビス カブシキガイシヤ", "name": "トヨタモビリティサービス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋久松町", "banchi": "9-9", "postal_code": "1038489", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシヒサマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038439','{"jis": "13102", "kana": "トリイヤクヒン (カブ)", "name": "鳥居薬品　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "3丁目4-1", "postal_code": "1038439", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038487','{"jis": "13102", "kana": "ナガセランダウア カブシキガイシヤ", "name": "長瀬ランダウア　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋久松町", "banchi": "11-6", "postal_code": "1038487", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシヒサマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038536','{"jis": "13102", "kana": "ニツシンセイトウ カブシキカイシヤ ウエルネオシユガ- カブシキカイシヤ", "name": "日新製糖　株式会社　ウェルネオシュガー　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋小網町", "banchi": "14番1号", "postal_code": "1038536", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシコアミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038650','{"jis": "13102", "kana": "ニツシンボウホ-ルデイングス カブシキガイシヤ", "name": "日清紡ホールディングス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋人形町", "banchi": "2-31-11(日本橋郵便局私書箱第100号)", "postal_code": "1038650", "old_code": "103  ", "post_office": "日本橋", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシニンギョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038456','{"jis": "13102", "kana": "ニツシンボウマイクロデバイス カブシキガイシヤ", "name": "日清紡マイクロデバイス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋横山町", "banchi": "3番10号", "postal_code": "1038456", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシヨコヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038422','{"jis": "13102", "kana": "ニツソウシヨウジ (カブ)", "name": "日曹商事　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "3丁目3-6", "postal_code": "1038422", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038282','{"jis": "13102", "kana": "ニツポンデンコウ カブシキガイシヤ", "name": "日本電工　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "1丁目4番16号", "postal_code": "1038282", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
@@ -126232,17 +126237,17 @@
 INSERT INTO office_data VALUES('1038424','{"jis": "13102", "kana": "ポリマテツク (カブ)", "name": "ポリマテック　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "4丁目8-16", "postal_code": "1038424", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038388','{"jis": "13102", "kana": "マ-ビ- カブシキガイシヤ", "name": "マービー　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋馬喰町", "banchi": "2丁目4-12", "postal_code": "1038388", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシバクロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038502','{"jis": "13102", "kana": "マツクス (カブ)", "name": "マックス　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "6-6", "postal_code": "1038502", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038245','{"jis": "13102", "kana": "マルゼン (カブ)", "name": "丸善　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目3-10", "postal_code": "1038245", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038577','{"jis": "13102", "kana": "マルブン (カブ)", "name": "丸文　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋大伝馬町", "banchi": "8-1", "postal_code": "1038577", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシオオデンマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038328','{"jis": "13102", "kana": "マンダリン・オリエンタルトウキヨウ カブシキガイシヤ", "name": "マンダリン・オリエンタル東京　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "2丁目1-1", "postal_code": "1038328", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038323','{"jis": "13102", "kana": "ミツイシンタクギンコウ (カブ)", "name": "三井信託銀行　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "2丁目1-1", "postal_code": "1038323", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1038263','{"jis": "13102", "kana": "ミツイゾウセン カブシキガイシヤ", "name": "三井造船　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "1丁目3-16", "postal_code": "1038263", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038556','{"jis": "13102", "kana": "ミツイブツサンフユ-チヤ-ズ カブシキガイシヤ", "name": "三井物産フューチャーズ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "1丁目11-12TK堀留ビル5F", "postal_code": "1038556", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038273','{"jis": "13102", "kana": "ミツイリ-スジギヨウ カブシキガイシヤ", "name": "三井リース事業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "1丁目4-1", "postal_code": "1038273", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
+INSERT INTO office_data VALUES('1038520','{"jis": "13102", "kana": "ミツビシジシヨホテルズアンドリゾ-ツ カブシキガイシヤ ロイヤルパ-クホテル トウキヨウ・ニホンバシ", "name": "三菱地所ホテルズ＆リゾーツ　株式会社　ロイヤルパークホテル（東京・日本橋）", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "2丁目1-1", "postal_code": "1038520", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038460','{"jis": "13102", "kana": "ミツワデンキ (カブ)", "name": "ミツワ電機　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "東日本橋", "banchi": "2丁目26-3", "postal_code": "1038460", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヒガシニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038301','{"jis": "13102", "kana": "ミドリヤデンキ カブシキガイシヤ", "name": "緑屋電気　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "1-2-6日本橋大栄ビル5階", "postal_code": "1038301", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038571','{"jis": "13102", "kana": "ヤマト (カブ)", "name": "ヤマト　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋大伝馬町", "banchi": "9-10", "postal_code": "1038571", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシオオデンマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038432','{"jis": "13102", "kana": "ヤマトカガク (カブ)", "name": "ヤマト科学　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "2丁目1-6", "postal_code": "1038432", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038333','{"jis": "13102", "kana": "ユ-エフジエイツバサシヨウケン カブシキガイシヤ", "name": "ＵＦＪつばさ証券　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "1丁目6-2", "postal_code": "1038333", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038537','{"jis": "13102", "kana": "ユ-シ-カ-ド カブシキガイシヤ", "name": "ユーシーカード　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋小網町", "banchi": "6-1", "postal_code": "1038537", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシコアミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038321','{"jis": "13102", "kana": "ユニチカ カブシキガイシヤ トウキヨウホンシヤ", "name": "ユニチカ　株式会社　東京本社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本石町", "banchi": "4丁目6-7日本橋日銀通りビル8階", "postal_code": "1038321", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンゴクチョウ", "alternates": []}');
@@ -126327,15 +126332,15 @@
 INSERT INTO office_data VALUES('1048505','{"jis": "13102", "kana": "カブシキガイシヤ ヒノデシユツパン", "name": "株式会社　日之出出版", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5-6-10浜離宮パークサイドプレイス7階", "postal_code": "1048505", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048340','{"jis": "13102", "kana": "カブシキガイシヤ ブリヂストン", "name": "株式会社　ブリヂストン", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "3-1-1", "postal_code": "1048340", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1008621','{"jis": "13102", "kana": "カブシキガイシヤ プランニングオフイス トライ・アングル", "name": "株式会社　プランニングオフィス　トライ・アングル", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "1丁目5-4(銀座郵便局私書箱第366号)", "postal_code": "1008621", "old_code": "104  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048104','{"jis": "13102", "kana": "カブシキガイシヤ ホウケン", "name": "株式会社　法研", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "1丁目10-1", "postal_code": "1048104", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048003','{"jis": "13102", "kana": "カブシキガイシヤ マガジンハウス", "name": "株式会社　マガジンハウス", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目13-10", "postal_code": "1048003", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048130','{"jis": "13102", "kana": "カブシキガイシヤ マツヤ ギンザホンテン", "name": "株式会社　松屋　銀座本店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目6-1", "postal_code": "1048130", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048145','{"jis": "13102", "kana": "カブシキガイシヤ ミキモト ギンザヨンチヨウメホンテン", "name": "株式会社　ミキモト　銀座４丁目本店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "4-5-5", "postal_code": "1048145", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
-INSERT INTO office_data VALUES('1048439','{"jis": "13102", "kana": "カブシキガイシヤ ミツイイ-アンドエス", "name": "株式会社　三井Ｅ＆Ｓ", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "五丁目6番4号", "postal_code": "1048439", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
+INSERT INTO office_data VALUES('1048439','{"jis": "13102", "kana": "カブシキガイシヤ ミツイイ-アンドエス", "name": "株式会社　三井Ｅ＆Ｓ", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "五丁目6番4号", "postal_code": "1048439", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048442','{"jis": "13102", "kana": "カブシキガイシヤ ミツイスミトモギンコウ サイケンビジネスジムセンタ-", "name": "株式会社　三井住友銀行　債権ビジネス事務センター", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "3丁目16番9号築地室町ビル", "postal_code": "1048442", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048212','{"jis": "13102", "kana": "カブシキガイシヤ ミツコシ ギンザテン", "name": "株式会社　三越　銀座店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "4丁目6-16", "postal_code": "1048212", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048306','{"jis": "13102", "kana": "カブシキガイシヤ メイジ", "name": "株式会社　明治", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2-1号京橋エドグラン12階", "postal_code": "1048306", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048302','{"jis": "13102", "kana": "カブシキガイシヤ メイヂヤ", "name": "株式会社　明治屋", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目2番8号", "postal_code": "1048302", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048488','{"jis": "13102", "kana": "カブシキガイシヤ ヤエスシユツパン", "name": "株式会社　八重洲出版", "prefecture": "東京都", "city": "中央区", "neighborhood": "八丁堀", "banchi": "4丁目5-9", "postal_code": "1048488", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハッチョウボリ", "alternates": []}');
 INSERT INTO office_data VALUES('1048456','{"jis": "13102", "kana": "カブシキガイシヤ ヤエスブツクセンタ-", "name": "株式会社　八重洲ブックセンター", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "2丁目5番1号", "postal_code": "1048456", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1048325','{"jis": "13102", "kana": "カブシキガイシヤ ヨミウリシンブンシヤ ジギヨウキヨク", "name": "株式会社　読売新聞社　事業局", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目9-2第一ぬり彦ビル", "postal_code": "1048325", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
@@ -126492,15 +126497,15 @@
 INSERT INTO office_data VALUES('1058583','{"jis": "13103", "kana": "カブシキガイシヤ オレンジペ-ジ", "name": "株式会社　オレンジページ", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "4-11-1TK新橋ビル", "postal_code": "1058583", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058603','{"jis": "13103", "kana": "カブシキガイシヤ キブンサンギヨウ", "name": "株式会社　紀文産業", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "2丁目1-7住友不動産竹芝ビル", "postal_code": "1058603", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1058626','{"jis": "13103", "kana": "カブシキガイシヤ キブンシヨクヒン", "name": "株式会社　紀文食品", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "2丁目1-7", "postal_code": "1058626", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1058468','{"jis": "13103", "kana": "カブシキガイシヤ グルメキネヤ トウキヨウシシヤ", "name": "株式会社　グルメ杵屋　東京支社", "prefecture": "東京都", "city": "港区", "neighborhood": "浜松町", "banchi": "2丁目13-10", "postal_code": "1058468", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ハママツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1058318','{"jis": "13103", "kana": "カブシキガイシヤ コウサイドウホ-ルデイングス", "name": "株式会社　広済堂ホールディングス", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2番3号シーバンスS館", "postal_code": "1058318", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058475','{"jis": "13103", "kana": "カブシキガイシヤ コウボガイドシヤ", "name": "株式会社　公募ガイド社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "1-8-21芝公園リッジビル5階", "postal_code": "1058475", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1058642','{"jis": "13103", "kana": "カブシキガイシヤ コシダテツク", "name": "株式会社　コシダテック", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "2丁目2-9", "postal_code": "1058642", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1058316','{"jis": "13103", "kana": "カブシキガイシヤ コマツセイサクシヨ", "name": "株式会社　小松製作所", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "1-2-20汐留ビルディング9F", "postal_code": "1058316", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
+INSERT INTO office_data VALUES('1058316','{"jis": "13103", "kana": "カブシキガイシヤ コマツセイサクシヨ", "name": "株式会社　小松製作所", "prefecture": "東京都", "city": "港区", "neighborhood": "海岸", "banchi": "1-2-20汐留ビルディング9F", "postal_code": "1058316", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "カイガン", "alternates": []}');
 INSERT INTO office_data VALUES('1058670','{"jis": "13103", "kana": "カブシキガイシヤ ゴルフダイジエストシヤ", "name": "株式会社　ゴルフダイジェスト社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6丁目18-5", "postal_code": "1058670", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058310','{"jis": "13103", "kana": "カブシキガイシヤ シセイドウ", "name": "株式会社　資生堂", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目6-2", "postal_code": "1058310", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058335','{"jis": "13103", "kana": "カブシキガイシヤ ジエイテイ-ビ-コミユニケ-シヨンデザイン", "name": "株式会社　ＪＴＢコミュニケーションデザイン", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目23番1号セレスティン芝三井ビルディング12階", "postal_code": "1058335", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058407','{"jis": "13103", "kana": "カブシキガイシヤ ジヤパンエナジ-", "name": "（株）　ジャパンエナジー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "2丁目10-1", "postal_code": "1058407", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1056050','{"jis": "13103", "kana": "カブシキガイシヤ スタ-・チヤンネル", "name": "株式会社　スター・チャンネル", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4-3-1城山トラストタワー23階", "postal_code": "1056050", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058415','{"jis": "13103", "kana": "カブシキガイシヤ ソニ-・ピクチヤ-ズエンタテインメント", "name": "株式会社　ソニー・ピクチャーズエンタテインメント", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目1-28虎ノ門タワーズオフィス", "postal_code": "1058415", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058658','{"jis": "13103", "kana": "カブシキガイシヤ ダイコウ", "name": "株式会社　大広", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "2丁目14-5", "postal_code": "1058658", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
@@ -126627,31 +126632,32 @@
 INSERT INTO office_data VALUES('1058579','{"jis": "13103", "kana": "ニホンマスタ-トラストシンタクギンコウ カブシキガイシヤ", "name": "日本マスタートラスト信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "浜松町", "banchi": "2丁目11-3MTBJビル", "postal_code": "1058579", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ハママツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1058301','{"jis": "13103", "kana": "パナソニツク カブシキガイシヤ", "name": "パナソニック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1丁目5-1", "postal_code": "1058301", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058581','{"jis": "13103", "kana": "パナソニツク カブシキガイシヤ トウキヨウパナソニツクビルイチゴウカン", "name": "パナソニック　株式会社　東京パナソニックビル１号館", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "1丁目1-2", "postal_code": "1058581", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1058418','{"jis": "13103", "kana": "パンパシフイツク・カツパ- カブシキガイシヤ", "name": "パンパシフィック・カッパー　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "2丁目10番4号", "postal_code": "1058418", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058614','{"jis": "13103", "kana": "ヒタチキンゾク カブシキガイシヤ", "name": "日立金属　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2-1シーバンスN館", "postal_code": "1058614", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058410','{"jis": "13103", "kana": "ヒタチグロ-バルライフソリユ-シヨンズ カブシキガイシヤ", "name": "日立グローバルライフソリューションズ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "2-15-12", "postal_code": "1058410", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058644','{"jis": "13103", "kana": "ビ-エスニツテレ", "name": "ＢＳ日テレ", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1-6-1日テレタワー23F", "postal_code": "1058644", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
-INSERT INTO office_data VALUES('1058433','{"jis": "13103", "kana": "ピ-エイチシ- カブシキガイシヤ", "name": "ＰＨＣ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "2-38-5", "postal_code": "1058433", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": [{"jis": "13103", "kana": "ピ-エイチシ-ホ-ルデイングス カブシキガイシヤ", "name": "ＰＨＣホールディングス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "2-38-5", "postal_code": "1058433", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}]}');
+INSERT INTO office_data VALUES('1058433','{"jis": "13103", "kana": "ピ-エイチシ- カブシキガイシヤ", "name": "ＰＨＣ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "3丁目7-1", "postal_code": "1058433", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058668','{"jis": "13103", "kana": "フジツウエフ・アイ・ピ- カブシキガイシヤ アクテイブオフイス", "name": "富士通エフ・アイ・ピー　株式会社　アクティブオフィス", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2-1シーバンスN館", "postal_code": "1058668", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058630','{"jis": "13103", "kana": "フルカワサンギヨウ カブシキガイシヤ", "name": "古河産業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "4丁目21-3新橋東急ビル", "postal_code": "1058630", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058435','{"jis": "13103", "kana": "ホツカイドウシンブン トウキヨウシシヤ", "name": "北海道新聞　東京支社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "2丁目2-5", "postal_code": "1058435", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058553','{"jis": "13103", "kana": "ポケツトカ-ド カブシキガイシヤ", "name": "ポケットカード　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "1丁目5-9", "postal_code": "1058553", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058484','{"jis": "13103", "kana": "マグレガ-ゴルフジヤパン カブシキガイシヤ", "name": "マグレガーゴルフジャパン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝大門", "banchi": "2-10-12KDX芝大門", "postal_code": "1058484", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバダイモン", "alternates": []}');
-INSERT INTO office_data VALUES('1058466','{"jis": "13103", "kana": "ミツイシヨクヒン カブシキガイシヤ", "name": "三井食品　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目1番1号", "postal_code": "1058466", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058574','{"jis": "13103", "kana": "ミツイスミトモシンタクギンコウ カブシキガイシヤ", "name": "三井住友信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3-33-1", "postal_code": "1058574", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058464','{"jis": "13103", "kana": "ミツイスミトモフアイナンスアンドリ-ス カブシキガイシヤ", "name": "三井住友ファイナンス＆リース　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "3丁目9-4", "postal_code": "1058464", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058427','{"jis": "13103", "kana": "ミツイノウリン カブシキガイシヤ", "name": "三井農林　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目2-9日比谷セントラルビル", "postal_code": "1058427", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
+INSERT INTO office_data VALUES('1058466','{"jis": "13103", "kana": "ミツイブツサンリユウツウグル-プ カブシキガイシヤ", "name": "三井物産流通グループ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目1番1号", "postal_code": "1058466", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058712','{"jis": "13103", "kana": "ミツビシエイチシ-キヤピタル カブシキガイシヤ", "name": "三菱ＨＣキャピタル　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "西新橋", "banchi": "1丁目3番1号", "postal_code": "1058712", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ニシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058501','{"jis": "13103", "kana": "ミツビシユ-エフジエイリサ-チアンドコンサルテイング カブシキガイシヤ", "name": "三菱ＵＦＪリサーチ＆コンサルティング　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "5丁目11番2号", "postal_code": "1058501", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058516','{"jis": "13103", "kana": "ミナトクシバウラコウナンチク ソウゴウシシヨ", "name": "港区芝浦港南地区　総合支所", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目16番1号", "postal_code": "1058516", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058317','{"jis": "13103", "kana": "ミネベアミツミ カブシキガイシヤ", "name": "ミネベアミツミ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "東新橋", "banchi": "1-9-3", "postal_code": "1058317", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ヒガシシンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058437','{"jis": "13103", "kana": "ミハマ カ)", "name": "美浜　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "1丁目2-8虎ノ門琴平タワー18階", "postal_code": "1058437", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058510','{"jis": "13103", "kana": "ミワロツク カブシキガイシヤ", "name": "美和ロック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目1-12", "postal_code": "1058510", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1058582','{"jis": "13103", "kana": "メルパルク トウキヨウ", "name": "メルパルク　ＴＯＫＹＯ", "prefecture": "東京都", "city": "港区", "neighborhood": "芝公園", "banchi": "2丁目5-20", "postal_code": "1058582", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバコウエン", "alternates": []}');
+INSERT INTO office_data VALUES('1058309','{"jis": "13103", "kana": "モリナガセイカ カブシキガイシヤ", "name": "森永製菓　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目13-16", "postal_code": "1058309", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058451','{"jis": "13103", "kana": "モリムラシヨウジ カブシキガイシヤ", "name": "森村商事　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門", "banchi": "4丁目1番28号虎ノ門タワーズオフィス", "postal_code": "1058451", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモン", "alternates": []}');
 INSERT INTO office_data VALUES('1058686','{"jis": "13103", "kana": "ヤシマデンキ カブシキガイシヤ", "name": "八洲電機　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "3丁目1番1号", "postal_code": "1058686", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058577','{"jis": "13103", "kana": "ユ-シ-シ-ウエシマコ-ヒ- カブシキガイシヤ トウキヨウホンブ", "name": "ＵＣＣ上島珈琲　株式会社　東京本部", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "6丁目1-11タウィンチ御成門", "postal_code": "1058577", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058449','{"jis": "13103", "kana": "ユ-ビ-イ- カブシキカイシヤ", "name": "ＵＢＥ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "1丁目2番1号シーバンスN館20階", "postal_code": "1058449", "old_code": "105  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1058608','{"jis": "13103", "kana": "ユウゲンガイシヤ ツキプランニング", "name": "有限会社　つきプランニング", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "5丁目20-3新橋STビル3F", "postal_code": "1058608", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058685','{"jis": "13103", "kana": "ヨコハマゴム カブシキガイシヤ", "name": "横浜ゴム　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "新橋", "banchi": "5丁目36-11", "postal_code": "1058685", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1058503','{"jis": "13103", "kana": "リコ-ジヤパン カブシキガイシヤ", "name": "リコージャパン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "3丁目8番2号芝公園ファーストビル", "postal_code": "1058503", "old_code": "105  ", "post_office": "芝", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
@@ -126815,15 +126821,15 @@
 INSERT INTO office_data VALUES('1078560','{"jis": "13103", "kana": "ダイイチホウキシユツパン カブシキガイシヤ", "name": "第一法規出版　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "南青山", "banchi": "2丁目11-17", "postal_code": "1078560", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミナミアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078545','{"jis": "13103", "kana": "チユウオウブツサン カブシキガイシヤ", "name": "中央物産　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "南青山", "banchi": "2-2-3", "postal_code": "1078545", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミナミアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078320','{"jis": "13103", "kana": "ト-ヨ-マテリア カブシキガイシヤ", "name": "トーヨーマテリア　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "7丁目6-38", "postal_code": "1078320", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078636','{"jis": "13103", "kana": "トウカイカ-ボン カブシキガイシヤ", "name": "東海カーボン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "北青山", "banchi": "1丁目2-3青山ビル", "postal_code": "1078636", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "キタアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078616','{"jis": "13103", "kana": "ニツカウイスキ- カブシキガイシヤ", "name": "ニッカウイスキー　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "南青山", "banchi": "5丁目4-31", "postal_code": "1078616", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミナミアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078527','{"jis": "13103", "kana": "ニツテツブツサン カブシキカイシヤ", "name": "日鉄物産　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "8丁目5番27号", "postal_code": "1078527", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078456','{"jis": "13103", "kana": "ニツポンカルミツク カブシキガイシヤ", "name": "日本カルミック　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "4丁目8-19(赤坂表町ビル)", "postal_code": "1078456", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
-INSERT INTO office_data VALUES('1078431','{"jis": "13103", "kana": "ニホンカンザイセンタ- カブシキガイシヤ", "name": "日本管財センター　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "1-1-14", "postal_code": "1078431", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
+INSERT INTO office_data VALUES('1078431','{"jis": "13103", "kana": "ニホンカンザイセンタ- カブシキガイシヤ", "name": "日本管材センター　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "1-1-14", "postal_code": "1078431", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078404','{"jis": "13103", "kana": "ニホンザイダン", "name": "日本財団", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "1丁目2-2", "postal_code": "1078404", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078472','{"jis": "13103", "kana": "ニホンマスタ-トラストシンタクギンコウ カブシキガイシヤ", "name": "日本マスタートラスト信託銀行　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "一丁目8-1赤坂インターシティAIR", "postal_code": "1078472", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078546','{"jis": "13103", "kana": "ハ-バライフ・オブ・ジヤパン カブシキガイシヤ", "name": "ハーバライフ・オブ・ジャパン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "2丁目9-11", "postal_code": "1078546", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078340','{"jis": "13103", "kana": "フアミリ-ゲキジヨウ", "name": "ファミリー劇場", "prefecture": "東京都", "city": "港区", "neighborhood": "赤坂", "banchi": "4丁目8-10", "postal_code": "1078340", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "アカサカ", "alternates": []}');
 INSERT INTO office_data VALUES('1078633','{"jis": "13103", "kana": "ブラジルタイシカン", "name": "ブラジル大使館", "prefecture": "東京都", "city": "港区", "neighborhood": "北青山", "banchi": "2丁目11-12", "postal_code": "1078633", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "キタアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078556','{"jis": "13103", "kana": "ホンダギケンコウギヨウ カブシキガイシヤ", "name": "本田技研工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "南青山", "banchi": "2丁目1-1", "postal_code": "1078556", "old_code": "107  ", "post_office": "赤坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミナミアオヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('1078650','{"jis": "13103", "kana": "ミツビシユウエフジエイシンタクギンコウ", "name": "三菱ＵＦＪ信託銀行", "prefecture": "東京都", "city": "港区", "neighborhood": "北青山", "banchi": "1丁目5-4(赤坂郵便局私書箱第55号)", "postal_code": "1078650", "old_code": "107  ", "post_office": "赤坂", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "キタアオヤマ", "alternates": []}');
@@ -126950,14 +126956,15 @@
 INSERT INTO office_data VALUES('1088232','{"jis": "13103", "kana": "ダイセルバリユ-コ-テイング (カブ)", "name": "ダイセルバリューコーティング　（株）", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目18-1", "postal_code": "1088232", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088233','{"jis": "13103", "kana": "ダイセルブツリユウ カブシキガイシヤ", "name": "ダイセル物流　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目18-1", "postal_code": "1088233", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088231','{"jis": "13103", "kana": "ダイセルミライズ カブシキガイシヤ", "name": "ダイセルミライズ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2-18-1JR品川イーストビル15F", "postal_code": "1088231", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088211','{"jis": "13103", "kana": "ダイトウケンタク カブシキガイシヤ", "name": "大東建託　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-1", "postal_code": "1088211", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088478','{"jis": "13103", "kana": "ダイドウトクシユコウ カブシキガイシヤ トウキヨウホンシヤ", "name": "大同特殊鋼　株式会社　東京本社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1丁目6-35", "postal_code": "1088478", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088616','{"jis": "13103", "kana": "チイキイリヨウキノウスイシンキコウケンコウホケンクミアイ", "name": "地域医療機能推進機構健康保険組合", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "3丁目22番12号", "postal_code": "1088616", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
 INSERT INTO office_data VALUES('1088222','{"jis": "13103", "kana": "ツバキモトコウギヨウ カブシキガイシヤ トウキヨウホンシヤ", "name": "椿本興業　（株）　東京本社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-2太陽生命品川ビル", "postal_code": "1088222", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
+INSERT INTO office_data VALUES('1088331','{"jis": "13103", "kana": "テイ-デイ-シネツクス カブシキガイシヤ", "name": "ＴＤ　ＳＹＮＮＥＸ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "3-1-1msbTamachiステーションタワーN41F", "postal_code": "1088331", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088506','{"jis": "13103", "kana": "テイエチケ- カブシキカイシヤ", "name": "ＴＨＫ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "2丁目12番10号", "postal_code": "1088506", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088521','{"jis": "13103", "kana": "テクノレント カブシキカイシヤ", "name": "テクノレント　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目13番23号", "postal_code": "1088521", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088588','{"jis": "13103", "kana": "テクマトリツクス カブシキガイシヤ", "name": "テクマトリックス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-2-70品川シーズンテラス24F", "postal_code": "1088588", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088360','{"jis": "13103", "kana": "デイ-ケ-エスエイチジヤパン カブシキガイシヤ", "name": "ＤＫＳＨジャパン　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目4-19DKSH三田ビルディング", "postal_code": "1088360", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088477','{"jis": "13103", "kana": "トウキヨウカイヨウダイガク", "name": "東京海洋大学", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "4丁目5-7", "postal_code": "1088477", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088512','{"jis": "13103", "kana": "トウキヨウコカコ-ラボトリング カブシキガイシヤ", "name": "東京コカコーラボトリング　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "2丁目15-6", "postal_code": "1088512", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088606','{"jis": "13103", "kana": "トウキヨウセンインホケンビヨウイン", "name": "東京船員保険病院", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "3丁目10-11", "postal_code": "1088606", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
@@ -127307,15 +127314,15 @@
 INSERT INTO office_data VALUES('1630655','{"jis": "13104", "kana": "テイ-ビイ-シ-グル-プ カブシキガイシヤ", "name": "ＴＢＣグループ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目25-1新宿センタービル43F", "postal_code": "1630655", "old_code": "16306", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630777','{"jis": "13104", "kana": "カブシキガイシヤ ニツポンシステムデイベロツプメント", "name": "株式会社　日本システムディベロップメント", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目7-1小田急第一生命ビル", "postal_code": "1630777", "old_code": "16307", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630867','{"jis": "13104", "kana": "カブシキガイシヤ ケイオウエ-ジエンシ-", "name": "株式会社　京王エージェンシー", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2-4-1新宿NSビル23階", "postal_code": "1630867", "old_code": "16308", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1630938','{"jis": "13104", "kana": "エボニツク デグサ ジヤパン カブシキガイシヤ", "name": "エボニック　デグサ　ジャパン　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目3-1新宿モノリス", "postal_code": "1630938", "old_code": "16309", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1631066','{"jis": "13104", "kana": "カブシキガイシヤ ジエイテイ-ビ-ホウジントウキヨウ", "name": "株式会社　ＪＴＢ法人東京", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目7-1新宿パークタワー27F", "postal_code": "1631066", "old_code": "16310", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1631065','{"jis": "13104", "kana": "カブシキガイシヤ ジエイテイ-ビ-ホウジントウキヨウ", "name": "株式会社　ＪＴＢ法人東京", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目7-1新宿パークタワー26F", "postal_code": "1631065", "old_code": "16310", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1631061','{"jis": "13104", "kana": "カブシキガイシヤ ニツポ カントウダイイチシテン", "name": "株式会社　ＮＩＰＰＯ　関東第一支店", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3-7-1", "postal_code": "1631061", "old_code": "16310", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('1631349','{"jis": "13104", "kana": "オ-タジムシヨ カブシキガイシヤ", "name": "オータ事務所　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目5-1新宿アイランドタワー6F", "postal_code": "1631349", "old_code": "16313", "post_office": "新宿", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
+INSERT INTO office_data VALUES('1631349','{"jis": "13104", "kana": "オ-タジムシヨ カブシキガイシヤ", "name": "オータ事務所　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目5-1新宿アイランドタワー6F", "postal_code": "1631349", "old_code": "16313", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638677','{"jis": "13104", "kana": "ガツコウホウジン コウガクインダイガク", "name": "学校法人　工学院大学", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "1丁目24-2(新宿郵便局私書箱第13号)", "postal_code": "1638677", "old_code": "16391", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638660','{"jis": "13104", "kana": "ザイダンホウジン ジツムキヨウイクケンキユウジヨ", "name": "財団法人　実務教育研究所", "prefecture": "東京都", "city": "新宿区", "neighborhood": "大京町", "banchi": "4(新宿郵便局私書箱第400号)", "postal_code": "1638660", "old_code": "16391", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ダイキョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1698885','{"jis": "13104", "kana": "アキレス カブシキガイシヤ", "name": "アキレス　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "北新宿", "banchi": "2丁目21番1号新宿フロントタワー", "postal_code": "1698885", "old_code": "169  ", "post_office": "新宿北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "キタシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1698517','{"jis": "13104", "kana": "オオクボケンシンセンタ-", "name": "大久保健診センター", "prefecture": "東京都", "city": "新宿区", "neighborhood": "百人町", "banchi": "2丁目27-6", "postal_code": "1698517", "old_code": "169  ", "post_office": "新宿北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヒャクニンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1698520','{"jis": "13104", "kana": "カブシキガイシヤ イセイ", "name": "株式会社　井成", "prefecture": "東京都", "city": "新宿区", "neighborhood": "百人町", "banchi": "1丁目16-21", "postal_code": "1698520", "old_code": "169  ", "post_office": "新宿北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヒャクニンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1698558','{"jis": "13104", "kana": "カブシキガイシヤ カワダ", "name": "株式会社　カワダ", "prefecture": "東京都", "city": "新宿区", "neighborhood": "大久保", "banchi": "2丁目5-25", "postal_code": "1698558", "old_code": "169  ", "post_office": "新宿北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "オオクボ", "alternates": []}');
 INSERT INTO office_data VALUES('1698578','{"jis": "13104", "kana": "カブシキガイシヤ ガイドワ-クス", "name": "株式会社　ガイドワークス", "prefecture": "東京都", "city": "新宿区", "neighborhood": "高田馬場", "banchi": "4-28-12", "postal_code": "1698578", "old_code": "169  ", "post_office": "新宿北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "タカダノババ", "alternates": []}');
@@ -127975,16 +127982,14 @@
 INSERT INTO office_data VALUES('1358306','{"jis": "13108", "kana": "トウキヨウセイコウ カブシキカイシヤ", "name": "東京製綱　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "二丁目37番28号(澁澤シティプレイス永代)", "postal_code": "1358306", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358615','{"jis": "13108", "kana": "トウキヨウゼイカン", "name": "東京税関", "prefecture": "東京都", "city": "江東区", "neighborhood": "青海", "banchi": "2-7-11東京港湾合同庁舎内", "postal_code": "1358615", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358481','{"jis": "13108", "kana": "トウキヨウソウコキヨウカイ", "name": "東京倉庫協会", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目13-3", "postal_code": "1358481", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358383','{"jis": "13108", "kana": "トウキヨウトコウトウクヤクシヨ", "name": "東京都江東区役所", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "4丁目11-28", "postal_code": "1358383", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358639','{"jis": "13108", "kana": "トウキヨウトセキジユウジケツエキセンタ-", "name": "東京都赤十字血液センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358639", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": [{"jis": "13108", "kana": "ニホンセキジユウジシヤ カントウコウシンエツブロツクケツエキセンタ-", "name": "日本赤十字社　関東甲信越ブロック血液センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358639", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}]}');
 INSERT INTO office_data VALUES('1358134','{"jis": "13108", "kana": "トウトスイサン カブシキカイシヤ", "name": "東都水産　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "6-6-2", "postal_code": "1358134", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358532','{"jis": "13108", "kana": "ニツコウビジネスシステムズ カブシキガイシヤ", "name": "日興ビジネスシステムズ　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "木場", "banchi": "1丁目5-55", "postal_code": "1358532", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "キバ", "alternates": []}');
-INSERT INTO office_data VALUES('1358570','{"jis": "13108", "kana": "ニツシンセイトウ カブシキガイシヤ トヨスコウジヨウ", "name": "日新製糖　株式会社　豊洲工場", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "4丁目9-11", "postal_code": "1358570", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
-INSERT INTO office_data VALUES('1358553','{"jis": "13108", "kana": "ニツシンセイトウ カブシキガイシヤ ヨカカイハツホンブ ドウ.スポ-ツプラザハルミ", "name": "日新製糖　株式会社　余暇開発本部　ドゥ・スポーツプラザ晴海", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6-41", "postal_code": "1358553", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358477','{"jis": "13108", "kana": "ニツポンチユウオウケイバカイ デンワトウヒヨウセンタ-", "name": "日本中央競馬会　電話投票センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目14-5永代ダイヤビル内", "postal_code": "1358477", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358797','{"jis": "13108", "kana": "ニツポンユウビン カブシキガイシヤ トウキヨウシシヤ", "name": "日本郵便　株式会社　東京支社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "5-29-30ニッテイビル東陽", "postal_code": "1358797", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358511','{"jis": "13108", "kana": "ニホンアイ・ビ-・エム カブシキガイシヤ トヨスジギヨウシヨ", "name": "日本アイ・ビー・エム　株式会社　豊洲事業所", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "5丁目6-52", "postal_code": "1358511", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358552','{"jis": "13108", "kana": "ニホンエイセイホウソウ (カブ) ワウワウ", "name": "日本衛星放送　（株）　ＷＯＷＯＷ", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-58", "postal_code": "1358552", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358568','{"jis": "13108", "kana": "ニホンオフイス・システム カブシキガイシヤ", "name": "日本オフィス・システム　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "有明", "banchi": "3-4-10", "postal_code": "1358568", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アリアケ", "alternates": []}');
 INSERT INTO office_data VALUES('1358427','{"jis": "13108", "kana": "ニホンクウチヨウサ-ビス カブシキガイシヤ", "name": "日本空調サービス　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2-1-7", "postal_code": "1358427", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358521','{"jis": "13108", "kana": "ニホンセキジユウジシヤ ケツエキジギヨウホンブ タツミブンシツ", "name": "日本赤十字社　血液事業本部　辰巳分室", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "2丁目1-67", "postal_code": "1358521", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
@@ -128007,14 +128012,15 @@
 INSERT INTO office_data VALUES('1358370','{"jis": "13108", "kana": "リコ-テクノネツト カブシキガイシヤ トウキヨウホンシヤ", "name": "リコーテクノネット　株式会社　東京本社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "7丁目5-8", "postal_code": "1358370", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358518','{"jis": "13108", "kana": "リコ-リ-ス カブシキガイシヤ", "name": "リコーリース　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東雲", "banchi": "1丁目7-12KDX豊洲グランスクエア7階", "postal_code": "1358518", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シノノメ", "alternates": []}');
 INSERT INTO office_data VALUES('1358385','{"jis": "13108", "kana": "メイジヤスダシステム・テクノロジ- カブシキガイシヤ エムビ-エスジギヨウブモン", "name": "明治安田システム・テクノロジー　株式会社　ＭＢＳ事業部門", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "2丁目2-20", "postal_code": "1358385", "old_code": "13500", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358731','{"jis": "13108", "kana": "イシカワジマハリマジユウコウギヨウ カブシキガイシヤ トウキヨウダイイチコウジヨウ", "name": "石川島播磨重工業　株式会社　東京第一工場", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "2丁目1-1(深川郵便局私書箱第18号)", "postal_code": "1358731", "old_code": "13591", "post_office": "深川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358732','{"jis": "13108", "kana": "イシカワジマハリマジユウコウギヨウ カブシキガイシヤ トウニテクニカルセンタ-", "name": "石川島播磨重工業　株式会社　東二テクニカルセンター", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "3丁目1-15(深川郵便局私書箱第19号)", "postal_code": "1358732", "old_code": "13591", "post_office": "深川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358733','{"jis": "13108", "kana": "イシカワジマハリマジユウコウギヨウ カブシキガイシヤ トヨスソウゴウジムシヨ", "name": "石川島播磨重工業　株式会社　豊洲総合事務所", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "3丁目2-16(深川郵便局私書箱第6号)", "postal_code": "1358733", "old_code": "13591", "post_office": "深川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358720','{"jis": "13108", "kana": "メイジセイメイホケンソウゴガイシヤ", "name": "明治生命保険相互会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "2丁目2-15(深川郵便局私書箱第2号)", "postal_code": "1358720", "old_code": "13591", "post_office": "深川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
+INSERT INTO office_data VALUES('1368881','{"jis": "13108", "kana": "(カ) ミキモト", "name": "株式会社　ミキモト", "prefecture": "東京都", "city": "江東区", "neighborhood": "南砂", "banchi": "7-11-24", "postal_code": "1368881", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "ミナミスナ", "alternates": []}');
 INSERT INTO office_data VALUES('1368581','{"jis": "13108", "kana": "(カブ) シ-ア-ルシ-ソウゴウケンキユウシヨ", "name": "（株）　ＣＲＣ総合研究所", "prefecture": "東京都", "city": "江東区", "neighborhood": "南砂", "banchi": "2丁目7-5", "postal_code": "1368581", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "ミナミスナ", "alternates": []}');
 INSERT INTO office_data VALUES('1368603','{"jis": "13108", "kana": "(カブ) トクマシヨテン", "name": "（株）　徳間書店", "prefecture": "東京都", "city": "江東区", "neighborhood": "新木場", "banchi": "1丁目6-26", "postal_code": "1368603", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンキバ", "alternates": []}');
 INSERT INTO office_data VALUES('1368585','{"jis": "13108", "kana": "アシツクスジヤパン カブシキガイシヤ", "name": "アシックスジャパン　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "新砂", "banchi": "3丁目1番18号", "postal_code": "1368585", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンスナ", "alternates": []}');
 INSERT INTO office_data VALUES('1368607','{"jis": "13108", "kana": "ウチダシヨクヒン カブシキガイシヤ", "name": "内田食品　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "新木場", "banchi": "4丁目12-22", "postal_code": "1368607", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンキバ", "alternates": []}');
 INSERT INTO office_data VALUES('1368651','{"jis": "13108", "kana": "エツクスフロンテイア", "name": "Ｘフロンティア", "prefecture": "東京都", "city": "江東区", "neighborhood": "新砂", "banchi": "3-2-9", "postal_code": "1368651", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンスナ", "alternates": []}');
 INSERT INTO office_data VALUES('1368630','{"jis": "13108", "kana": "エドガワモクザイコウギヨウ カブシキガイシヤ", "name": "江戸川木材工業　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "新木場", "banchi": "1丁目3-16", "postal_code": "1368630", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンキバ", "alternates": []}');
 INSERT INTO office_data VALUES('1368627','{"jis": "13108", "kana": "エヌイ-シ-ソリユ-シヨンイノベ-タ カブシキガイシヤ", "name": "ＮＥＣソリューションイノベータ　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "新木場", "banchi": "1丁目18番7号", "postal_code": "1368627", "old_code": "136  ", "post_office": "城東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンキバ", "alternates": []}');
@@ -128081,15 +128087,15 @@
 INSERT INTO office_data VALUES('1408661','{"jis": "13109", "kana": "(カブ) コウヨウシヤインサツ", "name": "（株）　恒陽社印刷", "prefecture": "東京都", "city": "品川区", "neighborhood": "南品川", "banchi": "5丁目11-45", "postal_code": "1408661", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408576','{"jis": "13109", "kana": "(カブ) ロキテクノ", "name": "（株）　ロキテクノ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目20-12", "postal_code": "1408576", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408626','{"jis": "13109", "kana": "アイ.シ-.アイ.ジヤパン カブシキガイシヤ", "name": "アイ・シー・アイ・ジャパン　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目2-20天王洲郵船ビル13階", "postal_code": "1408626", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408663','{"jis": "13109", "kana": "アオイ テイ-ワイオ- ホ-ルデイングス カブシキガイシヤ", "name": "ＡＯＩ　ＴＹＯ　Ｈｏｌｄｉｎｇｓ　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目2番24号", "postal_code": "1408663", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408722','{"jis": "13109", "kana": "イスズジドウシヤ カブシキガイシヤ", "name": "いすゞ自動車　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6-26-1", "postal_code": "1408722", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408522','{"jis": "13109", "kana": "イリヨウホウジンシヤダンミドリノカイ トウキヨウシナガワビヨウイン", "name": "医療法人社団緑野会　東京品川病院", "prefecture": "東京都", "city": "品川区", "neighborhood": "東大井", "banchi": "6-3-22", "postal_code": "1408522", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408547','{"jis": "13109", "kana": "インタ-ワイヤ-ド カブシキガイシヤ", "name": "インターワイヤード　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "5丁目19-8", "postal_code": "1408547", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
-INSERT INTO office_data VALUES('1408586','{"jis": "13109", "kana": "エフシ-エルコンポ-ネント カブシキガイシヤ", "name": "ＦＣＬコンポーネント　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "四丁目12番4号品川シーサイドパークタワー", "postal_code": "1408586", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
+INSERT INTO office_data VALUES('1408586','{"jis": "13109", "kana": "エフシ-エルコンポ-ネント カブシキガイシヤ", "name": "ＦＣＬコンポーネント　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "四丁目12番4号品川シーサイドパークタワー", "postal_code": "1408586", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408688','{"jis": "13109", "kana": "オキデンキコウジ カブシキガイシヤ", "name": "沖電気工事　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "1丁目19-4", "postal_code": "1408688", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1408511','{"jis": "13109", "kana": "カブシキカイシヤ ニツセイコム", "name": "株式会社　ニッセイコム", "prefecture": "東京都", "city": "品川区", "neighborhood": "大井", "banchi": "1丁目47-1", "postal_code": "1408511", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408572','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目27-18日立大森第二別館", "postal_code": "1408572", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408573','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシングル-プ", "name": "株式会社　日立製作所　情報・通信グループ", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6丁目26-2大森ベルポートB館", "postal_code": "1408573", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408512','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシンシステムシヤ", "name": "株式会社　日立製作所　情報・通信システム社", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "6-23-1日立大森ビル", "postal_code": "1408512", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408574','{"jis": "13109", "kana": "カブシキカイシヤ ヒタチセイサクシヨデジタルシステムアンドサ-ビストウカツホンブ", "name": "株式会社　日立製作所デジタルシステム＆サービス統括本部", "prefecture": "東京都", "city": "品川区", "neighborhood": "南大井", "banchi": "六丁目26-1大森ベルポートA館", "postal_code": "1408574", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ミナミオオイ", "alternates": []}');
 INSERT INTO office_data VALUES('1408619','{"jis": "13109", "kana": "カブシキガイシヤ アクセスコクサイネツトワ-ク", "name": "株式会社　アクセス国際ネットワーク", "prefecture": "東京都", "city": "品川区", "neighborhood": "東品川", "banchi": "2丁目4番11号野村不動産天王洲ビル", "postal_code": "1408619", "old_code": "140  ", "post_office": "品川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシシナガワ", "alternates": []}');
@@ -128860,15 +128866,14 @@
 INSERT INTO office_data VALUES('1648567','{"jis": "13114", "kana": "カブシキガイシヤ アポロシヤ", "name": "株式会社　アポロ社", "prefecture": "東京都", "city": "中野区", "neighborhood": "東中野", "banchi": "3丁目12-2", "postal_code": "1648567", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヒガシナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648504','{"jis": "13114", "kana": "カブシキガイシヤ インタ-コミユニケ-シヨンズ", "name": "株式会社　インターコミュニケーションズ", "prefecture": "東京都", "city": "中野区", "neighborhood": "本町", "banchi": "1丁目32-4ハーモニーウィング5F", "postal_code": "1648504", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648677','{"jis": "13114", "kana": "カブシキガイシヤ ヴイアツクス", "name": "株式会社　ヴィアックス", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "2-8-15", "postal_code": "1648677", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648601','{"jis": "13114", "kana": "カブシキガイシヤ エイトニホンギジユツカイハツ", "name": "株式会社　エイト日本技術開発", "prefecture": "東京都", "city": "中野区", "neighborhood": "本町", "banchi": "5丁目33番11号", "postal_code": "1648601", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648505','{"jis": "13114", "kana": "カブシキガイシヤ エスシ-シ-", "name": "株式会社　ＳＣＣ", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "5丁目62-1", "postal_code": "1648505", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648611','{"jis": "13114", "kana": "カブシキガイシヤ カ-メイト", "name": "株式会社　カーメイト", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "3丁目35-13", "postal_code": "1648611", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648644','{"jis": "13114", "kana": "カブシキガイシヤ ジヤパン イマジネ-シヨン", "name": "株式会社　ジャパン　イマジネーション", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "1丁目10番1号", "postal_code": "1648644", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1648512','{"jis": "13114", "kana": "カブシキガイシヤ ナカノサンプラザ", "name": "株式会社　中野サンプラザ", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目1-1", "postal_code": "1648512", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648705','{"jis": "13114", "kana": "カブシキガイシヤ ニホンヴオ-グシヤ", "name": "株式会社　日本ヴォーグ社", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "5-6-11", "postal_code": "1648705", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648701','{"jis": "13114", "kana": "カブシキガイシヤ マルイ", "name": "株式会社　丸井", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目3-2(中野郵便局私書箱第2号)", "postal_code": "1648701", "old_code": "164  ", "post_office": "中野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648620','{"jis": "13114", "kana": "カブシキガイシヤ ヤノケイザイケンキユウジヨ", "name": "株式会社　矢野経済研究所", "prefecture": "東京都", "city": "中野区", "neighborhood": "本町", "banchi": "2丁目46-2中野坂上セントラルビル", "postal_code": "1648620", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648585','{"jis": "13114", "kana": "ガツコウホウジン クボタガクエン クボタリヨウビヨウセンモンガツコウ", "name": "学校法人　窪田学園　窪田理容美容専門学校", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目11-1", "postal_code": "1648585", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648678','{"jis": "13114", "kana": "ガツコウホウジン トウキヨウコウゲイダイガク", "name": "学校法人　東京工芸大学", "prefecture": "東京都", "city": "中野区", "neighborhood": "本町", "banchi": "2丁目9-5", "postal_code": "1648678", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648638','{"jis": "13114", "kana": "ガツコウホウジン ニトベブンカガクエン", "name": "学校法人　新渡戸文化学園", "prefecture": "東京都", "city": "中野区", "neighborhood": "本町", "banchi": "6丁目38番1号", "postal_code": "1648638", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648525','{"jis": "13114", "kana": "ガツコウホウジン メイジダイガク ナカノキヤンパス", "name": "学校法人　明治大学　中野キャンパス", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目21番1号", "postal_code": "1648525", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
@@ -128877,15 +128882,15 @@
 INSERT INTO office_data VALUES('1648503','{"jis": "13114", "kana": "サンキヨウタテヤマ カブシキガイシヤ", "name": "三協立山　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "中央", "banchi": "1丁目38番1号住友中野坂上ビル20階", "postal_code": "1648503", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648522','{"jis": "13114", "kana": "サンワデンキコウギヨウ カブシキガイシヤ", "name": "三和電気工業　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目15-9", "postal_code": "1648522", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648540','{"jis": "13114", "kana": "ゼンコクケンコウホケンキヨウカイ トウキヨウシブ", "name": "全国健康保険協会　東京支部", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4-10-2中野セントラルパークサウス7階", "postal_code": "1648540", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648608','{"jis": "13114", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキガイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4-10-2中野セントラルパークサウス5階", "postal_code": "1648608", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648530','{"jis": "13114", "kana": "テイキヨウヘイセイダイガク ナカノキヤンパス", "name": "帝京平成大学　中野キャンパス", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目21番2号", "postal_code": "1648530", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648541','{"jis": "13114", "kana": "トウキヨウケイサツビヨウイン", "name": "東京警察病院", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目22-1", "postal_code": "1648541", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648502','{"jis": "13114", "kana": "トウキヨウトスイドウキヨク ナカノエイギヨウシヨ", "name": "東京都水道局　中野営業所", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "1-5-7", "postal_code": "1648502", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
-INSERT INTO office_data VALUES('1648501','{"jis": "13114", "kana": "ナカノクヤクシヨ", "name": "中野区役所", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目8-1", "postal_code": "1648501", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
+INSERT INTO office_data VALUES('1648501','{"jis": "13114", "kana": "ナカノクヤクシヨ", "name": "中野区役所", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "四丁目11番19号", "postal_code": "1648501", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648686','{"jis": "13114", "kana": "ニツシヨウボキセンモンガツコウ(ニツシヨウクリエ-シヨン)", "name": "日商簿記専門学校（日商クリエーション）", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "2丁目14-22(中野郵便局私書箱第47号)", "postal_code": "1648686", "old_code": "164  ", "post_office": "中野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648666','{"jis": "13114", "kana": "ニホンアルミツト カブシキガイシヤ", "name": "日本アルミット　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "2丁目14-2", "postal_code": "1648666", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1648570','{"jis": "13114", "kana": "ニホンムセン カブシキガイシヤ", "name": "日本無線　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目10番1号中野セントラルパークイースト", "postal_code": "1648570", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648545','{"jis": "13114", "kana": "ホ-ヤ カブシキガイシヤ", "name": "ＨＯＹＡ　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "中野", "banchi": "4丁目10番2号中野セントラルパークサウス6F", "postal_code": "1648545", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648555','{"jis": "13114", "kana": "ミツイジヨウホウ カブシキガイシヤ", "name": "三井情報　株式会社", "prefecture": "東京都", "city": "中野区", "neighborhood": "東中野", "banchi": "2丁目7番14号", "postal_code": "1648555", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヒガシナカノ", "alternates": []}');
 INSERT INTO office_data VALUES('1648617','{"jis": "13114", "kana": "リツシヨウコウセイカイフゾクコウセイビヨウイン", "name": "立正佼成会附属佼成病院", "prefecture": "東京都", "city": "中野区", "neighborhood": "弥生町", "banchi": "5丁目25-15", "postal_code": "1648617", "old_code": "164  ", "post_office": "中野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1658630','{"jis": "13114", "kana": "カブシキガイシヤ キンダイセ-ルスシヤ", "name": "株式会社　近代セールス社", "prefecture": "東京都", "city": "中野区", "neighborhood": "新井", "banchi": "2-10-11ヤシマ1804ビル4階", "postal_code": "1658630", "old_code": "165  ", "post_office": "中野北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ナカノク", "neighborhood_kana": "アライ", "alternates": []}');
@@ -129155,15 +129160,15 @@
 INSERT INTO office_data VALUES('1168503','{"jis": "13118", "kana": "カブシキガイシヤ ハツコウ", "name": "株式会社　白興", "prefecture": "東京都", "city": "荒川区", "neighborhood": "荒川", "banchi": "3丁目33-1", "postal_code": "1168503", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "アラカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1168508','{"jis": "13118", "kana": "カブシキガイシヤ ヤマトメ", "name": "株式会社　ヤマトメ", "prefecture": "東京都", "city": "荒川区", "neighborhood": "荒川", "banchi": "3丁目62-4", "postal_code": "1168508", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "アラカワ", "alternates": []}');
 INSERT INTO office_data VALUES('1168587','{"jis": "13118", "kana": "クリナツプ カブシキガイシヤ", "name": "クリナップ　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "西日暮里", "banchi": "6丁目22-22", "postal_code": "1168587", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ニシニッポリ", "alternates": []}');
 INSERT INTO office_data VALUES('1168524','{"jis": "13118", "kana": "ジヨウシンビジネスサ-ビス カブシキガイシヤ", "name": "城信ビジネスサービス　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "南千住", "banchi": "5丁目19-5", "postal_code": "1168524", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ミナミセンジュ", "alternates": []}');
 INSERT INTO office_data VALUES('1168556','{"jis": "13118", "kana": "タカロクシヨウジ カブシキガイシヤ", "name": "高六商事　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "西日暮里", "banchi": "2丁目20-1ステーションポートタワービル602", "postal_code": "1168556", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ニシニッポリ", "alternates": []}');
 INSERT INTO office_data VALUES('1168549','{"jis": "13118", "kana": "トウエイサンギヨウ カブシキガイシヤ", "name": "東栄産業　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "西日暮里", "banchi": "1丁目61-18", "postal_code": "1168549", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ニシニッポリ", "alternates": []}');
 INSERT INTO office_data VALUES('1168548','{"jis": "13118", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "西日暮里", "banchi": "6丁目52-2", "postal_code": "1168548", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ニシニッポリ", "alternates": []}');
-INSERT INTO office_data VALUES('1168522','{"jis": "13118", "kana": "トウキヨウガス センジユビル", "name": "東京ガス　千住ビル", "prefecture": "東京都", "city": "荒川区", "neighborhood": "南千住", "banchi": "3丁目13番1号", "postal_code": "1168522", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ミナミセンジュ", "alternates": []}');
+INSERT INTO office_data VALUES('1168522','{"jis": "13118", "kana": "トウキヨウガス センジユビル", "name": "東京ガス　千住ビル", "prefecture": "東京都", "city": "荒川区", "neighborhood": "南千住", "banchi": "3丁目13番1号", "postal_code": "1168522", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ミナミセンジュ", "alternates": []}');
 INSERT INTO office_data VALUES('1168533','{"jis": "13118", "kana": "トウキヨウシンコ-レザ- カブシキガイシヤ", "name": "東京シンコーレザー　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "東日暮里", "banchi": "4丁目12-1", "postal_code": "1168533", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ヒガシニッポリ", "alternates": []}');
 INSERT INTO office_data VALUES('1168567','{"jis": "13118", "kana": "トウキヨウジヨシイカダイガクフゾクダイニビヨウイン", "name": "東京女子医科大学附属第二病院", "prefecture": "東京都", "city": "荒川区", "neighborhood": "西尾久", "banchi": "2丁目1-10", "postal_code": "1168567", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ニシオグ", "alternates": []}');
 INSERT INTO office_data VALUES('1168550','{"jis": "13118", "kana": "トウキヨウデンリヨクホ-ルデイングス カブシキガイシヤ", "name": "東京電力ホールディングス　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "東尾久", "banchi": "5丁目31-11", "postal_code": "1168550", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ヒガシオグ", "alternates": []}');
 INSERT INTO office_data VALUES('1168521','{"jis": "13118", "kana": "トウキヨウトスイドウキヨク アラカワエイギヨウシヨ", "name": "東京都水道局　荒川営業所", "prefecture": "東京都", "city": "荒川区", "neighborhood": "南千住", "banchi": "6丁目40-1", "postal_code": "1168521", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ミナミセンジュ", "alternates": []}');
 INSERT INTO office_data VALUES('1168551','{"jis": "13118", "kana": "トウキヨウトリツイリヨウギジユツタンキダイガク", "name": "東京都立医療技術短期大学", "prefecture": "東京都", "city": "荒川区", "neighborhood": "東尾久", "banchi": "7丁目2-10", "postal_code": "1168551", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ヒガシオグ", "alternates": []}');
 INSERT INTO office_data VALUES('1168523','{"jis": "13118", "kana": "トウキヨウトリツサンギヨウギジユツコウトウセンモンガツコウ アラカワキヤンパス", "name": "東京都立産業技術高等専門学校　荒川キャンパス", "prefecture": "東京都", "city": "荒川区", "neighborhood": "南千住", "banchi": "8丁目17番1号", "postal_code": "1168523", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "ミナミセンジュ", "alternates": []}');
 INSERT INTO office_data VALUES('1168552','{"jis": "13118", "kana": "ナガシマトクシユトリヨウ カブシキガイシヤ", "name": "長島特殊塗料　株式会社", "prefecture": "東京都", "city": "荒川区", "neighborhood": "荒川", "banchi": "2丁目1-5セントラル荒川ビル8F", "postal_code": "1168552", "old_code": "116  ", "post_office": "荒川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アラカワク", "neighborhood_kana": "アラカワ", "alternates": []}');
@@ -129703,15 +129708,14 @@
 INSERT INTO office_data VALUES('1968570','{"jis": "13207", "kana": "ホウムシヨウ コクレンアジアキヨクトウハンザイボウシケンシユウジヨ", "name": "法務省　国連アジア極東犯罪防止研修所", "prefecture": "東京都", "city": "昭島市", "neighborhood": "もくせいの杜", "banchi": "2-1-18", "postal_code": "1968570", "old_code": "196  ", "post_office": "昭島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アキシマシ", "neighborhood_kana": "モクセイノモリ", "alternates": [{"jis": "13207", "kana": "ホウムシヨウ ホウムソウゴウケンキユウジヨコクサイキヨウリヨクブ", "name": "法務省　法務総合研究所国際協力部", "prefecture": "東京都", "city": "昭島市", "neighborhood": "もくせいの杜", "banchi": "2-1-18", "postal_code": "1968570", "old_code": "196  ", "post_office": "昭島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アキシマシ", "neighborhood_kana": "モクセイノモリ", "alternates": []}]}');
 INSERT INTO office_data VALUES('1968533','{"jis": "13207", "kana": "モリパ-ク アウトドアヴイレツジ", "name": "ＭＯＲＩＰＡＲＫ　ＯｕｔｄｏｏｒＶｉｌｌａｇｅ", "prefecture": "東京都", "city": "昭島市", "neighborhood": "田中町", "banchi": "610-4", "postal_code": "1968533", "old_code": "196  ", "post_office": "昭島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "アキシマシ", "neighborhood_kana": "タナカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828006','{"jis": "13208", "kana": "アフラツク チヨウフスクエアビル", "name": "アフラック　調布スクエアビル", "prefecture": "東京都", "city": "調布市", "neighborhood": "小島町", "banchi": "2丁目33-2(調布郵便局私書箱第48号)", "postal_code": "1828006", "old_code": "182  ", "post_office": "調布", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "コジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828001','{"jis": "13208", "kana": "アフラツクチヨウフサウスゲ-トビル", "name": "アフラック調布サウスゲートビル", "prefecture": "東京都", "city": "調布市", "neighborhood": "小島町", "banchi": "2丁目48-26(調布郵便局私書箱第50号)", "postal_code": "1828001", "old_code": "182  ", "post_office": "調布", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "コジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828567','{"jis": "13208", "kana": "オダキユウバス カブシキガイシヤ", "name": "小田急バス　株式会社", "prefecture": "東京都", "city": "調布市", "neighborhood": "仙川町", "banchi": "2丁目19-5", "postal_code": "1828567", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "センガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828520','{"jis": "13208", "kana": "カブシキガイシヤ キヨウワデンギヨウ", "name": "株式会社　共和電業", "prefecture": "東京都", "city": "調布市", "neighborhood": "調布ケ丘", "banchi": "3丁目5-1", "postal_code": "1828520", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "チョウフガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('1828555','{"jis": "13208", "kana": "カブシキガイシヤ トウキヨウゲンゾウシヨ", "name": "株式会社　東京現像所", "prefecture": "東京都", "city": "調布市", "neighborhood": "富士見町", "banchi": "2丁目13", "postal_code": "1828555", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "フジミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1828686','{"jis": "13208", "kana": "カブシキガイシヤ フジカラ-サ-ビス トウキヨウジギヨウシヨ", "name": "株式会社　フジカラーサービス　東京事業所", "prefecture": "東京都", "city": "調布市", "neighborhood": "柴崎", "banchi": "1丁目67-1(調布郵便局私書箱第10号)", "postal_code": "1828686", "old_code": "182  ", "post_office": "調布", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "シバサキ", "alternates": []}');
 INSERT INTO office_data VALUES('1828558','{"jis": "13208", "kana": "キユ-ピ- カブシキガイシヤ センガワコウジヨウ", "name": "キユーピー　株式会社　仙川工場", "prefecture": "東京都", "city": "調布市", "neighborhood": "仙川町", "banchi": "2丁目5", "postal_code": "1828558", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "センガワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828522','{"jis": "13208", "kana": "コクリツケンキユウカイハツホウジン ウチユウコウクウケンキユウカイハツキコウ", "name": "国立研究開発法人　宇宙航空研究開発機構", "prefecture": "東京都", "city": "調布市", "neighborhood": "深大寺東町", "banchi": "7丁目44番地1", "postal_code": "1828522", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "ジンダイジヒガシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1828602','{"jis": "13208", "kana": "シマダリカコウギヨウ カブシキガイシヤ", "name": "島田理化工業　（株）", "prefecture": "東京都", "city": "調布市", "neighborhood": "柴崎", "banchi": "2丁目1-3(調布郵便局私書箱第11号)", "postal_code": "1828602", "old_code": "182  ", "post_office": "調布", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "シバサキ", "alternates": []}');
 INSERT INTO office_data VALUES('1828508','{"jis": "13208", "kana": "シヨウボウダイガツコウ", "name": "消防大学校", "prefecture": "東京都", "city": "調布市", "neighborhood": "深大寺東町", "banchi": "4丁目35-3", "postal_code": "1828508", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "ジンダイジヒガシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1828525','{"jis": "13208", "kana": "シラユリジヨシダイガク", "name": "白百合女子大学", "prefecture": "東京都", "city": "調布市", "neighborhood": "緑ケ丘", "banchi": "1丁目25", "postal_code": "1828525", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "ミドリガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('1828601','{"jis": "13208", "kana": "ダイヒヤクセイメイホケン ソウゴガイシヤ", "name": "第百生命保険　相互会社", "prefecture": "東京都", "city": "調布市", "neighborhood": "国領町", "banchi": "4丁目34-1(調布郵便局私書箱第7号)", "postal_code": "1828601", "old_code": "182  ", "post_office": "調布", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "コクリョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1828511','{"jis": "13208", "kana": "チヨウフシヤクシヨ", "name": "調布市役所", "prefecture": "東京都", "city": "調布市", "neighborhood": "小島町", "banchi": "2丁目35-1", "postal_code": "1828511", "old_code": "182  ", "post_office": "調布", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チョウフシ", "neighborhood_kana": "コジマチョウ", "alternates": []}');
@@ -130015,14 +130019,18 @@
 INSERT INTO office_data VALUES('2208521','{"jis": "14103", "kana": "ザイダンホウジン カナガワケンケイユウカイ ケイユウビヨウイン", "name": "財団法人　神奈川県警友会　けいゆう病院", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "3丁目7-3", "postal_code": "2208521", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208566','{"jis": "14103", "kana": "ザイダンホウジン カナガワケンコウトウガツコウキヨウイクカイカン", "name": "財団法人　神奈川県高等学校教育会館", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "藤棚町", "banchi": "2丁目197", "postal_code": "2208566", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "フジダナチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2208609','{"jis": "14103", "kana": "シヨウコウチユウキン ヨコハマニシグチシテン", "name": "商工中金　横浜西口支店", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "北幸", "banchi": "1丁目11番1号(横浜中央郵便局私書箱第310号)", "postal_code": "2208609", "old_code": "220  ", "post_office": "神奈川", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "キタサイワイ", "alternates": []}');
 INSERT INTO office_data VALUES('2208530','{"jis": "14103", "kana": "スミトモセイメイホケン ソウゴガイシヤ ヨコハマシシヤ", "name": "住友生命保険　相互会社　横浜支社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "北幸", "banchi": "1-11-15横浜STビル13階", "postal_code": "2208530", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "キタサイワイ", "alternates": []}');
 INSERT INTO office_data VALUES('2208684','{"jis": "14103", "kana": "スリ-エムジヤパン カブシキガイシヤ", "name": "スリーエムジャパン　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4-6-2みなとみらいグランドセントラルタワー4F", "postal_code": "2208684", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208538','{"jis": "14103", "kana": "ゼンコクケンコウホケンキヨウカイ カナガワシブ", "name": "全国健康保険協会　神奈川支部", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー9階", "postal_code": "2208538", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208750','{"jis": "14103", "kana": "ソニ-グル-プ カブシキガイシヤ ソニ-シテイミナトミライ", "name": "ソニーグループ　株式会社　ソニーシティみなとみらい", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "5-1-1", "postal_code": "2208750", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
+INSERT INTO office_data VALUES('2208562','{"jis": "14103", "kana": "タイヨウニツサン カブシキガイシヤ カントウシシヤ", "name": "大陽日酸　株式会社　関東支社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階", "postal_code": "2208562", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
+INSERT INTO office_data VALUES('2208561','{"jis": "14103", "kana": "タイヨウニツサン カブシキガイシヤ ミナトミライジギヨウシヨ", "name": "大陽日酸　株式会社　みなとみらい事業所", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階", "postal_code": "2208561", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
+INSERT INTO office_data VALUES('2208563','{"jis": "14103", "kana": "タイヨウニツサンエンジニアリング カブシキガイシヤ", "name": "大陽日酸エンジニアリング　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階", "postal_code": "2208563", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
+INSERT INTO office_data VALUES('2208564','{"jis": "14103", "kana": "タイヨウニツサンエンジニアリング カブシキガイシヤ カントウシテン", "name": "大陽日酸エンジニアリング　株式会社　関東支店", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4丁目6番2号みなとみらいグランドセントラルタワー7階", "postal_code": "2208564", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208620','{"jis": "14103", "kana": "ダイワハウスコウギヨウ (カ) ヨコハマシシヤ", "name": "大和ハウス工業　株式会社　横浜支社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "3-6-1みなとみらいセンタービル14階", "postal_code": "2208620", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208765','{"jis": "14103", "kana": "チヨダカコウケンセツ カブシキガイシヤ", "name": "千代田化工建設　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4-6-2みなとみらいグランドセントラルタワー", "postal_code": "2208765", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208565','{"jis": "14103", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "3丁目6-4", "postal_code": "2208565", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
 INSERT INTO office_data VALUES('2208520','{"jis": "14103", "kana": "トウキヨウデンリヨク カブシキガイシヤ ヨコハマシシヤ", "name": "東京電力　株式会社　横浜支社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "高島", "banchi": "2丁目7-30", "postal_code": "2208520", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "タカシマ", "alternates": []}');
 INSERT INTO office_data VALUES('2208580','{"jis": "14103", "kana": "トウデンドウソウデンキ カブシキガイシヤ", "name": "東電同窓電気　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "桜木町", "banchi": "7丁目40-3", "postal_code": "2208580", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2208686','{"jis": "14103", "kana": "ニツサンジドウシヤ カブシキガイシヤ", "name": "日産自動車　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "高島", "banchi": "1丁目1番1号", "postal_code": "2208686", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "タカシマ", "alternates": []}');
 INSERT INTO office_data VALUES('2208586','{"jis": "14103", "kana": "ニホンケ-エフシ-ホ-ルデイングス カブシキガイシヤ", "name": "日本ＫＦＣホールディングス　株式会社", "prefecture": "神奈川県", "city": "横浜市西区", "neighborhood": "みなとみらい", "banchi": "4-4-5横浜アイマークプレイス", "postal_code": "2208586", "old_code": "220  ", "post_office": "神奈川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシニシク", "neighborhood_kana": "ミナトミライ", "alternates": []}');
@@ -130134,14 +130142,15 @@
 INSERT INTO office_data VALUES('2368502','{"jis": "14108", "kana": "カントウガクインダイガク カナザワブンコキヤンパス", "name": "関東学院大学　金沢文庫キャンパス", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "釜利谷南", "banchi": "3丁目22-1", "postal_code": "2368502", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "カマリヤミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('2368504','{"jis": "14108", "kana": "カントウガクインムツウラチユウガツコウ・コウトウガツコウ", "name": "関東学院六浦中学校・高等学校", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "六浦東", "banchi": "1丁目50-1", "postal_code": "2368504", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "ムツウラヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('2368648','{"jis": "14108", "kana": "コクリツケンキユウカイハツホウジン スイサンケンキユウキヨウイクキコウ スイサンシゲンケンキユウジヨ", "name": "国立研究開発法人　水産研究・教育機構　水産資源研究所", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "福浦", "banchi": "2丁目12-4", "postal_code": "2368648", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "フクウラ", "alternates": []}');
 INSERT INTO office_data VALUES('2368653','{"jis": "14108", "kana": "サイセイカイワカクサビヨウイン", "name": "社会福祉法人　恩賜財団　済生会若草病院", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "平潟町", "banchi": "12-1", "postal_code": "2368653", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "ヒラカタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2368555','{"jis": "14108", "kana": "スギタゴルフジヨウ", "name": "杉田ゴルフ場", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "福浦", "banchi": "3丁目11-2", "postal_code": "2368555", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "フクウラ", "alternates": []}');
 INSERT INTO office_data VALUES('2368540','{"jis": "14108", "kana": "ニツポンヒコウキ カブシキガイシヤ", "name": "日本飛行機　株式会社", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "昭和町", "banchi": "3175番地", "postal_code": "2368540", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "ショウワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('2368515','{"jis": "14108", "kana": "ミツビシジユウコウギヨウ カブシキカイシヤ ヨコハマセイサクシヨ", "name": "三菱重工業　株式会社　横浜製作所", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "幸浦", "banchi": "1丁目8番地1", "postal_code": "2368515", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "サチウラ", "alternates": []}');
+INSERT INTO office_data VALUES('2368609','{"jis": "14108", "kana": "ヨコハマミナミコウキヨウシヨクギヨウアンテイシヨ", "name": "横浜南公共職業安定所", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "寺前", "banchi": "1-9-6", "postal_code": "2368609", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "テラマエ", "alternates": []}');
 INSERT INTO office_data VALUES('2368550','{"jis": "14108", "kana": "ヨコハマミナミゼイムシヨ", "name": "横浜南税務署", "prefecture": "神奈川県", "city": "横浜市金沢区", "neighborhood": "並木", "banchi": "3丁目2-9", "postal_code": "2368550", "old_code": "236  ", "post_office": "横浜金沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシカナザワク", "neighborhood_kana": "ナミキ", "alternates": []}');
 INSERT INTO office_data VALUES('2228556','{"jis": "14109", "kana": "アクサソンガイホケン カブシキガイシヤ", "name": "アクサ損害保険　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "新横浜", "banchi": "3丁目18番16号新横浜交通ビル7F", "postal_code": "2228556", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "シンヨコハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2228558','{"jis": "14109", "kana": "アマノ カブシキガイシヤ", "name": "アマノ　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "大豆戸町", "banchi": "275", "postal_code": "2228558", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "マメドチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2228564','{"jis": "14109", "kana": "アマノマネジメントサ-ビス カブシキガイシヤ", "name": "アマノマネジメントサービス　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "菊名", "banchi": "7丁目3-22", "postal_code": "2228564", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "キクナ", "alternates": []}');
 INSERT INTO office_data VALUES('2228565','{"jis": "14109", "kana": "アマノメンテナンスエンジニアリング カブシキガイシヤ", "name": "アマノメンテナンスエンジニアリング　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "菊名", "banchi": "7丁目3-22", "postal_code": "2228565", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "キクナ", "alternates": []}');
 INSERT INTO office_data VALUES('2228580','{"jis": "14109", "kana": "イノテツク カブシキガイシヤ", "name": "イノテック　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "新横浜", "banchi": "3丁目17-6", "postal_code": "2228580", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "シンヨコハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2228586','{"jis": "14109", "kana": "イノマイクロ カブシキガイシヤ", "name": "イノマイクロ　株式会社", "prefecture": "神奈川県", "city": "横浜市港北区", "neighborhood": "新横浜", "banchi": "2丁目13-13", "postal_code": "2228586", "old_code": "222  ", "post_office": "港北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシコウホクク", "neighborhood_kana": "シンヨコハマ", "alternates": []}');
@@ -130730,20 +130739,20 @@
 INSERT INTO office_data VALUES('2430460','{"jis": "14215", "kana": "リコ-テクノロジ-センタ-", "name": "リコーテクノロジーセンター", "prefecture": "神奈川県", "city": "海老名市", "neighborhood": "泉", "banchi": "二丁目7番1号", "postal_code": "2430460", "old_code": "24304", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "エビナシ", "neighborhood_kana": "イズミ", "alternates": []}');
 INSERT INTO office_data VALUES('2528540','{"jis": "14216", "kana": "エヌピ-オ-ホウジン カナガワケンシカクシヨウガイシヤフクシキヨウカイ", "name": "ＮＰＯ法人　神奈川県視覚障害者福祉協会", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "入谷", "banchi": "3丁目1707-16星野ハイツC102号", "postal_code": "2528540", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2528567','{"jis": "14216", "kana": "カブシキガイシヤ シ-イ-シ-", "name": "株式会社　シーイーシー", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "東原", "banchi": "5丁目1-11", "postal_code": "2528567", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒガシハラ", "alternates": []}');
 INSERT INTO office_data VALUES('2528539','{"jis": "14216", "kana": "カブシキガイシヤ マルスコ-ポレ-シヨン", "name": "株式会社　マルスコーポレーション", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "座間", "banchi": "2丁目2859", "postal_code": "2528539", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ザマ", "alternates": []}');
 INSERT INTO office_data VALUES('2528558','{"jis": "14216", "kana": "カブシキガイシヤ ユ-テムプレシジヨン", "name": "株式会社　ユーテムプレシジョン", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "ひばりが丘", "banchi": "4丁目21-1", "postal_code": "2528558", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒバリガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('2528511','{"jis": "14216", "kana": "キヤンプザマ", "name": "キャンプ座間", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "座間", "banchi": "無番地", "postal_code": "2528511", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ザマ", "alternates": []}');
 INSERT INTO office_data VALUES('2528566','{"jis": "14216", "kana": "ザマシヤクシヨ", "name": "座間市役所", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "緑ケ丘", "banchi": "1丁目1-1", "postal_code": "2528566", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ミドリガオカ", "alternates": []}');
-INSERT INTO office_data VALUES('2528550','{"jis": "14216", "kana": "トウキヨウコスモスデンキ カブシキガイシヤ", "name": "東京コスモス電機　株式会社", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "相武台", "banchi": "2丁目268", "postal_code": "2528550", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ソウブダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2528502','{"jis": "14216", "kana": "ニツサンジドウシヤ カブシキガイシヤ ザマジギヨウシヨ", "name": "日産自動車　株式会社　座間事業所", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "広野台", "banchi": "2丁目10-1", "postal_code": "2528502", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒロノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2528570','{"jis": "14216", "kana": "ニホンデンサント-ソク カブシキガイシヤ", "name": "日本電産トーソク　株式会社", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "相武台", "banchi": "2丁目215", "postal_code": "2528570", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ソウブダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2528585','{"jis": "14216", "kana": "ミキプ-リ (カブ) サガミジギヨウシヨ", "name": "三木プーリ　（株）　相模事業所", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "小松原", "banchi": "1丁目39-7", "postal_code": "2528585", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "コマツバラ", "alternates": []}');
 INSERT INTO office_data VALUES('2528572','{"jis": "14216", "kana": "イオンモ-ルザマ", "name": "イオンモール座間", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "広野台", "banchi": "2丁目10番4号", "postal_code": "2528572", "old_code": "252  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒロノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2528522','{"jis": "14216", "kana": "カブシキガイシヤ パルタツク ヨコハマシシヤ", "name": "株式会社　Ｐａｌｔａｃ　横浜支社", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "広野台", "banchi": "2丁目10番11号", "postal_code": "2528522", "old_code": "252  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒロノダイ", "alternates": []}');
+INSERT INTO office_data VALUES('2528550','{"jis": "14216", "kana": "トウキヨウコスモスデンキ カブシキガイシヤ", "name": "東京コスモス電機　株式会社", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "相武台", "banchi": "2丁目12番1号", "postal_code": "2528550", "old_code": "252  ", "post_office": "座間", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ソウブダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2528560','{"jis": "14216", "kana": "マガシ-クブツリユウセンタ-マガコ", "name": "マガシーク物流センターｍａｇａｃｏ", "prefecture": "神奈川県", "city": "座間市", "neighborhood": "広野台", "banchi": "2-10-8プロロジスパーク座間Ⅱ3F", "postal_code": "2528560", "old_code": "252  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ザマシ", "neighborhood_kana": "ヒロノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2500193','{"jis": "14217", "kana": "フジフイルム カブシキガイシヤ カナガワジギヨウジヨウ", "name": "富士フイルム　株式会社　神奈川事業場", "prefecture": "神奈川県", "city": "南足柄市", "neighborhood": "中沼", "banchi": "210", "postal_code": "2500193", "old_code": "25001", "post_office": "南足柄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミナミアシガラシ", "neighborhood_kana": "ナカヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('2500192','{"jis": "14217", "kana": "ミナミアシガラシヤクシヨ", "name": "南足柄市役所", "prefecture": "神奈川県", "city": "南足柄市", "neighborhood": "関本", "banchi": "440番地", "postal_code": "2500192", "old_code": "25001", "post_office": "南足柄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミナミアシガラシ", "neighborhood_kana": "セキモト", "alternates": []}');
 INSERT INTO office_data VALUES('2521192','{"jis": "14218", "kana": "アヤセシヤクシヨ", "name": "綾瀬市役所", "prefecture": "神奈川県", "city": "綾瀬市", "neighborhood": "早川", "banchi": "550", "postal_code": "2521192", "old_code": "252  ", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アヤセシ", "neighborhood_kana": "ハヤカワ", "alternates": []}');
 INSERT INTO office_data VALUES('2521195','{"jis": "14218", "kana": "カブシキガイシヤ ガステツク", "name": "株式会社　ガステック", "prefecture": "神奈川県", "city": "綾瀬市", "neighborhood": "深谷中", "banchi": "8丁目8番6号", "postal_code": "2521195", "old_code": "252  ", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アヤセシ", "neighborhood_kana": "フカヤナカ", "alternates": []}');
 INSERT INTO office_data VALUES('2521193','{"jis": "14218", "kana": "ザイダンホウジン サガミチユウオウカガクケンキユウジヨ", "name": "財団法人　相模中央化学研究所", "prefecture": "神奈川県", "city": "綾瀬市", "neighborhood": "早川", "banchi": "2743-1", "postal_code": "2521193", "old_code": "252  ", "post_office": "綾瀬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "アヤセシ", "neighborhood_kana": "ハヤカワ", "alternates": []}');
 INSERT INTO office_data VALUES('2400198','{"jis": "14301", "kana": "カブシキガイシヤ シヨウナンコクサイムラキヨウカイ", "name": "株式会社　湘南国際村協会", "prefecture": "神奈川県", "city": "三浦郡葉山町", "neighborhood": "上山口", "banchi": "1560-39", "postal_code": "2400198", "old_code": "24001", "post_office": "葉山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ミウラグンハヤママチ", "neighborhood_kana": "カミヤマグチ", "alternates": []}');
@@ -131251,16 +131260,16 @@
 INSERT INTO office_data VALUES('9490393','{"jis": "15216", "kana": "デンキカガクコウギヨウ カブシキガイシヤ オウミコウジヨウ", "name": "電気化学工業　株式会社　青海工場", "prefecture": "新潟県", "city": "糸魚川市", "neighborhood": "大字青海", "banchi": "2209番地", "postal_code": "9490393", "old_code": "94903", "post_office": "青海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9448601','{"jis": "15217", "kana": "アライシンヨウキンコ", "name": "新井信用金庫", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "栄町", "banchi": "2-3(新井郵便局私書箱第8号)", "postal_code": "9448601", "old_code": "944  ", "post_office": "新井", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ミョウコウシ", "neighborhood_kana": "サカエチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9448550','{"jis": "15217", "kana": "カブシキガイシヤ ダイセル アライコウジヨウ", "name": "株式会社　ダイセル　新井工場", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "新工町", "banchi": "1-1", "postal_code": "9448550", "old_code": "944  ", "post_office": "新井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ミョウコウシ", "neighborhood_kana": "シンコウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9448501','{"jis": "15217", "kana": "ケイナンソウゴウビヨウイン", "name": "けいなん総合病院", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "田町", "banchi": "2丁目4-7", "postal_code": "9448501", "old_code": "944  ", "post_office": "新井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ミョウコウシ", "neighborhood_kana": "タマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9448588','{"jis": "15217", "kana": "シンコウデンキコウギヨウ カブシキガイシヤ アライコウジヨウ", "name": "新光電気工業　株式会社　新井工場", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "大字姫川原", "banchi": "宮の前921-3", "postal_code": "9448588", "old_code": "944  ", "post_office": "新井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9448555','{"jis": "15217", "kana": "パナソニツク カブシキガイシヤ オ-トモ-テイブアンドインダストリアルシステムズシヤ セミコンダクタ-ジギヨウブ ホクリクコウジヨウ アライチク", "name": "パナソニック　株式会社　オートモーティブ＆インダストリアルシステムズ社　セミコンダクター事業部　北陸工場　新井地区", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "栗原", "banchi": "4丁目5番1号", "postal_code": "9448555", "old_code": "944  ", "post_office": "新井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ミョウコウシ", "neighborhood_kana": "クリハラ", "alternates": []}');
 INSERT INTO office_data VALUES('9448686','{"jis": "15217", "kana": "ミヨウコウシヤクシヨ", "name": "妙高市役所", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "栄町", "banchi": "5-1(新井郵便局私書箱第5号)", "postal_code": "9448686", "old_code": "944  ", "post_office": "新井", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ミョウコウシ", "neighborhood_kana": "サカエチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('9492193','{"jis": "15217", "kana": "シンニツポンデンコウ カブシキガイシヤ ミヨウコウコウジヨウ", "name": "新日本電工　株式会社　妙高工場", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "大字田口", "banchi": "272", "postal_code": "9492193", "old_code": "94921", "post_office": "妙高高原", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9492194','{"jis": "15217", "kana": "ダイイチデンコウ カブシキカイシヤ タグチコウジヨウ", "name": "第一電工　株式会社　田口工場", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "大字関川", "banchi": "70", "postal_code": "9492194", "old_code": "94921", "post_office": "妙高高原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('9492193','{"jis": "15217", "kana": "チユウオウデンキコウギヨウ カブシキカイシヤ タグチコウジヨウ", "name": "中央電気工業　株式会社　田口工場", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "大字田口", "banchi": "272", "postal_code": "9492193", "old_code": "94921", "post_office": "妙高高原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9492192','{"jis": "15217", "kana": "ミヨウコウシ ミヨウコウコウゲンシシヨ", "name": "妙高市　妙高高原支所", "prefecture": "新潟県", "city": "妙高市", "neighborhood": "大字関川", "banchi": "997", "postal_code": "9492192", "old_code": "94921", "post_office": "妙高高原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9591693','{"jis": "15218", "kana": "イ-グルブルグマンジヤパン カブシキガイシヤ", "name": "イーグルブルグマンジャパン　株式会社", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "中川新", "banchi": "514", "postal_code": "9591693", "old_code": "95916", "post_office": "五泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ゴセンシ", "neighborhood_kana": "ナカガワシン", "alternates": []}');
 INSERT INTO office_data VALUES('9591692','{"jis": "15218", "kana": "ゴセンシヤクシヨ", "name": "五泉市役所", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "大字太田", "banchi": "1094-1", "postal_code": "9591692", "old_code": "95916", "post_office": "五泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9591695','{"jis": "15218", "kana": "デンカセイケン カブシキカイシヤ ニイガタコウジヨウ", "name": "デンカ生研　株式会社　新潟工場", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "南本町", "banchi": "1丁目2-2", "postal_code": "9591695", "old_code": "95916", "post_office": "五泉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ゴセンシ", "neighborhood_kana": "ミナミホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9591795','{"jis": "15218", "kana": "カブシキガイシヤ アンナカセイサクシヨ", "name": "株式会社　安中製作所", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "本田屋", "banchi": "1144番地1", "postal_code": "9591795", "old_code": "95917", "post_office": "村松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ゴセンシ", "neighborhood_kana": "モトダイ", "alternates": []}');
 INSERT INTO office_data VALUES('9591797','{"jis": "15218", "kana": "カンバラテツドウ カブシキガイシヤ", "name": "蒲原鉄道　株式会社", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "村松", "banchi": "甲1364", "postal_code": "9591797", "old_code": "95917", "post_office": "村松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ゴセンシ", "neighborhood_kana": "ムラマツ", "alternates": []}');
 INSERT INTO office_data VALUES('9591794','{"jis": "15218", "kana": "タイマツシヨクヒン カブシキガイシヤ", "name": "たいまつ食品　株式会社", "prefecture": "新潟県", "city": "五泉市", "neighborhood": "村松", "banchi": "1345", "postal_code": "9591794", "old_code": "95917", "post_office": "村松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ゴセンシ", "neighborhood_kana": "ムラマツ", "alternates": []}');
@@ -131774,14 +131783,15 @@
 INSERT INTO office_data VALUES('9208623','{"jis": "17201", "kana": "カブシキガイシヤ ニツサンサテイオイシカワ", "name": "株式会社　日産サティオ石川", "prefecture": "石川県", "city": "金沢市", "neighborhood": "浅野本町", "banchi": "ロ124", "postal_code": "9208623", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "アサノホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208638','{"jis": "17201", "kana": "カブシキガイシヤ フクミツヤ", "name": "株式会社　福光屋", "prefecture": "石川県", "city": "金沢市", "neighborhood": "石引", "banchi": "2丁目8-3", "postal_code": "9208638", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "イシビキ", "alternates": []}');
 INSERT INTO office_data VALUES('9208521','{"jis": "17201", "kana": "カブシキガイシヤ ヘイワドウアル・プラザカナザワ", "name": "（株）　平和堂アル・プラザ金沢", "prefecture": "石川県", "city": "金沢市", "neighborhood": "諸江町", "banchi": "上丁30-1", "postal_code": "9208521", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "モロエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208515','{"jis": "17201", "kana": "カブシキガイシヤ ホクツウ", "name": "株式会社　ほくつう", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "1丁目65番地", "postal_code": "9208515", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208556','{"jis": "17201", "kana": "カブシキガイシヤ ホクリクアイテイエス", "name": "株式会社　北陸アイティエス", "prefecture": "石川県", "city": "金沢市", "neighborhood": "本多町", "banchi": "3丁目2番1号", "postal_code": "9208556", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ホンダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208686','{"jis": "17201", "kana": "カブシキガイシヤ ホクリクギンコウ カナザワシテン", "name": "株式会社　北陸銀行　金沢支店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "尾山町", "banchi": "2-22(金沢中央郵便局私書箱第88号)", "postal_code": "9208686", "old_code": "920  ", "post_office": "金沢中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "オヤママチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208588','{"jis": "17201", "kana": "カブシキガイシヤ ホツコクシンブンシヤ", "name": "株式会社　北國新聞社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "香林坊", "banchi": "2丁目5-1", "postal_code": "9208588", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コウリンボウ", "alternates": []}');
+INSERT INTO office_data VALUES('9208545','{"jis": "17201", "kana": "カブシキガイシヤ マルビシ", "name": "株式会社　丸菱", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "2丁目20番地", "postal_code": "9208545", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208625','{"jis": "17201", "kana": "カブシキガイシヤ ミナミシヨウテン", "name": "株式会社　南商店", "prefecture": "石川県", "city": "金沢市", "neighborhood": "京町", "banchi": "25-15", "postal_code": "9208625", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "キョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208665','{"jis": "17201", "kana": "カブシキガイシヤ ヤマコシ", "name": "株式会社　山越", "prefecture": "石川県", "city": "金沢市", "neighborhood": "兼六元町", "banchi": "3-78", "postal_code": "9208665", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ケンロクモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208535','{"jis": "17201", "kana": "カブシキガイシヤ ヨシカワ", "name": "株式会社　ヨシカワ", "prefecture": "石川県", "city": "金沢市", "neighborhood": "広岡", "banchi": "三丁目3番77号JR金沢駅西第一NKビル6F", "postal_code": "9208535", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ヒロオカ", "alternates": []}');
 INSERT INTO office_data VALUES('9208620','{"jis": "17201", "kana": "ガツコウホウジン イナオキガクエン カナザワセイリヨウダイガク", "name": "学校法人　稲置学園　金沢星稜大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "御所町", "banchi": "丑10番地1", "postal_code": "9208620", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "ゴショマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208554','{"jis": "17201", "kana": "ガツコウホウジン ヒシヨウ カナザワジヨウホウビジネスセンモンガツコウ", "name": "学校法人　飛翔　金沢情報ビジネス専門学校", "prefecture": "石川県", "city": "金沢市", "neighborhood": "高岡町", "banchi": "3番20号", "postal_code": "9208554", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "タカオカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208543','{"jis": "17201", "kana": "キタムラデンキサンギヨウ カブシキガイシヤ", "name": "北村電機産業　株式会社", "prefecture": "石川県", "city": "金沢市", "neighborhood": "問屋町", "banchi": "1丁目11", "postal_code": "9208543", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "トイヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9208656','{"jis": "17201", "kana": "コウリツダイガクホウジン カナザワビジユツコウゲイダイガク", "name": "公立大学法人　金沢美術工芸大学", "prefecture": "石川県", "city": "金沢市", "neighborhood": "小立野", "banchi": "2丁目40番1号", "postal_code": "9208656", "old_code": "920  ", "post_office": "金沢中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "カナザワシ", "neighborhood_kana": "コダツノ", "alternates": []}');
@@ -132670,14 +132680,15 @@
 INSERT INTO office_data VALUES('3808570','{"jis": "20201", "kana": "ナガノケンチヨウ", "name": "長野県庁", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長野", "banchi": "字巾下692-2", "postal_code": "3808570", "old_code": "38070", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808666','{"jis": "20201", "kana": "チユウブデンリヨク カブシキガイシヤ ナガノシテン", "name": "中部電力　株式会社　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "柳町", "banchi": "18(長野中央郵便局私書箱第42号)", "postal_code": "3808666", "old_code": "38091", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ヤナギマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3808686','{"jis": "20201", "kana": "ナガノシンヨウキンコ", "name": "長野信用金庫", "prefecture": "長野県", "city": "長野市", "neighborhood": "居町", "banchi": "133-1(長野中央郵便局私書箱第24号)", "postal_code": "3808686", "old_code": "38091", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "イマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3808612','{"jis": "20201", "kana": "ナガノゼイムシヨ", "name": "長野税務署", "prefecture": "長野県", "city": "長野市", "neighborhood": "", "banchi": "随後町608-2(長野中央郵便局私書箱第8号)", "postal_code": "3808612", "old_code": "38091", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808640','{"jis": "20201", "kana": "ノムラシヨウケン カブシキガイシヤ ナガノシテン", "name": "野村證券　株式会社　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長野", "banchi": "末広町1361(長野中央郵便局私書箱第49号)", "postal_code": "3808640", "old_code": "38091", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818530','{"jis": "20201", "kana": "アサバサンギヨウ カブシキガイシヤ", "name": "麻場産業　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字北長池", "banchi": "1443-2", "postal_code": "3818530", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818510','{"jis": "20201", "kana": "イツパンシヤダンホウジン ナガノケンジドウシヤセイビシンコウカイ", "name": "一般社団法人　長野県自動車整備振興会", "prefecture": "長野県", "city": "長野市", "neighborhood": "西和田", "banchi": "一丁目35番2号", "postal_code": "3818510", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ニシワダ", "alternates": []}');
+INSERT INTO office_data VALUES('3818501','{"jis": "20201", "kana": "エフアイシ-テイ カブシキガイシヤ", "name": "ＦＩＣＴ　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "北尾張部", "banchi": "36", "postal_code": "3818501", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "キタオワリベ", "alternates": []}');
 INSERT INTO office_data VALUES('3818560','{"jis": "20201", "kana": "オカヤサンソ カブシキガイシヤ ナガノジギヨウブ", "name": "岡谷酸素　株式会社　長野事業部", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字中越", "banchi": "1-1-1", "postal_code": "3818560", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818545','{"jis": "20201", "kana": "カブシキガイシヤ クリエイテイブヨ-コ", "name": "株式会社　クリエイティブヨーコ", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字高田", "banchi": "667-16", "postal_code": "3818545", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818520','{"jis": "20201", "kana": "カブシキガイシヤ シンエイハイテツク", "name": "株式会社　シンエイハイテック", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字柳原", "banchi": "1625-2", "postal_code": "3818520", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818508','{"jis": "20201", "kana": "カブシキガイシヤ デジタル・ラボラトリ-", "name": "株式会社　デジタル・ラボラトリー", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字北長池", "banchi": "1951-5", "postal_code": "3818508", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818525','{"jis": "20201", "kana": "カブシキガイシヤ デンセン", "name": "株式会社　デンセン", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長池", "banchi": "713-1", "postal_code": "3818525", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818548','{"jis": "20201", "kana": "カブシキガイシヤ ト-シス", "name": "株式会社　ＴＯＳＹＳ", "prefecture": "長野県", "city": "長野市", "neighborhood": "北長池", "banchi": "1898-10", "postal_code": "3818548", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "キタナガイケ", "alternates": []}');
 INSERT INTO office_data VALUES('3818588','{"jis": "20201", "kana": "カブシキガイシヤ モトキユウ", "name": "株式会社　本久", "prefecture": "長野県", "city": "長野市", "neighborhood": "桐原", "banchi": "1丁目3番5号", "postal_code": "3818588", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "キリハラ", "alternates": []}');
@@ -132688,15 +132699,14 @@
 INSERT INTO office_data VALUES('3818558','{"jis": "20201", "kana": "ナガノキタシヤカイホケンジムシヨ", "name": "長野北社会保険事務所", "prefecture": "長野県", "city": "長野市", "neighborhood": "吉田", "banchi": "3丁目6-15", "postal_code": "3818558", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ヨシダ", "alternates": []}');
 INSERT INTO office_data VALUES('3818577','{"jis": "20201", "kana": "ナガノケン シンタイシヨウガイシヤリハビリテ-シヨンセンタ-", "name": "長野県　身体障害者リハビリテーションセンター", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字下駒沢", "banchi": "618-1", "postal_code": "3818577", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818556','{"jis": "20201", "kana": "ナガノケン トラツクカイカン", "name": "長野県　トラック会館", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長池", "banchi": "710-3", "postal_code": "3818556", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818570','{"jis": "20201", "kana": "ナガノケンリツ ナガノヨシダコウコウ", "name": "長野県立　長野吉田高校", "prefecture": "長野県", "city": "長野市", "neighborhood": "吉田", "banchi": "2丁目12-9", "postal_code": "3818570", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ヨシダ", "alternates": []}');
 INSERT INTO office_data VALUES('3818550','{"jis": "20201", "kana": "ナガノコウギヨウコウトウセンモンガツコウ", "name": "長野工業高等専門学校", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字徳間", "banchi": "716", "postal_code": "3818550", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818551','{"jis": "20201", "kana": "ナガノシミンビヨウイン", "name": "長野市民病院", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字富竹", "banchi": "1333番地1", "postal_code": "3818551", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818503','{"jis": "20201", "kana": "ニイガタウンユキヨク ナガノリクウンシキヨク", "name": "新潟運輸局　長野陸運支局", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字西和田", "banchi": "428-1", "postal_code": "3818503", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3818501','{"jis": "20201", "kana": "フジツウ カブシキガイシヤ ナガノコウジヨウ", "name": "富士通　株式会社　長野工場", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字北尾張部", "banchi": "36", "postal_code": "3818501", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3818539','{"jis": "20201", "kana": "マツダサンギヨウ カブシキガイシヤ", "name": "松田産業　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長池", "banchi": "369-5", "postal_code": "3818539", "old_code": "381  ", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3810193','{"jis": "20201", "kana": "カブシキガイシヤ ト-シス", "name": "株式会社　ＴＯＳＹＳ", "prefecture": "長野県", "city": "長野市", "neighborhood": "若穂綿内", "banchi": "字東山1108-5", "postal_code": "3810193", "old_code": "38101", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ワカホワタウチ", "alternates": []}');
 INSERT INTO office_data VALUES('3810192','{"jis": "20201", "kana": "カブシキガイシヤ マルスイナガノケンスイ ナガノシテン", "name": "株式会社　丸水長野県水　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "若穂川田", "banchi": "字外新田3800-12", "postal_code": "3810192", "old_code": "38101", "post_office": "長野東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ワカホカワダ", "alternates": []}');
 INSERT INTO office_data VALUES('3812280','{"jis": "20201", "kana": "カブシキガイシヤ シユ-マ-ト", "name": "株式会社　シューマート", "prefecture": "長野県", "city": "長野市", "neighborhood": "稲里町中氷鉋", "banchi": "458", "postal_code": "3812280", "old_code": "38112", "post_office": "長野南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "イナサトマチナカヒガノ", "alternates": []}');
 INSERT INTO office_data VALUES('3812292','{"jis": "20201", "kana": "カブシキガイシヤ エス・エス・ブイ", "name": "株式会社　エス・エス・ブイ", "prefecture": "長野県", "city": "長野市", "neighborhood": "川中島町御厨", "banchi": "37", "postal_code": "3812292", "old_code": "38122", "post_office": "長野南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "カワナカジママチミクリヤ", "alternates": []}');
 INSERT INTO office_data VALUES('3812281','{"jis": "20201", "kana": "カブシキガイシヤ マルイチサンシヨウ", "name": "株式会社　マルイチ産商", "prefecture": "長野県", "city": "長野市", "neighborhood": "市場", "banchi": "3-48", "postal_code": "3812281", "old_code": "38122", "post_office": "長野南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "イチバ", "alternates": []}');
 INSERT INTO office_data VALUES('3812286','{"jis": "20201", "kana": "カブシキガイシヤ マルスイナガノケンスイ", "name": "株式会社　丸水長野県水", "prefecture": "長野県", "city": "長野市", "neighborhood": "市場", "banchi": "3-43", "postal_code": "3812286", "old_code": "38122", "post_office": "長野南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "イチバ", "alternates": []}');
@@ -132732,14 +132742,15 @@
 INSERT INTO office_data VALUES('3908610','{"jis": "20202", "kana": "カブシキカイシヤ エイコ-", "name": "株式会社　エイコー", "prefecture": "長野県", "city": "松本市", "neighborhood": "大字島内", "banchi": "3314", "postal_code": "3908610", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3908639','{"jis": "20202", "kana": "カブシキガイシヤ アスピア", "name": "株式会社　アスピア", "prefecture": "長野県", "city": "松本市", "neighborhood": "宮渕", "banchi": "1丁目3-30", "postal_code": "3908639", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ミヤブチ", "alternates": []}');
 INSERT INTO office_data VALUES('3908507','{"jis": "20202", "kana": "カブシキガイシヤ イノウエ", "name": "株式会社　井上", "prefecture": "長野県", "city": "松本市", "neighborhood": "深志", "banchi": "2丁目3-1", "postal_code": "3908507", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "フカシ", "alternates": []}');
 INSERT INTO office_data VALUES('3908539','{"jis": "20202", "kana": "カブシキガイシヤ シミンタイムス", "name": "（株）　市民タイムス", "prefecture": "長野県", "city": "松本市", "neighborhood": "大字島立", "banchi": "800", "postal_code": "3908539", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3908686','{"jis": "20202", "kana": "カブシキガイシヤ チユウブニホンイヤク", "name": "株式会社　中部日本医薬", "prefecture": "長野県", "city": "松本市", "neighborhood": "筑摩", "banchi": "2丁目26-17", "postal_code": "3908686", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ツカマ", "alternates": []}');
 INSERT INTO office_data VALUES('3908611','{"jis": "20202", "kana": "カブシキガイシヤ テレビシンシユウ", "name": "株式会社　テレビ信州", "prefecture": "長野県", "city": "松本市", "neighborhood": "丸の内", "banchi": "4-18", "postal_code": "3908611", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
 INSERT INTO office_data VALUES('3908630','{"jis": "20202", "kana": "カブシキガイシヤ ニシマ", "name": "株式会社　ニシマ", "prefecture": "長野県", "city": "松本市", "neighborhood": "大字島内", "banchi": "3503", "postal_code": "3908630", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('3908704','{"jis": "20202", "kana": "カブシキガイシヤ ハチジユウニギンコウ マツモトエイギヨウブ", "name": "株式会社　八十二銀行　松本営業部", "prefecture": "長野県", "city": "松本市", "neighborhood": "大手", "banchi": "3丁目1番1号(松本郵便局私書箱第30号)", "postal_code": "3908704", "old_code": "390  ", "post_office": "松本", "type": "box", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "オオテ", "alternates": []}');
 INSERT INTO office_data VALUES('3908623','{"jis": "20202", "kana": "ガツコウホウジン ガイゴガクエン シナノムツミコウトウガツコウ", "name": "学校法人　外語学園　信農むつみ高等学校", "prefecture": "長野県", "city": "松本市", "neighborhood": "南松本", "banchi": "1丁目13-26", "postal_code": "3908623", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ミナミマツモト", "alternates": []}');
 INSERT INTO office_data VALUES('3908535','{"jis": "20202", "kana": "コクミンセイカツキンユウコウコ", "name": "国民生活金融公庫", "prefecture": "長野県", "city": "松本市", "neighborhood": "中央", "banchi": "1丁目4-20", "postal_code": "3908535", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3908585','{"jis": "20202", "kana": "シナノマイニチシンブンシヤ マツモトホンシヤ(シンマイメデイアガ-デン)", "name": "信濃毎日新聞社　松本本社（信毎メディアガーデン）", "prefecture": "長野県", "city": "松本市", "neighborhood": "中央", "banchi": "2丁目20-2", "postal_code": "3908585", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('3908648','{"jis": "20202", "kana": "シヤカイイリヨウホウジン シロニシイリヨウザイダン シロニシビヨウイン", "name": "社会医療法人　城西医療財団　城西病院", "prefecture": "長野県", "city": "松本市", "neighborhood": "城西", "banchi": "1丁目5-16", "postal_code": "3908648", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ジョウセイ", "alternates": []}');
 INSERT INTO office_data VALUES('3908511','{"jis": "20202", "kana": "シヤダンホウジン サイノウキヨウイクケンキユウカイ", "name": "社団法人　才能教育研究会", "prefecture": "長野県", "city": "松本市", "neighborhood": "深志", "banchi": "3丁目10-3", "postal_code": "3908511", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "フカシ", "alternates": []}');
 INSERT INTO office_data VALUES('3908530','{"jis": "20202", "kana": "シンケン カブシキガイシヤ", "name": "シンケン　株式会社", "prefecture": "長野県", "city": "松本市", "neighborhood": "庄内", "banchi": "3丁目4-39", "postal_code": "3908530", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "ショウナイ", "alternates": []}');
 INSERT INTO office_data VALUES('3908621','{"jis": "20202", "kana": "シンシユウダイガク", "name": "信州大学", "prefecture": "長野県", "city": "松本市", "neighborhood": "旭", "banchi": "3丁目1-1", "postal_code": "3908621", "old_code": "390  ", "post_office": "松本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "マツモトシ", "neighborhood_kana": "アサヒ", "alternates": []}');
@@ -132920,15 +132931,14 @@
 INSERT INTO office_data VALUES('3828555','{"jis": "20207", "kana": "カブシキガイシヤ マエダテツコウジヨ", "name": "株式会社　前田鉄工所", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字豊丘", "banchi": "1385-1", "postal_code": "3828555", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828512','{"jis": "20207", "kana": "スコウギヨウセイジムクミアイ", "name": "須高行政事務組合", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字小山", "banchi": "字布田2104番地の36", "postal_code": "3828512", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828505','{"jis": "20207", "kana": "スザカシガツコウキユウシヨクセンタ-", "name": "須坂市学校給食センター", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字栃倉", "banchi": "420番地1", "postal_code": "3828505", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828511','{"jis": "20207", "kana": "スザカシヤクシヨ", "name": "須坂市役所", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字須坂", "banchi": "東横町1528-1", "postal_code": "3828511", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828633','{"jis": "20207", "kana": "ナガノケイムシヨ", "name": "長野刑務所", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字須坂", "banchi": "馬場町1200", "postal_code": "3828633", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828577','{"jis": "20207", "kana": "ナガノケンリツシンシユウイリヨウセンタ-", "name": "長野県立信州医療センター", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字須坂", "banchi": "1332", "postal_code": "3828577", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828587','{"jis": "20207", "kana": "ナガノノウギヨウキヨウドウクミアイ スザカシシヨ", "name": "ながの農業協同組合　須坂支所", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字小山", "banchi": "1253番地の5", "postal_code": "3828587", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3828501','{"jis": "20207", "kana": "フジツウ カブシキガイシヤ スザカコウジヨウ", "name": "富士通　株式会社　須坂工場", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字小山", "banchi": "460", "postal_code": "3828501", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828585','{"jis": "20207", "kana": "ホクリクコカ・コ-ラボトリング カブシキガイシヤ", "name": "北陸コカ・コーラボトリング　株式会社", "prefecture": "長野県", "city": "須坂市", "neighborhood": "大字井上", "banchi": "字砂田1700-8", "postal_code": "3828585", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3848511','{"jis": "20208", "kana": "カブシキガイシヤ コモロムラタセイサクジヨ", "name": "株式会社　小諸村田製作所", "prefecture": "長野県", "city": "小諸市", "neighborhood": "柏木", "banchi": "190番地", "postal_code": "3848511", "old_code": "384  ", "post_office": "小諸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "カシワギ", "alternates": []}');
 INSERT INTO office_data VALUES('3848605','{"jis": "20208", "kana": "コモロシヤカイホケンジムシヨ", "name": "小諸社会保険事務所", "prefecture": "長野県", "city": "小諸市", "neighborhood": "乙", "banchi": "294-23(小諸郵便局私書箱第27号)", "postal_code": "3848605", "old_code": "384  ", "post_office": "小諸", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "オツ", "alternates": []}');
 INSERT INTO office_data VALUES('3848501','{"jis": "20208", "kana": "コモロシヤクシヨ", "name": "小諸市役所", "prefecture": "長野県", "city": "小諸市", "neighborhood": "相生町", "banchi": "3丁目3ー3", "postal_code": "3848501", "old_code": "384  ", "post_office": "小諸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "アイオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3848558','{"jis": "20208", "kana": "ナカタナオンセン ナカタナソウ", "name": "中棚温泉　中棚荘", "prefecture": "長野県", "city": "小諸市", "neighborhood": "", "banchi": "古城乙1210", "postal_code": "3848558", "old_code": "384  ", "post_office": "小諸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3848588','{"jis": "20208", "kana": "ナガノケンコウセイノウギヨウキヨウドウクミアイレンゴウカイ アサマナンロクコモロイリヨウセンタ-", "name": "長野県厚生農業協同組合連合会　浅間南麓こもろ医療センター", "prefecture": "長野県", "city": "小諸市", "neighborhood": "相生町", "banchi": "三丁目3番21号", "postal_code": "3848588", "old_code": "384  ", "post_office": "小諸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "アイオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3848585','{"jis": "20208", "kana": "ニツセイエ-.エス.ビ-キカイ カブシキカイシヤ", "name": "日精エー・エス・ビー機械　株式会社", "prefecture": "長野県", "city": "小諸市", "neighborhood": "", "banchi": "天池4586ー3", "postal_code": "3848585", "old_code": "384  ", "post_office": "小諸", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "コモロシ", "neighborhood_kana": "", "alternates": []}');
@@ -132968,15 +132978,14 @@
 INSERT INTO office_data VALUES('3892192','{"jis": "20211", "kana": "ナカノシヤクシヨ トヨタシシヨ", "name": "中野市役所　豊田支所", "prefecture": "長野県", "city": "中野市", "neighborhood": "大字豊津", "banchi": "395-1", "postal_code": "3892192", "old_code": "38921", "post_office": "豊井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3988501','{"jis": "20212", "kana": "オオマチゼイムシヨ", "name": "大町税務署", "prefecture": "長野県", "city": "大町市", "neighborhood": "大字大町", "banchi": "3190-16", "postal_code": "3988501", "old_code": "398  ", "post_office": "大町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3988686','{"jis": "20212", "kana": "カブシキカイシヤ サガミグミ", "name": "株式会社　相模組", "prefecture": "長野県", "city": "大町市", "neighborhood": "大町", "banchi": "3052(大町郵便局私書箱第14号)", "postal_code": "3988686", "old_code": "398  ", "post_office": "大町", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "オオマチシ", "neighborhood_kana": "オオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3988602','{"jis": "20212", "kana": "ナガノケンオオマチゴウドウチヨウシヤ", "name": "長野県大町合同庁舎", "prefecture": "長野県", "city": "大町市", "neighborhood": "大町", "banchi": "1058-2(大町郵便局私書箱第15号)", "postal_code": "3988602", "old_code": "398  ", "post_office": "大町", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "オオマチシ", "neighborhood_kana": "オオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3988601','{"jis": "20212", "kana": "オオマチシヤクシヨ", "name": "大町市役所", "prefecture": "長野県", "city": "大町市", "neighborhood": "大町", "banchi": "3887(大町郵便局私書箱第5号)", "postal_code": "3988601", "old_code": "39891", "post_office": "大町", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "オオマチシ", "neighborhood_kana": "オオマチ", "alternates": []}');
 INSERT INTO office_data VALUES('3999192','{"jis": "20212", "kana": "オオマチシ ミアサシシヨ", "name": "大町市　美麻支所", "prefecture": "長野県", "city": "大町市", "neighborhood": "美麻", "banchi": "11399", "postal_code": "3999192", "old_code": "39991", "post_office": "大町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "オオマチシ", "neighborhood_kana": "ミアサ", "alternates": []}');
 INSERT INTO office_data VALUES('3892292','{"jis": "20213", "kana": "イイヤマシヤクシヨ", "name": "飯山市役所", "prefecture": "長野県", "city": "飯山市", "neighborhood": "大字飯山", "banchi": "1110-1", "postal_code": "3892292", "old_code": "38922", "post_office": "飯山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3892298','{"jis": "20213", "kana": "カブシキガイシヤ シナノフジツウ", "name": "株式会社　しなの富士通", "prefecture": "長野県", "city": "飯山市", "neighborhood": "大字野坂田", "banchi": "935", "postal_code": "3892298", "old_code": "38922", "post_office": "飯山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3918531','{"jis": "20214", "kana": "カブシキガイシヤ イ-スタン", "name": "株式会社　イースタン", "prefecture": "長野県", "city": "茅野市", "neighborhood": "塚原", "banchi": "1-8-37", "postal_code": "3918531", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "ツカハラ", "alternates": []}');
 INSERT INTO office_data VALUES('3918550','{"jis": "20214", "kana": "カブシキガイシヤ イイヌマゲ-ジセイサクジヨ", "name": "株式会社　飯沼ゲージ製作所", "prefecture": "長野県", "city": "茅野市", "neighborhood": "玉川", "banchi": "11400-1078", "postal_code": "3918550", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "タマガワ", "alternates": []}');
 INSERT INTO office_data VALUES('3918566','{"jis": "20214", "kana": "カブシキガイシヤ キツツマイクロフイルタ- チノコウジヨウ", "name": "株式会社　キッツマイクロフィルター　茅野工場", "prefecture": "長野県", "city": "茅野市", "neighborhood": "金沢", "banchi": "5125番地", "postal_code": "3918566", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "カナザワ", "alternates": []}');
 INSERT INTO office_data VALUES('3918555','{"jis": "20214", "kana": "カブシキガイシヤ キツツメタルワ-クス", "name": "株式会社　キッツメタルワークス", "prefecture": "長野県", "city": "茅野市", "neighborhood": "宮川", "banchi": "7377", "postal_code": "3918555", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "ミヤガワ", "alternates": []}');
 INSERT INTO office_data VALUES('3918580','{"jis": "20214", "kana": "カブシキガイシヤ ツチハシ", "name": "株式会社　ツチハシ", "prefecture": "長野県", "city": "茅野市", "neighborhood": "本町西", "banchi": "21番2号", "postal_code": "3918580", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3918558','{"jis": "20214", "kana": "カブシキガイシヤ ヤジマ", "name": "株式会社　矢島", "prefecture": "長野県", "city": "茅野市", "neighborhood": "金沢", "banchi": "3410-3", "postal_code": "3918558", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "カナザワ", "alternates": []}');
 INSERT INTO office_data VALUES('3918522','{"jis": "20214", "kana": "シンシユウスワノウギヨウキヨウドウクミアイ", "name": "信州諏訪農業協同組合", "prefecture": "長野県", "city": "茅野市", "neighborhood": "仲町", "banchi": "24番4号", "postal_code": "3918522", "old_code": "391  ", "post_office": "茅野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "チノシ", "neighborhood_kana": "ナカマチ", "alternates": []}');
@@ -133164,15 +133173,14 @@
 INSERT INTO office_data VALUES('3810296','{"jis": "20541", "kana": "カブシキガイシヤ ナガイコウギヨウシヨ", "name": "株式会社　永井工業所", "prefecture": "長野県", "city": "上高井郡小布施町", "neighborhood": "大字雁田", "banchi": "438", "postal_code": "3810296", "old_code": "38102", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3810298','{"jis": "20541", "kana": "サクライカンセイドウ", "name": "桜井甘精堂", "prefecture": "長野県", "city": "上高井郡小布施町", "neighborhood": "大字小布施", "banchi": "2460-1", "postal_code": "3810298", "old_code": "38102", "post_office": "小布施", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3810295','{"jis": "20541", "kana": "シンセイビヨウイン", "name": "新生病院", "prefecture": "長野県", "city": "上高井郡小布施町", "neighborhood": "大字小布施", "banchi": "851", "postal_code": "3810295", "old_code": "38102", "post_office": "小布施", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828508','{"jis": "20543", "kana": "アスザツク カブシキカイシヤ", "name": "アスザック　株式会社", "prefecture": "長野県", "city": "上高井郡高山村", "neighborhood": "大字中山", "banchi": "981", "postal_code": "3828508", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3828510','{"jis": "20543", "kana": "タカヤマムラヤクバ", "name": "高山村役場", "prefecture": "長野県", "city": "上高井郡高山村", "neighborhood": "大字高井", "banchi": "4972", "postal_code": "3828510", "old_code": "382  ", "post_office": "須坂", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3810497','{"jis": "20561", "kana": "シガコウゲンプリンスホテル", "name": "志賀高原プリンスホテル", "prefecture": "長野県", "city": "下高井郡山ノ内町", "neighborhood": "大字平穏", "banchi": "7149", "postal_code": "3810497", "old_code": "38104", "post_office": "湯田中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3810498','{"jis": "20561", "kana": "ヤマノウチマチヤクバ", "name": "山ノ内町役場", "prefecture": "長野県", "city": "下高井郡山ノ内町", "neighborhood": "大字平穏", "banchi": "3352-1", "postal_code": "3810498", "old_code": "38104", "post_office": "湯田中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3892392','{"jis": "20562", "kana": "キジマダイラムラヤクバ", "name": "木島平村役場", "prefecture": "長野県", "city": "下高井郡木島平村", "neighborhood": "大字往郷", "banchi": "973-1", "postal_code": "3892392", "old_code": "38923", "post_office": "木島平", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3892592','{"jis": "20563", "kana": "ノザワオンセンムラヤクバ", "name": "野沢温泉村役場", "prefecture": "長野県", "city": "下高井郡野沢温泉村", "neighborhood": "大字豊郷", "banchi": "9817", "postal_code": "3892592", "old_code": "38925", "post_office": "木島平", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3891392','{"jis": "20583", "kana": "シナノマチヤクバ", "name": "信濃町役場", "prefecture": "長野県", "city": "上水内郡信濃町", "neighborhood": "大字柏原", "banchi": "428-2", "postal_code": "3891392", "old_code": "38913", "post_office": "信濃町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3891293','{"jis": "20590", "kana": "イイヅナマチヤクバ", "name": "飯綱町役場", "prefecture": "長野県", "city": "上水内郡飯綱町", "neighborhood": "大字牟礼", "banchi": "2795-1", "postal_code": "3891293", "old_code": "38912", "post_office": "信濃町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3892792','{"jis": "20602", "kana": "サカエムラヤクバ", "name": "栄村役場", "prefecture": "長野県", "city": "下水内郡栄村", "neighborhood": "大字北信", "banchi": "3433", "postal_code": "3892792", "old_code": "38927", "post_office": "桑名川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('5008523','{"jis": "21201", "kana": "アサヒダイガクシガクブフゾクムラカミキネンビヨウイン", "name": "朝日大学歯学部附属村上記念病院", "prefecture": "岐阜県", "city": "岐阜市", "neighborhood": "橋本町", "banchi": "3丁目23", "postal_code": "5008523", "old_code": "500  ", "post_office": "岐阜中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ギフシ", "neighborhood_kana": "ハシモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5008558','{"jis": "21201", "kana": "アピ カブシキガイシヤ", "name": "アピ　株式会社", "prefecture": "岐阜県", "city": "岐阜市", "neighborhood": "加納桜田町", "banchi": "1丁目1番地", "postal_code": "5008558", "old_code": "500  ", "post_office": "岐阜中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ギフシ", "neighborhood_kana": "カノウサクラダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5008672','{"jis": "21201", "kana": "アライ カブシキガイシヤ", "name": "荒井　株式会社", "prefecture": "岐阜県", "city": "岐阜市", "neighborhood": "中鶉", "banchi": "2丁目6-2", "postal_code": "5008672", "old_code": "500  ", "post_office": "岐阜中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ギフケン", "city_kana": "ギフシ", "neighborhood_kana": "ナカウズラ", "alternates": []}');
@@ -133823,15 +133831,15 @@
 INSERT INTO office_data VALUES('4308540','{"jis": "22138", "kana": "ニツカン (カブ)", "name": "日管　（株）", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "池町", "banchi": "220-4", "postal_code": "4308540", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "イケマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4308670','{"jis": "22138", "kana": "ハママツイワタシンヨウキンコ", "name": "浜松磐田信用金庫", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "元城町", "banchi": "114番地の1", "postal_code": "4308670", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "モトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308611','{"jis": "22138", "kana": "ハママツエフエムホウソウ カブシキガイシヤ エフエム ハロ-!", "name": "浜松エフエム放送　株式会社　ＦＭ　Ｈａｒｏ！", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "鍛冶町", "banchi": "100番地の1ザザシティ浜松中央館4階", "postal_code": "4308611", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "カジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4308570','{"jis": "22138", "kana": "ハママツカンイサイバンシヨ", "name": "浜松簡易裁判所", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "中央", "banchi": "1丁目12番5号", "postal_code": "4308570", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308652','{"jis": "22138", "kana": "ハママツシヤクシヨ・チユウオウクヤクシヨ", "name": "浜松市役所・中央区役所", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "元城町", "banchi": "103-2(浜松郵便局私書箱第64号)", "postal_code": "4308652", "old_code": "430  ", "post_office": "浜松", "type": "box", "multiple": true, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "モトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308653','{"jis": "22138", "kana": "ハママツシヤクシヨ・チユウオウクヤクシヨ", "name": "浜松市役所・中央区役所", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "元城町", "banchi": "103-2(浜松郵便局私書箱第64号)", "postal_code": "4308653", "old_code": "430  ", "post_office": "浜松", "type": "box", "multiple": true, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "モトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308585','{"jis": "22138", "kana": "ハママツニシゼイムシヨ", "name": "浜松西税務署", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "中央", "banchi": "1丁目12-4", "postal_code": "4308585", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
-INSERT INTO office_data VALUES('4308667','{"jis": "22138", "kana": "ハママツヒガシゼイムシヨ", "name": "浜松東税務署", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "砂山町", "banchi": "1183番地", "postal_code": "4308667", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "スナヤマチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4308667','{"jis": "22138", "kana": "ハママツヒガシゼイムシヨ", "name": "浜松東税務署", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "砂山町", "banchi": "1183番地", "postal_code": "4308667", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "スナヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308587','{"jis": "22138", "kana": "ハママツホトニクス カブシキガイシヤ ホンシヤジムシヨ", "name": "浜松ホトニクス　株式会社　本社事務所", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "砂山町", "banchi": "325-6", "postal_code": "4308587", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "スナヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308639','{"jis": "22138", "kana": "ハママツロウドウキジユンカントクシヨ", "name": "浜松労働基準監督署", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "中央", "banchi": "1丁目12番4号浜松合同庁舎8階", "postal_code": "4308639", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('4308511','{"jis": "22138", "kana": "ホテル クラウンパレスハママツ", "name": "ホテル　クラウンパレス浜松", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "板屋町", "banchi": "110-17", "postal_code": "4308511", "old_code": "430  ", "post_office": "浜松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "イタヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4308650','{"jis": "22138", "kana": "ヤマハ カブシキガイシヤ", "name": "ヤマハ　株式会社", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "中沢町", "banchi": "10-1(浜松郵便局私書箱第1号)", "postal_code": "4308650", "old_code": "430  ", "post_office": "浜松", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "ナカザワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4300898','{"jis": "22138", "kana": "カブシキガイシヤ マルイチ", "name": "株式会社　マルイチ", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "瓜内町", "banchi": "540番地", "postal_code": "4300898", "old_code": "43008", "post_office": "浜松東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "ウリウチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4300897','{"jis": "22138", "kana": "ミナミギヨウセイセンタ-", "name": "南行政センター", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "江之島町", "banchi": "600番地の1", "postal_code": "4300897", "old_code": "43008", "post_office": "浜松東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "エノシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4310192','{"jis": "22138", "kana": "カブシキガイシヤ アツミテツク", "name": "株式会社　アツミテック", "prefecture": "静岡県", "city": "浜松市中央区", "neighborhood": "雄踏町宇布見", "banchi": "7111", "postal_code": "4310192", "old_code": "43101", "post_office": "浜松西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ハママツシチュウオウク", "neighborhood_kana": "ユウトウチョウウブミ", "alternates": []}');
@@ -133922,18 +133930,18 @@
 INSERT INTO office_data VALUES('4108504','{"jis": "22203", "kana": "カブシキガイシヤ フジクラ ヌマヅコウジヨウ", "name": "株式会社　フジクラ　沼津工場", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "双葉町", "banchi": "9-1", "postal_code": "4108504", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "フタバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108551','{"jis": "22203", "kana": "カブシキガイシヤ マルヤスイサン", "name": "株式会社　マルヤ水産", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "千本港町", "banchi": "2", "postal_code": "4108551", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "センボンミナトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108588','{"jis": "22203", "kana": "カブシキガイシヤ メイデンシヤ ヌマヅジギヨウシヨ", "name": "株式会社　明電舎　沼津事業所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "東間門", "banchi": "字上中溝515", "postal_code": "4108588", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ヒガシマカド", "alternates": []}');
 INSERT INTO office_data VALUES('4108567','{"jis": "22203", "kana": "コクドコウツウシヨウ チユウブチホウセイビキヨク ヌマヅカセンコクドウジムシヨ", "name": "国土交通省　中部地方整備局　沼津河川国道事務所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "下香貫", "banchi": "外原3244-2", "postal_code": "4108567", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "シモカヌキ", "alternates": []}');
 INSERT INTO office_data VALUES('4108575','{"jis": "22203", "kana": "ザイダンホウジン フツコウカイ ヌマヅチユウオウビヨウイン", "name": "財団法人　復康会　沼津中央病院", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "中瀬町", "banchi": "24番1号", "postal_code": "4108575", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ナカセチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108555','{"jis": "22203", "kana": "ザイダンホウジン フヨウキヨウカイ セイレイヌマヅビヨウイン", "name": "財団法人　芙蓉協会　聖隷沼津病院", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "本", "banchi": "字松下七反田902-6", "postal_code": "4108555", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4108550','{"jis": "22203", "kana": "シズオカチホウサイバンシヨ ヌマヅシブ シズオカカテイサイバンシヨ ヌマヅシブ ヌマヅカンイサイバンシヨ ヌマヅケンサツシンサカイ", "name": "静岡地方裁判所　沼津支部　静岡家庭裁判所　沼津支部　沼津簡易裁判所　沼津検察審査会", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "御幸町", "banchi": "21-1", "postal_code": "4108550", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ミユキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4108510','{"jis": "22203", "kana": "シバウラキカイ カブシキガイシヤ ヌマヅコウジヨウ", "name": "芝浦機械　株式会社　沼津工場", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "大岡", "banchi": "2068-3", "postal_code": "4108510", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "オオオカ", "alternates": []}');
+INSERT INTO office_data VALUES('4108510','{"jis": "22203", "kana": "シバウラキカイ カブシキガイシヤ ヌマヅコウジヨウ", "name": "芝浦機械　株式会社　沼津工場", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "大岡", "banchi": "2068-3", "postal_code": "4108510", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "オオオカ", "alternates": []}');
 INSERT INTO office_data VALUES('4108580','{"jis": "22203", "kana": "セイレイヌマヅケンコウシンダンセンタ-", "name": "聖隷沼津健康診断センター", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "本", "banchi": "字下一丁田895-1", "postal_code": "4108580", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4108522','{"jis": "22203", "kana": "トウブキヨウイクジムシヨ", "name": "東部教育事務所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "高島本町", "banchi": "1-3", "postal_code": "4108522", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "タカシマホンチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4108655','{"jis": "22203", "kana": "ニツポンネンキンキコウ ヌマヅネンキンジムシヨ", "name": "日本年金機構　沼津年金事務所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "日の出町", "banchi": "1-40(沼津郵便局私書箱第7号)", "postal_code": "4108655", "old_code": "410  ", "post_office": "沼津", "type": "box", "multiple": false, "new": true, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ヒノデチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4108655','{"jis": "22203", "kana": "ニツポンネンキンキコウ ヌマヅネンキンジムシヨ", "name": "日本年金機構　沼津年金事務所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "日の出町", "banchi": "1-40(沼津郵便局私書箱第7号)", "postal_code": "4108655", "old_code": "410  ", "post_office": "沼津", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ヒノデチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108602','{"jis": "22203", "kana": "ニホンセイメイホケン ソウゴガイシヤ ヌマヅシシヤ", "name": "日本生命保険　相互会社　沼津支社", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "大手町", "banchi": "2丁目10番17号(沼津郵便局私書箱第91号)", "postal_code": "4108602", "old_code": "410  ", "post_office": "沼津", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4108508','{"jis": "22203", "kana": "ヌマヅケイサツシヨ", "name": "沼津警察署", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "平町", "banchi": "19-11", "postal_code": "4108508", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ヒラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4108501','{"jis": "22203", "kana": "ヌマヅコウギヨウコウトウセンモンガツコウ", "name": "沼津工業高等専門学校", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "大岡", "banchi": "3600", "postal_code": "4108501", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "オオオカ", "alternates": []}');
 INSERT INTO office_data VALUES('4108520','{"jis": "22203", "kana": "ヌマヅザイムジムシヨ", "name": "沼津財務事務所", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "高島本町", "banchi": "1-3", "postal_code": "4108520", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "タカシマホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108533','{"jis": "22203", "kana": "ヌマヅシリツトシヨカン", "name": "沼津市立図書館", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "三枚橋町", "banchi": "9-1", "postal_code": "4108533", "old_code": "410  ", "post_office": "沼津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "サンマイバシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4108610','{"jis": "22203", "kana": "ヌマヅシンヨウキンコ ホンテン ホンブ", "name": "沼津信用金庫　本店　本部", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "大手町", "banchi": "5丁目6-16(沼津郵便局私書箱第51号)", "postal_code": "4108610", "old_code": "410  ", "post_office": "沼津", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4108686','{"jis": "22203", "kana": "ヌマヅゼイムシヨ", "name": "沼津税務署", "prefecture": "静岡県", "city": "沼津市", "neighborhood": "米山町", "banchi": "3-30(沼津郵便局私書箱第17号)", "postal_code": "4108686", "old_code": "410  ", "post_office": "沼津", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シズオカケン", "city_kana": "ヌマヅシ", "neighborhood_kana": "ヨネヤマチョウ", "alternates": []}');
@@ -134532,27 +134540,26 @@
 INSERT INTO office_data VALUES('4508503','{"jis": "23105", "kana": "ユウビンキヨク カタログハンバイセンタ-", "name": "郵便局　カタログ販売センター", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名駅", "banchi": "2丁目45-19桑山ビル8F", "postal_code": "4508503", "old_code": "450  ", "post_office": "名古屋中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイエキ", "alternates": []}');
 INSERT INTO office_data VALUES('4538558','{"jis": "23105", "kana": "アイチケンシンヨウホシヨウキヨウカイ", "name": "愛知県信用保証協会", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "椿町", "banchi": "7番9号", "postal_code": "4538558", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ツバキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538758','{"jis": "23105", "kana": "アイチダイガクセイカツキヨウドウクミアイ ナゴヤシヨセキコウバイテン", "name": "愛知大学生活協同組合　名古屋書籍購買店", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地6", "postal_code": "4538758", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538518','{"jis": "23105", "kana": "アイテツレンコウセイネンキンキキン", "name": "愛鉄連厚生年金基金", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "黄金通", "banchi": "1丁目18", "postal_code": "4538518", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "コガネドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538510','{"jis": "23105", "kana": "エスエスセイヤク カブシキガイシヤ ナゴヤシテン", "name": "エスエス製薬　株式会社　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "大秋町", "banchi": "2丁目32番地", "postal_code": "4538510", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "オオアキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538581','{"jis": "23105", "kana": "カブシキカイシヤ アイコ-", "name": "株式会社　アイコー", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": [{"jis": "23105", "kana": "カブシキカイシヤ エキサイト", "name": "株式会社　ＥＸＣＩＴＥ", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": []}, {"jis": "23105", "kana": "カブシキカイシヤ シンセイ", "name": "株式会社　シンセイ", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": []}, {"jis": "23105", "kana": "カブシキカイシヤ ニユ-ギン・アドバンス", "name": "株式会社　ニューギン・アドバンス", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": []}, {"jis": "23105", "kana": "カブシキカイシヤ ニユ-ギンハンバイ", "name": "株式会社　ニューギン販売", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": []}, {"jis": "23105", "kana": "カブシキガイシヤ ニユ-ギン", "name": "（株）　ニューギン", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "烏森町", "banchi": "3丁目56番地", "postal_code": "4538581", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "カスモリチョウ", "alternates": []}]}');
 INSERT INTO office_data VALUES('4538555','{"jis": "23105", "kana": "カブシキカイシヤ オクムラグミ ナゴヤシテン", "name": "株式会社　奥村組　名古屋支店", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "竹橋町", "banchi": "29番8号", "postal_code": "4538555", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タケバシチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4538702','{"jis": "23105", "kana": "カブシキガイシヤ サポ-テイングチユウキヨウ", "name": "株式会社　サポーティング中京", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地11", "postal_code": "4538702", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538512','{"jis": "23105", "kana": "カブシキガイシヤ ジユニア-", "name": "株式会社　ジュニアー", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "黄金通", "banchi": "5丁目28", "postal_code": "4538512", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "コガネドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538567','{"jis": "23105", "kana": "カブシキガイシヤ センコウデンキ", "name": "株式会社　扇港電機", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "名西通", "banchi": "1丁目1番地", "postal_code": "4538567", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "メイセイトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538577','{"jis": "23105", "kana": "カブシキガイシヤ ダイドウシヨウカイ", "name": "株式会社　大同商会", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "並木", "banchi": "2丁目67", "postal_code": "4538577", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ナミキ", "alternates": []}');
 INSERT INTO office_data VALUES('4538701','{"jis": "23105", "kana": "カブシキガイシヤ チユウキヨウテレビジギヨウ", "name": "株式会社　中京テレビ事業", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地11", "postal_code": "4538701", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538533','{"jis": "23105", "kana": "カブシキガイシヤ マンユウ", "name": "株式会社　萬勇", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "本陣通", "banchi": "4丁目13", "postal_code": "4538533", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ホンジントオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538765','{"jis": "23105", "kana": "カブシキガイシヤ ミスタ-ゴルフ", "name": "株式会社　ミスターゴルフ", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤", "banchi": "1丁目21-15", "postal_code": "4538765", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538608','{"jis": "23105", "kana": "カブシキガイシヤ ヤマナカ", "name": "株式会社　ヤマナカ", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "岩塚町", "banchi": "字西枝1番地の1", "postal_code": "4538608", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "イワツカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538585','{"jis": "23105", "kana": "カブシキガイシヤ ユ-ハイム トウカイシシヤ", "name": "株式会社　ユーハイム　東海支社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "大秋町", "banchi": "2丁目42", "postal_code": "4538585", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "オオアキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538539','{"jis": "23105", "kana": "カブシキガイシヤ レア-ルパスコベ-カリ-ズ", "name": "株式会社　レアールパスコベーカリーズ", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "並木", "banchi": "1丁目296番地", "postal_code": "4538539", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ナミキ", "alternates": []}');
 INSERT INTO office_data VALUES('4538611','{"jis": "23105", "kana": "カワダフエザ- カブシキカイシヤ", "name": "河田フェザー　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "並木", "banchi": "1丁目267番地", "postal_code": "4538611", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ナミキ", "alternates": []}');
 INSERT INTO office_data VALUES('4538540','{"jis": "23105", "kana": "ガツコウホウジン ドウホウガクエン", "name": "学校法人　同朋学園", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "稲葉地町", "banchi": "7丁目1", "postal_code": "4538540", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "イナバジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4538565','{"jis": "23105", "kana": "ガツコウホウジン リツシシヤナゴヤコウ", "name": "学校法人　立志舎名古屋校", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "椿町", "banchi": "14番8号", "postal_code": "4538565", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ツバキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4538565','{"jis": "23105", "kana": "ガツコウホウジン リツシシヤナゴヤコウ", "name": "学校法人　立志舎名古屋校", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "椿町", "banchi": "14番8号", "postal_code": "4538565", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ツバキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538521','{"jis": "23105", "kana": "ザイダンホウジン ナゴヤコウシユウイガクケンキユウシヨ", "name": "財団法人　名古屋公衆医学研究所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "長筬町", "banchi": "4丁目23", "postal_code": "4538521", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ナガオサチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538570','{"jis": "23105", "kana": "ダイワハウスコウギヨウ カブシキカイシヤ ナゴヤシシヤ", "name": "大和ハウス工業　株式会社　名古屋支社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60番地9", "postal_code": "4538570", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538704','{"jis": "23105", "kana": "チユウキヨウテレビホウソウ カブシキガイシヤ", "name": "中京テレビ放送　株式会社", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "平池町", "banchi": "4丁目60-11", "postal_code": "4538704", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "ヒライケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538601','{"jis": "23105", "kana": "チユウブデンリヨクパワ-グリツド カブシキガイシヤ ナカムラエイギヨウシヨ", "name": "中部電力パワーグリッド　株式会社　中村営業所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤通", "banchi": "7丁目32", "postal_code": "4538601", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウトオリ", "alternates": []}');
 INSERT INTO office_data VALUES('4538501','{"jis": "23105", "kana": "ナカムラクヤクシヨ", "name": "中村区役所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "松原町", "banchi": "1丁目23番地1", "postal_code": "4538501", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "マツバラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538505','{"jis": "23105", "kana": "ナカムラケンゼイジムシヨ", "name": "中村県税事務所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "太閤", "banchi": "1丁目20-10", "postal_code": "4538505", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "タイコウ", "alternates": []}');
 INSERT INTO office_data VALUES('4538626','{"jis": "23105", "kana": "ナゴヤシホンジンシゼイジムシヨ", "name": "名古屋市本陣市税事務所", "prefecture": "愛知県", "city": "名古屋市中村区", "neighborhood": "松原町", "banchi": "1丁目23番地の1", "postal_code": "4538626", "old_code": "453  ", "post_office": "中村", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ナゴヤシナカムラク", "neighborhood_kana": "マツバラチョウ", "alternates": []}');
@@ -135083,23 +135090,23 @@
 INSERT INTO office_data VALUES('4418545','{"jis": "23201", "kana": "ユ-アイデンシ カブシキガイシヤ", "name": "ユーアイ電子　株式会社", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "曙町", "banchi": "字松並101", "postal_code": "4418545", "old_code": "441  ", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "アケボノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4418520','{"jis": "23201", "kana": "ユタカジドウシヤソウギヨウ カブシキガイシヤ", "name": "ユタカ自動車総業　株式会社", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "中野町", "banchi": "字平北80", "postal_code": "4418520", "old_code": "441  ", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "ナカノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4413192','{"jis": "23201", "kana": "アサヒコウギヨウ カブシキガイシヤ", "name": "朝日工業　株式会社", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "原町", "banchi": "字蔵社88", "postal_code": "4413192", "old_code": "44131", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "ハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4413195','{"jis": "23201", "kana": "シンフオニアテクノロジ- カブシキガイシヤ トヨハシセイサクシヨ", "name": "シンフォニアテクノロジー　株式会社　豊橋製作所", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "三弥町", "banchi": "字元屋敷150", "postal_code": "4413195", "old_code": "44131", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "ミツヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4413194','{"jis": "23201", "kana": "ニツトウデンコウ カブシキガイシヤ トヨハシジギヨウシヨ", "name": "日東電工　株式会社　豊橋事業所", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "中原町", "banchi": "字平山18", "postal_code": "4413194", "old_code": "44131", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "ナカハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4413196','{"jis": "23201", "kana": "フクイギヨモウ カブシキガイシヤ", "name": "福井漁網　株式会社", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "中原町", "banchi": "字岩西5-1", "postal_code": "4413196", "old_code": "44131", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "ナカハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4413193','{"jis": "23201", "kana": "ホンダデンシ カブシキガイシヤ", "name": "本多電子　株式会社", "prefecture": "愛知県", "city": "豊橋市", "neighborhood": "大岩町", "banchi": "字小山塚20", "postal_code": "4413193", "old_code": "44131", "post_office": "豊橋南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨハシシ", "neighborhood_kana": "オオイワチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4448564','{"jis": "23202", "kana": "アイシン・エイ・ダブリユ (カブ) オカザキコウジヨウ", "name": "アイシン・エイ・ダブリュ　（株）　岡崎工場", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "岡町", "banchi": "字原山6-18", "postal_code": "4448564", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "オカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448520','{"jis": "23202", "kana": "アイチガクセンダイガク", "name": "愛知学泉大学", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "舳越町", "banchi": "字上川成28", "postal_code": "4448520", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ヘゴシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448612','{"jis": "23202", "kana": "アイチケンシンヨウホシヨウキヨウカイ ニシミカワシテン", "name": "愛知県信用保証協会　西三河支店", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "上明大寺町", "banchi": "二丁目13番地", "postal_code": "4448612", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "カミミョウダイジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448551','{"jis": "23202", "kana": "アイチケンニシミカワジムシヨ", "name": "愛知県西三河事務所", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "明大寺本町", "banchi": "1丁目4", "postal_code": "4448551", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ミョウダイジホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4448555','{"jis": "23202", "kana": "アイチケンリツオカザキコウギヨウコウトウガツコウ", "name": "愛知県立岡崎工業高等学校", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "羽根町", "banchi": "字陣場47", "postal_code": "4448555", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ハネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448545','{"jis": "23202", "kana": "オカザキシホケンジヨ", "name": "岡崎市保健所", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "若宮町", "banchi": "2丁目1-1", "postal_code": "4448545", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ワカミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448553','{"jis": "23202", "kana": "オカザキシミンビヨウイン", "name": "岡崎市民病院", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "高隆寺町", "banchi": "字五所合3番地1", "postal_code": "4448553", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "コウリュウジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448552','{"jis": "23202", "kana": "オカザキゼイムシヨ", "name": "岡崎税務署", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "羽根町", "banchi": "北乾地50番地1(岡崎合同庁舎1・2階)", "postal_code": "4448552", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ハネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448588','{"jis": "23202", "kana": "カブシキカイシヤ ミネザワ", "name": "株式会社　ＭＩＮＥＺＡＷＡ", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "井田南町", "banchi": "4番地5", "postal_code": "4448588", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "イダミナミマチ", "alternates": []}');
+INSERT INTO office_data VALUES('4448564','{"jis": "23202", "kana": "カブシキガイシヤ アイシン オカザキコウジヨウ", "name": "株式会社　アイシン　岡崎工場", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "岡町", "banchi": "字原山6-18", "postal_code": "4448564", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "オカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448530','{"jis": "23202", "kana": "カブシキガイシヤ カワモトセイサクシヨ オカザキコウジヨウ", "name": "株式会社　川本製作所　岡崎工場", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "橋目町", "banchi": "字御領田1", "postal_code": "4448530", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ハシメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448543','{"jis": "23202", "kana": "カブシキガイシヤ シントウ", "name": "株式会社　新東", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "錦町", "banchi": "4-17", "postal_code": "4448543", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ニシキマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4443593','{"jis": "23202", "kana": "カブシキガイシヤ ジエイテクト オカザキコウジヨウ", "name": "株式会社　ジェイテクト　岡崎工場", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "市場町", "banchi": "字桐山八番地", "postal_code": "4443593", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "イチバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448567','{"jis": "23202", "kana": "カブシキガイシヤ レツドバロン", "name": "株式会社　レッドバロン", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "大平町", "banchi": "字才勝8-1", "postal_code": "4448567", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "オオヒラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448581','{"jis": "23202", "kana": "シガタメ カブシキガイシヤ", "name": "志賀為　株式会社", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "羽根町", "banchi": "字東荒子35", "postal_code": "4448581", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "ハネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4448517','{"jis": "23202", "kana": "スミトモセイメイホケン ソウゴガイシヤ アイチヒガシシシヤ", "name": "住友生命保険　相互会社　愛知東支社", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "康生通南", "banchi": "3丁目5", "postal_code": "4448517", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "コウセイドオリミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('4448710','{"jis": "23202", "kana": "セイブヒヤツカテン オカザキテン", "name": "西武百貨店　岡崎店", "prefecture": "愛知県", "city": "岡崎市", "neighborhood": "戸崎町", "banchi": "字外山38-5", "postal_code": "4448710", "old_code": "444  ", "post_office": "岡崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オカザキシ", "neighborhood_kana": "トサキチョウ", "alternates": []}');
@@ -135334,21 +135341,21 @@
 INSERT INTO office_data VALUES('4478608','{"jis": "23209", "kana": "ニホンコ-ンスタ-チ カブシキガイシヤ キヌウラジギヨウシヨ", "name": "日本コーンスターチ　株式会社　衣浦事業所", "prefecture": "愛知県", "city": "碧南市", "neighborhood": "玉津浦町", "banchi": "1番地(碧南郵便局私書箱第27号)", "postal_code": "4478608", "old_code": "447  ", "post_office": "碧南", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヘキナンシ", "neighborhood_kana": "タマツウラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4478502','{"jis": "23209", "kana": "ヘキナンシミンビヨウイン", "name": "碧南市民病院", "prefecture": "愛知県", "city": "碧南市", "neighborhood": "平和町", "banchi": "3丁目6", "postal_code": "4478502", "old_code": "447  ", "post_office": "碧南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヘキナンシ", "neighborhood_kana": "ヘイワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4478601','{"jis": "23209", "kana": "ヘキナンシヤクシヨ", "name": "碧南市役所", "prefecture": "愛知県", "city": "碧南市", "neighborhood": "松本町", "banchi": "28(碧南郵便局私書箱第3号)", "postal_code": "4478601", "old_code": "447  ", "post_office": "碧南", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヘキナンシ", "neighborhood_kana": "マツモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4478501','{"jis": "23209", "kana": "ヘキナンシヨウコウカイギシヨ", "name": "碧南商工会議所", "prefecture": "愛知県", "city": "碧南市", "neighborhood": "音羽町", "banchi": "1丁目1", "postal_code": "4478501", "old_code": "447  ", "post_office": "碧南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヘキナンシ", "neighborhood_kana": "オトハマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4478512','{"jis": "23209", "kana": "マルエイトウギヨウ カブシキガイシヤ", "name": "丸栄陶業　株式会社", "prefecture": "愛知県", "city": "碧南市", "neighborhood": "白沢町", "banchi": "1丁目38", "postal_code": "4478512", "old_code": "447  ", "post_office": "碧南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ヘキナンシ", "neighborhood_kana": "シロサワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488605','{"jis": "23210", "kana": "アイシン・エンジニアリング カブシキガイシヤ", "name": "アイシン・エンジニアリング　株式会社", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "相生町", "banchi": "1丁目1番地1JRF刈谷駅前ビル7階・8階", "postal_code": "4488605", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "アイオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488525','{"jis": "23210", "kana": "アイシンカイハツ カブシキガイシヤ フジビル", "name": "アイシン開発　株式会社　富士ビル", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "相生町", "banchi": "3丁目3番地", "postal_code": "4488525", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "アイオイチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4488650','{"jis": "23210", "kana": "アイシンセイキ カブシキガイシヤ", "name": "アイシン精機　株式会社", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "朝日町", "banchi": "2丁目1(刈谷郵便局私書箱第13号)", "postal_code": "4488650", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488543','{"jis": "23210", "kana": "アイチキヨウイクダイガク セイカツキヨウドウクミアイ", "name": "愛知教育大学　生活協同組合", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "井ケ谷町", "banchi": "広沢1", "postal_code": "4488543", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "イガヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488653','{"jis": "23210", "kana": "アイチケンリツ カリヤヒガシコウトウガツコウ", "name": "愛知県立　刈谷東高等学校", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "半城土町", "banchi": "三ツ又20(刈谷郵便局私書箱第35号)", "postal_code": "4488653", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ハジョウドチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488601','{"jis": "23210", "kana": "アイリスオ-ヤマ カブシキガイシヤ ナゴヤエイギヨウシヨ", "name": "アイリスオーヤマ　株式会社　名古屋営業所", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "一ツ木町", "banchi": "東新割57-7", "postal_code": "4488601", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ヒトツギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488655','{"jis": "23210", "kana": "オオタシヨウジ カブシキガイシヤ", "name": "太田商事　株式会社", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "南桜町", "banchi": "1丁目73(刈谷郵便局私書箱第1号)", "postal_code": "4488655", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ミナミサクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488652','{"jis": "23210", "kana": "カブシキカイシヤ ジエイテクト", "name": "株式会社　ジェイテクト", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "朝日町", "banchi": "1丁目1番地", "postal_code": "4488652", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488731','{"jis": "23210", "kana": "カブシキカイシヤ トウヨウ", "name": "株式会社　東陽", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "中山町", "banchi": "3丁目38番地", "postal_code": "4488731", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ナカヤマチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4488650','{"jis": "23210", "kana": "カブシキガイシヤ アイシン", "name": "株式会社　アイシン", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "朝日町", "banchi": "2丁目1(刈谷郵便局私書箱第13号)", "postal_code": "4488650", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488688','{"jis": "23210", "kana": "カブシキガイシヤ アドヴイツクス", "name": "株式会社　アドヴィックス", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "昭和町", "banchi": "2丁目1番地", "postal_code": "4488688", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ショウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488622','{"jis": "23210", "kana": "カブシキガイシヤ コンドウグミ", "name": "株式会社　近藤組", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "一里山町", "banchi": "伐払123", "postal_code": "4488622", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "イチリヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488661','{"jis": "23210", "kana": "カブシキガイシヤ デンソ-ホンシヤ", "name": "株式会社　デンソー本社", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "昭和町", "banchi": "1丁目1(刈谷郵便局私書箱第11号)", "postal_code": "4488661", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ショウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488531','{"jis": "23210", "kana": "カブシキガイシヤ トウヨウ", "name": "株式会社　東陽", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "中山町", "banchi": "5丁目10番地", "postal_code": "4488531", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "ナカヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488671','{"jis": "23210", "kana": "カブシキガイシヤ トヨタジドウシヨツキ", "name": "株式会社　豊田自動織機", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "豊田町", "banchi": "2丁目1番地(刈谷郵便局私書箱第6号)", "postal_code": "4488671", "old_code": "448  ", "post_office": "刈谷", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "トヨダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4488686','{"jis": "23210", "kana": "カブシキガイシヤ トヨタジドウシヨツキ ジヨウホウギジユツケンキユウジヨ", "name": "株式会社　豊田自動織機　情報技術研究所", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "城町", "banchi": "1丁目25-4", "postal_code": "4488686", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "シロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4488602','{"jis": "23210", "kana": "カブシキガイシヤ ブツクセンタ-メイホウ", "name": "株式会社　ブックセンター名豊", "prefecture": "愛知県", "city": "刈谷市", "neighborhood": "稲場町", "banchi": "3丁目303", "postal_code": "4488602", "old_code": "448  ", "post_office": "刈谷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "カリヤシ", "neighborhood_kana": "イナバチョウ", "alternates": []}');
@@ -135427,34 +135434,34 @@
 INSERT INTO office_data VALUES('4718535','{"jis": "23211", "kana": "トリニテイコウギヨウ カブシキガイシヤ", "name": "トリニティ工業　株式会社", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "柿本町", "banchi": "1丁目9", "postal_code": "4718535", "old_code": "471  ", "post_office": "豊田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "カキモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4718585','{"jis": "23211", "kana": "ナゴヤホウムキヨク トヨタシキヨク", "name": "名古屋法務局　豊田支局", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "常盤町", "banchi": "1丁目105番地3", "postal_code": "4718585", "old_code": "471  ", "post_office": "豊田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4718565','{"jis": "23211", "kana": "ニホンセキジユウジトヨタカンゴダイガク", "name": "日本赤十字豊田看護大学", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "白山町", "banchi": "七曲12-33", "postal_code": "4718565", "old_code": "471  ", "post_office": "豊田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "ハクサンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4718536','{"jis": "23211", "kana": "ミツイカイジヨウカサイホケン カブシキガイシヤ", "name": "三井海上火災保険　株式会社", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "山之手", "banchi": "4丁目46", "postal_code": "4718536", "old_code": "471  ", "post_office": "豊田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "ヤマノテ", "alternates": []}');
 INSERT INTO office_data VALUES('4718571','{"jis": "23211", "kana": "トヨタジドウシヤ カブシキガイシヤ", "name": "トヨタ自動車　株式会社", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "トヨタ町", "banchi": "1", "postal_code": "4718571", "old_code": "47171", "post_office": "豊田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "トヨタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4738501','{"jis": "23211", "kana": "アイシンタカオカ カブシキガイシヤ", "name": "アイシン高丘　株式会社", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "高丘新町", "banchi": "天王1", "postal_code": "4738501", "old_code": "473  ", "post_office": "豊田高岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "タカオカシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4738511','{"jis": "23211", "kana": "フジセイコウ カブシキガイシヤ", "name": "富士精工　株式会社", "prefecture": "愛知県", "city": "豊田市", "neighborhood": "吉原町", "banchi": "平子26", "postal_code": "4738511", "old_code": "473  ", "post_office": "豊田高岡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "トヨタシ", "neighborhood_kana": "ヨシワラチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4441192','{"jis": "23212", "kana": "アイシン・エイ・ダブリユ カブシキガイシヤ", "name": "アイシン・エイ・ダブリュ　株式会社", "prefecture": "愛知県", "city": "安城市", "neighborhood": "藤井町", "banchi": "高根10", "postal_code": "4441192", "old_code": "44411", "post_office": "桜井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フジイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4441192','{"jis": "23212", "kana": "カブシキガイシヤ アイシン アンジヨウチク", "name": "株式会社　アイシン　安城地区", "prefecture": "愛知県", "city": "安城市", "neighborhood": "藤井町", "banchi": "高根10", "postal_code": "4441192", "old_code": "44411", "post_office": "桜井", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フジイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441195','{"jis": "23212", "kana": "カブシキガイシヤ イノアツクコ-ポレ-シヨン サクライジギヨウシヨ", "name": "株式会社　イノアックコーポレーション　桜井事業所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "藤井町", "banchi": "東長先8番1", "postal_code": "4441195", "old_code": "44411", "post_office": "桜井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フジイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441198','{"jis": "23212", "kana": "カブシキガイシヤ ナンザンエン", "name": "株式会社　南山園", "prefecture": "愛知県", "city": "安城市", "neighborhood": "藤井町", "banchi": "南山20番地", "postal_code": "4441198", "old_code": "44411", "post_office": "桜井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フジイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441193','{"jis": "23212", "kana": "トウヨウリコウ カブシキガイシヤ", "name": "東洋理工　株式会社", "prefecture": "愛知県", "city": "安城市", "neighborhood": "藤井町", "banchi": "南山178番地", "postal_code": "4441193", "old_code": "44411", "post_office": "桜井", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フジイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441298','{"jis": "23212", "kana": "イズミセイカ カブシキガイシヤ", "name": "いずみ製菓　株式会社", "prefecture": "愛知県", "city": "安城市", "neighborhood": "和泉町", "banchi": "井ノ上3-1", "postal_code": "4441298", "old_code": "44412", "post_office": "明治", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "イズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441296','{"jis": "23212", "kana": "カブシキガイシヤ タケヒロ", "name": "株式会社　タケヒロ", "prefecture": "愛知県", "city": "安城市", "neighborhood": "和泉町", "banchi": "北大木4-14", "postal_code": "4441296", "old_code": "44412", "post_office": "明治", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "イズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4441295','{"jis": "23212", "kana": "カブシキガイシヤ トヨダジドウシヨツキ アンジヨウコウジヨウ", "name": "株式会社　豊田自動織機　安城工場", "prefecture": "愛知県", "city": "安城市", "neighborhood": "根崎町西石谷", "banchi": "8番地", "postal_code": "4441295", "old_code": "44412", "post_office": "明治", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4441297','{"jis": "23212", "kana": "カブシキガイシヤ ニツセイ", "name": "株式会社　ニッセイ", "prefecture": "愛知県", "city": "安城市", "neighborhood": "和泉町", "banchi": "井ノ上1番地1", "postal_code": "4441297", "old_code": "44412", "post_office": "明治", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "イズミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4468524','{"jis": "23212", "kana": "アイシンセイキ カブシキガイシヤ アンジヨウコウジヨウ", "name": "アイシン精機　株式会社　安城工場", "prefecture": "愛知県", "city": "安城市", "neighborhood": "三河安城町", "banchi": "1丁目11番地2", "postal_code": "4468524", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ミカワアンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468602','{"jis": "23212", "kana": "アイチケン コウセイノウギヨウキヨウドウクミアイレンゴウカイ アンジヨウコウセイビヨウイン", "name": "愛知県　厚生農業協同組合連合会　安城更生病院", "prefecture": "愛知県", "city": "安城市", "neighborhood": "安城町", "banchi": "東広畔28", "postal_code": "4468602", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "アンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468506','{"jis": "23212", "kana": "アイチケンケイザイノウギヨウキヨウドウクミアイレンゴウカイ ニシミカワセンタ-", "name": "愛知県経済農業協同組合連合会　西三河センター", "prefecture": "愛知県", "city": "安城市", "neighborhood": "今本町", "banchi": "東向山6番地の1", "postal_code": "4468506", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "イマホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468508','{"jis": "23212", "kana": "アイチケンニシミカワケンゼイジムシヨ アンジヨウケンゼイセンタ-", "name": "愛知県西三河県税事務所　安城県税センター", "prefecture": "愛知県", "city": "安城市", "neighborhood": "桜町", "banchi": "7番10号", "postal_code": "4468508", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "サクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468601','{"jis": "23212", "kana": "アイチチユウオウノウギヨウ キヨウドウクミアイ", "name": "あいち中央農業　協同組合", "prefecture": "愛知県", "city": "安城市", "neighborhood": "御幸本町", "banchi": "9-6(安城郵便局私書箱第1号)", "postal_code": "4468601", "old_code": "446  ", "post_office": "安城", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ミユキホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468526','{"jis": "23212", "kana": "アンジヨウカンイサイバンシヨ", "name": "安城簡易裁判所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "横山町", "banchi": "毛賀知24-2", "postal_code": "4468526", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ヨコヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468635','{"jis": "23212", "kana": "アンジヨウガクエンコウトウガツコウ", "name": "安城学園高等学校", "prefecture": "愛知県", "city": "安城市", "neighborhood": "小堤町", "banchi": "4丁目25(安城郵便局私書箱第35号)", "postal_code": "4468635", "old_code": "446  ", "post_office": "安城", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "コヅツミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468501','{"jis": "23212", "kana": "アンジヨウシヤクシヨ", "name": "安城市役所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "桜町", "banchi": "18-23", "postal_code": "4468501", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "サクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468512','{"jis": "23212", "kana": "アンジヨウシヨウコウカイギシヨ", "name": "安城商工会議所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "桜町", "banchi": "16-1", "postal_code": "4468512", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "サクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468503','{"jis": "23212", "kana": "アンデン カブシキガイシヤ", "name": "アンデン　株式会社", "prefecture": "愛知県", "city": "安城市", "neighborhood": "篠目町", "banchi": "井山3", "postal_code": "4468503", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ササメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468550','{"jis": "23212", "kana": "イツパンザイダンホウジン スギウラチイキイリヨウシンコウザイダン", "name": "一般財団法人　杉浦地域医療振興財団", "prefecture": "愛知県", "city": "安城市", "neighborhood": "三河安城町", "banchi": "1丁目8番地4", "postal_code": "4468550", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ミカワアンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468588','{"jis": "23212", "kana": "オオミコウギヨウ カブシキガイシヤ", "name": "大見工業　株式会社", "prefecture": "愛知県", "city": "安城市", "neighborhood": "新明町", "banchi": "27-7", "postal_code": "4468588", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "シンメイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4468524','{"jis": "23212", "kana": "カブシキガイシヤ アイシン アンジヨウコウジヨウ", "name": "株式会社　アイシン　安城工場", "prefecture": "愛知県", "city": "安城市", "neighborhood": "三河安城町", "banchi": "1丁目11番地2", "postal_code": "4468524", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ミカワアンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468504','{"jis": "23212", "kana": "カブシキガイシヤ イノアツクコ-ポレ-シヨン アンジヨウジギヨウシヨ", "name": "株式会社　イノアックコーポレーション　安城事業所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "今池町", "banchi": "3丁目1-36", "postal_code": "4468504", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "イマイケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468535','{"jis": "23212", "kana": "カブシキガイシヤ エスケイコ-ポレ-シヨン", "name": "株式会社　ＳＫコーポレーション", "prefecture": "愛知県", "city": "安城市", "neighborhood": "三河安城東町", "banchi": "1丁目6-28", "postal_code": "4468535", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "ミカワアンジョウヒガシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4468518','{"jis": "23212", "kana": "カブシキガイシヤ クオリ", "name": "株式会社　クオリ", "prefecture": "愛知県", "city": "安城市", "neighborhood": "福釜町", "banchi": "河原18", "postal_code": "4468518", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "フカマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468511','{"jis": "23212", "kana": "カブシキガイシヤ デンソ- アンジヨウセイサクシヨ", "name": "株式会社　デンソー　安城製作所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "里町", "banchi": "長根2-1", "postal_code": "4468511", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "サトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468507','{"jis": "23212", "kana": "カブシキガイシヤ デンソ- タカタナセイサクシヨ", "name": "株式会社　デンソー　高棚製作所", "prefecture": "愛知県", "city": "安城市", "neighborhood": "高棚町", "banchi": "新道1", "postal_code": "4468507", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "タカタナチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468502','{"jis": "23212", "kana": "カブシキガイシヤ マキタ", "name": "株式会社　マキタ", "prefecture": "愛知県", "city": "安城市", "neighborhood": "住吉町", "banchi": "3丁目11-8", "postal_code": "4468502", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "スミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4468520','{"jis": "23212", "kana": "カブシキガイシヤ ムロコ-ポレ-シヨン", "name": "株式会社　ムロコーポレーション", "prefecture": "愛知県", "city": "安城市", "neighborhood": "桜町", "banchi": "12-28", "postal_code": "4468520", "old_code": "446  ", "post_office": "安城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "アンジョウシ", "neighborhood_kana": "サクラマチ", "alternates": []}');
@@ -135498,15 +135505,15 @@
 INSERT INTO office_data VALUES('4458511','{"jis": "23213", "kana": "ナゴヤホウムキヨク ニシオシキヨク", "name": "名古屋法務局　西尾支局", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "熊味町", "banchi": "南十五夜60", "postal_code": "4458511", "old_code": "445  ", "post_office": "西尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "クマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458510','{"jis": "23213", "kana": "ニシオシミンビヨウイン", "name": "西尾市民病院", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "熊味町", "banchi": "上泡原6", "postal_code": "4458510", "old_code": "445  ", "post_office": "西尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "クマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458501','{"jis": "23213", "kana": "ニシオシヤクシヨ", "name": "西尾市役所", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "寄住町", "banchi": "下田22", "postal_code": "4458501", "old_code": "445  ", "post_office": "西尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "ヨリズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458505','{"jis": "23213", "kana": "ニシオシヨウコウカイギシヨ", "name": "西尾商工会議所", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "錦城町", "banchi": "234", "postal_code": "4458505", "old_code": "445  ", "post_office": "西尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "キンジョウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458601','{"jis": "23213", "kana": "ニシオシンヨウキンコ", "name": "西尾信用金庫", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "寄住町", "banchi": "洲田51(西尾郵便局私書箱第4号)", "postal_code": "4458601", "old_code": "445  ", "post_office": "西尾", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "ヨリズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458602','{"jis": "23213", "kana": "ニシオゼイムシヨ", "name": "西尾税務署", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "熊味町", "banchi": "南十五夜41-1(西尾郵便局私書箱第17号)", "postal_code": "4458602", "old_code": "445  ", "post_office": "西尾", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "クマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4458503','{"jis": "23213", "kana": "ニシオニユ-タウンカイハツ カブシキガイシヤ", "name": "西尾ニュータウン開発　株式会社", "prefecture": "愛知県", "city": "西尾市", "neighborhood": "下町", "banchi": "御城下23-1", "postal_code": "4458503", "old_code": "445  ", "post_office": "西尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ニシオシ", "neighborhood_kana": "シモマチ", "alternates": []}');
-INSERT INTO office_data VALUES('4438555','{"jis": "23214", "kana": "アイシン・エイ・ダブリユ カブシキガイシヤ ガマゴオリコウジヨウ", "name": "アイシン・エイ・ダブリュ　株式会社　蒲郡工場", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "浜町", "banchi": "24番3", "postal_code": "4438555", "old_code": "443  ", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "ハマチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4438555','{"jis": "23214", "kana": "カブシキガイシヤ アイシン ガマゴオリコウジヨウ", "name": "株式会社　アイシン　蒲郡工場", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "浜町", "banchi": "24番3", "postal_code": "4438555", "old_code": "443  ", "post_office": "蒲郡", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "ハマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4438588','{"jis": "23214", "kana": "ガツコウホウジン カイヨウガクエン カイヨウチユウトウキヨウイクガツコウ", "name": "学校法人　海陽学園　海陽中等教育学校", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "海陽町", "banchi": "3丁目12番1", "postal_code": "4438588", "old_code": "443  ", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "カイヨウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4438601','{"jis": "23214", "kana": "ガマゴオリシヤクシヨ", "name": "蒲郡市役所", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "旭町", "banchi": "17-1(蒲郡郵便局私書箱第25号)", "postal_code": "4438601", "old_code": "443  ", "post_office": "蒲郡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4438505','{"jis": "23214", "kana": "ガマゴオリシヨウコウカイギシヨ", "name": "蒲郡商工会議所", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "港町", "banchi": "18番23号", "postal_code": "4438505", "old_code": "443  ", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "ミナトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4430194','{"jis": "23214", "kana": "カネキスイサン カブシキガイシヤ", "name": "カネキ水産　株式会社", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "形原町", "banchi": "港町155", "postal_code": "4430194", "old_code": "44301", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "カタハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4430193','{"jis": "23214", "kana": "カブシキガイシヤ ガマサシヨクヒン", "name": "株式会社　蒲サ食品", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "西浦町", "banchi": "川東31", "postal_code": "4430193", "old_code": "44301", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "ニシウラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4430192','{"jis": "23214", "kana": "タイコウ カブシキガイシヤ", "name": "泰興　株式会社", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "金平町", "banchi": "土橋6-2", "postal_code": "4430192", "old_code": "44301", "post_office": "蒲郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "カネヒラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4438611','{"jis": "23214", "kana": "タケモトユシ カブシキガイシヤ", "name": "竹本油脂　株式会社", "prefecture": "愛知県", "city": "蒲郡市", "neighborhood": "港町", "banchi": "2-5(蒲郡郵便局私書箱第15号)", "postal_code": "4438611", "old_code": "44391", "post_office": "蒲郡", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "ガマゴオリシ", "neighborhood_kana": "ミナトマチ", "alternates": []}');
@@ -135577,14 +135584,15 @@
 INSERT INTO office_data VALUES('4858551','{"jis": "23219", "kana": "シ-ケ-デイ カブシキガイシヤ", "name": "ＣＫＤ　株式会社", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "応時", "banchi": "2丁目250番地", "postal_code": "4858551", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "コマキシ", "neighborhood_kana": "オウジ", "alternates": []}');
 INSERT INTO office_data VALUES('4858550','{"jis": "23219", "kana": "スミトモリコウ カブシキガイシヤ", "name": "住友理工　株式会社", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "東", "banchi": "三丁目1番地", "postal_code": "4858550", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "コマキシ", "neighborhood_kana": "ヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('4858522','{"jis": "23219", "kana": "センコ- カブシキガイシヤ コマキエイギヨウシヨ", "name": "センコー　株式会社　小牧営業所", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字河内屋新田", "banchi": "高笹480-1", "postal_code": "4858522", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858516','{"jis": "23219", "kana": "ダイニツポントリヨウ カブシキガイシヤ コマキコウジヨウ", "name": "大日本塗料　株式会社　小牧工場", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字三ツ渕", "banchi": "西ノ門878", "postal_code": "4858516", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858750','{"jis": "23219", "kana": "チユウブデンリヨク カブシキガイシヤ コマキエイギヨウシヨ コマキデンリヨクセンタ-", "name": "中部電力　株式会社　小牧営業所　小牧電力センター", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字久保一色", "banchi": "佃1010-1", "postal_code": "4858750", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858563','{"jis": "23219", "kana": "ナゴヤゾウケイゲイジユツダイガク・タンキダイガク", "name": "名古屋造形芸術大学・短期大学", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字大草", "banchi": "字年上坂6004", "postal_code": "4858563", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858510','{"jis": "23219", "kana": "ニツポントクシユトウギヨウ カブシキガイシヤ コマキコウジヨウ", "name": "日本特殊陶業　株式会社　小牧工場", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字岩崎", "banchi": "2808", "postal_code": "4858510", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('4858566','{"jis": "23219", "kana": "ニホンガイシ カブシキガイシヤ コマキジギヨウシヨ", "name": "日本ガイシ　株式会社　小牧事業所", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字二重堀", "banchi": "字田神1155", "postal_code": "4858566", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858505','{"jis": "23219", "kana": "マルビシコウギヨウ カブシキガイシヤ", "name": "丸菱工業　株式会社", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字本庄", "banchi": "1251-3", "postal_code": "4858505", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858561','{"jis": "23219", "kana": "ミツビシジユウコウギヨウ カブシキガイシヤ ナゴヤユウドウスイシンシステムセイサクシヨ", "name": "三菱重工業　株式会社　名古屋誘導推進システム製作所", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字東田中", "banchi": "1200", "postal_code": "4858561", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4858511','{"jis": "23219", "kana": "ミツボシベルトハンバイ カブシキガイシヤ コマキエイギヨウシヨ", "name": "三ツ星ベルト販賣　株式会社　小牧営業所", "prefecture": "愛知県", "city": "小牧市", "neighborhood": "大字西之島", "banchi": "1168", "postal_code": "4858511", "old_code": "485  ", "post_office": "小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('4901392','{"jis": "23220", "kana": "イナザワシ ヘイワシシヨ", "name": "稲沢市　平和支所", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "平和町中三宅", "banchi": "二丁割60番地", "postal_code": "4901392", "old_code": "49013", "post_office": "一宮", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ヘイワチョウナカミヤケ", "alternates": []}');
 INSERT INTO office_data VALUES('4928528','{"jis": "23220", "kana": "アイシヨウケンセツ カブシキガイシヤ", "name": "愛松建設　株式会社", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "松下", "banchi": "2丁目3-7", "postal_code": "4928528", "old_code": "492  ", "post_office": "稲沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "マツシタ", "alternates": []}');
 INSERT INTO office_data VALUES('4928529','{"jis": "23220", "kana": "アイチケイセイコウトウガツコウ", "name": "愛知啓成高等学校", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "西町", "banchi": "1丁目1-41", "postal_code": "4928529", "old_code": "492  ", "post_office": "稲沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ニシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4928521','{"jis": "23220", "kana": "アイチブンキヨウジヨシタンキダイガク", "name": "愛知文教女子短期大学", "prefecture": "愛知県", "city": "稲沢市", "neighborhood": "西町", "banchi": "1丁目1-41", "postal_code": "4928521", "old_code": "492  ", "post_office": "稲沢", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "イナザワシ", "neighborhood_kana": "ニシマチ", "alternates": []}');
@@ -135641,15 +135649,15 @@
 INSERT INTO office_data VALUES('4748557','{"jis": "23223", "kana": "(カブ) トウカイリキセイサクシヨ ヨコネコウジヨウ", "name": "（株）　東海理機製作所　横根工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "横根町", "banchi": "惣作70", "postal_code": "4748557", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ヨコネマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4748686','{"jis": "23223", "kana": "(カブ) トヨタジドウシヨツキセイサクシヨ ナガクサコウジヨウ", "name": "（株）　豊田自動織機製作所　長草工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "長草町", "banchi": "山口9-2", "postal_code": "4748686", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ナガクサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4748666','{"jis": "23223", "kana": "(カブ) メイキセイサクシヨ", "name": "（株）　名機製作所", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "大根2", "postal_code": "4748666", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748505','{"jis": "23223", "kana": "アイキヨウサンギヨウ カブシキガイシヤ", "name": "愛協産業　株式会社", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共栄町", "banchi": "7丁目1-1", "postal_code": "4748505", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748588','{"jis": "23223", "kana": "アイサンコウギヨウ カブシキガイシヤ", "name": "愛三工業　株式会社", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共和町", "banchi": "1丁目1-1", "postal_code": "4748588", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748580','{"jis": "23223", "kana": "アイサンコンピユ-タサ-ビス カブシキガイシヤ", "name": "アイサンコンピュータサービス　株式会社", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共栄町", "banchi": "七丁目3-3", "postal_code": "4748580", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748701','{"jis": "23223", "kana": "アイチケンオオブシヤクシヨ", "name": "愛知県大府市役所", "prefecture": "愛知県", "city": "大府市", "neighborhood": "中央町", "banchi": "5丁目70(大府郵便局私書箱第2号)", "postal_code": "4748701", "old_code": "474  ", "post_office": "大府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('4748710','{"jis": "23223", "kana": "アイチシヨウニホケンイリヨウソウゴウセンタ-", "name": "あいち小児保健医療総合センター", "prefecture": "愛知県", "city": "大府市", "neighborhood": "森岡町", "banchi": "7丁目426番地", "postal_code": "4748710", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": true, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "モリオカチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('4748710','{"jis": "23223", "kana": "アイチシヨウニホケンイリヨウソウゴウセンタ-", "name": "あいち小児保健医療総合センター", "prefecture": "愛知県", "city": "大府市", "neighborhood": "森岡町", "banchi": "7丁目426番地", "postal_code": "4748710", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "モリオカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748510','{"jis": "23223", "kana": "イヅミコウギヨウ カブシキガイシヤ", "name": "イヅミ工業　株式会社", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "清水1-3", "postal_code": "4748510", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748503','{"jis": "23223", "kana": "オオブシヨウコウカイギシヨ", "name": "大府商工会議所", "prefecture": "愛知県", "city": "大府市", "neighborhood": "中央町", "banchi": "5丁目70番地", "postal_code": "4748503", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748585','{"jis": "23223", "kana": "カブシキガイシヤ アペツクス", "name": "株式会社　アペックス", "prefecture": "愛知県", "city": "大府市", "neighborhood": "大府町", "banchi": "柊山11", "postal_code": "4748585", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "オオブマチ", "alternates": []}');
 INSERT INTO office_data VALUES('4748581','{"jis": "23223", "kana": "カブシキガイシヤ アンセイ", "name": "株式会社　アンセイ", "prefecture": "愛知県", "city": "大府市", "neighborhood": "北崎町", "banchi": "大島30", "postal_code": "4748581", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キタサキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748558','{"jis": "23223", "kana": "カブシキガイシヤ トウカイリキセイサクジヨ ナガネコウジヨウ", "name": "株式会社　東海理機製作所　長根工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "長根町", "banchi": "2丁目290", "postal_code": "4748558", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "ナガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748611','{"jis": "23223", "kana": "カブシキガイシヤ トミシンジユウタクセツビ", "name": "株式会社　富新住宅設備", "prefecture": "愛知県", "city": "大府市", "neighborhood": "共栄町", "banchi": "9丁目1-4", "postal_code": "4748611", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "キョウエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('4748668','{"jis": "23223", "kana": "カブシキガイシヤ トヨタジドウシヨツキ オオブコウジヨウ", "name": "株式会社　豊田自動織機　大府工場", "prefecture": "愛知県", "city": "大府市", "neighborhood": "江端町", "banchi": "一丁目一番地", "postal_code": "4748668", "old_code": "474  ", "post_office": "大府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "アイチケン", "city_kana": "オオブシ", "neighborhood_kana": "エバタチョウ", "alternates": []}');
@@ -136097,15 +136105,15 @@
 INSERT INTO office_data VALUES('5180495','{"jis": "24208", "kana": "ボルグワ-ナ-・モ-ルステツク・ジヤパン カブシキガイシヤ", "name": "ボルグワーナー・モールステック・ジャパン　株式会社", "prefecture": "三重県", "city": "名張市", "neighborhood": "八幡", "banchi": "1300-50", "postal_code": "5180495", "old_code": "51804", "post_office": "名張", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "ナバリシ", "neighborhood_kana": "ヤバタ", "alternates": []}');
 INSERT INTO office_data VALUES('5193692','{"jis": "24209", "kana": "オワセシヤカイホケンジムシヨ", "name": "尾鷲社会保険事務所", "prefecture": "三重県", "city": "尾鷲市", "neighborhood": "林町", "banchi": "2-23", "postal_code": "5193692", "old_code": "51936", "post_office": "尾鷲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "オワセシ", "neighborhood_kana": "ハヤシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5193696','{"jis": "24209", "kana": "オワセシヤクシヨ", "name": "尾鷲市役所", "prefecture": "三重県", "city": "尾鷲市", "neighborhood": "中央町", "banchi": "10-43(尾鷲郵便局私書箱第10号)", "postal_code": "5193696", "old_code": "51936", "post_office": "尾鷲", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "オワセシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5193694','{"jis": "24209", "kana": "オワセゼイムシヨ", "name": "尾鷲税務署", "prefecture": "三重県", "city": "尾鷲市", "neighborhood": "末広町", "banchi": "1-30", "postal_code": "5193694", "old_code": "51936", "post_office": "尾鷲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "オワセシ", "neighborhood_kana": "スエヒロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5193693','{"jis": "24209", "kana": "オワセソウゴウビヨウイン", "name": "尾鷲総合病院", "prefecture": "三重県", "city": "尾鷲市", "neighborhood": "上野町", "banchi": "5-25", "postal_code": "5193693", "old_code": "51936", "post_office": "尾鷲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "オワセシ", "neighborhood_kana": "ウエノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5193695','{"jis": "24209", "kana": "ミエケン キホクケンミンキヨク", "name": "三重県　紀北県民局", "prefecture": "三重県", "city": "尾鷲市", "neighborhood": "坂場西町", "banchi": "1-1", "postal_code": "5193695", "old_code": "51936", "post_office": "尾鷲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "オワセシ", "neighborhood_kana": "サカバニシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5190197','{"jis": "24210", "kana": "カブシキガイシヤ エイチワン カメヤマセイサクシヨ", "name": "株式会社　エイチワン　亀山製作所", "prefecture": "三重県", "city": "亀山市", "neighborhood": "下庄町", "banchi": "1701", "postal_code": "5190197", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "シモノショウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5190194','{"jis": "24210", "kana": "カブシキガイシヤ スズカミライ ツナグセンタ-", "name": "株式会社　スズカ未来　ＴＳＵＮＡＧＵセンター", "prefecture": "三重県", "city": "亀山市", "neighborhood": "白木町", "banchi": "字押之尾60番37", "postal_code": "5190194", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "シラキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5190194','{"jis": "24210", "kana": "カブシキガイシヤ スズカミライ ツナグセンタ-", "name": "株式会社　スズカ未来　ＴＳＵＮＡＧＵセンター", "prefecture": "三重県", "city": "亀山市", "neighborhood": "白木町", "banchi": "字押之尾60番37", "postal_code": "5190194", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "シラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5190196','{"jis": "24210", "kana": "カメヤマ カブシキガイシヤ", "name": "カメヤマ　株式会社", "prefecture": "三重県", "city": "亀山市", "neighborhood": "栄町", "banchi": "1504-1", "postal_code": "5190196", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5190195','{"jis": "24210", "kana": "カメヤマシヤクシヨ", "name": "亀山市役所", "prefecture": "三重県", "city": "亀山市", "neighborhood": "本丸町", "banchi": "577", "postal_code": "5190195", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "ホンマルチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5190198','{"jis": "24210", "kana": "シヤ-プ カブシキガイシヤ カメヤマコウジヨウ", "name": "シャープ　株式会社　亀山工場", "prefecture": "三重県", "city": "亀山市", "neighborhood": "白木町", "banchi": "幸川464番", "postal_code": "5190198", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "シラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5190193','{"jis": "24210", "kana": "ニツトウデンコウ カブシキガイシヤ カメヤマジギヨウシヨ", "name": "日東電工　株式会社　亀山事業所", "prefecture": "三重県", "city": "亀山市", "neighborhood": "布気町", "banchi": "919", "postal_code": "5190193", "old_code": "51901", "post_office": "亀山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "フケチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5190292','{"jis": "24210", "kana": "フルカワデンキコウギヨウ カブシキガイシヤ ミエジムシヨ", "name": "古河電気工業　株式会社　三重事務所", "prefecture": "三重県", "city": "亀山市", "neighborhood": "能褒野町", "banchi": "20-16", "postal_code": "5190292", "old_code": "51902", "post_office": "川崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "ノボノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5191192','{"jis": "24210", "kana": "カメヤマシ セキシシヨ", "name": "亀山市関支所", "prefecture": "三重県", "city": "亀山市", "neighborhood": "関町木崎", "banchi": "919番地の1", "postal_code": "5191192", "old_code": "51911", "post_office": "関", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "カメヤマシ", "neighborhood_kana": "セキチョウコザキ", "alternates": []}');
 INSERT INTO office_data VALUES('5178501','{"jis": "24211", "kana": "コクリツトバシヨウセンコウトウセンモンガツコウ", "name": "国立鳥羽商船高等専門学校", "prefecture": "三重県", "city": "鳥羽市", "neighborhood": "池上町", "banchi": "1-1", "postal_code": "5178501", "old_code": "517  ", "post_office": "鳥羽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミエケン", "city_kana": "トバシ", "neighborhood_kana": "イケガミチョウ", "alternates": []}');
@@ -136274,16 +136282,15 @@
 INSERT INTO office_data VALUES('5288510','{"jis": "25209", "kana": "ホヤ カブシキカイシヤ ミナクチラボラトリ-", "name": "ＨＯＹＡ　株式会社　水口ラボラトリー", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町さつきが丘", "banchi": "37", "postal_code": "5288510", "old_code": "528  ", "post_office": "水口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウサツキガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('5288555','{"jis": "25209", "kana": "ミナクチゼイムシヨ", "name": "水口税務署", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町水口", "banchi": "5587-3", "postal_code": "5288555", "old_code": "528  ", "post_office": "水口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウミナクチ", "alternates": []}');
 INSERT INTO office_data VALUES('5291892','{"jis": "25209", "kana": "コウカシヤクシヨ シガラキシシヨ", "name": "甲賀市役所　信楽支所", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "信楽町長野", "banchi": "1203", "postal_code": "5291892", "old_code": "52918", "post_office": "信楽", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "シガラキチョウナガノ", "alternates": []}');
 INSERT INTO office_data VALUES('5202394','{"jis": "25210", "kana": "(カブ) チヨウフセイサクシヨ シガコウジヨウ", "name": "（株）　長府製作所　滋賀工場", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "野洲", "banchi": "1473-1", "postal_code": "5202394", "old_code": "52023", "post_office": "野洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヤス", "alternates": []}');
 INSERT INTO office_data VALUES('5202392','{"jis": "25210", "kana": "ソニ-モバイルデイスプレイ カブシキガイシヤ", "name": "ソニーモバイルディスプレイ　株式会社", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "市三宅", "banchi": "800", "postal_code": "5202392", "old_code": "52023", "post_office": "野洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "イチミヤケ", "alternates": []}');
 INSERT INTO office_data VALUES('5202393','{"jis": "25210", "kana": "ムラタセイサクシヨ ヤスジギヨウシヨ", "name": "（株）　村田製作所　野洲事業所", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "大篠原", "banchi": "2288", "postal_code": "5202393", "old_code": "52023", "post_office": "野洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "オオシノハラ", "alternates": []}');
 INSERT INTO office_data VALUES('5202395','{"jis": "25210", "kana": "ヤスシヤクシヨ ホンチヨウシヤ", "name": "野洲市役所　本庁舎", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "小篠原", "banchi": "2100-1", "postal_code": "5202395", "old_code": "52023", "post_office": "野洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "コシノハラ", "alternates": []}');
-INSERT INTO office_data VALUES('5202492','{"jis": "25210", "kana": "ヤスシ シミンサ-ビスセンタ-", "name": "野洲市　市民サービスセンター", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "西河原", "banchi": "2400番地", "postal_code": "5202492", "old_code": "52024", "post_office": "中主", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ニシガワラ", "alternates": []}');
-INSERT INTO office_data VALUES('5240292','{"jis": "25210", "kana": "カブシキガイシヤ アユヤ", "name": "株式会社　鮎家", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "吉川", "banchi": "4187番地", "postal_code": "5240292", "old_code": "52402", "post_office": "幸津川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヨシカワ", "alternates": []}');
+INSERT INTO office_data VALUES('5202492','{"jis": "25210", "kana": "ヤスシ シミンサ-ビスセンタ-", "name": "野洲市　市民サービスセンター", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "西河原", "banchi": "2400番地", "postal_code": "5202492", "old_code": "52024", "post_office": "野洲", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ニシガワラ", "alternates": []}');
 INSERT INTO office_data VALUES('5203182','{"jis": "25211", "kana": "カブシキガイシヤ エム・エス・コミユニケ-シヨンズ オオサカブツリユウブ ブツリユウセンタ-", "name": "株式会社　エム・エス・コミュニケーションズ　大阪物流部　物流センター", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部口", "banchi": "4丁目3-1", "postal_code": "5203182", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベグチ", "alternates": []}');
 INSERT INTO office_data VALUES('5203189','{"jis": "25211", "kana": "カブシキガイシヤ ゴ-シユ-", "name": "株式会社　ゴーシュー", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部緑台", "banchi": "2丁目1-1(甲西郵便局私書箱第1号)", "postal_code": "5203189", "old_code": "52031", "post_office": "甲西", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベミドリダイ", "alternates": []}');
 INSERT INTO office_data VALUES('5203188','{"jis": "25211", "kana": "コウガコウブンシ カブシキガイシヤ", "name": "甲賀高分子　株式会社", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部北", "banchi": "1丁目4-26", "postal_code": "5203188", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベキタ", "alternates": []}');
 INSERT INTO office_data VALUES('5203195','{"jis": "25211", "kana": "コナンシヤクシヨ ニシチヨウシヤ", "name": "湖南市役所　西庁舎", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部中央", "banchi": "1丁目1番1号", "postal_code": "5203195", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベチュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('5203185','{"jis": "25211", "kana": "シ-アイカセイ カブシキガイシヤ シガジギヨウシヨ", "name": "シーアイ化成　株式会社　滋賀事業所", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "丸山", "banchi": "3丁目3-1", "postal_code": "5203185", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "マルヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('5203194','{"jis": "25211", "kana": "シヤカイフクシホウジン オオキカイ", "name": "社会福祉法人　大木会", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部が丘", "banchi": "2丁目1番1号", "postal_code": "5203194", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('5203180','{"jis": "25211", "kana": "ニツポンセイコウ カブシキガイシヤ イシベコウジヨウ", "name": "日本精工　株式会社　石部工場", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部が丘", "banchi": "1丁目1-1", "postal_code": "5203180", "old_code": "52031", "post_office": "甲西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベガオカ", "alternates": []}');
@@ -136303,15 +136310,15 @@
 INSERT INTO office_data VALUES('5211295','{"jis": "25213", "kana": "ニツポンデンキガラス カブシキカイシヤ ノトガワジギヨウジヨウ", "name": "日本電気硝子　株式会社　能登川事業場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "今町", "banchi": "906番地", "postal_code": "5211295", "old_code": "52112", "post_office": "能登川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "イマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5211292','{"jis": "25213", "kana": "ヒガシオウミシノトガワシシヨ", "name": "東近江市能登川支所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "", "banchi": "躰光寺262番地", "postal_code": "5211292", "old_code": "52112", "post_office": "能登川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('5278567','{"jis": "25213", "kana": "イリヨウホウジン ケイアイカイ", "name": "医療法人　敬愛会", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "八日市東本町", "banchi": "8番16号", "postal_code": "5278567", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヨウカイチヒガシホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5278508','{"jis": "25213", "kana": "カブシキガイシヤ テイラド シガセイサクシヨ", "name": "株式会社　ティラド　滋賀製作所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "五智町", "banchi": "297番地", "postal_code": "5278508", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ゴチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278588','{"jis": "25213", "kana": "カブシキガイシヤ ノエビア シガジギヨウシヨ", "name": "株式会社　ノエビア　滋賀事業所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "岡田町", "banchi": "112-1", "postal_code": "5278588", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "オカダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278558','{"jis": "25213", "kana": "カブシキガイシヤ ムラタセイサクシヨ ヨウカイチジギヨウシヨ", "name": "株式会社　村田製作所　八日市事業所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "東沖野", "banchi": "4丁目4番1号", "postal_code": "5278558", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヒガシオキノ", "alternates": []}');
 INSERT INTO office_data VALUES('5278585','{"jis": "25213", "kana": "カンサイデンリヨク カブシキガイシヤ ヨウカイチエイギヨウシヨ", "name": "関西電力　株式会社　八日市営業所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "八日市緑町", "banchi": "24-15", "postal_code": "5278585", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヨウカイチミドリマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5278555','{"jis": "25213", "kana": "キヨウセラ カブシキガイシヤ シガヨウカイチコウジヨウ", "name": "京セラ　株式会社　滋賀八日市工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "蛇溝町", "banchi": "長谷野1166番地の6", "postal_code": "5278555", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヘビミゾチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5278555','{"jis": "25213", "kana": "キヨウセラ カブシキガイシヤ シガヒガシオウミコウジヨウ ダイイチブロツク", "name": "京セラ　株式会社　滋賀東近江工場　第１ブロック", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "蛇溝町", "banchi": "1166-6", "postal_code": "5278555", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヘビミゾチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278542','{"jis": "25213", "kana": "サンコウゴウセイ カブシキガイシヤ シガコウジヨウ", "name": "三光合成　株式会社　滋賀工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "蛇溝町", "banchi": "1554", "postal_code": "5278542", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヘビミゾチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278512','{"jis": "25213", "kana": "シガケンヒガシオウミチイキシンコウキヨク チイキケンコウフクシブ", "name": "滋賀県東近江地域振興局　地域健康福祉部", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "八日市緑町", "banchi": "8番22号", "postal_code": "5278512", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヨウカイチミドリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5278577','{"jis": "25213", "kana": "シキボウ カブシキガイシヤ ヨウカイチコウジヨウ", "name": "シキボウ　株式会社　八日市工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "柴原南町", "banchi": "1500-5", "postal_code": "5278577", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "シバハラミナミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278580','{"jis": "25213", "kana": "タキロン カブシキガイシヤ ヨウカイチコウジヨウ", "name": "タキロン　株式会社　八日市工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "東沖野", "banchi": "3丁目7番7号", "postal_code": "5278580", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ヒガシオキノ", "alternates": []}');
 INSERT INTO office_data VALUES('5278566','{"jis": "25213", "kana": "トツパンインサツ カブシキガイシヤ エレクトロニクスジギヨウホンブ", "name": "凸版印刷　株式会社　エレクトロニクス事業本部", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "妙法寺町", "banchi": "1101-20", "postal_code": "5278566", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ミョウホウジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278505','{"jis": "25213", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ シガビヨウイン", "name": "独立行政法人　国立病院機構　滋賀病院", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "五智町", "banchi": "255", "postal_code": "5278505", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ゴチチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278501','{"jis": "25213", "kana": "パナソニツク カブシキガイシヤ ランドリ-・クリ-ナ-ジギヨウブ ヨウカイチコウジヨウ", "name": "パナソニック　株式会社　ランドリー・クリーナー事業部　八日市工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "林田町", "banchi": "1500番地", "postal_code": "5278501", "old_code": "527  ", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ハヤシダチョウ", "alternates": []}');
@@ -136322,15 +136329,15 @@
 INSERT INTO office_data VALUES('5270195','{"jis": "25213", "kana": "ヒガシオウミシヤクシヨ コトウシシヨ", "name": "東近江市役所　湖東支所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "池庄町", "banchi": "505番地", "postal_code": "5270195", "old_code": "52701", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "イケショウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5278687','{"jis": "25213", "kana": "コトウシンヨウキンコ", "name": "湖東信用金庫", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "青葉町", "banchi": "1番1号(八日市郵便局私書箱第17号)", "postal_code": "5278687", "old_code": "52791", "post_office": "八日市", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "アオバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291492','{"jis": "25213", "kana": "ヒガシオウミシヤクシヨ ゴカシヨウシシヨ", "name": "東近江市役所　五個荘支所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "五個荘小幡町", "banchi": "318番地", "postal_code": "5291492", "old_code": "52914", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ゴカショウオバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291493','{"jis": "25213", "kana": "フジノシヨウジ カブシキガイシヤ", "name": "藤野商事　株式会社", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "五個荘簗瀬町", "banchi": "11-3", "postal_code": "5291493", "old_code": "52914", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ゴカショウヤナゼチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291495','{"jis": "25213", "kana": "フジノシヨクヒン カブシキガイシヤ", "name": "フジノ食品　株式会社", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "宮荘町", "banchi": "610", "postal_code": "5291495", "old_code": "52914", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "ミヤショウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291598','{"jis": "25213", "kana": "アサヒノカントリ-クラブ", "name": "朝日野カントリー倶楽部", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "鈴町", "banchi": "1120", "postal_code": "5291598", "old_code": "52915", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "スズチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291597','{"jis": "25213", "kana": "カブシキガイシヤ メイシンヨウカイチカントリ-クラブ", "name": "株式会社　名神八日市カントリー倶楽部", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "石塔町", "banchi": "983-150", "postal_code": "5291597", "old_code": "52915", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "イシドウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5291595','{"jis": "25213", "kana": "キヨウセラ カブシキガイシヤ シガガモウコウジヨウ", "name": "京セラ　株式会社　滋賀蒲生工場", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "川合町", "banchi": "10-1", "postal_code": "5291595", "old_code": "52915", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "カワイチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5291595','{"jis": "25213", "kana": "キヨウセラ カブシキガイシヤ シガヒガシオウミコウジヨウ ダイニブロツク", "name": "京セラ　株式会社　滋賀東近江工場　第２ブロック", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "川合町", "banchi": "10-1", "postal_code": "5291595", "old_code": "52915", "post_office": "八日市", "type": "office", "multiple": false, "new": true, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "カワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291592','{"jis": "25213", "kana": "ヒガシオウミシ ガモウシシヨ", "name": "東近江市　蒲生支所", "prefecture": "滋賀県", "city": "東近江市", "neighborhood": "市子川原町", "banchi": "676番地", "postal_code": "5291592", "old_code": "52915", "post_office": "八日市", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "ヒガシオウミシ", "neighborhood_kana": "イチコカワラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5218601','{"jis": "25214", "kana": "マイバラシヤクシヨ オウミチヨウシヤ", "name": "米原市役所　近江庁舎", "prefecture": "滋賀県", "city": "米原市", "neighborhood": "顔戸", "banchi": "488-3", "postal_code": "5218601", "old_code": "521  ", "post_office": "米原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "マイバラシ", "neighborhood_kana": "ゴウド", "alternates": []}');
 INSERT INTO office_data VALUES('5218501','{"jis": "25214", "kana": "マイバラシヤクシヨ マイバラチヨウシヤ", "name": "米原市役所　米原庁舎", "prefecture": "滋賀県", "city": "米原市", "neighborhood": "下多良", "banchi": "3-3", "postal_code": "5218501", "old_code": "521  ", "post_office": "米原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "マイバラシ", "neighborhood_kana": "シモタラ", "alternates": []}');
 INSERT INTO office_data VALUES('5218511','{"jis": "25214", "kana": "ヤンマ-ホ-ルデイングス カブシキガイシヤ", "name": "ヤンマーホールディングス　株式会社", "prefecture": "滋賀県", "city": "米原市", "neighborhood": "梅ケ原", "banchi": "2481番地", "postal_code": "5218511", "old_code": "521  ", "post_office": "米原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "マイバラシ", "neighborhood_kana": "ウメガハラ", "alternates": []}');
 INSERT INTO office_data VALUES('5210292','{"jis": "25214", "kana": "マイバラシヤクシヨ サントウチヨウシヤ", "name": "米原市役所　山東庁舎", "prefecture": "滋賀県", "city": "米原市", "neighborhood": "長岡", "banchi": "1206", "postal_code": "5210292", "old_code": "52102", "post_office": "山東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "マイバラシ", "neighborhood_kana": "ナガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('5210392','{"jis": "25214", "kana": "マイバラシヤクシヨ イブキチヨウシヤ", "name": "米原市役所　伊吹庁舎", "prefecture": "滋賀県", "city": "米原市", "neighborhood": "春照", "banchi": "490-1", "postal_code": "5210392", "old_code": "52103", "post_office": "山東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シガケン", "city_kana": "マイバラシ", "neighborhood_kana": "スイジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5291692','{"jis": "25383", "kana": "カブシキガイシヤ ダイフク シガジギヨウシヨ", "name": "株式会社　ダイフク　滋賀事業所", "prefecture": "滋賀県", "city": "蒲生郡日野町", "neighborhood": "大字中在寺", "banchi": "1225", "postal_code": "5291692", "old_code": "52916", "post_office": "近江日野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -136951,29 +136958,29 @@
 INSERT INTO office_data VALUES('5408550','{"jis": "27128", "kana": "キンキザイムキヨク", "name": "近畿財務局", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "4丁目1-76", "postal_code": "5408550", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408795','{"jis": "27128", "kana": "キンキソウゴウツウシンキヨク", "name": "近畿総合通信局", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "1丁目5番44号大阪合同庁舎第1号館", "postal_code": "5408795", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408622','{"jis": "27128", "kana": "ケイ・オプテイコムビル", "name": "ケイ・オプティコムビル", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "二丁目1番5号", "postal_code": "5408622", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5408586','{"jis": "27128", "kana": "コクドコウツウシヨウ キンキチホウセイビキヨク", "name": "国土交通省　近畿地方整備局", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "3丁目1番41号", "postal_code": "5408586", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408615','{"jis": "27128", "kana": "コクドコウツウシヨウ キンキチホウセイビキヨク ケンセイブ ケンセツサンギヨウダイイツカ", "name": "国土交通省　近畿地方整備局　建政部　建設産業第一課", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "3丁目1-41大手前合同庁舎9階", "postal_code": "5408615", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408555','{"jis": "27128", "kana": "ザイダンホウジン ニホンチユウシヨウキギヨウフクシジギヨウダン (ニホンフルハツプ)", "name": "財団法人　日本中小企業福祉事業財団　（日本フルハップ）", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "2丁目1-2", "postal_code": "5408555", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408512','{"jis": "27128", "kana": "スミトモセイメイホケン ソウゴガイシヤ", "name": "住友生命保険　相互会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "1丁目4-35", "postal_code": "5408512", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
+INSERT INTO office_data VALUES('5408519','{"jis": "27128", "kana": "テレビオオサカ カブシキガイシヤ", "name": "テレビ大阪　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "1丁目1番7号", "postal_code": "5408519", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408505','{"jis": "27128", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "2丁目2-53", "postal_code": "5408505", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5408511','{"jis": "27128", "kana": "ニシニホンデンシンデンワ カブシキガイシヤ", "name": "西日本電信電話　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "馬場町", "banchi": "3-15", "postal_code": "5408511", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "バンバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5408515','{"jis": "27128", "kana": "ニシマツケンセツ カブシキガイシヤ カンサイシテン", "name": "西松建設　株式会社　関西支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "釣鐘町", "banchi": "2丁目4-7", "postal_code": "5408515", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ツリガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5408581','{"jis": "27128", "kana": "ニホンチヨクハン カブシキガイシヤ", "name": "日本直販　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "谷町", "banchi": "2丁目9番3号ガレリア大手前ビル11F", "postal_code": "5408581", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "タニマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408551','{"jis": "27128", "kana": "ニホンデンキ カブシキガイシヤ カンサイシシヤ", "name": "日本電気　株式会社　関西支社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "1丁目4-24", "postal_code": "5408551", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5308793','{"jis": "27128", "kana": "ニホンユウビン カブシキガイシヤ キンキシシヤ ユウビンジギヨウホンブ (サンシユ)", "name": "日本郵便　株式会社　近畿支社　郵便事業本部　（三種）", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜東", "banchi": "3番9号", "postal_code": "5308793", "old_code": "540  ", "post_office": "大阪北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5408517','{"jis": "27128", "kana": "ネンキンキロクカクニンオオサカチホウダイサンシヤイインカイ", "name": "年金記録確認大阪地方第三者委員会", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "谷町", "banchi": "2丁目1-17大阪第2法務合同庁舎5階", "postal_code": "5408517", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "タニマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408604','{"jis": "27128", "kana": "ノムラシヨウケン カブシキガイシヤ", "name": "野村證券　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "平野町", "banchi": "3丁目5-12(大阪東郵便局私書箱第171号)", "postal_code": "5408604", "old_code": "540  ", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ヒラノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5406255','{"jis": "27128", "kana": "パナソニツク カブシキガイシヤ", "name": "パナソニック　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "2丁目1-61ツイン21OBPパナソニックタワー", "postal_code": "5406255", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5408553','{"jis": "27128", "kana": "パナソニツク カブシキガイシヤ コネクテイツドソリユ-シヨンズシヤ ワイテイヴイキヨウバシビル", "name": "パナソニック　株式会社　コネクティッドソリューションズ社　ｙｔｖ京橋ビル", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "2丁目2番33号", "postal_code": "5408553", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5408566','{"jis": "27128", "kana": "モリシタジンタン カブシキガイシヤ", "name": "森下仁丹　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "玉造", "banchi": "1丁目2-40", "postal_code": "5408566", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "タマツクリ", "alternates": []}');
 INSERT INTO office_data VALUES('5408552','{"jis": "27128", "kana": "ヨシオカ カブシキガイシヤ オオサカシテン", "name": "吉岡　株式会社　大阪支店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "南新町", "banchi": "2-2-16", "postal_code": "5408552", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ミナミシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5308610','{"jis": "27128", "kana": "ヨミウリテレビホウソウ カブシキガイシヤ", "name": "読売テレビ放送　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "城見", "banchi": "2丁目2-33(大阪北郵便局私書箱第646号)", "postal_code": "5308610", "old_code": "540  ", "post_office": "大阪北", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "シロミ", "alternates": []}');
 INSERT INTO office_data VALUES('5408534','{"jis": "27128", "kana": "ワイケイケイ エ-ピ- カブシキガイシヤ", "name": "ＹＫＫ　ＡＰ　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "谷町", "banchi": "4丁目8-7", "postal_code": "5408534", "old_code": "540  ", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "タニマチ", "alternates": []}');
-INSERT INTO office_data VALUES('5408519','{"jis": "27128", "kana": "テレビオオサカ カブシキガイシヤ", "name": "テレビ大阪　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "1丁目2-18", "postal_code": "5408519", "old_code": "54019", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408570','{"jis": "27128", "kana": "オオサカフチヨウ", "name": "大阪府庁", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "2丁目1-22", "postal_code": "5408570", "old_code": "54070", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408571','{"jis": "27128", "kana": "オオサカフチヨウ (オオサカフキヨウイクイインカイ)", "name": "大阪府庁　（大阪府教育委員会）", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "大手前", "banchi": "2丁目1-22", "postal_code": "5408571", "old_code": "54070", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "オオテマエ", "alternates": []}');
 INSERT INTO office_data VALUES('5408606','{"jis": "27128", "kana": "カブシキガイシヤ ジエ-シ-ビ- オオサカシシヤ", "name": "株式会社　ジェーシービー　大阪支社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜東", "banchi": "4-33大阪大林ビル", "postal_code": "5408606", "old_code": "54091", "post_office": "大阪東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('5408620','{"jis": "27128", "kana": "カブシキガイシヤ スミトモギンコウ ホンテン", "name": "株式会社　住友銀行　本店", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "北浜", "banchi": "4丁目6-5(大阪東郵便局私書箱第21号)", "postal_code": "5408620", "old_code": "54091", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5408660','{"jis": "27128", "kana": "カブシキガイシヤ ヤギ", "name": "株式会社　ヤギ", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "久太郎町", "banchi": "2丁目2-8(大阪東郵便局私書箱第39号)", "postal_code": "5408660", "old_code": "54091", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "キュウタロウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408642','{"jis": "27128", "kana": "サンキヨウセイコウ カブシキガイシヤ", "name": "三共生興　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "安土町", "banchi": "2丁目5-6(大阪東郵便局私書箱第42号)", "postal_code": "5408642", "old_code": "54091", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "アヅチマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5408611','{"jis": "27128", "kana": "シオノギセイヤク カブシキガイシヤ", "name": "塩野義製薬　株式会社", "prefecture": "大阪府", "city": "大阪市中央区", "neighborhood": "道修町", "banchi": "3丁目1-8(大阪東郵便局私書箱第333号)", "postal_code": "5408611", "old_code": "54091", "post_office": "大阪東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "オオサカシチュウオウク", "neighborhood_kana": "ドショウマチ", "alternates": []}');
@@ -137197,15 +137204,15 @@
 INSERT INTO office_data VALUES('5691098','{"jis": "27207", "kana": "カンサイダイガク タカツキミユ-ズキヤンパス", "name": "関西大学　高槻ミューズキャンパス", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "白梅町", "banchi": "7-1", "postal_code": "5691098", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "ハクバイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5691195','{"jis": "27207", "kana": "サンスタ- カブシキガイシヤ", "name": "サンスター　株式会社", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "朝日町", "banchi": "3-1", "postal_code": "5691195", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5691096','{"jis": "27207", "kana": "タカツキセキジユウジビヨウイン", "name": "高槻赤十字病院", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "阿武野", "banchi": "1丁目1-1", "postal_code": "5691096", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "アブノ", "alternates": []}');
 INSERT INTO office_data VALUES('5698660','{"jis": "27207", "kana": "トリシマセイサクシヨ", "name": "酉島製作所", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "宮田町", "banchi": "1丁目1-8(高槻郵便局私書箱第5号)", "postal_code": "5698660", "old_code": "56911", "post_office": "高槻", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "ミヤダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5691194','{"jis": "27207", "kana": "パ-ソルエ-ブイシ-テクノロジ- カブシキガイシヤ", "name": "パーソルＡＶＣテクノロジー　株式会社", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "幸町", "banchi": "1番1号", "postal_code": "5691194", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "サイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5691193','{"jis": "27207", "kana": "パナソニツクライテイングデバイス カブシキガイシヤ パナソニツクフオト・ライテイング カブシキガイシヤ", "name": "パナソニックライティングデバイス　株式会社　パナソニックフォト・ライティング　株式会社", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "幸町", "banchi": "1番1号", "postal_code": "5691193", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "サイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5691092','{"jis": "27207", "kana": "ヘイアンジヨガクインダイガク", "name": "平安女学院大学", "prefecture": "大阪府", "city": "高槻市", "neighborhood": "南平台", "banchi": "5丁目81-1", "postal_code": "5691092", "old_code": "56911", "post_office": "高槻北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "タカツキシ", "neighborhood_kana": "ナンペイダイ", "alternates": []}');
-INSERT INTO office_data VALUES('5978577','{"jis": "27208", "kana": "オオサカフカイヅカコドモカテイセンタ-", "name": "大阪府貝塚子ども家庭センター", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "畠中", "banchi": "1丁目17-2", "postal_code": "5978577", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ハタケナカ", "alternates": []}');
+INSERT INTO office_data VALUES('5978577','{"jis": "27208", "kana": "オオサカフカイヅカコドモカテイセンタ-", "name": "大阪府貝塚子ども家庭センター", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "畠中", "banchi": "1丁目17-2", "postal_code": "5978577", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ハタケナカ", "alternates": []}');
 INSERT INTO office_data VALUES('5978515','{"jis": "27208", "kana": "オクモトセイフン カブシキガイシヤ", "name": "奥本製粉　株式会社", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "港", "banchi": "15", "postal_code": "5978515", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ミナト", "alternates": []}');
 INSERT INTO office_data VALUES('5978585','{"jis": "27208", "kana": "カイヅカシヤクシヨ", "name": "貝塚市役所", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "畠中", "banchi": "1丁目17-1", "postal_code": "5978585", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ハタケナカ", "alternates": []}');
 INSERT INTO office_data VALUES('5978501','{"jis": "27208", "kana": "カブシキガイシヤ テザツクニシキノハマセイゾウシヨ", "name": "株式会社　デザック二色浜製造所", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "二色中町", "banchi": "11-1", "postal_code": "5978501", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ニシキナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5978555','{"jis": "27208", "kana": "スミトモジユウキカイギヤボツクス カブシキガイシヤ", "name": "住友重機械ギヤボックス　株式会社", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "脇浜", "banchi": "4丁目16番1号", "postal_code": "5978555", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ワキハマ", "alternates": []}');
 INSERT INTO office_data VALUES('5978511','{"jis": "27208", "kana": "テラダボウセキ カブシキガイシヤ", "name": "寺田紡績　株式会社", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "津田南町", "banchi": "28番55号", "postal_code": "5978511", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ツダミナミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5978686','{"jis": "27208", "kana": "ニツポンネンキンキコウ カイヅカネンキンジムシヨ", "name": "日本年金機構　貝塚年金事務所", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "海塚", "banchi": "305-1(貝塚郵便局私書箱第17号)", "postal_code": "5978686", "old_code": "597  ", "post_office": "貝塚", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ウミヅカ", "alternates": []}');
 INSERT INTO office_data VALUES('5978502','{"jis": "27208", "kana": "ネゴロサンギヨウ カブシキガイシヤ", "name": "根来産業　株式会社", "prefecture": "大阪府", "city": "貝塚市", "neighborhood": "二色中町", "banchi": "1-1", "postal_code": "5978502", "old_code": "597  ", "post_office": "貝塚", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "カイヅカシ", "neighborhood_kana": "ニシキナカマチ", "alternates": []}');
@@ -138746,15 +138753,15 @@
 INSERT INTO office_data VALUES('7088507','{"jis": "33203", "kana": "ナンバ カブシキガイシヤ", "name": "ナンバ　株式会社", "prefecture": "岡山県", "city": "津山市", "neighborhood": "材木町", "banchi": "1328-25", "postal_code": "7088507", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "ザイモクマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7088652','{"jis": "33203", "kana": "ニホンシヨクセイ カブシキガイシヤ", "name": "日本植生　株式会社", "prefecture": "岡山県", "city": "津山市", "neighborhood": "高尾", "banchi": "573-1", "postal_code": "7088652", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "タカオ", "alternates": []}');
 INSERT INTO office_data VALUES('7088517','{"jis": "33203", "kana": "パナソニツク インダストリ- カブシキガイシヤ", "name": "パナソニック　インダストリー　株式会社", "prefecture": "岡山県", "city": "津山市", "neighborhood": "河辺", "banchi": "字下閂1111-1", "postal_code": "7088517", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "カワナベ", "alternates": []}');
 INSERT INTO office_data VALUES('7088511','{"jis": "33203", "kana": "ミマサカダイガク", "name": "美作大学", "prefecture": "岡山県", "city": "津山市", "neighborhood": "北園町", "banchi": "50", "postal_code": "7088511", "old_code": "708  ", "post_office": "津山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "キタゾノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7081198','{"jis": "33203", "kana": "サンヨウロ-ドコウギヨウ カブシキガイシヤ", "name": "山陽ロード工業　株式会社", "prefecture": "岡山県", "city": "津山市", "neighborhood": "下高倉西", "banchi": "1203-1(成名郵便局私書箱第3号)", "postal_code": "7081198", "old_code": "70811", "post_office": "成名", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "シモタカクラニシ", "alternates": []}');
 INSERT INTO office_data VALUES('7081193','{"jis": "33203", "kana": "ト-ステ カブシキガイシヤ サニタリ-ジギヨウホンブ", "name": "トーステ　株式会社　サニタリー事業本部", "prefecture": "岡山県", "city": "津山市", "neighborhood": "草加部", "banchi": "1170番地9", "postal_code": "7081193", "old_code": "70811", "post_office": "成名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ツヤマシ", "neighborhood_kana": "クサカベ", "alternates": []}');
 INSERT INTO office_data VALUES('7068555','{"jis": "33204", "kana": "オカヤマケンリツタマノコウトウガツコウ", "name": "岡山県立玉野高等学校", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "築港", "banchi": "3丁目11-1", "postal_code": "7068555", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "チッコウ", "alternates": []}');
-INSERT INTO office_data VALUES('7068651','{"jis": "33204", "kana": "カブシキガイシヤ ミツイイ-アンドエスホ-ルデイングスタマノソウゴウジムシヨ", "name": "株式会社　三井Ｅ＆Ｓホールディングス玉野総合事務所", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "玉", "banchi": "3丁目1番1号(玉野郵便局私書箱第1号)", "postal_code": "7068651", "old_code": "706  ", "post_office": "玉野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "タマ", "alternates": []}');
+INSERT INTO office_data VALUES('7068651','{"jis": "33204", "kana": "カブシキガイシヤ ミツイイ-アンドエスタマノソウゴウジムシヨ", "name": "株式会社　三井Ｅ＆Ｓ玉野総合事務所", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "玉", "banchi": "3丁目1番1号(玉野郵便局私書箱第1号)", "postal_code": "7068651", "old_code": "706  ", "post_office": "玉野", "type": "box", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "タマ", "alternates": []}');
 INSERT INTO office_data VALUES('7068510','{"jis": "33204", "kana": "タマノシヤクシヨ", "name": "玉野市役所", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "宇野", "banchi": "1丁目27-1", "postal_code": "7068510", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "ウノ", "alternates": []}');
 INSERT INTO office_data VALUES('7068533','{"jis": "33204", "kana": "タマノシヨウコウカイギシヨ", "name": "玉野商工会議所", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "築港", "banchi": "1丁目1番3号", "postal_code": "7068533", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "チッコウ", "alternates": []}');
 INSERT INTO office_data VALUES('7068655','{"jis": "33204", "kana": "タマノゼイムシヨ", "name": "玉野税務署", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "宇野", "banchi": "2丁目4-12(玉野郵便局私書箱第27号)", "postal_code": "7068655", "old_code": "706  ", "post_office": "玉野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "ウノ", "alternates": []}');
 INSERT INTO office_data VALUES('7068531','{"jis": "33204", "kana": "チホウドクリツギヨウセイホウジン タマノイリヨウセンタ- タマノシミンビヨウイン", "name": "地方独立行政法人　玉野医療センター　玉野市民病院", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "宇野", "banchi": "2丁目3番1号", "postal_code": "7068531", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "ウノ", "alternates": []}');
 INSERT INTO office_data VALUES('7068511','{"jis": "33204", "kana": "ミツイキンゾクコウギヨウカブシキガイシヤ キンゾクジギヨウブ ヒビセイレンジヨ", "name": "三井金属鉱業株式会社　金属事業部　日比製煉所", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "日比", "banchi": "6丁目1-1", "postal_code": "7068511", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "ヒビ", "alternates": []}');
 INSERT INTO office_data VALUES('7068501','{"jis": "33204", "kana": "ミツイゾウセンセイカツ キヨウドウクミアイ", "name": "三井造船生活　協同組合", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "玉", "banchi": "2丁目5-5", "postal_code": "7068501", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "タマ", "alternates": []}');
 INSERT INTO office_data VALUES('7068588','{"jis": "33204", "kana": "ミツビシジユウコウマリタイムシステムズ カブシキガイシヤ", "name": "三菱重工マリタイムシステムズ　株式会社", "prefecture": "岡山県", "city": "玉野市", "neighborhood": "玉", "banchi": "3丁目1番1号", "postal_code": "7068588", "old_code": "706  ", "post_office": "玉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タマノシ", "neighborhood_kana": "タマ", "alternates": []}');
@@ -138774,15 +138781,15 @@
 INSERT INTO office_data VALUES('7191195','{"jis": "33208", "kana": "ユニチカ カブシキガイシヤ トキワコウジヨウ", "name": "ユニチカ　株式会社　常盤工場", "prefecture": "岡山県", "city": "総社市", "neighborhood": "中原", "banchi": "88", "postal_code": "7191195", "old_code": "71911", "post_office": "総社", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ソウジャシ", "neighborhood_kana": "ナカバラ", "alternates": []}');
 INSERT INTO office_data VALUES('7168511','{"jis": "33209", "kana": "イ-グルコウギヨウ カブシキガイシヤ オカヤマジギヨウジヨウ", "name": "イーグル工業　株式会社　岡山事業場", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "落合町阿部", "banchi": "1212", "postal_code": "7168511", "old_code": "716  ", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "オチアイチョウアベ", "alternates": []}');
 INSERT INTO office_data VALUES('7168585','{"jis": "33209", "kana": "オカヤマケン タカハシチホウシンコウキヨク", "name": "岡山県　高梁地方振興局", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "落合町近似", "banchi": "286-1", "postal_code": "7168585", "old_code": "716  ", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "オチアイチョウチカノリ", "alternates": []}');
 INSERT INTO office_data VALUES('7168508','{"jis": "33209", "kana": "ガツコウホウジン タカハシガクエン", "name": "学校法人　高梁学園", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "伊賀町", "banchi": "8", "postal_code": "7168508", "old_code": "716  ", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "イガマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7168501','{"jis": "33209", "kana": "タカハシシヤクシヨ", "name": "高梁市役所", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "松原通", "banchi": "2043", "postal_code": "7168501", "old_code": "716  ", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "マツバラドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7168601','{"jis": "33209", "kana": "タカハシシヨウコウカイギシヨ", "name": "高梁商工会議所", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "南町", "banchi": "16-2(高梁郵便局私書箱第6号)", "postal_code": "7168601", "old_code": "716  ", "post_office": "高梁", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "ミナミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7160192','{"jis": "33209", "kana": "スミトモデンコウシヨウケツゴウキン カブシキガイシヤ", "name": "住友電工焼結合金　株式会社", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "成羽町成羽", "banchi": "2901", "postal_code": "7160192", "old_code": "71601", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "ナリワチョウナリワ", "alternates": []}');
-INSERT INTO office_data VALUES('7160295','{"jis": "33209", "kana": "タカハシシカワカミチイキキヨク", "name": "高梁市川上地域局", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "川上町地頭", "banchi": "1819-1", "postal_code": "7160295", "old_code": "71602", "post_office": "吉備川上", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "カワカミチョウジトウ", "alternates": []}');
+INSERT INTO office_data VALUES('7160295','{"jis": "33209", "kana": "タカハシシカワカミチイキキヨク", "name": "高梁市川上地域局", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "川上町地頭", "banchi": "1822番地", "postal_code": "7160295", "old_code": "71602", "post_office": "吉備川上", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "カワカミチョウジトウ", "alternates": []}');
 INSERT INTO office_data VALUES('7160396','{"jis": "33209", "kana": "タカハシシビツチユウチイキキヨク", "name": "高梁市備中地域局", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "備中町布賀", "banchi": "29-2", "postal_code": "7160396", "old_code": "71603", "post_office": "備中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "ビッチュウチョウフカ", "alternates": []}');
 INSERT INTO office_data VALUES('7161392','{"jis": "33209", "kana": "タカハシシウカンチイキキヨク", "name": "高梁市有漢地域局", "prefecture": "岡山県", "city": "高梁市", "neighborhood": "有漢町有漢", "banchi": "3387", "postal_code": "7161392", "old_code": "71613", "post_office": "高梁", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "タカハシシ", "neighborhood_kana": "ウカンチョウウカン", "alternates": []}');
 INSERT INTO office_data VALUES('7188530','{"jis": "33210", "kana": "アシンノウギヨウキヨウドウクミアイ", "name": "阿新農業協同組合", "prefecture": "岡山県", "city": "新見市", "neighborhood": "高尾", "banchi": "2423", "postal_code": "7188530", "old_code": "718  ", "post_office": "新見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ニイミシ", "neighborhood_kana": "タカオ", "alternates": []}');
 INSERT INTO office_data VALUES('7188550','{"jis": "33210", "kana": "オカヤマケン ビツチユウケンミンキヨク ニイミシキヨク", "name": "岡山県　備中県民局　新見支局", "prefecture": "岡山県", "city": "新見市", "neighborhood": "高尾", "banchi": "2400", "postal_code": "7188550", "old_code": "718  ", "post_office": "新見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ニイミシ", "neighborhood_kana": "タカオ", "alternates": []}');
 INSERT INTO office_data VALUES('7188585','{"jis": "33210", "kana": "コウリツダイガクホウジン ニイミコウリツダイガク", "name": "公立大学法人　新見公立大学", "prefecture": "岡山県", "city": "新見市", "neighborhood": "西方", "banchi": "1263-2", "postal_code": "7188585", "old_code": "718  ", "post_office": "新見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ニイミシ", "neighborhood_kana": "ニシガタ", "alternates": []}');
 INSERT INTO office_data VALUES('7188501','{"jis": "33210", "kana": "ニイミシヤクシヨ", "name": "新見市役所", "prefecture": "岡山県", "city": "新見市", "neighborhood": "新見", "banchi": "310-3", "postal_code": "7188501", "old_code": "718  ", "post_office": "新見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ニイミシ", "neighborhood_kana": "ニイミ", "alternates": []}');
 INSERT INTO office_data VALUES('7188510','{"jis": "33210", "kana": "ニイミゼイムシヨ", "name": "新見税務署", "prefecture": "岡山県", "city": "新見市", "neighborhood": "新見", "banchi": "721-1", "postal_code": "7188510", "old_code": "718  ", "post_office": "新見", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "ニイミシ", "neighborhood_kana": "ニイミ", "alternates": []}');
@@ -139319,15 +139326,15 @@
 INSERT INTO office_data VALUES('7372295','{"jis": "34215", "kana": "エタジマシフクシジムシヨ", "name": "江田島市福祉事務所", "prefecture": "広島県", "city": "江田島市", "neighborhood": "大柿町大原", "banchi": "505番地", "postal_code": "7372295", "old_code": "73722", "post_office": "江田島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "エタジマシ", "neighborhood_kana": "オオガキチョウオオバラ", "alternates": []}');
 INSERT INTO office_data VALUES('7372297','{"jis": "34215", "kana": "エタジマシヤクシヨ", "name": "江田島市役所", "prefecture": "広島県", "city": "江田島市", "neighborhood": "大柿町大原", "banchi": "505番地", "postal_code": "7372297", "old_code": "73722", "post_office": "江田島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "エタジマシ", "neighborhood_kana": "オオガキチョウオオバラ", "alternates": []}');
 INSERT INTO office_data VALUES('7372293','{"jis": "34215", "kana": "フルサワケンセツコウギヨウ カブシキガイシヤ", "name": "古澤建設工業　株式会社", "prefecture": "広島県", "city": "江田島市", "neighborhood": "大柿町小古江", "banchi": "1982-2", "postal_code": "7372293", "old_code": "73722", "post_office": "江田島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "エタジマシ", "neighborhood_kana": "オオガキチョウオブレ", "alternates": []}');
 INSERT INTO office_data VALUES('7372393','{"jis": "34215", "kana": "エタジマシヤクシヨ オキミシシヨ", "name": "江田島市役所　沖美支所", "prefecture": "広島県", "city": "江田島市", "neighborhood": "沖美町畑", "banchi": "358番地", "postal_code": "7372393", "old_code": "73723", "post_office": "江田島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "エタジマシ", "neighborhood_kana": "オキミチョウハタ", "alternates": []}');
 INSERT INTO office_data VALUES('7372397','{"jis": "34215", "kana": "エタジマシヤクシヨ ノウミシシヨ", "name": "江田島市役所　能美支所", "prefecture": "広島県", "city": "江田島市", "neighborhood": "能美町中町", "banchi": "4859番地9", "postal_code": "7372397", "old_code": "73723", "post_office": "江田島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "エタジマシ", "neighborhood_kana": "ノウミチョウナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7308670','{"jis": "34302", "kana": "マツダ カブシキガイシヤ", "name": "マツダ　株式会社", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "新地", "banchi": "3-1(広島中央郵便局私書箱第18号)", "postal_code": "7308670", "old_code": "73091", "post_office": "広島中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "シンチ", "alternates": []}');
 INSERT INTO office_data VALUES('7358577','{"jis": "34302", "kana": "イオン カブシキガイシヤ ジヤスコヒロシマフチユウテン", "name": "イオン　株式会社　ジャスコ広島府中店", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "2丁目1-1", "postal_code": "7358577", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
-INSERT INTO office_data VALUES('7358588','{"jis": "34302", "kana": "イオンモ-ル ヒロシマフチユウ", "name": "イオンモール　広島府中", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "2丁目1-1", "postal_code": "7358588", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
+INSERT INTO office_data VALUES('7358588','{"jis": "34302", "kana": "イオンモ-ル ヒロシマフチユウ", "name": "イオンモール　広島府中", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "2丁目1-1", "postal_code": "7358588", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
 INSERT INTO office_data VALUES('7358511','{"jis": "34302", "kana": "カブシキガイシヤ サンリブヒロシマチクテンポウンエイブ", "name": "株式会社　サンリブ広島地区店舗運営部", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "4丁目2-10", "postal_code": "7358511", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
 INSERT INTO office_data VALUES('7358670','{"jis": "34302", "kana": "カブシキガイシヤ マツダ", "name": "株式会社　マツダ", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "新地", "banchi": "3-1", "postal_code": "7358670", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "シンチ", "alternates": []}');
 INSERT INTO office_data VALUES('7358510','{"jis": "34302", "kana": "キリンビ-ル カブシキガイシヤ チユウゴクチクホンブ", "name": "キリンビール　株式会社　中国地区本部", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "2丁目1-1", "postal_code": "7358510", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
 INSERT INTO office_data VALUES('7358501','{"jis": "34302", "kana": "デルタコウギヨウ", "name": "デルタ工業", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "新地", "banchi": "1-14", "postal_code": "7358501", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "シンチ", "alternates": []}');
 INSERT INTO office_data VALUES('7358686','{"jis": "34302", "kana": "フチユウチヨウヤクバ", "name": "府中町役場", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大通", "banchi": "3丁目5-1(安芸府中郵便局私書箱第1号)", "postal_code": "7358686", "old_code": "735  ", "post_office": "安芸府中", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7358555','{"jis": "34302", "kana": "メイコウドウ", "name": "明光堂", "prefecture": "広島県", "city": "安芸郡府中町", "neighborhood": "大須", "banchi": "4丁目1-36", "postal_code": "7358555", "old_code": "735  ", "post_office": "安芸府中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンフチュウチョウ", "neighborhood_kana": "オオス", "alternates": []}');
 INSERT INTO office_data VALUES('7368505','{"jis": "34304", "kana": "カイタ ゼイムシヨ", "name": "海田　税務署", "prefecture": "広島県", "city": "安芸郡海田町", "neighborhood": "大正町", "banchi": "1-13", "postal_code": "7368505", "old_code": "736  ", "post_office": "海田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒロシマケン", "city_kana": "アキグンカイタチョウ", "neighborhood_kana": "タイショウマチ", "alternates": []}');
@@ -139782,15 +139789,15 @@
 INSERT INTO office_data VALUES('7608671','{"jis": "37201", "kana": "カブシキガイシヤ アワギンコウ タカマツシテン", "name": "株式会社　阿波銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "番町", "banchi": "1丁目1-5(高松中央郵便局私書箱第53号)", "postal_code": "7608671", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "バンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7608614','{"jis": "37201", "kana": "カブシキガイシヤ イヨギンコウ タカマツシテン", "name": "（株）　伊予銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "番町", "banchi": "1丁目7-1(高松中央郵便局私書箱第34号)", "postal_code": "7608614", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "バンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7608547','{"jis": "37201", "kana": "カブシキガイシヤ エヌ・テイ・テイ・ドコモ シコクシシヤ", "name": "株式会社　エヌ・ティ・ティ・ドコモ　四国支社", "prefecture": "香川県", "city": "高松市", "neighborhood": "サンポート", "banchi": "2番1号", "postal_code": "7608547", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "サンポート", "alternates": []}');
 INSERT INTO office_data VALUES('7608555','{"jis": "37201", "kana": "カブシキガイシヤ エヌ・テイ・テイ・ドコモ シコクシシヤ", "name": "株式会社　エヌ・ティ・ティ・ドコモ　四国支社", "prefecture": "香川県", "city": "高松市", "neighborhood": "錦町", "banchi": "2丁目4-8", "postal_code": "7608555", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "ニシキマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608621','{"jis": "37201", "kana": "カブシキガイシヤ エヒメギンコウ タカマツシテン", "name": "株式会社　愛媛銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "瓦町", "banchi": "1丁目2-3(高松中央郵便局私書箱第21号)", "postal_code": "7608621", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "カワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608552','{"jis": "37201", "kana": "カブシキガイシヤ コウノ", "name": "株式会社　河野", "prefecture": "香川県", "city": "高松市", "neighborhood": "丸亀町", "banchi": "6-1", "postal_code": "7608552", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "マルガメマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608603','{"jis": "37201", "kana": "カブシキガイシヤ シコクギンコウ タカマツシテン", "name": "株式会社　四国銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "丸亀町", "banchi": "8-23(高松中央郵便局私書箱第39号)", "postal_code": "7608603", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "マルガメマチ", "alternates": []}');
-INSERT INTO office_data VALUES('7608545','{"jis": "37201", "kana": "カブシキガイシヤ タカマツリビングシンブンシヤ", "name": "株式会社　高松リビング新聞社", "prefecture": "香川県", "city": "高松市", "neighborhood": "丸亀町", "banchi": "8-23丸亀町グリーン東館3階", "postal_code": "7608545", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "マルガメマチ", "alternates": []}');
+INSERT INTO office_data VALUES('7608545','{"jis": "37201", "kana": "カブシキガイシヤ タカマツリビングシンブンシヤ", "name": "株式会社　高松リビング新聞社", "prefecture": "香川県", "city": "高松市", "neighborhood": "古新町", "banchi": "8-1高松スクエアビル2階", "postal_code": "7608545", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "フルジンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608667','{"jis": "37201", "kana": "カブシキガイシヤ チユウゴクギンコウ タカマツシテン", "name": "株式会社　中国銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "丸亀町", "banchi": "3-6(高松中央郵便局私書箱第7号)", "postal_code": "7608667", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "マルガメマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608688','{"jis": "37201", "kana": "カブシキガイシヤ テイコクデ-タバンク タカマツシテン", "name": "株式会社　帝国データバンク　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "錦町", "banchi": "1丁目11-3(高松中央郵便局私書箱第18号)", "postal_code": "7608688", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "ニシキマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608638','{"jis": "37201", "kana": "カブシキガイシヤ ヒヤクジユウシギンコウ タカマツシテン", "name": "株式会社　百十四銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "丸亀町", "banchi": "15-7(高松中央郵便局私書箱第38号)", "postal_code": "7608638", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "マルガメマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608630','{"jis": "37201", "kana": "カブシキガイシヤ ミツビシトウキヨウユ-エフジエイギンコウ タカマツシテン", "name": "株式会社　三菱東京ＵＦＪ銀行　高松支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "鍛冶屋町", "banchi": "2-1", "postal_code": "7608630", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "カジヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608588','{"jis": "37201", "kana": "カブシキガイシヤ ヨンデンコウ カガワシテン", "name": "株式会社　四電工　香川支店", "prefecture": "香川県", "city": "高松市", "neighborhood": "西宝町", "banchi": "1丁目8-24", "postal_code": "7608588", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "サイホウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7608505','{"jis": "37201", "kana": "カブシキガイシヤニシヤマ-", "name": "株式会社ニシやマー", "prefecture": "香川県", "city": "高松市", "neighborhood": "塩屋町", "banchi": "1-7", "postal_code": "7608505", "old_code": "760  ", "post_office": "高松中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "シオヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7608636','{"jis": "37201", "kana": "カンイホケンカニユウシヤキヨウカイ", "name": "簡易保険加入者協会", "prefecture": "香川県", "city": "高松市", "neighborhood": "大工町", "banchi": "5-18(高松中央郵便局私書箱第36号)", "postal_code": "7608636", "old_code": "760  ", "post_office": "高松中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "カガワケン", "city_kana": "タカマツシ", "neighborhood_kana": "ダイクマチ", "alternates": []}');
@@ -140211,15 +140218,14 @@
 INSERT INTO office_data VALUES('7928586','{"jis": "38205", "kana": "ザイダンホウジン セキゼンカイフゾクジユウゼンソウゴウビヨウイン", "name": "財団法人　積善会附属十全総合病院", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "北新町", "banchi": "1-5", "postal_code": "7928586", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "キタシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7928521','{"jis": "38205", "kana": "スミトモカガクコウギヨウ カブシキガイシヤ エヒメコウジヨウ", "name": "住友化学工業　株式会社　愛媛工場", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "惣開町", "banchi": "5-1", "postal_code": "7928521", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ソウビラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928520','{"jis": "38205", "kana": "スミトモキヨウドウデンリヨク カブシキガイシヤ", "name": "住友共同電力株式会社", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "磯浦町", "banchi": "2-1", "postal_code": "7928520", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "イソウラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928555','{"jis": "38205", "kana": "スミトモキンゾクコウザン カブシキガイシヤ ベツシジギヨウシヨ", "name": "住友金属鉱山　株式会社　別子事業所", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "西原町", "banchi": "3丁目5-3", "postal_code": "7928555", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ニシバラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928567','{"jis": "38205", "kana": "スミトモケンセツ カブシキガイシヤ シコクシテン", "name": "住友建設　株式会社　四国支店", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "磯浦町", "banchi": "16-6", "postal_code": "7928567", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "イソウラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928588','{"jis": "38205", "kana": "スミトモジユウキカイコウギヨウ カブシキガイシヤ", "name": "住友重機械工業　株式会社", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "惣開町", "banchi": "5-2", "postal_code": "7928588", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ソウビラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928543','{"jis": "38205", "kana": "スミトモベツシビヨウイン", "name": "住友別子病院", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "王子町", "banchi": "3-1", "postal_code": "7928543", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "オウジチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('7928501','{"jis": "38205", "kana": "ダイワシヨウケン カブシキガイシヤ ニイハマシテン", "name": "大和証券　株式会社　新居浜支店", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "港町", "banchi": "2-10", "postal_code": "7928501", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ミナトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7928670','{"jis": "38205", "kana": "トウヨシンヨウキンコ", "name": "東予信用金庫", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "中須賀町", "banchi": "1丁目6-37(新居浜郵便局私書箱第14号)", "postal_code": "7928670", "old_code": "792  ", "post_office": "新居浜", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ナカスカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928580','{"jis": "38205", "kana": "ニイハマコウギヨウコウトウセンモンガツコウ", "name": "新居浜工業高等専門学校", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "八雲町", "banchi": "7-1", "postal_code": "7928580", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ヤグモチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928686','{"jis": "38205", "kana": "ニイハマシヤカイホケンジムシヨ", "name": "新居浜社会保険事務所", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "庄内町", "banchi": "1丁目9-7", "postal_code": "7928686", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ショウナイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928585','{"jis": "38205", "kana": "ニイハマシヤクシヨ", "name": "新居浜市役所", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "一宮町", "banchi": "1丁目5-1", "postal_code": "7928585", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "イックチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7928505','{"jis": "38205", "kana": "モリザネウンユ カブシキガイシヤ", "name": "森実運輸　株式会社", "prefecture": "愛媛県", "city": "新居浜市", "neighborhood": "惣開町", "banchi": "2-13", "postal_code": "7928505", "old_code": "792  ", "post_office": "新居浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "ニイハマシ", "neighborhood_kana": "ソウビラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7910593','{"jis": "38206", "kana": "シユウソウノウキヨウ", "name": "周桑農協", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "丹原町池田", "banchi": "1701-1(丹原郵便局私書箱第7号)", "postal_code": "7910593", "old_code": "79105", "post_office": "丹原", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "タンバラチョウイケダ", "alternates": []}');
 INSERT INTO office_data VALUES('7910594','{"jis": "38206", "kana": "トウヨエンゲイ", "name": "東予園芸", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "丹原町今井", "banchi": "431", "postal_code": "7910594", "old_code": "79105", "post_office": "丹原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "タンバラチョウイマイ", "alternates": []}');
@@ -140782,15 +140788,15 @@
 INSERT INTO office_data VALUES('8128558','{"jis": "40132", "kana": "ヒノデ カブシキガイシヤ", "name": "日野出　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅南", "banchi": "6丁目12-30", "postal_code": "8128558", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('8128636','{"jis": "40132", "kana": "ヒノデスイドウキキ カブシキガイシヤ", "name": "日之出水道機器　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "堅粕", "banchi": "5丁目8-18", "postal_code": "8128636", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "カタカス", "alternates": []}');
 INSERT INTO office_data VALUES('8128625','{"jis": "40132", "kana": "ヒノマル カブシキガイシヤ フクオカシテン", "name": "ヒノマル　株式会社　福岡支店", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "大博町", "banchi": "1-2", "postal_code": "8128625", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "タイハクマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8128643','{"jis": "40132", "kana": "ピツプフジモト カブシキガイシヤ フクオカシテン", "name": "ピップフジモト　株式会社　福岡支店", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "榎田", "banchi": "1丁目4-72", "postal_code": "8128643", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "エノキダ", "alternates": []}');
 INSERT INTO office_data VALUES('8128532','{"jis": "40132", "kana": "フクオカケン シヤカイホケンシンリヨウホウシユウシハライキキン", "name": "福岡県　社会保険診療報酬支払基金", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "美野島", "banchi": "1丁目1-8", "postal_code": "8128532", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ミノシマ", "alternates": []}');
 INSERT INTO office_data VALUES('8128555','{"jis": "40132", "kana": "フクオカケン シンヨウホシヨウキヨウカイ", "name": "福岡県　信用保証協会", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅南", "banchi": "2丁目2-1", "postal_code": "8128555", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('8128521','{"jis": "40132", "kana": "フクオカケンコクミンケンコウホケンダンタイレンゴウカイ", "name": "福岡県国民健康保険団体連合会", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "吉塚本町", "banchi": "13-47", "postal_code": "8128521", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ヨシヅカホンマチ", "alternates": []}');
-INSERT INTO office_data VALUES('8128542','{"jis": "40132", "kana": "フクオカケンハカタケンゼイジムシヨ", "name": "福岡県博多県税事務所", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅東", "banchi": "1丁目17番1号(コネクトスクエア博多内)", "postal_code": "8128542", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキヒガシ", "alternates": []}');
+INSERT INTO office_data VALUES('8128542','{"jis": "40132", "kana": "フクオカケンハカタケンゼイジムシヨ", "name": "福岡県博多県税事務所", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅東", "banchi": "1丁目17番1号(コネクトスクエア博多内)", "postal_code": "8128542", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('8128547','{"jis": "40132", "kana": "フクオカコクゼイキヨク", "name": "福岡国税局", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅東", "banchi": "2丁目11-1", "postal_code": "8128547", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('8128635','{"jis": "40132", "kana": "フクオカコンピユ-タ-サ-ビス カブシキガイシヤ", "name": "福岡コンピューターサービス　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "千代", "banchi": "3丁目5-30", "postal_code": "8128635", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "チヨ", "alternates": []}');
 INSERT INTO office_data VALUES('8128512','{"jis": "40132", "kana": "フクオカシ ハカタクヤクシヨ", "name": "福岡市　博多区役所", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅前", "banchi": "2丁目9-3", "postal_code": "8128512", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('8128620','{"jis": "40132", "kana": "フクオカシコウワンクウコウキヨク", "name": "福岡市港湾空港局", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "沖浜町", "banchi": "12番1号", "postal_code": "8128620", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "オキハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8128505','{"jis": "40132", "kana": "フクオカシヨウコウカイギシヨ", "name": "福岡商工会議所", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "博多駅前", "banchi": "2丁目9-28", "postal_code": "8128505", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ハカタエキマエ", "alternates": []}');
 INSERT INTO office_data VALUES('8128632','{"jis": "40132", "kana": "フクオカニツサンジドウシヤ カブシキガイシヤ", "name": "福岡日産自動車　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "千代", "banchi": "1丁目21-37", "postal_code": "8128632", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "チヨ", "alternates": []}');
 INSERT INTO office_data VALUES('8128631','{"jis": "40132", "kana": "フクオカニツサンジドウシヤ カブシキガイシヤ", "name": "福岡日産自動車　株式会社", "prefecture": "福岡県", "city": "福岡市博多区", "neighborhood": "東比恵", "banchi": "2丁目14番33号", "postal_code": "8128631", "old_code": "812  ", "post_office": "博多北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクオカシハカタク", "neighborhood_kana": "ヒガシヒエ", "alternates": []}');
@@ -141387,15 +141393,15 @@
 INSERT INTO office_data VALUES('8491394','{"jis": "41207", "kana": "ユウトクイナリジンジヤ", "name": "祐徳稲荷神社", "prefecture": "佐賀県", "city": "鹿島市", "neighborhood": "古枝", "banchi": "乙1855", "postal_code": "8491394", "old_code": "84913", "post_office": "鹿島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カシマシ", "neighborhood_kana": "フルエダ", "alternates": []}');
 INSERT INTO office_data VALUES('8491393','{"jis": "41207", "kana": "ユウトクヤクヒンコウギヨウ カブシキガイシヤ", "name": "祐徳薬品工業　株式会社", "prefecture": "佐賀県", "city": "鹿島市", "neighborhood": "大字納富分", "banchi": "2596番地1(鹿島郵便局私書箱第8号)", "postal_code": "8491393", "old_code": "84913", "post_office": "鹿島", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8458501','{"jis": "41208", "kana": "オギシヤクシヨ オギチヨウシヤ", "name": "小城市役所　小城庁舎", "prefecture": "佐賀県", "city": "小城市", "neighborhood": "小城町", "banchi": "253-21", "postal_code": "8458501", "old_code": "845  ", "post_office": "小城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "オギシ", "neighborhood_kana": "オギマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8458511','{"jis": "41208", "kana": "オギシヤクシヨ ミカヅキチヨウシヤ", "name": "小城市役所　三日月庁舎", "prefecture": "佐賀県", "city": "小城市", "neighborhood": "三日月町長神田", "banchi": "2312-2", "postal_code": "8458511", "old_code": "845  ", "post_office": "小城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "オギシ", "neighborhood_kana": "ミカツキチョウチョウカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('8458510','{"jis": "41208", "kana": "タケシタセイカ カブシキガイシヤ", "name": "竹下製菓　株式会社", "prefecture": "佐賀県", "city": "小城市", "neighborhood": "小城町池上", "banchi": "2500", "postal_code": "8458510", "old_code": "845  ", "post_office": "小城", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "オギシ", "neighborhood_kana": "オギマチイケノウエ", "alternates": []}');
 INSERT INTO office_data VALUES('8430394','{"jis": "41209", "kana": "イリヨウホウジンザイダン ユウホウカイ", "name": "医療法人財団　友朋会", "prefecture": "佐賀県", "city": "嬉野市", "neighborhood": "嬉野町大字下宿", "banchi": "乙1919番地", "postal_code": "8430394", "old_code": "84303", "post_office": "嬉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8430392','{"jis": "41209", "kana": "ウレシノシヤクシヨ ウレシノソウゴウシシヨ", "name": "嬉野市役所　嬉野総合支所", "prefecture": "佐賀県", "city": "嬉野市", "neighborhood": "嬉野町大字下宿", "banchi": "乙1185(嬉野郵便局私書箱第12号)", "postal_code": "8430392", "old_code": "84303", "post_office": "嬉野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('8430393','{"jis": "41209", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ウレシノイリヨウセンタ-", "name": "独立行政法人　国立病院機構　嬉野医療センター", "prefecture": "佐賀県", "city": "嬉野市", "neighborhood": "嬉野町大字下宿", "banchi": "甲4279-3", "postal_code": "8430393", "old_code": "84303", "post_office": "嬉野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('8430393','{"jis": "41209", "kana": "ドクリツギヨウセイホウジン コクリツビヨウインキコウ ウレシノイリヨウセンタ-", "name": "独立行政法人　国立病院機構　嬉野医療センター", "prefecture": "佐賀県", "city": "嬉野市", "neighborhood": "嬉野町大字下宿", "banchi": "甲4760-1", "postal_code": "8430393", "old_code": "84303", "post_office": "嬉野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8491492','{"jis": "41209", "kana": "ウレシノシヤクシヨ", "name": "嬉野市役所", "prefecture": "佐賀県", "city": "嬉野市", "neighborhood": "塩田町大字馬場下", "banchi": "甲1769", "postal_code": "8491492", "old_code": "84914", "post_office": "武雄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8428502','{"jis": "41210", "kana": "カンザキシ チヨダソウゴウシシヨ", "name": "神埼市　千代田総合支所", "prefecture": "佐賀県", "city": "神埼市", "neighborhood": "千代田町直鳥", "banchi": "166-1", "postal_code": "8428502", "old_code": "842  ", "post_office": "神埼", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキシ", "neighborhood_kana": "チヨダチョウナオトリ", "alternates": []}');
 INSERT INTO office_data VALUES('8428601','{"jis": "41210", "kana": "カンザキシヤクシヨ", "name": "神埼市役所", "prefecture": "佐賀県", "city": "神埼市", "neighborhood": "神埼町鶴", "banchi": "3542番地1(神埼郵便局私書箱第2号)", "postal_code": "8428601", "old_code": "842  ", "post_office": "神埼", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキシ", "neighborhood_kana": "カンザキマチツル", "alternates": []}');
 INSERT INTO office_data VALUES('8428585','{"jis": "41210", "kana": "ニシキユウシユウダイガク", "name": "西九州大学", "prefecture": "佐賀県", "city": "神埼市", "neighborhood": "神埼町尾崎", "banchi": "4490-9", "postal_code": "8428585", "old_code": "842  ", "post_office": "神埼", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキシ", "neighborhood_kana": "カンザキマチオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('8420292','{"jis": "41210", "kana": "カンザキシ セフリソウゴウシシヨ", "name": "神埼市　脊振総合支所", "prefecture": "佐賀県", "city": "神埼市", "neighborhood": "脊振町広滝", "banchi": "558-2", "postal_code": "8420292", "old_code": "84202", "post_office": "脊振", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキシ", "neighborhood_kana": "セフリマチヒロタキ", "alternates": []}');
 INSERT INTO office_data VALUES('8420293','{"jis": "41210", "kana": "コウクウジエイタイ セフリヤマブントンキチ", "name": "航空自衛隊　脊振山分屯基地", "prefecture": "佐賀県", "city": "神埼市", "neighborhood": "脊振町服巻", "banchi": "1358", "postal_code": "8420293", "old_code": "84202", "post_office": "脊振", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキシ", "neighborhood_kana": "セフリマチハラマキ", "alternates": []}');
 INSERT INTO office_data VALUES('8428501','{"jis": "41327", "kana": "ヨシノガリチヨウヤクバ", "name": "吉野ヶ里町役場", "prefecture": "佐賀県", "city": "神埼郡吉野ヶ里町", "neighborhood": "吉田", "banchi": "321-2", "postal_code": "8428501", "old_code": "842  ", "post_office": "神埼", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サガケン", "city_kana": "カンザキグンヨシノガリチョウ", "neighborhood_kana": "ヨシダ", "alternates": []}');
@@ -141423,15 +141429,15 @@
 INSERT INTO office_data VALUES('8508566','{"jis": "42201", "kana": "イツパンザイダンホウジン ナガサキケンキヨウシヨクインゴジヨクミアイ", "name": "一般財団法人　長崎県教職員互助組合", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "尾上町", "banchi": "3番1号", "postal_code": "8508566", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "オノウエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508511','{"jis": "42201", "kana": "イツパンシヤダンホウジン ナガサキシイシカイ", "name": "一般社団法人　長崎市医師会", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "栄町", "banchi": "2-22", "postal_code": "8508511", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508611','{"jis": "42201", "kana": "カブシキガイシヤ エヌテイテイマ-ケテイングアクトキユウシユウ", "name": "株式会社　エヌ・ティ・ティ・マーケティングアクト九州", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "出島町", "banchi": "14-7", "postal_code": "8508611", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "デジママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508550','{"jis": "42201", "kana": "カブシキガイシヤ エフエムナガサキ", "name": "株式会社　エフエム長崎", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "栄町", "banchi": "5-5", "postal_code": "8508550", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508577','{"jis": "42201", "kana": "カブシキガイシヤ サセボタマヤ ナガサキシテン", "name": "株式会社　佐世保玉屋　長崎支店", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "新大工町", "banchi": "5-35", "postal_code": "8508577", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "シンダイクマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508530','{"jis": "42201", "kana": "カブシキガイシヤ タナカヤ", "name": "株式会社　タナカヤ", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "浜町", "banchi": "8-30", "postal_code": "8508530", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "ハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508551','{"jis": "42201", "kana": "カブシキガイシヤ テレビナガサキ", "name": "株式会社　テレビ長崎", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "金屋町", "banchi": "1番7号", "postal_code": "8508551", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "カナヤマチ", "alternates": []}');
-INSERT INTO office_data VALUES('8508505','{"jis": "42201", "kana": "カブシキガイシヤ トウビ", "name": "株式会社　東美", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "栄町", "banchi": "5-5FM長崎ビル3F", "postal_code": "8508505", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
+INSERT INTO office_data VALUES('8508505','{"jis": "42201", "kana": "カブシキガイシヤ トウビ", "name": "株式会社　東美", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "栄町", "banchi": "5-5FM長崎ビル3F", "postal_code": "8508505", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508545','{"jis": "42201", "kana": "カブシキガイシヤ ナガサキケンシユハン", "name": "株式会社　長崎県酒販", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "出島町", "banchi": "15-7", "postal_code": "8508545", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "デジママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508504','{"jis": "42201", "kana": "カブシキガイシヤ ナガサキコクサイテレビ", "name": "株式会社　長崎国際テレビ", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "出島町", "banchi": "11-1", "postal_code": "8508504", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "デジママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508580','{"jis": "42201", "kana": "カブシキガイシヤ ハカタダイマル ナガサキテン", "name": "株式会社　博多大丸　長崎店", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "浜町", "banchi": "4-11", "postal_code": "8508580", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "ハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508510','{"jis": "42201", "kana": "カブシキガイシヤ ハマヤヒヤツカテン", "name": "株式会社　浜屋百貨店", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "浜町", "banchi": "7-11", "postal_code": "8508510", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "ハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508508','{"jis": "42201", "kana": "カブシキガイシヤ マルモト", "name": "株式会社　丸本", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "大井手町", "banchi": "51-2", "postal_code": "8508508", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "オオイデマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508586','{"jis": "42201", "kana": "ガツコウホウジン カイセイガクエン カイセイチユウガツコウ・カイセイコウトウガツコウ", "name": "学校法人　海星学園　海星中学校・海星高等学校", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "東山手町", "banchi": "5番3号", "postal_code": "8508586", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "ヒガシヤマテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8508515','{"jis": "42201", "kana": "ガツコウホウジン カツスイガクイン", "name": "学校法人　活水学院", "prefecture": "長崎県", "city": "長崎市", "neighborhood": "東山手町", "banchi": "1-50", "postal_code": "8508515", "old_code": "850  ", "post_office": "長崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガサキケン", "city_kana": "ナガサキシ", "neighborhood_kana": "ヒガシヤマテマチ", "alternates": []}');
@@ -141681,14 +141687,15 @@
 INSERT INTO office_data VALUES('8608739','{"jis": "43101", "kana": "クマモトワイエムシ-エ-", "name": "熊本ＹＭＣＡ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "段山本町", "banchi": "4-1", "postal_code": "8608739", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ダニヤマホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608524','{"jis": "43101", "kana": "コウエキザイダンホウジン ニホンムセンキヨウカイ キユウシユウシブ", "name": "公益財団法人　日本無線協会　九州支部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "6-7いちご熊本ビル", "postal_code": "8608524", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608530','{"jis": "43101", "kana": "サンリブシテイクマナン", "name": "サンリブシティくまなん", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "平成", "banchi": "3丁目23-30", "postal_code": "8608530", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヘイセイ", "alternates": []}');
 INSERT INTO office_data VALUES('8608650','{"jis": "43101", "kana": "ザイダンホウジン カンイホケンカニユウシヤキヨウカイ キユウシユウチホウホンブ", "name": "財団法人　簡易保険加入者協会　九州地方本部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水道町", "banchi": "3-37九特会館2階", "postal_code": "8608650", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイドウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608587','{"jis": "43101", "kana": "スミトモセイメイホケン ソウゴガイシヤ クマモトシシヤ", "name": "住友生命保険　相互会社　熊本支社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "9番24号", "postal_code": "8608587", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608502','{"jis": "43101", "kana": "ゼンコクケンコウホケンキヨウカイ クマモトシブ", "name": "全国健康保険協会　熊本支部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5-1日本生命熊本ビル10階", "postal_code": "8608502", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608526','{"jis": "43101", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキカイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "10-26", "postal_code": "8608526", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('8608688','{"jis": "43101", "kana": "ダイワシヨウケン カブシキガイシヤ クマモトシテン", "name": "大和証券　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5-1(熊本中央郵便局私書箱第120号)", "postal_code": "8608688", "old_code": "860  ", "post_office": "熊本中央", "type": "box", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608618','{"jis": "43101", "kana": "チユオウクヤクシヨ", "name": "中央区役所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "手取本町", "banchi": "1番1号", "postal_code": "8608618", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "テトリホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608521','{"jis": "43101", "kana": "ツルハラヨシイ カブシキガイシヤ", "name": "鶴原吉井　株式会社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安町", "banchi": "356", "postal_code": "8608521", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤスマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608504','{"jis": "43101", "kana": "テルウエルニシニホン (カブ) キユウシユウシテン ナカキユウシユウエイギヨウシテン", "name": "テルウェル西日本　（株）　九州支店　中九州営業支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "南熊本", "banchi": "5丁目1-1", "postal_code": "8608504", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ミナミクマモト", "alternates": []}');
 INSERT INTO office_data VALUES('8608581','{"jis": "43101", "kana": "ニツシンイリヨウシヨクヒン カブシキカイシヤ ミナミキユウシユウシテン", "name": "日清医療食品　株式会社　南九州支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5番1号日本生命熊本ビル9階", "postal_code": "8608581", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608602','{"jis": "43101", "kana": "ニツポンホウソウキヨウカイ クマモトホウソウキヨク", "name": "日本放送協会　熊本放送局", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "5-1", "postal_code": "8608602", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8628793','{"jis": "43101", "kana": "ニホンユウビン カブシキガイシヤ キユウシユウシシヤ ユウビンジギヨウホンブ (サンシユ)", "name": "日本郵便　株式会社　九州支社　郵便事業本部　（三種）", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1-1", "postal_code": "8628793", "old_code": "860  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608510','{"jis": "43101", "kana": "フジツウ カブシキガイシヤ クマモトシテン", "name": "富士通　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "紺屋今町", "banchi": "9-6", "postal_code": "8608510", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "コウヤイママチ", "alternates": []}');
@@ -141699,15 +141706,14 @@
 INSERT INTO office_data VALUES('8608686','{"jis": "43101", "kana": "カブシキガイシヤ ニツセンレンフアイナンス", "name": "株式会社　日専連ファイナンス", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "安政町", "banchi": "6-5(熊本中央郵便局私書箱第139号)", "postal_code": "8608686", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "アンセイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608606','{"jis": "43101", "kana": "カブシキガイシヤ フクオカギンコウ クマモトシテン", "name": "株式会社　福岡銀行　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "12-3(熊本中央郵便局私書箱第84号)", "postal_code": "8608606", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608601','{"jis": "43101", "kana": "クマモトシヤクシヨ", "name": "熊本市役所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "手取本町", "banchi": "1-1(熊本中央郵便局私書箱第110号)", "postal_code": "8608601", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "テトリホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608655','{"jis": "43101", "kana": "クマモトシンヨウキンコ", "name": "熊本信用金庫", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "手取本町", "banchi": "2-1(熊本中央郵便局私書箱第28号)", "postal_code": "8608655", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "テトリホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608681','{"jis": "43101", "kana": "クマモトダイイチシンヨウキンコ", "name": "熊本第一信用金庫", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "10-29(熊本中央郵便局私書箱第71号)", "postal_code": "8608681", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608624','{"jis": "43101", "kana": "クマモトニシゼイムシヨ", "name": "熊本西税務署", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "二の丸", "banchi": "1-4(熊本中央郵便局私書箱第57号)", "postal_code": "8608624", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ニノマル", "alternates": []}');
 INSERT INTO office_data VALUES('8608660','{"jis": "43101", "kana": "シヨウコウクミアイチユウオウキンコ クマモトシテン", "name": "商工組合中央金庫　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "2-23(熊本中央郵便局私書箱第17号)", "postal_code": "8608660", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}');
-INSERT INTO office_data VALUES('8608688','{"jis": "43101", "kana": "ダイワシヨウケン カブシキガイシヤ クマモトシテン", "name": "大和証券　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "12-28(熊本中央郵便局私書箱第120号)", "postal_code": "8608688", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608605','{"jis": "43101", "kana": "ニホンセイメイホケン ソウゴガイシヤ クマモトシシヤ", "name": "日本生命保険　相互会社　熊本支社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "中央街", "banchi": "2-11(熊本中央郵便局私書箱第16号)", "postal_code": "8608605", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "チュウオウガイ", "alternates": []}');
 INSERT INTO office_data VALUES('8608604','{"jis": "43101", "kana": "ノムラシヨウケン カブシキガイシヤ クマモトシテン", "name": "野村證券　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "12-30(熊本中央郵便局私書箱第81号)", "postal_code": "8608604", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8628716','{"jis": "43101", "kana": "(ザイ) ポスタルサ-ビスセンタ- キユウシユウチホウホンブ", "name": "（財）　ポスタルサービスセンター　九州地方本部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "神水", "banchi": "2丁目7-10神水中島ビル1F(熊本東郵便局私書箱第50号)", "postal_code": "8628716", "old_code": "862  ", "post_office": "熊本東", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "クワミズ", "alternates": []}');
 INSERT INTO office_data VALUES('8628655','{"jis": "43101", "kana": "イリヨウホウジン ソウキカイ クマモトシントソウゴウビヨウイン", "name": "医療法人　創起会　くまもと森都総合病院", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "3-2-65", "postal_code": "8628655", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": []}');
 INSERT INTO office_data VALUES('8628677','{"jis": "43101", "kana": "カイシンコウトウガツコウ", "name": "開新高等学校", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "6丁目1-33", "postal_code": "8628677", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": []}');
 INSERT INTO office_data VALUES('8628601','{"jis": "43101", "kana": "カブシキガイシヤ クマモトギンコウ", "name": "株式会社　熊本銀行", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目29-20", "postal_code": "8628601", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628504','{"jis": "43101", "kana": "カブシキガイシヤ クマモトケンミンテレビ", "name": "株式会社　熊本県民テレビ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "2丁目1番10号", "postal_code": "8628504", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": []}');
@@ -141956,15 +141962,15 @@
 INSERT INTO office_data VALUES('8700189','{"jis": "44201", "kana": "シヨウワデンコウ カブシキガイシヤ オオイタジムシヨ", "name": "昭和電工　株式会社　大分事務所", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字中ノ洲", "banchi": "2", "postal_code": "8700189", "old_code": "87001", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700194','{"jis": "44201", "kana": "スミトモカガクコウギヨウ カブシキガイシヤ オオイタコウジヨウ", "name": "住友化学工業　株式会社　大分工場", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字鶴崎", "banchi": "2200", "postal_code": "8700194", "old_code": "87001", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700196','{"jis": "44201", "kana": "ツルサキカイリクウンユ カブシキガイシヤ", "name": "鶴崎海陸運輸　株式会社", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字三佐", "banchi": "1000", "postal_code": "8700196", "old_code": "87001", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700292','{"jis": "44201", "kana": "オオイタキヤノン カブシキガイシヤ オオイタジギヨウシヨ", "name": "大分キヤノン　株式会社　大分事業所", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字迫", "banchi": "564-1", "postal_code": "8700292", "old_code": "87002", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700392','{"jis": "44201", "kana": "アサヒカセイコウギヨウ カブシキガイシヤ オオイタコウジヨウ", "name": "旭化成工業　株式会社　大分工場", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字里", "banchi": "2620", "postal_code": "8700392", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700396','{"jis": "44201", "kana": "アサヒカセイメデイカルエムテイ- カブシキガイシヤ", "name": "旭化成メディカルＭＴ　株式会社", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字里", "banchi": "2111-2", "postal_code": "8700396", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700393','{"jis": "44201", "kana": "オオイタケンリツ オオイタヒガシコウトウガツコウ", "name": "大分県立　大分東高等学校", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字屋山", "banchi": "2009", "postal_code": "8700393", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('8700395','{"jis": "44201", "kana": "カブシキガイシヤ ミツイイ-アンドエスマシナリ- オオイタコウジヨウ", "name": "株式会社　三井Ｅ＆Ｓマシナリー　大分工場", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字日吉原", "banchi": "3番地", "postal_code": "8700395", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('8700395','{"jis": "44201", "kana": "カブシキガイシヤ ミツイイ-アンドエス オオイタジギヨウバ", "name": "株式会社　三井Ｅ＆Ｓ　大分事業場", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字日吉原", "banchi": "3番地", "postal_code": "8700395", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700397','{"jis": "44201", "kana": "ニホンブンリダイガク", "name": "日本文理大学", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字一木", "banchi": "1727-162", "postal_code": "8700397", "old_code": "87003", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700401','{"jis": "44201", "kana": "オオイタケンウンテンメンキヨセンタ-", "name": "大分県運転免許センター", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字松岡", "banchi": "6687", "postal_code": "8700401", "old_code": "87004", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8700992','{"jis": "44201", "kana": "ニツポンセイテツ カブシキカイシヤ キユウシユウセイテツシヨオオイタチク", "name": "日本製鉄　株式会社　九州製鉄所大分地区", "prefecture": "大分県", "city": "大分市", "neighborhood": "西ノ洲", "banchi": "一番地", "postal_code": "8700992", "old_code": "87009", "post_office": "大分東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオイタケン", "city_kana": "オオイタシ", "neighborhood_kana": "ニシノス", "alternates": []}');
 INSERT INTO office_data VALUES('8701195','{"jis": "44201", "kana": "オオイタシイシカイリツ アルメイダビヨウイン", "name": "大分市医師会立　アルメイダ病院", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字宮崎", "banchi": "1509-2", "postal_code": "8701195", "old_code": "87011", "post_office": "大分南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8701192','{"jis": "44201", "kana": "オオイタダイガク", "name": "大分大学", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字旦野原", "banchi": "700", "postal_code": "8701192", "old_code": "87011", "post_office": "大分南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8701198','{"jis": "44201", "kana": "カブシキガイシヤ トキハワサダテン", "name": "株式会社　トキハ稙田店", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字玉沢", "banchi": "字楠本755-1", "postal_code": "8701198", "old_code": "87011", "post_office": "大分南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8701292','{"jis": "44201", "kana": "オオイタシヤクシヨ ノツハルシシヨ", "name": "大分市役所　野津原支所", "prefecture": "大分県", "city": "大分市", "neighborhood": "大字野津原", "banchi": "800", "postal_code": "8701292", "old_code": "87012", "post_office": "野津原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -142066,15 +142072,14 @@
 INSERT INTO office_data VALUES('8791592','{"jis": "44341", "kana": "ヒジマチヤクバ", "name": "日出町役場", "prefecture": "大分県", "city": "速見郡日出町", "neighborhood": "", "banchi": "2974番地の1", "postal_code": "8791592", "old_code": "87915", "post_office": "別府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオイタケン", "city_kana": "ハヤミグンヒジマチ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8791593','{"jis": "44341", "kana": "ホンダタイヨウ カブシキカイシヤ", "name": "ホンダ太陽　株式会社", "prefecture": "大分県", "city": "速見郡日出町", "neighborhood": "大字川崎", "banchi": "3968", "postal_code": "8791593", "old_code": "87915", "post_office": "日出", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8794692','{"jis": "44461", "kana": "ヤツシカシユゾウ カブシキガイシヤ", "name": "八鹿酒造　株式会社", "prefecture": "大分県", "city": "玖珠郡九重町", "neighborhood": "大字右田", "banchi": "3364", "postal_code": "8794692", "old_code": "87946", "post_office": "恵良", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8794492','{"jis": "44462", "kana": "クスマチヤクバ", "name": "玖珠町役場", "prefecture": "大分県", "city": "玖珠郡玖珠町", "neighborhood": "大字帆足", "banchi": "268-5(玖珠郵便局私書箱第1号)", "postal_code": "8794492", "old_code": "87944", "post_office": "玖珠", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8794498','{"jis": "44462", "kana": "リクジヨウジエイタイクスチユウトンチ", "name": "陸上自衛隊玖珠駐屯地", "prefecture": "大分県", "city": "玖珠郡玖珠町", "neighborhood": "大字帆足", "banchi": "2494", "postal_code": "8794498", "old_code": "87944", "post_office": "玖珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8808625','{"jis": "45201", "kana": "エスエムビ-シ-ニツコウシヨウケン カブシキガイシヤ ミヤザキシテン", "name": "ＳＭＢＣ日興証券　株式会社　宮崎支店", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "橘通西", "banchi": "4丁目1番32号(宮崎中央郵便局私書箱第25号)", "postal_code": "8808625", "old_code": "880  ", "post_office": "宮崎中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "タチバナドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('8808725','{"jis": "45201", "kana": "エスエムビ-シ-ニツコウシヨウケン カブシキガイシヤ ミヤザキシテン", "name": "ＳＭＢＣ日興証券　株式会社　宮崎支店", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "橘通西", "banchi": "4丁目1番32号", "postal_code": "8808725", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "タチバナドオリニシ", "alternates": []}');
-INSERT INTO office_data VALUES('8808583','{"jis": "45201", "kana": "カブシキガイシヤ エフエムミヤザキ", "name": "株式会社　エフエム宮崎", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "祇園", "banchi": "2丁目78", "postal_code": "8808583", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "ギオン", "alternates": []}');
 INSERT INTO office_data VALUES('8808550','{"jis": "45201", "kana": "カブシキガイシヤ シダグミ", "name": "株式会社　志多組", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "高千穂通", "banchi": "1丁目4-30", "postal_code": "8808550", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "タカチホドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8808586','{"jis": "45201", "kana": "カブシキガイシヤ タチバナヒヤツカテン", "name": "株式会社　橘百貨店", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "橘通西", "banchi": "3丁目10-32", "postal_code": "8808586", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "タチバナドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('8808535','{"jis": "45201", "kana": "カブシキガイシヤ テレビミヤザキ", "name": "株式会社　テレビ宮崎", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "祇園", "banchi": "2丁目78", "postal_code": "8808535", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "ギオン", "alternates": []}');
 INSERT INTO office_data VALUES('8808576','{"jis": "45201", "kana": "カブシキガイシヤ ミヤザキサンシヤインエフエム", "name": "株式会社　宮崎サンシャインエフエム", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "大淀", "banchi": "4丁目6番28号宮交シティ3F", "postal_code": "8808576", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "オオヨド", "alternates": []}');
 INSERT INTO office_data VALUES('8808606','{"jis": "45201", "kana": "カブシキガイシヤ ミヤザキタイヨウギンコウ", "name": "株式会社　宮崎太陽銀行", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "広島", "banchi": "2丁目1-31(宮崎中央郵便局私書箱第20号)", "postal_code": "8808606", "old_code": "880  ", "post_office": "宮崎中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "ヒロシマ", "alternates": []}');
 INSERT INTO office_data VALUES('8808559','{"jis": "45201", "kana": "カブシキガイシヤ ライフ ミヤザキシテン", "name": "株式会社　ライフ　宮崎支店", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "高千穂通", "banchi": "2丁目5番32号", "postal_code": "8808559", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "タカチホドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('8808503','{"jis": "45201", "kana": "ガツコウホウジン ミヤザキガクエン ミヤザキガクエンコウトウガツコウ", "name": "学校法人　宮崎学園　宮崎学園高等学校", "prefecture": "宮崎県", "city": "宮崎市", "neighborhood": "昭和町", "banchi": "3", "postal_code": "8808503", "old_code": "880  ", "post_office": "宮崎中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ミヤザキケン", "city_kana": "ミヤザキシ", "neighborhood_kana": "ショウワチョウ", "alternates": []}');
@@ -142481,15 +142486,15 @@
 INSERT INTO office_data VALUES('8917192','{"jis": "46530", "kana": "トクノシマチヨウヤクバ", "name": "徳之島町役場", "prefecture": "鹿児島県", "city": "大島郡徳之島町", "neighborhood": "亀津", "banchi": "7203番地", "postal_code": "8917192", "old_code": "89171", "post_office": "亀津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カゴシマケン", "city_kana": "オオシマグントクノシマチョウ", "neighborhood_kana": "カメツ", "alternates": []}');
 INSERT INTO office_data VALUES('8917692','{"jis": "46531", "kana": "アマギチヨウヤクバ", "name": "天城町役場", "prefecture": "鹿児島県", "city": "大島郡天城町", "neighborhood": "大字平土野", "banchi": "2691番地1", "postal_code": "8917692", "old_code": "89176", "post_office": "平土野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8918293','{"jis": "46532", "kana": "イセンチヨウヤクバ", "name": "伊仙町役場", "prefecture": "鹿児島県", "city": "大島郡伊仙町", "neighborhood": "大字伊仙", "banchi": "1842", "postal_code": "8918293", "old_code": "89182", "post_office": "面縄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8919192','{"jis": "46533", "kana": "ワドマリチヨウヤクバ", "name": "和泊町役場", "prefecture": "鹿児島県", "city": "大島郡和泊町", "neighborhood": "大字和泊", "banchi": "10", "postal_code": "8919192", "old_code": "89191", "post_office": "和泊", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8919294','{"jis": "46534", "kana": "アマミノウギヨウキヨウドウクミアイ チナジギヨウホンブ", "name": "あまみ農業協同組合　知名事業本部", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字瀬利覚", "banchi": "2117", "postal_code": "8919294", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8919296','{"jis": "46534", "kana": "オキエラブトクシユウカイビヨウイン", "name": "沖永良部徳洲会病院", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字瀬利覚", "banchi": "2208", "postal_code": "8919296", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8919293','{"jis": "46534", "kana": "カゴシマケンリツ オキエラブコウトウガツコウ", "name": "鹿児島県立　沖永良部高等学校", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字余多", "banchi": "241", "postal_code": "8919293", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('8919292','{"jis": "46534", "kana": "コウクウジエイタイダイ55ケイカイグン", "name": "航空自衛隊第５５警戒群", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字上平川", "banchi": "2081-1", "postal_code": "8919292", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('8919292','{"jis": "46534", "kana": "コウクウジエイタイダイ55ケイカイタイ", "name": "航空自衛隊第５５警戒隊", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字瀬利覚", "banchi": "3196-1", "postal_code": "8919292", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8919295','{"jis": "46534", "kana": "チナチヨウヤクバ", "name": "知名町役場", "prefecture": "鹿児島県", "city": "大島郡知名町", "neighborhood": "大字知名", "banchi": "307", "postal_code": "8919295", "old_code": "89192", "post_office": "知名", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9008556','{"jis": "47201", "kana": "イリヨウホウジン シヨウアンカイ オモロマチメデイカルセンタ-", "name": "医療法人　祥杏会　おもろまちメディカルセンター", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "上之屋", "banchi": "1丁目3-1", "postal_code": "9008556", "old_code": "900  ", "post_office": "那覇中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "ウエノヤ", "alternates": []}');
 INSERT INTO office_data VALUES('9008560','{"jis": "47201", "kana": "ウエハラロウムカンリジムシヨ", "name": "上原労務管理事務所", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "おもろまち", "banchi": "4丁目7番7号URビル2F", "postal_code": "9008560", "old_code": "900  ", "post_office": "那覇中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "オモロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9008535','{"jis": "47201", "kana": "エヌエイチケイオキナワホウソウキヨク", "name": "ＮＨＫ沖縄放送局", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "おもろまち", "banchi": "2丁目6-21", "postal_code": "9008535", "old_code": "900  ", "post_office": "那覇中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "オモロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9008545','{"jis": "47201", "kana": "エヌテイテイ オキナワシテン", "name": "ＮＴＴ　沖縄支店", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "楚辺", "banchi": "1丁目14-16楚辺ビル", "postal_code": "9008545", "old_code": "900  ", "post_office": "那覇中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "ソベ", "alternates": []}');
 INSERT INTO office_data VALUES('9008686','{"jis": "47201", "kana": "オキナワカイホウギンコウ", "name": "沖縄海邦銀行", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "前島", "banchi": "2-21-7(那覇中央郵便局私書箱第432号)", "postal_code": "9008686", "old_code": "900  ", "post_office": "那覇中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "マエジマ", "alternates": []}');
 INSERT INTO office_data VALUES('9008796','{"jis": "47201", "kana": "オキナワカンサシツ", "name": "沖縄監査室", "prefecture": "沖縄県", "city": "那覇市", "neighborhood": "東町", "banchi": "26-29(4F)", "postal_code": "9008796", "old_code": "900  ", "post_office": "那覇中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "ナハシ", "neighborhood_kana": "ヒガシマチ", "alternates": []}');
```

### Comparing `posuto-2024.4.0/posuto/posuto.py` & `posuto-2024.5.0/posuto/posuto.py`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/posuto/prep.py` & `posuto-2024.5.0/posuto/prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             # handle notes
             neighborhood, note = re.search(NOTE_REGEX, row['neighborhood']).groups()
             if note:
                 row['neighborhood'] = neighborhood
                 row['note'] = note[1:-1] # trim parens
                 row['note'] = mojimoji.zen_to_han(row['note'], kana=False) # no zengaku :P
                 # don't need kana for note
-                row['neighborhood_kana'] = re.sub('\(.*\)?', '', row['neighborhood_kana'])
+                row['neighborhood_kana'] = re.sub(r'\(.*\)?', '', row['neighborhood_kana'])
 
             # fix hankaku
             for field in PARTS:
                 key = field + '_kana'
                 row[key] = mojimoji.han_to_zen(row[key])
 
             # handle flags
```

### Comparing `posuto-2024.4.0/posuto/tests/test_basic.py` & `posuto-2024.5.0/posuto/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `posuto-2024.4.0/posuto.egg-info/PKG-INFO` & `posuto-2024.5.0/posuto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `posuto-2024.4.0/setup.cfg` & `posuto-2024.5.0/setup.cfg`

 * *Files identical despite different names*

