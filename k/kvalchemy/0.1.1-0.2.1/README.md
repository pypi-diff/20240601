# Comparing `tmp/kvalchemy-0.1.1.tar.gz` & `tmp/kvalchemy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.1.1.tar", last modified: Thu May 30 01:30:19 2024, max compression
+gzip compressed data, was "kvalchemy-0.2.1.tar", last modified: Sat Jun  1 18:34:21 2024, max compression
```

## Comparing `kvalchemy-0.1.1.tar` & `kvalchemy-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.764027 kvalchemy-0.1.1/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.723262 kvalchemy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:34:21.723262 kvalchemy-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_time.py
```

### Comparing `kvalchemy-0.1.1/LICENSE.md` & `kvalchemy-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.1.1/PKG-INFO` & `kvalchemy-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.1.1
+Version: 0.2.1
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -15,19 +15,25 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: backoff
 Requires-Dist: sqlalchemy
 Provides-Extra: dev
+Requires-Dist: func-timeout; extra == "dev"
+Requires-Dist: oracledb; extra == "dev"
+Requires-Dist: psycopg2-binary; extra == "dev"
 Requires-Dist: PyMySQL[rsa]; extra == "dev"
+Requires-Dist: pymssql; platform_system != "Darwin" and extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
 
@@ -77,10 +83,15 @@
 
 For example: Version 0.0.1 will be fully compatible with all releases in the 0.0.X family.
 Though Version 0.1.0 may not be directly compatible without a manual data migration.
 
 Make sure to pin the version family you want: kvalachemy<X.(Y+1).0
 ```
 
+## Testing
+KVAlchemy is tested across multiple database backends including MySQL, Postgres, SQLite, and Oracle.
+
+[![Run tests and release](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml)
+
 ## More Documentation
 
 For more documentation visit: https://csm10495.github.io/kvalchemy
```

### Comparing `kvalchemy-0.1.1/README.md` & `kvalchemy-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # KVAlchemy
 
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
 
@@ -53,10 +55,15 @@
 
 For example: Version 0.0.1 will be fully compatible with all releases in the 0.0.X family.
 Though Version 0.1.0 may not be directly compatible without a manual data migration.
 
 Make sure to pin the version family you want: kvalachemy<X.(Y+1).0
 ```
 
+## Testing
+KVAlchemy is tested across multiple database backends including MySQL, Postgres, SQLite, and Oracle.
+
+[![Run tests and release](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml)
+
 ## More Documentation
 
 For more documentation visit: https://csm10495.github.io/kvalchemy
```

### Comparing `kvalchemy-0.1.1/kvalchemy/client.py` & `kvalchemy-0.2.1/kvalchemy/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 log = logging.getLogger(__name__)
 
 
 retry_integrity_errors = backoff.on_exception(
     backoff.constant, IntegrityError, interval=0.1, max_time=30
 )
 
+DEFAULT_TAG = "__default__"
+
 
 class KVAlchemy:
     """
     Client for working with the key-value store.
     """
 
     def __init__(self, url: str, create_models: bool = True) -> None:
@@ -94,15 +96,15 @@
                     session.commit()
 
     @retry_integrity_errors
     def get(
         self,
         key: str,
         default: Any = ENOVAL,
-        tag: str = "",
+        tag: str = DEFAULT_TAG,
         return_expiration: bool = False,
     ) -> Any:
         """
         Retrieves the value for the given key and tag.
 
         If the key/tag combo is not found (or expired), and a default is provided, the
         default value is returned. If no default is provided, a KeyError is raised.
@@ -126,44 +128,48 @@
             if return_expiration:
                 return result.value, getattr(result, "expire", None)
 
             return result.value
 
     @retry_integrity_errors
     def set(
-        self, key: str, value: Any, tag: str = "", expire: ExpirationType = None
+        self,
+        key: str,
+        value: Any,
+        tag: str = DEFAULT_TAG,
+        expire: ExpirationType = None,
     ) -> None:
         """
         Sets the given key/tag combo to the value provided.
 
         If expire is provided, it must be something that can be processed by
         the to_expire function in kvalchemy.time.
         """
         with self.session() as session:
             session.merge(
                 KVStore(key=key, value=value, tag=tag, expire=to_expire(expire))
             )
 
     @retry_integrity_errors
-    def delete(self, key: str, tag: str = "") -> None:
+    def delete(self, key: str, tag: str = DEFAULT_TAG) -> None:
         """
         Deletes the given key/tag combo from the store.
         """
         with self.session() as session:
             query = (
                 session.query(KVStore)
                 .filter(KVStore.non_expired_filter())
                 .filter_by(key=key, tag=tag)
             )
             result = query.one_or_none()
 
             if result is not None:
                 session.delete(result)
 
-    def pop(self, key: str, default: Any = ENOVAL, tag: str = "") -> None:
+    def pop(self, key: str, default: Any = ENOVAL, tag: str = DEFAULT_TAG) -> None:
         """
         Pops the given key/tag combo from the store.
 
         If the key/tag combo is not found (or expired), and a default is provided, the
         default value is returned. If no default is provided, a KeyError is raised.
         """
         sentinel = object()
@@ -183,24 +189,26 @@
     def clear(self) -> None:
         """
         Clears all key-value pairs from the store.
         """
         with self.session() as session:
             session.query(KVStore).delete()
 
-    def get_proxy(self, key: str, default: Any = ENOVAL, tag: str = "") -> Proxy:
+    def get_proxy(
+        self, key: str, default: Any = ENOVAL, tag: str = DEFAULT_TAG
+    ) -> Proxy:
         """
         Returns a Proxy object for the given key, tag, default.
         """
         return Proxy(self, key, default, tag)
 
     @retry_integrity_errors
-    def delete_tag(self, tag: str) -> int:
+    def delete_tag(self, tag: str = DEFAULT_TAG) -> int:
         """
-        Deletes all keys under a given tag.
+        Deletes all keys under a given tag. Defaults to the default tag.
 
         Returns the number of keys deleted.
         """
         with self.session() as session:
             return session.query(KVStore).filter(KVStore.tag == tag).delete()
 
     def memoize(
```

### Comparing `kvalchemy-0.1.1/kvalchemy/models.py` & `kvalchemy-0.2.1/kvalchemy/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Home to models for KVAlchemy.
 """
 from datetime import datetime
 
-from sqlalchemy import Column, ColumnElement, UniqueConstraint, or_
+from sqlalchemy import Column, ColumnElement, PrimaryKeyConstraint, event, or_
 from sqlalchemy.dialects.mysql import LONGBLOB
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.types import LargeBinary, PickleType, Unicode
 
 from kvalchemy.time import db_now
 
 KEY_MAX_LENGTH = 256
@@ -38,18 +38,18 @@
 class KVStore(Base, ValueMixIn):
     """
     The table for storing key-value pairs.
     """
 
     __tablename__ = "kvstore"
 
-    __table_args__ = (UniqueConstraint("key", "tag", name="key_tag_unique"),)
+    __table_args__ = (PrimaryKeyConstraint("key", "tag", name="key_tag_unique"),)
 
-    key: Mapped[str] = Column(Unicode(KEY_MAX_LENGTH), primary_key=True)
-    tag: Mapped[str] = Column(Unicode(TAG_MAX_LENGTH), primary_key=True)
+    key: Mapped[str] = Column(Unicode(KEY_MAX_LENGTH))
+    tag: Mapped[str] = Column(Unicode(TAG_MAX_LENGTH))
 
     # Naive datetime (though expected to be UTC)
     expire: Mapped[datetime] = mapped_column(nullable=True)
 
     @classmethod
     def non_expired_filter(cls) -> ColumnElement[bool]:
         """
```

### Comparing `kvalchemy-0.1.1/kvalchemy/proxy.py` & `kvalchemy-0.2.1/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.1.1/kvalchemy/time.py` & `kvalchemy-0.2.1/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.1.1/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.2.1/kvalchemy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.1.1
+Version: 0.2.1
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -15,19 +15,25 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: backoff
 Requires-Dist: sqlalchemy
 Provides-Extra: dev
+Requires-Dist: func-timeout; extra == "dev"
+Requires-Dist: oracledb; extra == "dev"
+Requires-Dist: psycopg2-binary; extra == "dev"
 Requires-Dist: PyMySQL[rsa]; extra == "dev"
+Requires-Dist: pymssql; platform_system != "Darwin" and extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
 
@@ -77,10 +83,15 @@
 
 For example: Version 0.0.1 will be fully compatible with all releases in the 0.0.X family.
 Though Version 0.1.0 may not be directly compatible without a manual data migration.
 
 Make sure to pin the version family you want: kvalachemy<X.(Y+1).0
 ```
 
+## Testing
+KVAlchemy is tested across multiple database backends including MySQL, Postgres, SQLite, and Oracle.
+
+[![Run tests and release](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml/badge.svg)](https://github.com/csm10495/kvalchemy/actions/workflows/test_and_release.yml)
+
 ## More Documentation
 
 For more documentation visit: https://csm10495.github.io/kvalchemy
```

### Comparing `kvalchemy-0.1.1/pyproject.toml` & `kvalchemy-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 [project.urls]
 homepage = "https://github.com/csm10495/kvalchemy"
 repository = "https://github.com/csm10495/kvalchemy"
 documentation  = "https://csm10495.github.io/kvalchemy"
 
 [project.optional-dependencies]
 dev = [
+    "func-timeout",
+    'oracledb',
+    "psycopg2-binary",
     "PyMySQL[rsa]",
+    'pymssql; platform_system != "Darwin"',
     "pytest"
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `kvalchemy-0.1.1/tests/test_client.py` & `kvalchemy-0.2.1/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime, timedelta
 from unittest.mock import patch
 from uuid import UUID, uuid4
 
 import pytest
 
 from kvalchemy import KVAlchemy
+from kvalchemy.client import DEFAULT_TAG
 from kvalchemy.models import KVStore
 from kvalchemy.time import db_now
 
 
 @patch("kvalchemy.client.Base.metadata.create_all")
 def test_kvalchemy_init_create_all_true(mock_create_all):
     k = KVAlchemy("sqlite://", create_models=True)
@@ -37,43 +38,43 @@
 def test_session_commit_true_delete_expired_false(kvalchemy, kvstore):
     with kvalchemy.session(delete_expired=False) as session:
         session.add(kvstore)
         session.add(
             KVStore(
                 key="key2",
                 value="value2",
-                tag="",
+                tag=" ",
                 expire=(db_now() - timedelta(days=1)),
             )
         )
 
     with kvalchemy.session() as session:
-        result = session.query(KVStore).filter_by(key="key", tag="").one()
+        result = session.query(KVStore).filter_by(key="key", tag=" ").one()
         assert result.value == "value"
 
-        result = session.query(KVStore).filter_by(key="key2", tag="").one()
+        result = session.query(KVStore).filter_by(key="key2", tag=" ").one()
         assert result.value == "value2"
 
         assert session.query(KVStore).count() == 2
 
 
 def test_session_commit_true_delete_expired_true(kvalchemy, kvstore):
     with kvalchemy.session() as session:
         session.add(kvstore)
         session.add(
             KVStore(
                 key="key2",
                 value="value2",
-                tag="",
+                tag=" ",
                 expire=(db_now() - timedelta(days=1)),
             )
         )
 
     with kvalchemy.session() as session:
-        result = session.query(KVStore).filter_by(key="key", tag="").one()
+        result = session.query(KVStore).filter_by(key="key", tag=" ").one()
         assert result.value == "value"
         assert session.query(KVStore).count() == 1
 
 
 def test_session_access_thrash(kvalchemy):
     if "sqlite" in kvalchemy.url:
         pytest.skip("sqlite backend doesn't support multiple accesses at once")
@@ -96,15 +97,15 @@
 
 
 def test_session_commit_false(kvalchemy, kvstore):
     with kvalchemy.session(commit=False) as session:
         session.add(kvstore)
 
     with kvalchemy.session() as session:
-        result = session.query(KVStore).filter_by(key="key", tag="").one_or_none()
+        result = session.query(KVStore).filter_by(key="key", tag=" ").one_or_none()
         assert result is None
 
 
 def test_get_no_default(kvalchemy):
     with pytest.raises(KeyError):
         assert kvalchemy.get("key")
 
@@ -113,27 +114,27 @@
     assert kvalchemy.get("key", "lolcats") == "lolcats"
 
 
 def test_get_expired_no_default(kvalchemy):
     with kvalchemy.session() as session:
         session.add(
             KVStore(
-                key="key", value="value", tag="", expire=(db_now() - timedelta(days=1))
+                key="key", value="value", tag=" ", expire=(db_now() - timedelta(days=1))
             )
         )
 
     with pytest.raises(KeyError):
         kvalchemy.get("key")
 
 
 def test_get_expired_default(kvalchemy):
     with kvalchemy.session() as session:
         session.add(
             KVStore(
-                key="key", value="value", tag="", expire=(db_now() - timedelta(days=1))
+                key="key", value="value", tag=" ", expire=(db_now() - timedelta(days=1))
             )
         )
 
         assert kvalchemy.get("key", "lolcats") == "lolcats"
 
 
 def test_set_get(kvalchemy):
@@ -175,19 +176,19 @@
     kvalchemy.set("b", "value3", tag="tag")
 
     items = list(kvalchemy)
     assert len(items) == 3
 
     assert items[0].key == "a"
     assert items[0].value == "value"
-    assert items[0].tag == ""
+    assert items[0].tag == DEFAULT_TAG
 
     assert items[1].key == "b"
     assert items[1].value == "value2"
-    assert items[1].tag == ""
+    assert items[1].tag == DEFAULT_TAG
 
     assert items[2].key == "b"
     assert items[2].value == "value3"
     assert items[2].tag == "tag"
 
 
 def test_len(kvalchemy):
@@ -263,14 +264,23 @@
     assert kvalchemy.delete_tag("tag") == 2
     assert len(kvalchemy) == 1
     assert kvalchemy.delete_tag("tag2") == 1
     assert len(kvalchemy) == 0
     assert kvalchemy.delete_tag("tag3") == 0
 
 
+def test_delete_default_tag(kvalchemy):
+    kvalchemy.set("test", 123)
+    kvalchemy.set("hello", "world")
+    assert len(kvalchemy) == 2
+
+    assert kvalchemy.delete_tag() == 2
+    assert len(kvalchemy) == 0
+
+
 def test_memoize_simple(kvalchemy):
     global ret_val
 
     # with parenthesis
     ret_val = True
 
     @kvalchemy.memoize()
```

### Comparing `kvalchemy-0.1.1/tests/test_proxy.py` & `kvalchemy-0.2.1/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.1.1/tests/test_time.py` & `kvalchemy-0.2.1/tests/test_time.py`

 * *Files identical despite different names*

