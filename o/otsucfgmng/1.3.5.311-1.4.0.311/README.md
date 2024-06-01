# Comparing `tmp/otsucfgmng-1.3.5.311-py3-none-any.whl.zip` & `tmp/otsucfgmng-1.4.0.311-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 12258 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      272 b- defN 24-May-26 01:00 otsucfgmng/__init__.py
--rw-rw-rw-  2.0 fat    10373 b- defN 24-May-26 01:21 otsucfgmng/configuration_manager.py
--rw-rw-rw-  2.0 fat     2055 b- defN 24-May-26 01:06 otsucfgmng/funcs.py
--rw-rw-rw-  2.0 fat     1087 b- defN 24-May-26 01:30 otsucfgmng-1.3.5.311.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    20264 b- defN 24-May-26 01:30 otsucfgmng-1.3.5.311.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 01:30 otsucfgmng-1.3.5.311.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-26 01:30 otsucfgmng-1.3.5.311.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      673 b- defN 24-May-26 01:30 otsucfgmng-1.3.5.311.dist-info/RECORD
-8 files, 34827 bytes uncompressed, 11080 bytes compressed:  68.2%
+Zip file size: 14823 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      319 b- defN 24-Jun-01 17:06 otsucfgmng/__init__.py
+-rw-rw-rw-  2.0 fat    10378 b- defN 24-Jun-01 17:06 otsucfgmng/configuration_manager.py
+-rw-rw-rw-  2.0 fat     2055 b- defN 24-Jun-01 15:58 otsucfgmng/funcs.py
+-rw-rw-rw-  2.0 fat     3790 b- defN 24-Jun-01 17:06 otsucfgmng/protocol.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-Jun-01 17:11 otsucfgmng-1.4.0.311.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    25108 b- defN 24-Jun-01 17:11 otsucfgmng-1.4.0.311.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 17:11 otsucfgmng-1.4.0.311.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Jun-01 17:11 otsucfgmng-1.4.0.311.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      752 b- defN 24-Jun-01 17:11 otsucfgmng-1.4.0.311.dist-info/RECORD
+9 files, 43592 bytes uncompressed, 13525 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: otsucfgmng/configuration_manager.py
 Comment: 
 
 Filename: otsucfgmng/funcs.py
 Comment: 
 
-Filename: otsucfgmng-1.3.5.311.dist-info/LICENSE.txt
+Filename: otsucfgmng/protocol.py
 Comment: 
 
-Filename: otsucfgmng-1.3.5.311.dist-info/METADATA
+Filename: otsucfgmng-1.4.0.311.dist-info/LICENSE.txt
 Comment: 
 
-Filename: otsucfgmng-1.3.5.311.dist-info/WHEEL
+Filename: otsucfgmng-1.4.0.311.dist-info/METADATA
 Comment: 
 
-Filename: otsucfgmng-1.3.5.311.dist-info/top_level.txt
+Filename: otsucfgmng-1.4.0.311.dist-info/WHEEL
 Comment: 
 
-Filename: otsucfgmng-1.3.5.311.dist-info/RECORD
+Filename: otsucfgmng-1.4.0.311.dist-info/top_level.txt
+Comment: 
+
+Filename: otsucfgmng-1.4.0.311.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otsucfgmng/__init__.py

```diff
@@ -1,11 +1,13 @@
 """設定ファイルの生成、管理を補助するライブラリ。
 """
 
 __all__ = (
     "BaseCM",
+    "PBaseCM",
     "get_dict_keys_places",
     "support_json_dump",
 )
 
 from .configuration_manager import BaseCM
 from .funcs import get_dict_keys_places, support_json_dump
+from .protocol import PBaseCM
```

## otsucfgmng/configuration_manager.py

```diff
@@ -108,15 +108,15 @@
                     raise AttributeError(msg)
             else:
                 msg = f'"{n}"属性が存在しないため、その初期値を表す"{name}"属性も存在しません。'
                 raise AttributeError(msg)
         super().__setattr__(name, value)
 
     @property
-    def attributes_cm(self) -> set:
+    def attributes_cm(self) -> set[str]:
         """クラス定義の属性名セット。"""
         return copy.deepcopy(self.__attr_keys__)
 
     @property
     def key_place_cm(self) -> dict[str, list[str] | None]:
         """各属性の保存先を記録する辞書。"""
         return copy.deepcopy(self.__key_place__)
```

## Comparing `otsucfgmng-1.3.5.311.dist-info/LICENSE.txt` & `otsucfgmng-1.4.0.311.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `otsucfgmng-1.3.5.311.dist-info/METADATA` & `otsucfgmng-1.4.0.311.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otsucfgmng
-Version: 1.3.5.311
+Version: 1.4.0.311
 Summary: 設定ファイルを扱うクラスを生成するライブラリです。
 Home-page: https://github.com/Otsuhachi/OtsuConfigurationManager.git
 Author: Otsuhachi
 Author-email: agequodagis.tufuiegoeris@gmail.com
 License: MIT License
         
         Copyright (c) 2021 Otsuhachi
@@ -35,26 +35,27 @@
 Requires-Dist: otsutil
 
 - [概要](#概要)
   - [インストール](#インストール)
   - [使い方](#使い方)
   - [メソッド一覧](#メソッド一覧)
   - [Q\&A](#qa)
+  - [プロトコル](#プロトコル)
 
 
 # 概要
 
 このライブラリはjson形式の設定ファイルの読み書きを補助するための基底クラスです。  
 `BaseCM`クラスを継承し、`__defaults__`, `<attributes>`を定義するだけで必要な操作を行えるようになります。  
 
 ~~現在~~違うセクションに同じキーを持つような設定ファイルには対応していません。  
 **対応しないことに決定しました。**([理由はこちら](#なぜ異なるセクションで同名キーを持てないようにしましたか？))  
 
 このライブラリは以下の環境で作成されています。
-`Windows10(64bit)`, `Python3.11.1`
+`Windows10(64bit)`, `Python3.11.4`
 
 ```python
 # 違うセクションに同じキーを持つ例
 {
     'app': {'name': 'Hello'},
     'default': {'name': 'Python'}
 }
@@ -611,7 +612,190 @@
 ---------------------------------------------------------------------------
 manager
 None
 ---------------------------------------------------------------------------
 chief
 None
 ```
+
+## プロトコル
+
+コーディングの最中、docstringが欲しくなった時の場合のために`otsucfgmng.protocol.PBaseCM`(以後、`PBaseCM`)があります。  
+
+<!-- omit in toc -->
+### 使い方-プロトコル
+[ここ](#作成-設定ファイル管理クラス)で定義した`ConfigurationManager`クラスのプロトコルを作成して利用する例を示します。  
+
+設定ファイルのパスは一度決めてしまえば不変である可能性が高いので、引数無しで`ConfigurationManager`インスタンスを生成して返す関数を作成します。
+
+
+1. `ConfigurationManager`と`PBaseCM`, `型ヒントに使用するクラス`をインポートする。
+1. `PBaseCM`を継承した`PConfigurationManager`クラスを定義する。
+   1. プロパティとして各属性を定義していく。
+   1. 必要であれば、常に各属性の初期値を返す`default_<attribute>_cm`も同様に定義していく。
+   1. コーディング中の警告が気になるなら`2.i`で定義したプロパティのセッターも定義しておく。
+1. インスタンス生成用関数を定義する。
+   1. `PConfigurationManager`を返り値の型として指定する。
+   1. `ConfigurationManager`インスタンスを生成し、返す。
+   1. 厳密には対応していないと警告されるので、気になるなら`# type: ignore`で無視するようにする。
+
+```python
+
+# 1.
+from pathlib import Path
+from typing import Any
+
+from otsucfgmng import PBaseCM
+from test2 import ConfigurationManager
+
+
+# 2.
+class PConfigurationManager(PBaseCM):
+    # 2.1
+    @property
+    def library(self) -> Path:
+        """外部ライブラリのパス。"""
+        ...
+
+    @property
+    def scripts(self) -> Path:
+        """外部スクリプトのパス。"""
+        ...
+
+    @property
+    def title(self) -> str:
+        """アプリケーションのタイトル。"""
+        ...
+
+    @property
+    def fullscreen(self) -> bool:
+        """フルスクリーンで起動するか。"""
+        ...
+
+    @property
+    def bgm(self) -> int:
+        """BGM音量。"""
+        ...
+
+    @property
+    def bgs(self) -> int:
+        """BGS音量。"""
+        ...
+
+    @property
+    def se(self) -> int:
+        """SE音量。"""
+        ...
+
+    @property
+    def me(self) -> int:
+        """ME音量。"""
+        ...
+
+    # 2.2
+    @property
+    def default_library_cm(self) -> Path:
+        """外部ライブラリのパス。"""
+        ...
+
+    @property
+    def default_scripts_cm(self) -> Path:
+        """外部スクリプトのパス。"""
+        ...
+
+    @property
+    def default_title_cm(self) -> str:
+        """アプリケーションのタイトル。"""
+        ...
+
+    @property
+    def default_fullscreen_cm(self) -> bool:
+        """フルスクリーンで起動するか。"""
+        ...
+
+    @property
+    def default_bgm_cm(self) -> int:
+        """BGM音量。"""
+        ...
+
+    @property
+    def default_bgs_cm(self) -> int:
+        """BGS音量。"""
+        ...
+
+    @property
+    def default_se_cm(self) -> int:
+        """SE音量。"""
+        ...
+
+    @property
+    def default_me_cm(self) -> int:
+        """ME音量。"""
+        ...
+
+    # 2.3
+    @library.setter
+    def library(self, value: Any) -> None: ...
+
+    @scripts.setter
+    def scripts(self, value: Any) -> None: ...
+
+    @title.setter
+    def title(self, value: Any) -> None: ...
+
+    @fullscreen.setter
+    def fullscreen(self, value: Any) -> None: ...
+
+    @bgm.setter
+    def bgm(self, value: Any) -> None: ...
+
+    @bgs.setter
+    def bgs(self, value: Any) -> None: ...
+
+    @se.setter
+    def se(self, value: Any) -> None: ...
+
+    @me.setter
+    def me(self, value: Any) -> None: ...
+
+
+# 3.
+def CfgMng() -> PConfigurationManager:  # 3.1
+    # 3.2, 3.3
+    return ConfigurationManager("cfg.json", True)  # type: ignore
+
+
+with CfgMng() as cm:
+    # "cm."まで入力した時点で、各属性のdocstring付き候補が表示されるようになる。
+    cm.bgm = 10  # 2.iを省略すると警告される。
+    print(cm.cfg_to_str_cm(True))
+
+```
+
+出力
+```json
+
+### 出力は以下のようになります ###
+{
+    "defaults": {
+        "app": {
+            "fullscreen": false,
+            "library": "SampleLibrary.dll",
+            "scripts": "SampleScripts.scrpt",
+            "title": "Sample Program"
+        },
+        "audio": {
+            "bgm": 100,
+            "bgs": 100,
+            "me": 85,
+            "se": 100
+        }
+    },
+    "user": {
+        "app": {},
+        "audio": {
+            "bgm": 10
+        }
+    }
+}
+
+```
```

## Comparing `otsucfgmng-1.3.5.311.dist-info/RECORD` & `otsucfgmng-1.4.0.311.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-otsucfgmng/__init__.py,sha256=xy_Ld_mn8B4qr5MYKy0vZf2tElAtn4roZ5RV2oPB18Y,272
-otsucfgmng/configuration_manager.py,sha256=NZf2Sb9_dGnMEoDcTw4-ENxXZPQ9apBsEWliddWxevE,10373
+otsucfgmng/__init__.py,sha256=wtUpRTNy5yEf1al_2pmmRGdVwBSSaJnw_EVWI2YC8Hc,319
+otsucfgmng/configuration_manager.py,sha256=rSlFTiv7HRPnArHrpeIGXlc7jYupuGCiapgmS9wjgys,10378
 otsucfgmng/funcs.py,sha256=dNY1GATo_NTskoPp-PyuveKB0968WKES0D0TMwYGn10,2055
-otsucfgmng-1.3.5.311.dist-info/LICENSE.txt,sha256=XeWySNtE4_U7F-7QZKewFrVrDFEknE9jIi_JAaiNoMI,1087
-otsucfgmng-1.3.5.311.dist-info/METADATA,sha256=-ZkgP2WmKpwDjU0EwwzpICNdAzNwUwiFw5Z4ZUvadBI,20264
-otsucfgmng-1.3.5.311.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-otsucfgmng-1.3.5.311.dist-info/top_level.txt,sha256=WbA_UQ2H_eHmEOv1a3F6NoCx_2Gmp9h9BO3UQTWXQuU,11
-otsucfgmng-1.3.5.311.dist-info/RECORD,,
+otsucfgmng/protocol.py,sha256=jJvwCo4qxqQvYUCQ0B2yob_LUm6osPJi07Qtzz-f_xI,3790
+otsucfgmng-1.4.0.311.dist-info/LICENSE.txt,sha256=XeWySNtE4_U7F-7QZKewFrVrDFEknE9jIi_JAaiNoMI,1087
+otsucfgmng-1.4.0.311.dist-info/METADATA,sha256=KufcSPtzQ5NRC7j2T95ISVqegpnNdr-ptUp60lDC0PA,25108
+otsucfgmng-1.4.0.311.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+otsucfgmng-1.4.0.311.dist-info/top_level.txt,sha256=WbA_UQ2H_eHmEOv1a3F6NoCx_2Gmp9h9BO3UQTWXQuU,11
+otsucfgmng-1.4.0.311.dist-info/RECORD,,
```

