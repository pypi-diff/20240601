# Comparing `tmp/qenerate_custom-0.6.4.tar.gz` & `tmp/qenerate_custom-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qenerate_custom-0.6.4.tar", max compression
+gzip compressed data, was "qenerate_custom-0.6.5.tar", max compression
```

## Comparing `qenerate_custom-0.6.4.tar` & `qenerate_custom-0.6.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11350 2024-01-28 03:42:33.193282 qenerate_custom-0.6.4/LICENSE
--rw-r--r--   0        0        0     6551 2024-02-19 04:06:37.654447 qenerate_custom-0.6.4/README.md
--rw-r--r--   0        0        0     1544 2024-05-30 01:42:14.782705 qenerate_custom-0.6.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/__init__.py
--rw-r--r--   0        0        0     1528 2024-02-19 04:11:27.322090 qenerate_custom-0.6.4/qenerate/cli.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/__init__.py
--rw-r--r--   0        0        0     3797 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/code_command.py
--rw-r--r--   0        0        0     2105 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/feature_flag_parser.py
--rw-r--r--   0        0        0      440 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/introspection_command.py
--rw-r--r--   0        0        0      856 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/plugin.py
--rw-r--r--   0        0        0     5302 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/preprocessor.py
--rw-r--r--   0        0        0     1652 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/core/unwrapper.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/__init__.py
--rw-r--r--   0        0        0     2123 2024-01-28 04:03:16.335007 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/mapper.py
--rw-r--r--   0        0        0    18838 2024-05-30 01:38:06.562076 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/plugin.py
--rw-r--r--   0        0        0     7188 2024-01-28 09:04:19.752624 qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/typed_ast.py
--rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 qenerate_custom-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11350 2024-01-28 03:42:33.193282 qenerate_custom-0.6.5/LICENSE
+-rw-r--r--   0        0        0     6551 2024-02-19 04:06:37.654447 qenerate_custom-0.6.5/README.md
+-rw-r--r--   0        0        0     1544 2024-06-01 04:10:26.574248 qenerate_custom-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/__init__.py
+-rw-r--r--   0        0        0     1528 2024-02-19 04:11:27.322090 qenerate_custom-0.6.5/qenerate/cli.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/__init__.py
+-rw-r--r--   0        0        0     3797 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/code_command.py
+-rw-r--r--   0        0        0     2105 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/feature_flag_parser.py
+-rw-r--r--   0        0        0      440 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/introspection_command.py
+-rw-r--r--   0        0        0      856 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/plugin.py
+-rw-r--r--   0        0        0     5302 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/preprocessor.py
+-rw-r--r--   0        0        0     1652 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/core/unwrapper.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-28 03:42:33.233283 qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0     2123 2024-06-01 04:08:17.734726 qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/mapper.py
+-rw-r--r--   0        0        0    18838 2024-05-30 01:38:06.562076 qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/plugin.py
+-rw-r--r--   0        0        0     7188 2024-01-28 09:04:19.752624 qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/typed_ast.py
+-rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 qenerate_custom-0.6.5/PKG-INFO
```

### Comparing `qenerate_custom-0.6.4/LICENSE` & `qenerate_custom-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/README.md` & `qenerate_custom-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/pyproject.toml` & `qenerate_custom-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qenerate-custom"
-version = "0.6.4"
+version = "0.6.5"
 description = "Code Generator for GraphQL Query and Fragment Data Classes"
 authors = ["Red Hat - Service Delivery - AppSRE <sd-app-sre@redhat.com>"]
 maintainers = ["Red Hat - Service Delivery - AppSRE <sd-app-sre@redhat.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/app-sre/qenerate"
 repository = "https://github.com/app-sre/qenerate"
 documentation = "https://github.com/app-sre/qenerate"
```

### Comparing `qenerate_custom-0.6.4/qenerate/cli.py` & `qenerate_custom-0.6.5/qenerate/cli.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/core/code_command.py` & `qenerate_custom-0.6.5/qenerate/core/code_command.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/core/feature_flag_parser.py` & `qenerate_custom-0.6.5/qenerate/core/feature_flag_parser.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/core/plugin.py` & `qenerate_custom-0.6.5/qenerate/core/plugin.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/core/preprocessor.py` & `qenerate_custom-0.6.5/qenerate/core/preprocessor.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/core/unwrapper.py` & `qenerate_custom-0.6.5/qenerate/core/unwrapper.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/mapper.py` & `qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "id": "q_id",
         "to": "q_to",
         "format": "q_format",
     }
     if s in keyword_remapping:
         return keyword_remapping[s]
     elif s.startswith("_"):
-        return f"m{s}"
+        return f"q{s}"
 
     return s
 
 
 def graphql_class_name_to_python(graphql_type: GraphQLOutputType) -> str:
     return graphql_class_name_str_to_python(str(graphql_type))
```

### Comparing `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/plugin.py` & `qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/plugin.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/qenerate/plugins/pydantic_v1/typed_ast.py` & `qenerate_custom-0.6.5/qenerate/plugins/pydantic_v1/typed_ast.py`

 * *Files identical despite different names*

### Comparing `qenerate_custom-0.6.4/PKG-INFO` & `qenerate_custom-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qenerate-custom
-Version: 0.6.4
+Version: 0.6.5
 Summary: Code Generator for GraphQL Query and Fragment Data Classes
 Home-page: https://github.com/app-sre/qenerate
 License: Apache-2.0
 Author: Red Hat - Service Delivery - AppSRE
 Author-email: sd-app-sre@redhat.com
 Maintainer: Red Hat - Service Delivery - AppSRE
 Maintainer-email: sd-app-sre@redhat.com
```

