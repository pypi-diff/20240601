# Comparing `tmp/aiomql-3.21.tar.gz` & `tmp/aiomql-3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomql-3.21.tar", last modified: Sat May  4 23:10:05 2024, max compression
+gzip compressed data, was "aiomql-3.22.tar", last modified: Sat Jun  1 11:29:09 2024, max compression
```

## Comparing `aiomql-3.21.tar` & `aiomql-3.22.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.304194 aiomql-3.21/
--rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-3.21/LICENSE
--rw-rw-rw-   0        0        0     5059 2024-05-04 23:10:05.301197 aiomql-3.21/PKG-INFO
--rw-rw-rw-   0        0        0     4252 2024-05-04 23:06:46.000000 aiomql-3.21/README.md
--rw-rw-rw-   0        0        0      870 2024-04-27 10:38:39.000000 aiomql-3.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 23:10:05.304194 aiomql-3.21/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-3.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.020059 aiomql-3.21/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.119129 aiomql-3.21/src/aiomql/
--rw-rw-rw-   0        0        0      664 2024-04-10 01:11:51.000000 aiomql-3.21/src/aiomql/__init__.py
--rw-rw-rw-   0        0        0     3696 2024-04-27 10:38:39.000000 aiomql-3.21/src/aiomql/account.py
--rw-rw-rw-   0        0        0     5721 2024-04-27 10:38:39.000000 aiomql-3.21/src/aiomql/bot_builder.py
--rw-rw-rw-   0        0        0    11834 2024-04-28 22:35:40.000000 aiomql-3.21/src/aiomql/candle.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.221470 aiomql-3.21/src/aiomql/core/
--rw-rw-rw-   0        0        0      227 2024-02-12 18:34:51.000000 aiomql-3.21/src/aiomql/core/__init__.py
--rw-rw-rw-   0        0        0     4487 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/base.py
--rw-rw-rw-   0        0        0     6140 2024-04-27 22:17:47.000000 aiomql-3.21/src/aiomql/core/config.py
--rw-rw-rw-   0        0        0    36149 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/constants.py
--rw-rw-rw-   0        0        0     1136 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/errors.py
--rw-rw-rw-   0        0        0      574 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/core/exceptions.py
--rw-rw-rw-   0        0        0    15519 2024-04-29 12:23:17.000000 aiomql-3.21/src/aiomql/core/meta_trader.py
--rw-rw-rw-   0        0        0    15024 2024-02-12 18:54:21.000000 aiomql-3.21/src/aiomql/core/models.py
--rw-rw-rw-   0        0        0     1509 2024-05-04 12:54:41.000000 aiomql-3.21/src/aiomql/core/task_queue.py
--rw-rw-rw-   0        0        0     3343 2024-02-12 19:02:36.000000 aiomql-3.21/src/aiomql/executor.py
--rw-rw-rw-   0        0        0    11512 2024-04-29 12:22:52.000000 aiomql-3.21/src/aiomql/history.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.232647 aiomql-3.21/src/aiomql/lib/
--rw-rw-rw-   0        0        0       75 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.249775 aiomql-3.21/src/aiomql/lib/strategies/
--rw-rw-rw-   0        0        0       67 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/lib/strategies/__init__.py
--rw-rw-rw-   0        0        0     5270 2024-05-04 13:19:33.000000 aiomql-3.21/src/aiomql/lib/strategies/finger_trap.py
--rw-rw-rw-   0        0        0     1136 2024-02-11 20:59:21.000000 aiomql-3.21/src/aiomql/lib/strategies/tracker.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.283192 aiomql-3.21/src/aiomql/lib/symbols/
--rw-rw-rw-   0        0        0       39 2024-01-24 23:56:43.000000 aiomql-3.21/src/aiomql/lib/symbols/__init__.py
--rw-rw-rw-   0        0        0     4265 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/symbols/forex_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.297197 aiomql-3.21/src/aiomql/lib/traders/
--rw-rw-rw-   0        0        0       41 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/traders/__init__.py
--rw-rw-rw-   0        0        0     1971 2024-02-12 19:30:57.000000 aiomql-3.21/src/aiomql/lib/traders/simple_trader.py
--rw-rw-rw-   0        0        0     5778 2024-04-22 12:13:27.000000 aiomql-3.21/src/aiomql/order.py
--rw-rw-rw-   0        0        0     5681 2024-04-22 13:08:33.000000 aiomql-3.21/src/aiomql/positions.py
--rw-rw-rw-   0        0        0     2484 2024-04-29 08:17:47.000000 aiomql-3.21/src/aiomql/ram.py
--rw-rw-rw-   0        0        0     4400 2024-04-01 00:45:04.000000 aiomql-3.21/src/aiomql/records.py
--rw-rw-rw-   0        0        0     3512 2024-04-22 14:36:06.000000 aiomql-3.21/src/aiomql/result.py
--rw-rw-rw-   0        0        0     8753 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/sessions.py
--rw-rw-rw-   0        0        0     2993 2024-02-03 13:05:20.000000 aiomql-3.21/src/aiomql/strategy.py
--rw-rw-rw-   0        0        0    17986 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/symbol.py
--rw-rw-rw-   0        0        0     2803 2024-02-12 19:18:28.000000 aiomql-3.21/src/aiomql/terminal.py
--rw-rw-rw-   0        0        0     8323 2024-04-28 22:45:31.000000 aiomql-3.21/src/aiomql/ticks.py
--rw-rw-rw-   0        0        0     5931 2024-04-10 10:12:59.000000 aiomql-3.21/src/aiomql/trade_records.py
--rw-rw-rw-   0        0        0     5777 2024-04-27 10:45:41.000000 aiomql-3.21/src/aiomql/trader.py
--rw-rw-rw-   0        0        0     1413 2024-02-12 20:00:12.000000 aiomql-3.21/src/aiomql/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:10:05.299196 aiomql-3.21/src/aiomql.egg-info/
--rw-rw-rw-   0        0        0     5059 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1173 2024-05-04 23:10:05.000000 aiomql-3.21/src/aiomql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 23:10:04.000000 aiomql-3.21/src/aiomql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.248284 aiomql-3.22/
+-rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-3.22/LICENSE
+-rw-rw-rw-   0        0        0     5059 2024-06-01 11:29:09.244282 aiomql-3.22/PKG-INFO
+-rw-rw-rw-   0        0        0     4252 2024-05-04 23:06:46.000000 aiomql-3.22/README.md
+-rw-rw-rw-   0        0        0      870 2024-06-01 11:22:54.000000 aiomql-3.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:29:09.250287 aiomql-3.22/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-3.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:08.498795 aiomql-3.22/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:08.852352 aiomql-3.22/src/aiomql/
+-rw-rw-rw-   0        0        0      664 2024-04-10 01:11:51.000000 aiomql-3.22/src/aiomql/__init__.py
+-rw-rw-rw-   0        0        0     3841 2024-06-01 11:13:07.000000 aiomql-3.22/src/aiomql/account.py
+-rw-rw-rw-   0        0        0     5721 2024-04-27 10:38:39.000000 aiomql-3.22/src/aiomql/bot_builder.py
+-rw-rw-rw-   0        0        0    11717 2024-06-01 11:07:08.000000 aiomql-3.22/src/aiomql/candle.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.050277 aiomql-3.22/src/aiomql/core/
+-rw-rw-rw-   0        0        0      227 2024-02-12 18:34:51.000000 aiomql-3.22/src/aiomql/core/__init__.py
+-rw-rw-rw-   0        0        0     4487 2024-02-12 18:54:21.000000 aiomql-3.22/src/aiomql/core/base.py
+-rw-rw-rw-   0        0        0     6388 2024-06-01 11:13:07.000000 aiomql-3.22/src/aiomql/core/config.py
+-rw-rw-rw-   0        0        0    36149 2024-02-12 18:54:21.000000 aiomql-3.22/src/aiomql/core/constants.py
+-rw-rw-rw-   0        0        0     1136 2024-02-12 18:54:21.000000 aiomql-3.22/src/aiomql/core/errors.py
+-rw-rw-rw-   0        0        0      574 2024-01-24 23:56:43.000000 aiomql-3.22/src/aiomql/core/exceptions.py
+-rw-rw-rw-   0        0        0    15461 2024-06-01 09:42:34.000000 aiomql-3.22/src/aiomql/core/meta_trader.py
+-rw-rw-rw-   0        0        0    15076 2024-05-31 10:29:36.000000 aiomql-3.22/src/aiomql/core/models.py
+-rw-rw-rw-   0        0        0     1509 2024-05-04 12:54:41.000000 aiomql-3.22/src/aiomql/core/task_queue.py
+-rw-rw-rw-   0        0        0     3343 2024-02-12 19:02:36.000000 aiomql-3.22/src/aiomql/executor.py
+-rw-rw-rw-   0        0        0    11219 2024-06-01 09:48:40.000000 aiomql-3.22/src/aiomql/history.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.069283 aiomql-3.22/src/aiomql/lib/
+-rw-rw-rw-   0        0        0       75 2024-01-24 23:56:43.000000 aiomql-3.22/src/aiomql/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.158277 aiomql-3.22/src/aiomql/lib/strategies/
+-rw-rw-rw-   0        0        0       67 2024-02-12 19:18:28.000000 aiomql-3.22/src/aiomql/lib/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5270 2024-05-04 13:19:33.000000 aiomql-3.22/src/aiomql/lib/strategies/finger_trap.py
+-rw-rw-rw-   0        0        0     1136 2024-02-11 20:59:21.000000 aiomql-3.22/src/aiomql/lib/strategies/tracker.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.182279 aiomql-3.22/src/aiomql/lib/symbols/
+-rw-rw-rw-   0        0        0       39 2024-01-24 23:56:43.000000 aiomql-3.22/src/aiomql/lib/symbols/__init__.py
+-rw-rw-rw-   0        0        0     4267 2024-06-01 11:07:08.000000 aiomql-3.22/src/aiomql/lib/symbols/forex_symbol.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.234284 aiomql-3.22/src/aiomql/lib/traders/
+-rw-rw-rw-   0        0        0       41 2024-02-12 19:30:57.000000 aiomql-3.22/src/aiomql/lib/traders/__init__.py
+-rw-rw-rw-   0        0        0     1971 2024-02-12 19:30:57.000000 aiomql-3.22/src/aiomql/lib/traders/simple_trader.py
+-rw-rw-rw-   0        0        0     5925 2024-06-01 10:02:40.000000 aiomql-3.22/src/aiomql/order.py
+-rw-rw-rw-   0        0        0     5675 2024-06-01 08:54:50.000000 aiomql-3.22/src/aiomql/positions.py
+-rw-rw-rw-   0        0        0     2484 2024-04-29 08:17:47.000000 aiomql-3.22/src/aiomql/ram.py
+-rw-rw-rw-   0        0        0     4400 2024-04-01 00:45:04.000000 aiomql-3.22/src/aiomql/records.py
+-rw-rw-rw-   0        0        0     3512 2024-04-22 14:36:06.000000 aiomql-3.22/src/aiomql/result.py
+-rw-rw-rw-   0        0        0     8753 2024-02-12 19:18:28.000000 aiomql-3.22/src/aiomql/sessions.py
+-rw-rw-rw-   0        0        0     2993 2024-02-03 13:05:20.000000 aiomql-3.22/src/aiomql/strategy.py
+-rw-rw-rw-   0        0        0    17929 2024-06-01 11:07:08.000000 aiomql-3.22/src/aiomql/symbol.py
+-rw-rw-rw-   0        0        0     2803 2024-02-12 19:18:28.000000 aiomql-3.22/src/aiomql/terminal.py
+-rw-rw-rw-   0        0        0     8323 2024-04-28 22:45:31.000000 aiomql-3.22/src/aiomql/ticks.py
+-rw-rw-rw-   0        0        0     5931 2024-04-10 10:12:59.000000 aiomql-3.22/src/aiomql/trade_records.py
+-rw-rw-rw-   0        0        0     5371 2024-06-01 08:54:50.000000 aiomql-3.22/src/aiomql/trader.py
+-rw-rw-rw-   0        0        0     1414 2024-06-01 11:07:08.000000 aiomql-3.22/src/aiomql/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:29:09.240335 aiomql-3.22/src/aiomql.egg-info/
+-rw-rw-rw-   0        0        0     5059 2024-06-01 11:29:08.000000 aiomql-3.22/src/aiomql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1173 2024-06-01 11:29:08.000000 aiomql-3.22/src/aiomql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:29:08.000000 aiomql-3.22/src/aiomql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-06-01 11:29:08.000000 aiomql-3.22/src/aiomql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 11:29:08.000000 aiomql-3.22/src/aiomql.egg-info/top_level.txt
```

### Comparing `aiomql-3.21/LICENSE` & `aiomql-3.22/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/PKG-INFO` & `aiomql-3.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 3.21
+Version: 3.22
 Summary: Asynchronous MetaTrader5 library and Algorithmic Trading Framework
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiomql-3.21/README.md` & `aiomql-3.22/README.md`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/pyproject.toml` & `aiomql-3.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiomql"
-version = "3.21"
+version = "3.22"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aiomql-3.21/src/aiomql/__init__.py` & `aiomql-3.22/src/aiomql/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/account.py` & `aiomql-3.22/src/aiomql/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, '_instance'):
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if not self.login:
-            acc = self.config.account_info()
-            self.set_attributes(**acc)
+        acc = self.config.account_info()
+        acc_details = {k: v for k, v in self.get_dict(include={'login', 'server', 'password'}).items() if v}
+        acc |= acc_details
+        self.config.set_attributes(**acc)
+        self.set_attributes(**acc)
 
     async def refresh(self):
         """Refreshes the account instance with the latest account details from the MetaTrader 5 terminal"""
         account_info = await self.mt5.account_info()
         acc = account_info._asdict()
         self.set_attributes(**acc)
```

### Comparing `aiomql-3.21/src/aiomql/bot_builder.py` & `aiomql-3.22/src/aiomql/bot_builder.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/candle.py` & `aiomql-3.22/src/aiomql/candle.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
                 % {"class": self.__class__.__name__, "open": self.open, "high": self.high,
                    "low": self.low, "close": self.close, "time": self.time, 'Index': self.Index})
 
     def __str__(self):
         return str(self.dict())
 
     def __eq__(self, other: "Candle"):
-        return self.time == other.time
+        eq = self.open == other.open and self.high == other.high and self.low == other.low and self.close == other.close
+        return eq
 
     def __hash__(self):
         return hash(self.time)
 
     def __lt__(self, other: "Candle"):
         return self.time < other.time
 
@@ -214,18 +215,14 @@
         if item == 'Index':
             return Series(self._data.index)
         raise AttributeError(f"Attribute {item} not defined on class {self.__class__.__name__}")
 
     def __iter__(self):
         return (self.Candle(**row._asdict()) for row in self._data.itertuples())
 
-    def __add__(self, other: _Candles | _Candle):
-        other = other.data if isinstance(other, type(self)) else other.dict()
-        return self.__class__(data=self._data.append(other.data, ignore_index=True))
-
     @property
     def timeframe(self):
         tf = self.time[1] - self.time[0]
         return TimeFrame.get(abs(tf))
 
     @property
     def ta(self):
```

### Comparing `aiomql-3.21/src/aiomql/core/base.py` & `aiomql-3.22/src/aiomql/core/base.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/core/config.py` & `aiomql-3.22/src/aiomql/core/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,22 @@
         self.root_dir = self.root
 
     def __setattr__(self, key, value):
         if key == 'path':
             value = str(self.root_dir / Path(value).absolute().resolve())
         super().__setattr__(key, value)
 
+    def set_attributes(self, **kwargs):
+        """Set keyword arguments as object attributes
+
+        Keyword Args:
+            **kwargs: Object attributes and values as keyword arguments
+        """
+        [setattr(self, key, value) for key, value in kwargs.items()]
+
     @staticmethod
     def walk_to_root(path: str | Path) -> Iterator[str]:
         if not os.path.exists(path):
             raise IOError("Starting path not found")
 
         if os.path.isfile(path):
             path = os.path.dirname(path)
@@ -137,15 +145,15 @@
         if (file := (file or self.find_config())) is None:
             logger.warning("No Config File Found")
         else:
             fh = open(file, mode="r")
             data = json.load(fh)
             fh.close()
         data |= kwargs
-        [setattr(self, key, value) for key, value in data.items()]
+        self.set_attributes(**data)
         self._initialize = False
 
     def account_info(self) -> dict[str, int | str]:
         """Returns Account login details as found in the config object if available
 
         Returns:
             dict: A dictionary of login details
```

### Comparing `aiomql-3.21/src/aiomql/core/constants.py` & `aiomql-3.22/src/aiomql/core/constants.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/core/errors.py` & `aiomql-3.22/src/aiomql/core/errors.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/core/exceptions.py` & `aiomql-3.22/src/aiomql/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/core/meta_trader.py` & `aiomql-3.22/src/aiomql/core/meta_trader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import datetime
 import asyncio
 from logging import getLogger
 from typing import Callable
 
 import MetaTrader5
-
 from MetaTrader5 import BookInfo, SymbolInfo, AccountInfo, Tick, TerminalInfo, TradeOrder, TradeDeal, \
     TradePosition, OrderSendResult, OrderCheckResult
 
 from .constants import TimeFrame, CopyTicks, OrderType
 from .errors import Error
 from .config import Config
 
@@ -57,15 +56,14 @@
     _terminal_info: Callable
     _version: Callable
     error: Error
     config: Config
 
     def __init__(self):
         self.config = Config()
-        self.error = Error(1, 'Successful')
 
     async def __aenter__(self) -> 'MetaTrader':
         """
         Async context manager entry point.
         Initializes the connection to the MetaTrader terminal.
 
         Returns:
@@ -126,15 +124,15 @@
         return await asyncio.to_thread(self._shutdown)
 
     async def last_error(self) -> tuple[int, str]:
         try:
             return await asyncio.to_thread(self._last_error)
         except Exception as err:
             logger.warning(f'Error in obtaining last error.')
-            return 0, str(err)
+            return -1, str(err)
 
     async def version(self) -> tuple[int, int, str] | None:
         """"""
         res = await asyncio.to_thread(self._version)
         if res is None:
             err = await self.last_error()
             self.error = Error(*err)
@@ -342,10 +340,10 @@
                                 group: str = '', ticket: int = None, position: int = None) -> tuple[TradeDeal] | None:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('position', position)) if value}
         args = tuple(arg for arg in (date_from, date_to) if arg)
         res = await asyncio.to_thread(self._history_deals_get, *args, **kwargs)
         if res is None:
             err = await self.last_error()
             self.error = Error(*err)
-            logger.warning(f'Error in getting deals.{self.error.description}')
+            logger.warning(f'Error in getting deals.{self.error}')
             return res
         return res
```

### Comparing `aiomql-3.21/src/aiomql/core/models.py` & `aiomql-3.22/src/aiomql/core/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,32 +499,34 @@
         retcode: int
         deal: int
         order: int
         volume: float
         price: float
         bid: float
         ask: float
+        profit: float
+        loss: float
         comment: str
         request: TradeRequest
         request_id: int
         retcode_external: int
-        profit: float
     """
     retcode: int
     deal: int
     order: int
     volume: float
     price: float
     bid: float
     ask: float
     comment: str
     request: mt5.TradeRequest
     request_id: int
     retcode_external: int
-    profit: float
+    profit: float = None
+    loss: float = None
 
 
 class TradePosition(Base):
     """Trade Position
 
     Attributes:
         ticket: int
```

### Comparing `aiomql-3.21/src/aiomql/core/task_queue.py` & `aiomql-3.22/src/aiomql/core/task_queue.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/executor.py` & `aiomql-3.22/src/aiomql/executor.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/history.py` & `aiomql-3.22/src/aiomql/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         deals (list[TradeDeal]): Iterable of trade deals
         orders (list[TradeOrder]): Iterable of trade orders
         total_deals: Total number of deals
         total_orders (int): Total number orders
         group (str): Filter for selecting history by symbols.
         ticket (int): Filter for selecting history by ticket number
         position (int): Filter for selecting history deals by position
-        initialized (bool): check if initial request has been sent to the terminal to get history.
         mt5 (MetaTrader): MetaTrader instance
         config (Config): Config instance
     """
     mt5: MetaTrader
     config: Config
 
     def __init__(self, *, date_from: datetime | int = None, date_to: datetime | int = None,
@@ -51,32 +50,26 @@
         self.group = group
         self.ticket = ticket
         self.position = position
         self.deals: list[TradeDeal] = []
         self.orders: list[TradeOrder] = []
         self.total_deals: int = 0
         self.total_orders: int = 0
-        self.initialized = False
 
-    async def init(self, deals=True, orders=True) -> bool:
+    async def init(self, deals=True, orders=True):
         """Get history deals and orders
 
         Keyword Args:
             deals (bool): If true get history deals during initial request to terminal
             orders (bool): If true get history orders during initial request to terminal
-
-        Returns:
-            bool: True if all requests were successful else False
         """
-        tasks = []
-        tasks.append(self.get_deals()) if deals else ...
-        tasks.append(self.get_orders()) if orders else ...
-        res = await asyncio.gather(*tasks)
-        self.initialized = all(res)
-        return self.initialized
+        self.deals = await self.get_deals() if deals else tuple()
+        self.orders = await self.get_orders() if orders else tuple()
+        self.total_deals = len(self.deals)
+        self.total_orders = len(self.orders)
 
     async def get_deals(self, *, date_from: datetime | int = None, date_to: datetime | int = None, group: str = '',
                         retries: int = 3) -> tuple[TradeDeal, ...]:
         """Get deals from trading history using the parameters set in the constructor.
 
         Returns:
             tuple[TradeDeal]: A list of trade deals
@@ -85,17 +78,15 @@
             logger.warning(f'Failed to get deals: {self.mt5.error}')
             return tuple()
 
         date_from, date_to, group = date_from or self.date_from, date_to or self.date_to, group or self.group
         deals = await self.mt5.history_deals_get(date_from=date_from, date_to=date_to, group=group)
 
         if deals is not None:
-            self.deals = tuple(TradeDeal(**deal._asdict()) for deal in deals)
-            self.total_deals = len(self.deals)
-            return self.deals
+            return tuple(TradeDeal(**deal._asdict()) for deal in deals)
 
         if self.mt5.error.is_connection_error():
             await asyncio.sleep(retries)
             return await self.get_deals(date_from=date_from, date_to=date_to, group=group, retries=retries-1)
 
         logger.warning(f'Failed to get deals: {self.mt5.error}')
         return tuple()
@@ -109,29 +100,29 @@
 
         Returns:
             tuple[TradeDeal]: A tuple of all deals with the order ticket
         """
         ticket = ticket or self.ticket
         assert ticket is not None, 'ticket not provided'
         deals = await self.mt5.history_deals_get(ticket=ticket)
-        return tuple(sorted([TradeDeal(**deal._asdict()) for deal in deals], key=lambda x: x.time_msc))
+        return tuple(sorted([TradeDeal(**deal._asdict()) for deal in deals or []], key=lambda x: x.time_msc))
 
     async def get_deals_position(self, *, position: int = None) -> tuple[TradeDeal, ...]:
         """
         Get all deals with the specified position ticket in the DEAL_POSITION_ID property
         Args:
             position (int): The position ticket
 
         Returns:
             tuple[TradeDeal]: A tuple of all deals with the position ticket
         """
         position = position or self.position
         assert position is not None, 'position not provided'
         deals = await self.mt5.history_deals_get(position=position)
-        return tuple(sorted([TradeDeal(**deal._asdict()) for deal in deals], key=lambda x: x.time_msc))
+        return tuple(sorted([TradeDeal(**deal._asdict()) for deal in deals or []], key=lambda x: x.time_msc))
 
     async def deals_total(self, *, date_from: int | datetime = None, date_to: int | datetime = None) -> int:
         """Get total number of deals within the specified period in the constructor.
         Args:
             date_from (int|datetime): Date the orders are requested from. Set by the 'datetime' object or as a number of
                 seconds elapsed since 1970.01.01.
             date_to (int|datetime): Date up to which the orders are requested. Set by the 'datetime' object or as a
@@ -163,21 +154,21 @@
         if self.mt5.error.is_connection_error():
             await asyncio.sleep(retries)
             return await self.get_orders(date_from=date_from, date_to=date_to, group=group, retries=retries - 1)
 
         logger.warning(f'Failed to get orders: {self.mt5.error}')
         return tuple()
 
-    async def get_order_ticket(self, ticket: int | None = None) -> TradeOrder:
+    async def get_order_ticket(self, ticket: int | None = None) -> TradeOrder | None:
         ticket = ticket or self.ticket
         assert isinstance(ticket, int), 'ticket not provided'
         orders = await self.mt5.history_orders_get(ticket=ticket)
-        order = orders[0]
-        assert order.ticket == ticket
-        return TradeOrder(**order._asdict())
+        if orders and (order := orders[0]).ticket == ticket:
+            return TradeOrder(**order._asdict())
+        return None
 
     async def get_orders_position(self, position: int = None) -> tuple[TradeOrder, ...]:
         """
         Call specifying the position ticket. Return all orders with a position ticket specified in the
         ORDER_POSITION_ID property
 
         Args:
@@ -185,15 +176,15 @@
 
         Returns:
             tuple[TradeOrder]: A tuple of all orders with the position ticket
         """
         position = position or self.position
         assert isinstance(position, int), 'position not provided'
         orders = await self.mt5.history_orders_get(position=position)
-        return tuple(sorted([TradeOrder(**order._asdict()) for order in orders], key=lambda x: x.time_done_msc))
+        return tuple(sorted([TradeOrder(**order._asdict()) for order in orders or []], key=lambda x: x.time_done_msc))
 
     async def orders_total(self, date_from: int | datetime = None, date_to: int | datetime = None) -> int:
         """Get total number of orders within the specified period in the constructor.
 
         Returns:
             int: Total number of orders
         """
```

### Comparing `aiomql-3.21/src/aiomql/lib/strategies/finger_trap.py` & `aiomql-3.22/src/aiomql/lib/strategies/finger_trap.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/lib/strategies/tracker.py` & `aiomql-3.22/src/aiomql/lib/strategies/tracker.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/lib/symbols/forex_symbol.py` & `aiomql-3.22/src/aiomql/lib/symbols/forex_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         Args:
             amount (float): Amount to trade
             volume (float): Volume to trade
         """
         points = amount / (volume * self.point * self.trade_contract_size)
         return points
     
-    async def compute_volume_points(self, *, amount: float, points: float, use_limits=False, round_down: bool = True,
+    async def compute_volume_points(self, *, amount: float, points: float, use_limits=False, round_down: bool = False,
                                     adjust: float = False) -> tuple[float, float]:
         """Compute the volume and points required for a trade. Given the amount and the number of points.
 
         Args:
             amount (float): Amount to trade
             points (float): Number of points
             round_down: round down the computed volume to the nearest step default True
@@ -36,16 +36,16 @@
         if use_limits:
             vol = chk_vol[1]
             if adjust:
                 points = self.compute_points(amount=amount, volume=vol)
             return vol, points
         raise VolumeError(f"Incorrect Volume. Computed Volume outside the range of permitted volumes")
 
-    async def compute_volume_sl(self, *, amount: float, price: float, sl: float,
-                                use_limits=False, adjust: bool = False, round_down: bool = True) -> tuple[float, float]:
+    async def compute_volume_sl(self, *, amount: float, price: float, sl: float, use_limits=False, adjust: bool = False,
+                                round_down: bool = False) -> tuple[float, float]:
         amount = await self.check_amount(amount)
         volume = amount / ((price - sl) * self.trade_contract_size)
         volume = self.round_off_volume(volume, round_down=round_down)
         sign = volume / abs(volume) if volume else 1
         if (chk_vol := self.check_volume(abs(volume)))[0]:
             if adjust:
                 sl = price - (amount / (volume * self.trade_contract_size))
```

### Comparing `aiomql-3.21/src/aiomql/lib/traders/simple_trader.py` & `aiomql-3.22/src/aiomql/lib/traders/simple_trader.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/order.py` & `aiomql-3.22/src/aiomql/trader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,128 @@
-import asyncio
+"""Trader class module. Handles the creation of an order and the placing of trades"""
+from abc import ABC, abstractmethod
+from datetime import datetime
+from typing import TypeVar
 from logging import getLogger
+from zoneinfo import ZoneInfo
 
-from .core.models import TradeRequest, OrderSendResult, OrderCheckResult, TradeOrder
-from .core.constants import TradeAction, OrderTime, OrderFilling
-from .core.exceptions import OrderError
-logger = getLogger(__name__)
+from .order import Order
+from .symbol import Symbol as _Symbol
+from .ticks import Tick
+from .ram import RAM
+from .core.models import OrderType, OrderSendResult
+from .core.config import Config
+from .result import Result
 
+logger = getLogger(__name__)
+Symbol = TypeVar("Symbol", bound=_Symbol)
 
-class Order(TradeRequest):
-    """Trade order related functions and properties. Subclass of TradeRequest."""
 
-    def __init__(self, **kwargs):
-        """Initialize the order object with keyword arguments, symbol must be provided.
-        Provide default values for action, type_time and type_filling if not provided.
+class Trader(ABC):
+    """Base class for creating a Trader object. Handles the creation of an order and the placing of trades.
 
-        Args:
-            **kwargs: Keyword arguments must match the attributes of TradeRequest as well as the attributes of
-             Order class as specified in the annotations in the class definition.
+    Attributes:
+        symbol (Symbol): The financial instrument.
+        ram (RAM): RAM instance
+        order (Order): Trade order
 
-        Default Values:
-            action (TradeAction.DEAL): Trade action
-            type_time (OrderTime.DAY): Order time
-            type_filling (OrderFilling.FOK): Order filling
-        """
-        if 'symbol' in kwargs:
-            kwargs['symbol'] = str(kwargs['symbol'])
-        self.action = kwargs.pop('action', TradeAction.DEAL)
-        self.type_time = kwargs.pop('type_time', OrderTime.DAY)
-        self.type_filling = kwargs.pop('type_filling', OrderFilling.FOK)
-        super().__init__(**kwargs)
+    Class Attributes:
+        config (Config): Config instance.
+    """
+    config: Config
 
-    async def orders_total(self):
-        """Get the number of active orders.
-
-        Returns:
-            (int): total number of active orders
-        """
-        return await self.mt5.orders_total()
+    def __init__(self, *, symbol: Symbol, ram: RAM = None):
+        """Initializes the order object and RAM instance
 
-    async def get_order(self, *, ticket: int, retries: int = 3) -> TradeOrder:
-        """
-        Get the order by ticket number.
         Args:
-            ticket (int): Order ticket number
-            retries (int): Number of retries
-        Returns:
-        """
-        if retries < 1:
-            raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
-        orders = await self.mt5.orders_get(ticket=ticket)
-        if orders is not None:
-            order = TradeOrder(**orders[0]._asdict())
-            assert order.ticket == ticket, f'Order ticket mismatch {order.ticket} != {ticket}'
-            return order
-        if self.mt5.error.is_connection_error():
-            await asyncio.sleep(retries)
-            return await self.get_order(ticket=ticket, retries=retries-1)
-        raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
-
-    async def get_orders(self, *, ticket: int = 0, symbol: str = '', group: str = '', retries=3)\
-            -> tuple[TradeOrder, ...]:
-        """Get the list of active orders for the current symbol.
-        Keyword Args:
-            ticket (int): Order ticket number
-            symbol (str): Symbol name
-            group (str): Group name
-        Returns:
-            tuple[TradeOrder]: A Tuple of active trade orders as TradeOrder objects
+            symbol (Symbol): Financial instrument
+            ram (RAM): Risk Assessment and Management instance
         """
-        if retries < 1:
-            raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
-        symbol = getattr(self, 'symbol', symbol)
-        orders = await self.mt5.orders_get(symbol=symbol, ticket=ticket, group=group)
-        if orders is not None:
-            orders = (TradeOrder(**order._asdict()) for order in orders)
-            return tuple(orders)
-        if self.mt5.error.is_connection_error():
-            await asyncio.sleep(retries)
-            return await self.get_orders(ticket=ticket, symbol=symbol, group=group, retries=retries-1)
-        raise OrderError(f'Failed to get orders for {self.symbol}: {self.mt5.error}')
+        self.config = Config()
+        self.symbol = symbol
+        self.order = Order(symbol=symbol.name)
+        self.ram = ram or RAM()
+        self.parameters = {}
 
-    async def check(self) -> OrderCheckResult:
-        """Check funds sufficiency for performing a required trading operation and the possibility of executing it.
+    def set_order_limits(self, *, pips: float, tick: Tick):
+        """Sets the stop loss and take profit for the order. This method uses pips as defined for forex instruments.
 
-        Returns:
-            OrderCheckResult: An OrderCheckResult object
-
-        Raises:
-            OrderError: If not successful
-        """
-        res = await self.mt5.order_check(self.dict)
-        if res is None:
-            raise OrderError(f'Failed to check order due to {self.mt5.error.description}')
-        return OrderCheckResult(**res._asdict())
-
-    async def send(self) -> OrderSendResult:
-        """Send a request to perform a trading operation from the terminal to the trade server.
-
-        Returns:
-             OrderSendResult: An OrderSendResult object
-
-        Raises:
-            OrderError: If not successful
+        Args:
+            pips: Target pips
+            tick: Tick object
         """
-        res = await self.mt5.order_send(self.dict)
-        if res is None:
-            raise OrderError(f'Failed to send order {self.symbol} due to {self.mt5.error.description}')
-        return OrderSendResult(**res._asdict())
-
-    async def calc_margin(self) -> float:
-        """Return the required margin in the account currency to perform a specified trading operation.
+        pips = pips * self.symbol.pip
+        sl, tp = pips, pips * self.ram.risk_to_reward
+        if self.order.type == OrderType.BUY:
+            self.order.sl, self.order.tp = round(tick.ask - sl, self.symbol.digits), round(tick.ask + tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.ask
+        elif self.order.type == OrderType.SELL:
+            self.order.sl, self.order.tp = round(tick.bid + sl, self.symbol.digits), round(tick.bid - tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.bid
+        else:
+            raise ValueError(f"Invalid order type: {self.order.type}")
 
-        Returns:
-            float: Returns float value if successful
+    def set_trade_stop_levels(self, *, points: float, tick: Tick):
+        """Set the stop loss and take profit levels of the order based on the points and price tick.
 
-        Raises:
-            OrderError: If not successful
+        Args:
+            points: Target points
+            tick: Tick object
         """
-        res = await self.mt5.order_calc_margin(self.type, self.symbol, self.volume, self.price)
-        if res is None:
-            raise OrderError(f'Failed to calculate margin for {self.symbol} due to {self.mt5.error.description}')
-        return res
-
-    async def calc_profit(self) -> float:
-        """Return profit in the account currency for a specified trading operation.
-
-        Returns:
-            float: Returns float value if successful
+        points = points * self.symbol.point
+        sl, tp = points, points * self.ram.risk_to_reward
+        if self.order.type == OrderType.BUY:
+            self.order.sl, self.order.tp = round(tick.ask - sl, self.symbol.digits), round(tick.ask + tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.ask
+        else:
+            self.order.sl, self.order.tp = round(tick.bid + sl, self.symbol.digits), round(tick.bid - tp,
+                                                                                           self.symbol.digits)
+            self.order.price = tick.bid
+
+    async def check_order(self) -> bool:
+        """Check order before sending it to the broker.
+
+        Returns:
+            bool: True if order can go through else false
+        """
+        check = await self.order.check()
+        if check.retcode != 0:
+            logger.warning(f"Invalid order for {self.symbol} due to {check.comment}")
+            return False
+        return True
+
+    async def send_order(self) -> OrderSendResult:
+        """Send the order to the broker."""
+        result = await self.order.send()
+        if result.retcode != 10009:
+            logger.warning(f"Unable to place order for {self.symbol} due to {result.comment}")
+            return result
+        logger.info(f"Placed Trade for {self.symbol}")
+        return result
 
-        Raises:
-            OrderError: If not successful
-        """
-        res = await self.mt5.order_calc_profit(self.type, self.symbol, self.volume, self.price, self.tp)
-        if res is None:
-            raise OrderError(f'Failed to calculate profit for {self.symbol} due to {self.mt5.error.description}')
-        return res
+    async def record_trade(self, result: OrderSendResult, parameters: dict = None, name: str = '', exclude: set = None):
+        """Record the trade in csv or json.
+        Args:
+            result (OrderSendResult): Result of the order send
+            parameters: parameters of the trading strategy used to place the trade
+            name: Name of the trading strategy
+            exclude: Exclude these fields from the recorded trade
+        """
+        if result.retcode != 10009 or not self.config.record_trades:
+            return
+        params = parameters or self.parameters
+        params = {k: v for k, v in params.items() if k not in (exclude or set())}
+        profit = result.profit or await self.order.calc_profit()
+        params["expected_profit"] = profit
+        date = datetime.utcnow()
+        date = date.replace(tzinfo=ZoneInfo("UTC"))
+        params["date"] = str(date.date())
+        params["time"] = str(date.time())
+        res = Result(result=result, parameters=params, name=name)
+        self.config.task_queue.add_task(res.save)
+
+    @abstractmethod
+    async def place_trade(self, *args, **kwargs):
+        """Places a trade based on the order_type."""
```

### Comparing `aiomql-3.21/src/aiomql/positions.py` & `aiomql-3.22/src/aiomql/positions.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,27 +64,27 @@
             return [TradePosition(**pos._asdict()) for pos in positions]
         if self.mt5.error.is_connection_error():
             await asyncio.sleep(retries)
             return await self.positions_get(symbol, group, ticket, retries - 1)
         logger.warning(f'Failed to get positions for {symbol or self.symbol}. {self.mt5.error}')
         return []
 
-    async def position_get(self, *, ticket: int) -> TradePosition:
+    async def position_get(self, *, ticket: int) -> TradePosition | None:
         """Get an open position by ticket.
         Args:
             ticket (int): Position ticket.
 
         Returns:
             TradePosition: Return an open position
         """
         positions = await self.positions_get(ticket=ticket)
         position = positions[0] if positions else None
-        if position is None:
-            raise ValueError(f'Position with ticket {ticket} not found')
-        assert position.ticket == ticket, f'Position with ticket {ticket} not found'
+        if position is None or position.ticket != ticket:
+            logger.warning(f'Failed to get position for ticket {ticket}. {self.mt5.error}')
+            return None
         return position
 
     async def close(self, *, ticket: int, symbol: str, price: float, volume: float, order_type: OrderType):
         """Close an open position for the trading account using the ticket and other parameters.
         Args:
             ticket (int): Position ticket.
             symbol (str): Financial instrument name.
```

### Comparing `aiomql-3.21/src/aiomql/ram.py` & `aiomql-3.22/src/aiomql/ram.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/records.py` & `aiomql-3.22/src/aiomql/records.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/result.py` & `aiomql-3.22/src/aiomql/result.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/sessions.py` & `aiomql-3.22/src/aiomql/sessions.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/strategy.py` & `aiomql-3.22/src/aiomql/strategy.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/symbol.py` & `aiomql-3.22/src/aiomql/symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,23 +170,20 @@
         Args:
             volume (float): Volume to check
 
         Returns: tuple[bool, float]: Returns a tuple of a boolean and a float. The boolean indicates if the volume is
         within the limits of the symbol. The float is the volume to use if the volume is not within the limits of the
         symbol.
         """
-        check = self.volume_min <= volume <= self.volume_max
-        if check:
+        if check := self.volume_min <= volume <= self.volume_max:
             return check, volume
-        if not check and volume < self.volume_min:
-            return check, self.volume_min
         else:
-            return check, self.volume_max
+            return check, self.volume_min if volume <= self.volume_min else self.volume_max
 
-    def round_off_volume(self, volume: float, round_down: bool = True) -> float:
+    def round_off_volume(self, volume: float, round_down: bool = False) -> float:
         """Round off the volume to the nearest volume step.
 
         Args:
             volume (float): Volume to round off
             round_down (bool): If True, round down. If False, round up. Optional unnamed parameter. Defaults to True.
 
         Returns:
@@ -222,15 +219,15 @@
 
         Args:
             amount: amount to convert given in terms of the quote currency
             base: The base currency of the pair
             quote: The quote currency of the pair
 
         Returns:
-            float: Amount in terms of the base currency
+            float: Amount in terms of the quote currency
 
         Raises:
             ValueError: If conversion is impossible
         """
         try:
             pair = f'{base}{quote}'
             if self.account.has_symbol(pair):
```

### Comparing `aiomql-3.21/src/aiomql/terminal.py` & `aiomql-3.22/src/aiomql/terminal.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/ticks.py` & `aiomql-3.22/src/aiomql/ticks.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/trade_records.py` & `aiomql-3.22/src/aiomql/trade_records.py`

 * *Files identical despite different names*

### Comparing `aiomql-3.21/src/aiomql/utils.py` & `aiomql-3.22/src/aiomql/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Returns:
         str: The string representation of the dict.
     """
     sep = '\n' if multi else ', '
     return f"{sep}".join(f"{key}: {value}" for key, value in data.items())
 
 
-def round_off(value: float, step: float, round_down: bool = True) -> float:
+def round_off(value: float, step: float, round_down: bool = False) -> float:
     """Round off a number to the nearest step."""
     with decimal.localcontext() as ctx:
         ctx.rounding = decimal.ROUND_DOWN if round_down else decimal.ROUND_UP
         return float(decimal.Decimal(str(value)).quantize(decimal.Decimal(str(step))))
 
 
 def find_bearish_fractal(candles: Candles) -> Candle | None:
```

### Comparing `aiomql-3.21/src/aiomql.egg-info/PKG-INFO` & `aiomql-3.22/src/aiomql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 3.21
+Version: 3.22
 Summary: Asynchronous MetaTrader5 library and Algorithmic Trading Framework
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiomql-3.21/src/aiomql.egg-info/SOURCES.txt` & `aiomql-3.22/src/aiomql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

