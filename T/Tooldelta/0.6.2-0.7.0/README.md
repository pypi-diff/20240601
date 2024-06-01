# Comparing `tmp/tooldelta-0.6.2.tar.gz` & `tmp/tooldelta-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.6.2.tar", max compression
+gzip compressed data, was "tooldelta-0.7.0.tar", max compression
```

## Comparing `tooldelta-0.6.2.tar` & `tooldelta-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-05-30 11:53:36.472284 tooldelta-0.6.2/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-05-30 11:53:36.472284 tooldelta-0.6.2/README.md
--rw-r--r--   0        0        0      908 2024-05-30 11:53:45.568294 tooldelta-0.6.2/pyproject.toml
--rwxr-xr-x   0        0        0      618 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/auths.py
--rwxr-xr-x   0        0        0    12372 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10441 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/color_print.py
--rw-r--r--   0        0        0     1885 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/constants.py
--rwxr-xr-x   0        0        0    35083 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/frame.py
--rwxr-xr-x   0        0        0    13369 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    23814 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1832 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/logger.py
--rw-r--r--   0        0        0    29752 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1295 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15701 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     9073 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0    10499 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     6318 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/movent.py
--rw-r--r--   0        0        0     7025 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/utils.py
--rwxr-xr-x   0        0        0    17005 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16754 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1996 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/starter.py
--rwxr-xr-x   0        0        0     1110 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0    10039 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/urlmethod.py
--rw-r--r--   0        0        0    20711 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/utils.py
--rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-06-01 21:51:42.622132 tooldelta-0.7.0/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-06-01 21:51:42.622132 tooldelta-0.7.0/README.md
+-rw-r--r--   0        0        0      908 2024-06-01 21:51:51.138192 tooldelta-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0      658 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12563 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10441 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    35071 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13369 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23814 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    16729 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3504 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     9072 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0    10499 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7032 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17204 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16997 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1932 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0    10074 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20711 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/utils.py
+-rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.7.0/PKG-INFO
```

### Comparing `tooldelta-0.6.2/LICENSE` & `tooldelta-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/README.md` & `tooldelta-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/pyproject.toml` & `tooldelta-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.6.2" # This field is automatically set to the value in the version file
+version = "0.7.0" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.6.2/tooldelta/__init__.py` & `tooldelta-0.7.0/tooldelta/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,13 @@
     from tooldelta import start_tool_delta\n
     start_tool_delta()
 """
 from .color_print import Print
 from .plugin_load.PluginGroup import Plugin
 from .starter import plugin_group as plugins
 from .starter import start_tool_delta, safe_jump
+from .starter import frame as tooldelta
 from .frame import Config, Utils, Frame, GameCtrl
 from .launch_options import client_title
 
 # 重定向 Builtins
 Builtins = Utils
```

### Comparing `tooldelta-0.6.2/tooldelta/auths.py` & `tooldelta-0.7.0/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/cfg.py` & `tooldelta-0.7.0/tooldelta/cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,110 @@
 """配置文件模块"""
 
 import os
-from typing import Any
+from typing import Any, Union
 import ujson
 
 NoneType = type(None)
 
 PLUGINCFG_DEFAULT = {"配置版本": "0.0.1", "配置项": None}
-
 PLUGINCFG_STANDARD_TYPE = {"配置版本": str, "配置项": [type(None), dict]}
 
+def cfg_isinstance_single(obj, typ: type) -> bool:
+    if not isinstance(typ, type):
+        raise TypeError(f"cfg_isinstance arg 1 must be a type, not {typ}")
+    return {
+        Cfg.PInt: lambda: isinstance(obj, int) and obj > 0,
+        Cfg.NNInt: lambda: isinstance(obj, int) and obj >= 0,
+        Cfg.PFloat: lambda: isinstance(obj, float) and obj > 0,
+        Cfg.NNFloat: lambda: (isinstance(obj, float) or obj == 0) and obj >= 0,
+        Cfg.PNumber: lambda: isinstance(obj, (int, float)) and obj > 0,
+        Cfg.NNNumber: lambda: isinstance(obj, (int, float)) and obj >= 0,
+        int: lambda: obj not in (True, False) and isinstance(obj, int)
+    }.get(typ, lambda: isinstance(obj, typ))()
+
+def cfg_isinstance(obj: Any, typ: type | tuple[type]):
+    """
+    专用于Cfg的类型检测
+
+    Args:
+        obj (Any): 待检测对象
+        typ (Any | tuple[Any]): 类型或类型元组
 
-def _CfgIsinstance(obj, typ):
-    # 专用于Cfg的类型检测
+    Returns:
+        bool: 是否为对应类型
+    """
     if isinstance(typ, type):
-        return {
-            Cfg.PInt: lambda: isinstance(obj, int) and obj > 0,
-            Cfg.NNInt: lambda: isinstance(obj, int) and obj >= 0,
-            Cfg.PFloat: lambda: isinstance(obj, float) and obj > 0,
-            Cfg.NNFloat: lambda: (isinstance(obj, float) or obj == 0) and obj >= 0,
-            Cfg.PNumber: lambda: isinstance(obj, (int, float)) and obj > 0,
-            Cfg.NNNumber: lambda: isinstance(obj, (int, float)) and obj >= 0,
-        }.get(typ, lambda: isinstance(obj, typ))()
-    if isinstance(typ, tuple):
+        return cfg_isinstance_single(obj, typ)
+    elif isinstance(typ, tuple):
         try:
             for i in typ:
-                result = {
-                    Cfg.PInt: lambda: isinstance(obj, int) and obj > 0,
-                    Cfg.NNInt: lambda: isinstance(obj, int) and obj >= 0,
-                    Cfg.PFloat: lambda: isinstance(obj, float) and obj > 0,
-                    Cfg.NNFloat: lambda: (isinstance(obj, float) or obj == 0)
-                    and obj >= 0,
-                    Cfg.PNumber: lambda: isinstance(obj, (int, float)) and obj > 0,
-                    Cfg.NNNumber: lambda: isinstance(obj, (int, float)) and obj >= 0,
-                }.get(i, lambda: isinstance(obj, typ))()
-                if result:
+                if cfg_isinstance_single(obj, i):
                     return True
             return False
         except TypeError as e:
-            raise ValueError(f"Can't be: {typ}") from e
-    raise ValueError(f"Can't be: {typ}")
+            raise ValueError(f"cfg_isinstance arg 2 can't be: {typ}") from e
+    else:
+        raise ValueError(f"cfg_isinstance arg 2 can't be: {typ}")
 
 
 def _CfgShowType(typ: Any) -> str:
     """转换类型为中文字符串
 
     Args:
         typ (Any): 类型
 
     Returns:
         str: 中文字符串
     """
-    if isinstance(typ, type):
+    if not isinstance(typ, type):
         typ = type(typ)
     return {
         Cfg.PInt: "正整数",
         Cfg.NNInt: "非负整数",
         Cfg.PFloat: "正浮点小数",
         Cfg.NNFloat: "非负浮点小数",
         str: "字符串",
         float: "浮点小数",
         int: "整数",
         dict: "json对象",
         list: "列表",
+        bool: "true/false",
         NoneType: "null",
     }.get(typ, typ.__name__)
 
-
-FIND_NONE = r"%FindNone"
-
-
 class Cfg:
     """配置文件模块"""
-    class Group:
-        """配置文件的键组合, 用于检测多个键中的一个是否存在"""
-
-        def __init__(self, *keys):
-            self.members = keys
-
-        def __repr__(self) -> str:
-            return 'Cfg.Group("' + '", "'.join(self.members) + '")'
-
     class ConfigError(Exception):
         "配置文件错误"
 
         def __init__(self, errStr: str, errPos: list | None = None):
             if errPos is None:
                 errPos = []
             self.errPos = errPos
             self.args = (errStr,)
 
-    class UnneccessaryKey:
-        "配置文件的多余键"
+    class UnneccessaryKV:
+        "配置文件的不必要的键"
 
-        def __init__(self, key):
+        def __init__(self, key: str, val_type):
             self.key = key
+            self.type = val_type
 
-        def __repr__(self):
-            return f"Cfg.UnneccessaryKey({self.key})"
+    class JsonList:
+        "配置文件的列表类型"
+
+        def __init__(self, patt: type | dict | tuple[type | dict, ...], len_limit = -1):
+            self.patt = patt
+            self.len_limit = len_limit
+
+    class AnyKeyValue:
+        "配置文件的任意键名键值对类型"
+        def __init__(self, val_type: type | tuple[type]):
+            self.type = val_type
 
     class ConfigKeyError(ConfigError):
         "配置json的键错误"
 
     class ConfigValueError(ConfigError):
         "配置json的值错误"
 
@@ -122,24 +125,27 @@
 
     class PNumber:
         "配置文件的值限制: 正数"
 
     class NNNumber:
         "配置文件的值限制: 大于0的数"
 
+    class FindNone:
+        "找不到值"
+
     def get_cfg(self, path: str, standard_type: dict):
         "从path路径获取json文件文本信息, 并按照standard_type给出的标准形式进行检测."
         path = path if path.endswith(".json") else path + ".json"
         with open(path, "r", encoding="utf-8") as f:
             try:
                 obj = ujson.load(f)
             except ujson.JSONDecodeError as exc:
                 raise self.ConfigValueError(
                     "JSON配置文件格式不正确, 请修正或直接删除", None) from exc
-        self.check_dict_2(standard_type, obj)
+        self.check_dict(standard_type, obj)
         return obj
 
     @staticmethod
     def default_cfg(path: str, default: dict, force: bool = False) -> None:
         """生成默认配置文件
 
         Args:
@@ -160,21 +166,21 @@
             path (str): 路径
 
         Returns:
             bool: 是否存在
         """
         return os.path.isfile(path if path.endswith(".json") else path + ".json")
 
-    def getPluginConfigAndVersion(
+    def get_plugin_config_and_version(
         self,
         pluginName: str,
-        standardType: dict,
+        standardType: Any,
         default: dict,
         default_vers: tuple[int, int, int] | list,
-    ) -> tuple[dict[str, Any], tuple[int, ...]]:
+    ) -> tuple[dict[str, Any], tuple[int, int, int]]:
         """获取插件配置文件及版本
 
         Args:
             pluginName (str): 插件名
             standardType (dict): 标准类型
             default (dict): 默认配置
             default_vers (tuple[int, int, int]): 默认版本
@@ -191,128 +197,125 @@
             defaultCfg["配置版本"] = ".".join([str(n) for n in default_vers])
             self.check_auto(standardType, default)
             self.default_cfg(p + ".json", defaultCfg, force=True)
         cfg_stdtyp = PLUGINCFG_STANDARD_TYPE.copy()
         cfg_stdtyp["配置项"] = standardType
         cfgGet = self.get_cfg(p, cfg_stdtyp)
         cfgVers = tuple(int(c) for c in cfgGet["配置版本"].split("."))
+        if len(cfgVers) != 3:
+            raise ValueError("配置文件出错: 版本出错")
         return cfgGet["配置项"], cfgVers
 
-    def check_auto(self, standard: type | dict | list, val: Any, fromkey: Any = "?") -> None:
-        """检查配置文件
+    getPluginConfigAndVersion = get_plugin_config_and_version
+
+    def check_auto(self, standard: type | dict | JsonList | tuple[type | dict, ...], val: Any, fromkey: str = "?"):
+        """检查配置文件(自动类型判断)
 
         Args:
             standard (type, dict, list): 标准
             val (Any): 值
             fromkey (Any, optional): 键
 
         Raises:
-            ValueError: 未知类型
-            self.ConfigValueError: 值错误
-            ValueError: 未知类型
+            ValueError: 未知标准检测类型
+            ConfigValueError: 值错误
         """
 
-        if fromkey == FIND_NONE:
+        if fromkey == Cfg.FindNone:
             raise ValueError("不允许传入FindNone")
         if isinstance(standard, type):
-            if not _CfgIsinstance(val, standard):
-                raise self.ConfigValueError(
-                    f'JSON键"{fromkey}" 对应值的类型不正确: 需要 {_CfgShowType(standard)}, 实际上为 {_CfgShowType(val)}'
-                )
-        elif isinstance(standard, list):
-            # [%list] or [multi[type/dict]]
-            self.check_list_2(standard, val)
-        elif isinstance(standard, dict):
-            self.check_dict_2(standard, val)
+            if not cfg_isinstance(val, standard):
+                if isinstance(val, dict):
+                    raise self.ConfigValueError(
+                        f'JSON键"{fromkey}" 对应值的类型不正确: 需要 {_CfgShowType(standard)}, 实际上为 json对象: {ujson.dumps(val, ensure_ascii=False)}'
+                    )
+                else:
+                    raise self.ConfigValueError(
+                        f'JSON键"{fromkey}" 对应值的类型不正确: 需要 {_CfgShowType(standard)}, 实际上为 {_CfgShowType(val)}'
+                    )
+        elif isinstance(standard, Cfg.JsonList):
+            self.check_list(standard, val, fromkey)
+        elif isinstance(standard, tuple):
+            errs = []
+            for single_type in standard:
+                try:
+                    self.check_auto(single_type, val, fromkey)
+                    break
+                except Exception as err:
+                    errs.append(err)
+            else:
+                reason = "\n".join(str(err) for err in errs)
+                raise self.ConfigValueError(f'JSON键 对应的键"{fromkey}" 类型不正确, 以下为可能的原因: \n{reason}')
+        elif isinstance(standard, (dict, Cfg.AnyKeyValue, Cfg.UnneccessaryKV)):
+            self.check_dict(standard, val, fromkey)
         else:
             raise ValueError(
-                f'JSON键 "{fromkey}"未曾遇到过的类型: {standard.__class__.__name__}, 另外两个参数 standard={standard}, val={val}'
+                f'JSON键 "{fromkey}" 自动检测的标准类型传入异常: {standard.__class__.__name__}'
             )
 
-    def check_dict_2(self, pattern: dict, jsondict: dict):
+    def check_dict(self, pattern: dict | AnyKeyValue | UnneccessaryKV, jsondict: Any, from_key = "?"):
         """
         按照给定的标准配置样式比对传入的配置文件jsondict, 对不上则引发相应异常
 
         参数:
             pattern: 标准样式dict
             jsondict: 待检测的配置文件dict
         """
-        for key, std_val in pattern.items():
-            if key == r"%any":
-                # ANY key
-                for js_key, js_val in jsondict.items():
-                    self.check_auto(std_val, js_val, js_key)
-            elif isinstance(key, self.Group):
-                # any key in members?
-                js_val = FIND_NONE
-                for member_key in key.members:
-                    val_get = jsondict.get(member_key, FIND_NONE)
-                    if val_get != FIND_NONE:
-                        self.check_auto(std_val, val_get, member_key)
-            elif isinstance(key, self.UnneccessaryKey):
-                val_get = jsondict.get(key.key, FIND_NONE)
-                if val_get != FIND_NONE:
-                    self.check_auto(std_val, val_get, key.key)
-            else:
-                val_get = jsondict.get(key, FIND_NONE)
-                if val_get == FIND_NONE:
+        if not isinstance(jsondict, dict):
+            raise ValueError(f'json键"{from_key}" 需要json对象, 而不是 {_CfgShowType(jsondict)}')
+        if isinstance(pattern, Cfg.AnyKeyValue):
+            for key, val in jsondict.items():
+                self.check_auto(pattern.type, val, key)
+        elif isinstance(pattern, Cfg.UnneccessaryKV):
+            val_get = jsondict.get(pattern.key, Cfg.FindNone)
+            if val_get != Cfg.FindNone:
+                self.check_auto(pattern.type, val_get, pattern.key)
+        else:
+            for key, std_val in pattern.items():
+                val_get = jsondict.get(key, Cfg.FindNone)
+                if val_get == Cfg.FindNone:
                     raise self.ConfigKeyError(f"不存在的JSON键: {key}")
                 self.check_auto(std_val, val_get, key)
 
-    def check_list_2(self, pattern: list, value: Any, fromkey: Any = "?") -> None:
+    def check_list(self, pattern: JsonList, value: Any, fromkey: Any = "?") -> None:
         """检查列表
 
         Args:
             pattern (list): 标准
             value (Any): 值
             fromkey (Any, optional): 键
 
         Raises:
             ValueError: 不是合法的标准列表检测样式
             ValueError: 标准检测列表的长度不能为0
-            self.ConfigValueError: json键值错误
+            ConfigValueError: json键值错误
         """
-        if not isinstance(pattern, list):
+        if not isinstance(pattern, Cfg.JsonList):
             raise ValueError("不是合法的标准列表检测样式")
-        if len(pattern) == 0:
-            raise ValueError("标准检测列表的长度不能为0")
-        if isinstance(pattern[0], str) and pattern[0].startswith(r"%list"):
-            if not isinstance(value, list):
-                raise self.ConfigValueError(
-                    f'JSON键 "{fromkey}" 需要列表 而不是 {_CfgShowType(value)}'
-                )
-            limitNumber = 0
-            if pattern[0].replace(r"%list", "").isnumeric():
-                limitNumber = int(pattern[0].replace(r"%list", ""))
-            if limitNumber and len(value) != limitNumber:
-                raise self.ConfigValueError(
-                    f'JSON键 "{fromkey}" 所对应的值列表有误: 需要 {limitNumber} 项, 实际上为 {len(value)} 项'
-                )
-            for val in value:
-                self.check_auto(pattern[1], val, fromkey)
-        else:
-            for single_type in pattern:
-                try:
-                    self.check_auto(single_type, value, fromkey)
-                    return
-                except Exception:
-                    pass
+        if not isinstance(value, list):
             raise self.ConfigValueError(
-                f"JSON列表的值 \"{fromkey}\" 类型不正确: 需要 {' 或 '.join(_CfgShowType(i) for i in pattern)}, 实际上为 {_CfgShowType(value)}"
+                f'JSON键 "{fromkey}" 需要列表 而不是 {_CfgShowType(value)}'
             )
+        if pattern.len_limit != -1:
+            if len(value) != pattern.len_limit:
+                raise self.ConfigValueError(
+                    f'JSON键 "{fromkey}" 所对应的值列表有误: 需要 {pattern.len_limit} 项, 实际上为 {len(value)} 项'
+                )
+        for val in value:
+            self.check_auto(pattern.patt, val, fromkey)
 
     def auto_to_std(self, cfg):
         """
         自动以默认配置文件生成标准配置文件格式.
         注意: 不支持固定长度列表以及Cfg.NeccessaryKey与Cfg.Group的自动转换
 
-        参数:
+        Args:
             cfg: 默认的CFG配置文件
-        返回:
-            标准cfg样式, 用于 checkDict
+        Returns:
+            标准cfg样式, 用于 check_dict
         """
         if isinstance(cfg, dict):
             res = {}
             for k, v in cfg.items():
                 if isinstance(v, (dict, list)):
                     res[k] = self.auto_to_std(v)
                 elif isinstance(v, (str, int, float, bool)):
@@ -324,26 +327,24 @@
                 if isinstance(v, (dict, list)):
                     t = self.auto_to_std(v)
                 else:
                     t = type(v)
                 if t not in setting_types:
                     setting_types.append(t)
             if len(setting_types) == 1:
-                return [r"%list", setting_types[0]]
-            return [r"%list", setting_types]
+                return Cfg.JsonList(setting_types[0])
+            return Cfg.JsonList(tuple(setting_types))
         raise ValueError("auto_to_std() 仅接受 dict 与 list 参数")
 
-    checkDict = check_dict_2
+    checkDict = check_dict
 
+Config = Cfg()
 
 if __name__ == "__main__":
     # Test Part
     try:
-        test_cfg = [{"b": 1}]
-        a = [1, 2, 3, {"b": True}]
-        std = Cfg().auto_to_std(a)
-        print(std)
-        Cfg().check_auto(std, test_cfg)
+        test_cfg = {"key1": {"b": 2}, "key2": [{"key3": "6"}, 7]}
+        std = {"key1": Cfg.UnneccessaryKV("b", int), "key2": Cfg.JsonList(({"key3": str}, int))}
+        Config.check_auto(std, test_cfg)
     except Cfg.ConfigError:
         import traceback
-
         print(traceback.format_exc())
```

### Comparing `tooldelta-0.6.2/tooldelta/color_print.py` & `tooldelta-0.7.0/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/constants.py` & `tooldelta-0.7.0/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/frame.py` & `tooldelta-0.7.0/tooldelta/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,30 +24,29 @@
     plugin_market,
 )
 from .constants import PRG_NAME
 from .utils import Utils, safe_close
 from .plugin_load.injected_plugin import safe_jump
 from .get_tool_delta_version import get_tool_delta_version
 from .color_print import Print
-from .cfg import Cfg
+from .cfg import Config
 from .logger import publicLogger
 from .game_texts import GameTextsLoader, GameTextsHandle
 from .urlmethod import if_token, fbtokenFix
 from .sys_args import sys_args_to_dict
 from .launch_cli import (
     FrameNeOmg,
     FrameNeOmgRemote,
     SysStatus,
 )
 
 from .packets import PacketIDS
 
 sys_args_dict = sys_args_to_dict(sys.argv)
 VERSION = get_tool_delta_version()
-Config = Cfg()
 
 if TYPE_CHECKING:
     from .plugin_load.PluginGroup import PluginGroup
 
 LAUNCHERS: list[
     tuple[str, type[FrameNeOmg | FrameNeOmgRemote]]
 ] = [
```

### Comparing `tooldelta-0.6.2/tooldelta/game_texts.py` & `tooldelta-0.7.0/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/launch_cli.py` & `tooldelta-0.7.0/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/launch_options.py` & `tooldelta-0.7.0/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/logger.py` & `tooldelta-0.7.0/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/neo_conn.py` & `tooldelta-0.7.0/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/packets.py` & `tooldelta-0.7.0/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.7.0/tooldelta/plugin_load/PluginGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import traceback
 from typing import TYPE_CHECKING, Any, Callable, Union, TypeVar
 
 from ..color_print import Print
 from .classic_plugin import (
     Plugin,
     add_plugin,
-    add_plugin_as_api
+    add_plugin_as_api,
+    _init_frame,
+    _PLUGIN_CLS_TYPE
 )
 from ..utils import Utils
 from .injected_plugin import (
     execute_init,
     execute_player_prejoin,
     execute_player_join,
     execute_player_message,
@@ -29,15 +31,15 @@
     PluginAPIVersionError,
 )
 from ..constants import PRG_NAME
 from .utils import set_frame as _set_frame
 from .injected_plugin.movent import set_frame as _set_frame_inj
 
 if TYPE_CHECKING:
-    from ..frame import Frame, GameCtrl
+    from ..frame import Frame
 
 _TV = TypeVar("_TV")
 _SUPER_CLS = TypeVar("_SUPER_CLS")
 
 class PluginGroup:
     "插件组"
     plugins: list[Plugin] = []
@@ -67,14 +69,43 @@
         self.loaded_plugins_name = []
         self.linked_frame: Union["Frame" , None] = None
 
     add_plugin = staticmethod(add_plugin)
 
     add_plugin_as_api = staticmethod(add_plugin_as_api)
 
+    def instant_plugin_api(self, api_cls: type[_PLUGIN_CLS_TYPE]) -> _PLUGIN_CLS_TYPE:
+        """
+        对外源导入 (import) 的API插件类进行类型实例化。
+        可以使得你所使用的 IDE 对导入的插件API类进行识别和高亮其所含方法。
+
+        Args:
+            api_cls (type[_PLUGIN_CLS_TYPE]): 导入的API插件类
+
+        Raises:
+            ValueError: API插件类未被注册
+
+        Returns:
+            _PLUGIN_CLS_TYPE: API插件实例
+
+        使用方法如下:
+        ```
+            p_api = plugins.get_plugin_api("...")
+            from outer_api import api_cls_xx
+            p_api = plugins.instant_plugin_api(api_cls_xx)
+        ```
+        """
+        for v in self.plugins_api.values():
+            if isinstance(v, api_cls):
+                return v
+            else:
+                print(api_cls, v)
+        raise ValueError(f"无法找到API插件类 {api_cls.__name__}, 有可能是还没有注册")
+
+
     def add_packet_listener(self, pktID: int | list[int]):
         """
         添加数据包监听器
         将下面的方法作为一个MC数据包接收器
         Tips: 只能在插件主类里的函数使用此装饰器!
 
         Args:
@@ -199,14 +230,15 @@
             return None
 
     def set_frame(self, frame: "Frame") -> None:
         "设置关联的系统框架"
         self.linked_frame = frame
         _set_frame(frame)
         _set_frame_inj(frame)
+        _init_frame(frame)
 
     def read_all_plugins(self) -> None:
         """读取所有插件
 
         Raises:
             SystemExit: 读取插件出现问题
         """
```

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/__init__.py` & `tooldelta-0.7.0/tooldelta/plugin_load/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 "插件加载主模块"
 
+import os
 from typing import Any
-
+from tooldelta.constants import (
+    TOOLDELTA_CLASSIC_PLUGIN,
+    TOOLDELTA_INJECTED_PLUGIN,
+    TOOLDELTA_PLUGIN_DIR
+)
+TYPE_CHECKING = 0
 
 def NON_FUNC(*_) -> None:
     "空函数"
     return None
 
 
 class PluginSkip(EOFError):
@@ -61,14 +67,22 @@
         self.plugin_id = plugin_data.get("plugin-id", "???")
         self.is_registered = is_registered
         if plugin_data.get("enabled") is not None:
             self.is_enabled = plugin_data["enabled"]
         else:
             self.is_enabled = is_enabled
 
+    @property
+    def dir(self):
+        return os.path.join(
+            TOOLDELTA_PLUGIN_DIR,
+            {"classic": TOOLDELTA_CLASSIC_PLUGIN, "injected": TOOLDELTA_INJECTED_PLUGIN}[self.plugin_type],
+            self.name
+        )
+
     def dump(self) -> dict[str, Any]:
         "转储数据"
         return {
             "author": self.author,
             "version": ".".join([str(i) for i in self.version]),
             "plugin-type": self.plugin_type,
             "description": self.description,
```

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.7.0/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 "ToolDelta类式插件"
 import importlib
 import os
 import sys
 import traceback
 import zipfile
-from typing import TYPE_CHECKING, Union, Any, TypeVar
+from typing import TYPE_CHECKING, Union, TypeVar
 from ...color_print import Print
 from ...utils import Utils
 from ...cfg import Cfg
 from ...plugin_load import plugin_is_enabled, NotValidPluginError
 from ...constants import TOOLDELTA_CLASSIC_PLUGIN
 
 if TYPE_CHECKING:
     # 类型注释
     from ...frame import Frame
     from ...plugin_load.PluginGroup import PluginGroup
 
 __caches__ = {
     "plugin": None,
-    "api_name": ""
+    "api_name": "",
+    "frame": None
 }
 
 class Plugin:
     "插件信息主类"
     name: str = ""
     version = (0, 0, 1)
     author = "?"
@@ -59,15 +60,16 @@
     except TypeError as exc:
         raise NotValidPluginError(
             f"插件主类必须继承Plugin类 而不是 {plugin.__class__}") from exc
     if __caches__["plugin"] is not None:
         raise NotValidPluginError(
             "调用了多次 @add_plugin"
         )
-    __caches__["plugin"] = plugin
+    plugin_ins = plugin(__caches__["frame"]) # type: ignore
+    __caches__["plugin"] = plugin_ins
     return plugin
 
 def add_plugin_as_api(apiName: str):
     """添加ToolDelta类式插件主类, 同时作为API插件提供接口供其他插件进行使用
 
     Args:
         apiName (str): API名
@@ -75,15 +77,16 @@
     def _add_plugin_2_api(api_plugin: type[_PLUGIN_CLS_TYPE]) -> type[_PLUGIN_CLS_TYPE]:
         if not Plugin.__subclasscheck__(api_plugin):
             raise NotValidPluginError("API插件主类必须继承Plugin类")
         if __caches__["plugin"] is not None:
             raise NotValidPluginError(
                 "调用了多次 @add_plugin"
             )
-        __caches__["plugin"] = api_plugin
+        plugin_ins = api_plugin(__caches__["frame"]) # type: ignore
+        __caches__["plugin"] = plugin_ins
         __caches__["api_name"] = apiName
         return api_plugin
 
     return _add_plugin_2_api
 
 
 # Plugin get and execute
@@ -153,64 +156,61 @@
                 "插件文件", TOOLDELTA_CLASSIC_PLUGIN, plugin_dirname, "__init__.py"
             )
         ):
             importlib.import_module(plugin_dirname)
         else:
             Print.print_war(f"{plugin_dirname} 文件夹 未发现插件文件, 跳过加载")
             return
-        none = None # ...
-        if __caches__["plugin"] == none:
+        plugin_or_none : Plugin | None = __caches__.get("plugin")
+        if plugin_or_none is None:
             raise NotValidPluginError(
                 "需要调用1次 @plugins.add_plugin 以注册插件主类, 然而没有调用"
             )
-        plugin: type[Plugin] = __caches__["plugin"] # type: ignore
-        if plugin.name is None:
-            raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
-        plugin_ins = plugin(plugin_group.linked_frame)
-        if isinstance(plugin_ins, type(None)) or plugin_ins.name == "":
-            raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
-        plugin_group.plugins.append(plugin_ins)
-        _v0, _v1, _v2 = plugin_ins.version
+        plugin: Plugin = plugin_or_none
+        if plugin.name is None or plugin.name == "":
+            raise ValueError(f"插件主类 {plugin.__class__.__name__} 需要作者名")
+        plugin_group.plugins.append(plugin)
+        _v0, _v1, _v2 = plugin.version
         for evt_name in (
             "on_def",
             "on_inject",
             "on_player_prejoin",
             "on_player_join",
             "on_player_message",
             "on_player_death",
             "on_player_leave",
             "on_frame_exit"
         ):
-            if hasattr(plugin_ins, evt_name):
+            if hasattr(plugin, evt_name):
                 plugin_group.plugins_funcs[evt_name].append(
-                    [plugin_ins.name, getattr(plugin_ins, evt_name)]
+                    [plugin.name, getattr(plugin, evt_name)]
                 )
         Print.print_suc(
-            f"成功载入插件 {plugin_ins.name} 版本: {_v0}.{_v1}.{_v2} 作者：{plugin_ins.author}"
+            f"成功载入插件 {plugin.name} 版本: {_v0}.{_v1}.{_v2} 作者：{plugin.author}"
         )
         plugin_group.normal_plugin_loaded_num += 1
         if plugin_group.plugin_added_cache["packets"] != []:
             for pktType, func in plugin_group.plugin_added_cache["packets"]:
-                ins_func = getattr(plugin_ins, func.__name__)
+                ins_func = getattr(plugin, func.__name__)
                 if ins_func is None:
                     raise NotValidPluginError("数据包监听不能在主插件类以外定义")
                 plugin_group._add_listen_packet_id(pktType)
                 plugin_group._add_listen_packet_func(
                     pktType, ins_func
                 )
         if __caches__["api_name"] != "":
-            plugin_group.plugins_api[__caches__["api_name"]] = plugin_ins
+            plugin_group.plugins_api[__caches__["api_name"]] = plugin
         if plugin_group.broadcast_evts_cache != {}:
             for evt, funcs in plugin_group.broadcast_evts_cache.items():
                 for func in funcs:
-                    ins_func = getattr(plugin_ins, func.__name__)
+                    ins_func = getattr(plugin, func.__name__)
                     if ins_func is None:
                         raise NotValidPluginError("广播事件监听不能在主插件类以外定义")
                     plugin_group._add_broadcast_evt(evt, ins_func)
-        return plugin_ins
+        return plugin
     except NotValidPluginError as err:
         Print.print_err(f"插件 {plugin_dirname} 不合法: {err.args[0]}")
         raise SystemExit from err
     except Cfg.ConfigError as err:
         Print.print_err(f"插件 {plugin_dirname} 配置文件报错：{err}")
         Print.print_err("你也可以直接删除配置文件, 重新启动ToolDelta以自动生成配置文件")
         raise SystemExit from err
@@ -232,8 +232,11 @@
         exp_dir (str): 解压目录
     """
     try:
         f = zipfile.ZipFile(zip_dir, "r")
         f.extractall(exp_dir)
     except Exception as err:
         Print.print_err(f"zipfile: 解压失败: {err}")
-        raise EOFError("解压失败") from err
+        raise EOFError("解压失败") from err
+
+def _init_frame(frame: "Frame"):
+    __caches__["frame"] = frame
```

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/plugin_load/utils.py` & `tooldelta-0.7.0/tooldelta/plugin_load/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         timeout (int): 最长超时时间
     返回:
         tuple[float, float, float]
     """
     res = getPos(player, timeout=timeout)["position"]
     return res["x"], res["y"], res["z"]
 
-def getScore(scoreboardNameToGet: str, targetNameToGet: str) -> int:
+def getScore(scoreboardNameToGet: str, targetNameToGet: str) -> int | dict:
     """
     获取计分板分数
     参数:
         scoreboardNameToGet: 计分板名
         targetNameToGet: 获取分数的对象/目标选择器
     返回:
         分数: int
```

### Comparing `tooldelta-0.6.2/tooldelta/plugin_manager.py` & `tooldelta-0.7.0/tooldelta/plugin_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         "插件管理界面"
         clear_screen()
         np = self.autoRegisterPlugins()
         if np > 0:
             Print.clean_print(f"§a已自动注册{np}个未被注册的插件.")
         while 1:
             plugins = self.list_plugins_list()
-            with Print.lock:Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
-            with Print.lock:Print.clean_print("§f输入§ds§f同步插件注册表信息(在手动安装插件后使用)")
-            with Print.lock:r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
+            Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
+            Print.clean_print("§f输入§ds§f同步插件注册表信息(在手动安装插件后使用)")
+            r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
             r1 = r.strip().lower()
             if r1 == "":
                 continue
             elif r1 == "s":
                 self.sync_plugin_datas_to_register()
                 Print.clean_print("§a同步插件注册表数据成功.")
                 time.sleep(2)
@@ -140,15 +140,15 @@
         self.push_plugin_reg_data(plugin)
         input()
 
     def update_all_plugins(self, plugins: list[PluginRegData]) -> None:
         """更新全部插件
 
         Args:
-            plugins (list[&quot;PluginRegData&quot;]): 插件注册信息列表
+            plugins (list[PluginRegData]): 插件注册信息列表
         """
         market_datas = market.get_datas_from_market()["MarketPlugins"]
         need_updates: list[tuple[PluginRegData, str]] = []
         for i in plugins:
             s_data = market_datas.get(i.plugin_id)
             if s_data is None:
                 continue
@@ -160,30 +160,45 @@
             for plugin, v in need_updates:
                 Print.clean_print(
                     f" - {plugin.name} §6{plugin.version_str}§f -> §a{v}")
             r = input(Print.clean_fmt(
                 "§f输入§a y §f开始更新, §c n §f取消: ")).strip().lower()
             if r == "y":
                 for plugin, v in need_updates:
-                    market.download_plugin(plugin)
+                    self.update_plugin_from_market(plugin)
                 Print.clean_print("§a全部插件已更新完成")
             else:
                 Print.clean_print("§6已取消插件更新.")
             input("[Enter键继续...]")
         else:
             input(Print.clean_fmt("§a无可更新的插件. [Enter键继续]"))
 
+    def update_plugin_from_market(self, plugin: PluginRegData):
+        """
+        更新单个插件, 并且删除旧目录
+
+        Args:
+            plugin (PluginRegData): 插件注册信息, 新旧皆可
+        """
+        _, old_plugins = self.get_plugin_reg_name_dict_and_datas()
+        new_plugin_datas = market.get_plugin_data_from_market(plugin.plugin_id)
+        new_plugins = market.download_plugin(new_plugin_datas, False)
+        for new_plugin in new_plugins:
+            for old_plugin in old_plugins:
+                if new_plugin.plugin_id == old_plugin.plugin_id and new_plugin.name != old_plugin.name:
+                    shutil.rmtree(old_plugin.dir)
+
     def search_plugin(self, resp, plugins) -> Optional[PluginRegData]:
         """搜索插件
 
         Returns:
             None: 未找到插件
             PluginRegData: 插件注册信息
         """
-        res = self.search_plugin_by_kw(resp.split(" "), plugins)
+        res = self.search_plugin_by_kw(resp.split(), plugins)
         if not res:
             Print.clean_print("§c没有任何已安装插件匹配得上关键词")
             return None
         if len(res) > 1:
             Print.clean_print("§a☑ §f关键词查找到的插件:")
             for i, plugin in enumerate(res):
                 Print.clean_print(str(i + 1) + ". " +
@@ -298,15 +313,15 @@
         r = JsonIO.readFileFrom("主系统核心数据", self.plugin_reg_data_path)
         if not isinstance(r, dict):
             raise ValueError("插件注册表数据类型错误")
         del r[plugin_data.plugin_type][plugin_data.name]
         JsonIO.writeFileTo("主系统核心数据", self.plugin_reg_data_path, r)
 
     def get_plugin_reg_name_dict_and_datas(self) -> tuple[dict[str, list[str]], list[PluginRegData]]:
-        """获取插件注册表的插件名字字典和插件注册信息列表
+        """获取插件注册表的插件名字字典(插件类型:插件名列表)和插件注册信息列表
 
         Raises:
             ValueError: 插件注册表数据类型错误
             ValueError: 获取插件注册表出现问题
 
         Returns:
             tuple[dict[str, list[str]], list[PluginRegData]]: 插件名字字典和插件注册信息列表
@@ -336,15 +351,15 @@
                     or os.path.exists(os.path.join("插件文件", f_dirname[p.plugin_type], p.name + "+disabled"))
                 ):
                     res.append(p)
                     r0[p.plugin_type].append(p.name)
         return r0, res
 
     def get_2_compare_plugins_reg(self) -> list[PluginRegData]:
-        """获取用于比较的插件注册信息列表, 比较已注册与未注册插件
+        """获取全插件注册信息列表, 比较已注册与未注册插件
 
         Returns:
             list[PluginRegData]: 插件注册信息列表
         """
         f_plugins: list[PluginRegData] = []
         reg_dict, reg_list = self.get_plugin_reg_name_dict_and_datas()
         for p, k in {
@@ -395,28 +410,14 @@
         for i, t in enumerate(lfts):
             if i in range(len(rgts)):
                 Print.clean_print("§f" + Print.align(t, 35) +
                                   "§f" + Print.align(rgts[i]))
             else:
                 Print.clean_print("§f" + Print.align(t, 35))
 
-    @staticmethod
-    def test_name_same(name: str, dirname: str) -> None:
-        """测试插件名与文件夹名是否一致
-
-        Args:
-            name (str): 插件名
-            dirname (str): 文件夹名
-
-        Raises:
-            AssertionError: 插件名与文件夹名不一致
-        """
-        if name != dirname:
-            raise AssertionError(f"插件名: {name} 与文件夹名({dirname}) 不一致") from None
-
     def list_plugins_list(self) -> list[PluginRegData]:
         """列出插件列表
 
         Returns:
             list[PluginRegData]: 插件注册信息列表
         """
         Print.clean_print("§a☑ §f目前已安装的插件列表:")
```

### Comparing `tooldelta-0.6.2/tooldelta/plugin_market.py` & `tooldelta-0.7.0/tooldelta/plugin_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         clear_screen()
         Print.clean_print("§a已从插件市场返回 ToolDelta 控制台.")
 
     def get_datas_from_market(self, source_url: str | None = None) -> dict:
         """从插件市场获取数据
 
         Args:
-            source_url (str | None, optional): 插件市场源, 默认为None,有则替换整体插件市场源
+            source_url (str | None, optional): 插件市场源, 默认为None, 有则替换整体插件市场源
 
         Returns:
             dict: 插件市场数据
         """
         if isinstance(source_url, str):
             self.plugins_download_url = self.plugins_download_url
         market_datas = get_json_from_url(
@@ -291,36 +291,41 @@
         res.raise_for_status()
         res1: dict = json.loads(res.text)
         self.plugin_id_name_map = res1
         return res1
 
     def download_plugin(
         self,
-        plugin_data: PluginRegData
+        plugin_data: PluginRegData,
+        with_pres = True
     ) -> list[PluginRegData]:
-        """下载插件
+        """
+        下载插件
+        注意: 只能传入由 `get_plugin_data_from_market()` 生成的数据
 
         Args:
             plugin_data (PluginRegData): 插件注册数据
+            with_pres (bool): 是否一同下载前置插件
 
         Raises:
             ValueError: 未知插件类型
 
         Returns:
-            list[PluginRegData]: 插件注册数据列表
+            list[PluginRegData]: 本插件和其前置插件的注册数据列表
         """
         if self.plugin_id_name_map is None:
             self.plugin_id_name_map = self.get_plugin_id_name_map()
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
-        for plugin_id in plugin_data.pre_plugins:
-            plugin_name = self.plugin_id_name_map[plugin_id]
-            Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
-            plugin_datas = self.get_plugin_data_from_market(plugin_id)
-            pres += self.download_plugin(plugin_datas)
+        if with_pres:
+            for plugin_id in plugin_data.pre_plugins:
+                plugin_name = self.plugin_id_name_map[plugin_id]
+                Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
+                plugin_datas = self.get_plugin_data_from_market(plugin_id)
+                pres += self.download_plugin(plugin_datas)
         cache_dir = tempfile.mkdtemp()
         try:
             for paths in download_paths:
                 if not paths.strip():
                     Print.print_war("下载路径为空, 跳过")
                     continue
                 url = url_join(self.plugins_download_url, paths)
```

### Comparing `tooldelta-0.6.2/tooldelta/starter.py` & `tooldelta-0.7.0/tooldelta/starter.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,13 +46,13 @@
         exit_directly (bool, optional): 是否三秒强制直接退出
     """
     if out_task:
         frame.system_exit()
     frame.safelyExit()
     if exit_directly:
         for _ in range(2, 0, -1):
-            with Print.lock:Print.print_war(f"{_}秒后强制退出...", end="\r")
+            Print.print_war(f"{_}秒后强制退出...", end="\r")
             time.sleep(1)
-        with Print.lock:Print.print_war("0秒后强制退出...", end="\r")
-        with Print.lock:Print.print_suc("ToolDelta 已退出.")
+        Print.print_war("0秒后强制退出...", end="\r")
+        Print.print_suc("ToolDelta 已退出.")
         os._exit(0)
-    with Print.lock:Print.print_suc("ToolDelta 已退出.")
+    Print.print_suc("ToolDelta 已退出.")
```

### Comparing `tooldelta-0.6.2/tooldelta/sys_args.py` & `tooldelta-0.7.0/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/tooldelta/urlmethod.py` & `tooldelta-0.7.0/tooldelta/urlmethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,20 @@
     Args:
         url (str): 原始链接
 
     Returns:
         str: 原始链接
     """
     try:
-        if url.startswith("https://github.com/"):return requests.head(url, allow_redirects=True).url
-        else:return url
-    except:return url
+        if url.startswith("https://github.com/"):
+            return requests.head(url, allow_redirects=True).url
+        else:
+            return url
+    except:
+        return url
 
 def progress_bar(
     current: float | int, total: float | int, length: int | float = 20, color1: str = "§f", color2: str = "§b"
 ) -> str:
     """执行进度条
 
     Args:
```

### Comparing `tooldelta-0.6.2/tooldelta/utils.py` & `tooldelta-0.7.0/tooldelta/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.2/PKG-INFO` & `tooldelta-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.6.2
+Version: 0.7.0
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.2 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.7.0 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
```

