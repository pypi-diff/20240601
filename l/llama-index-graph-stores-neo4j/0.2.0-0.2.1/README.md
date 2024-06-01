# Comparing `tmp/llama_index_graph_stores_neo4j-0.2.0.tar.gz` & `tmp/llama_index_graph_stores_neo4j-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_neo4j-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_neo4j-0.2.1.tar", max compression
```

## Comparing `llama_index_graph_stores_neo4j-0.2.0.tar` & `llama_index_graph_stores_neo4j-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       45 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/README.md
--rw-r--r--   0        0        0      188 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/__init__.py
--rw-r--r--   0        0        0     9432 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/base.py
--rw-r--r--   0        0        0    33442 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/neo4j_property_graph.py
--rw-r--r--   0        0        0     1499 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/README.md
+-rw-r--r--   0        0        0      188 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/__init__.py
+-rw-r--r--   0        0        0     9432 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/base.py
+-rw-r--r--   0        0        0    33593 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/neo4j_property_graph.py
+-rw-r--r--   0        0        0     1499 2024-06-01 19:48:31.027687 llama_index_graph_stores_neo4j-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.2.1/PKG-INFO
```

### Comparing `llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/base.py` & `llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/neo4j_property_graph.py` & `llama_index_graph_stores_neo4j-0.2.1/llama_index/graph_stores/neo4j/neo4j_property_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,16 +349,18 @@
         """
         cypher_statement += return_statement
 
         response = self.structured_query(cypher_statement, param_map=params)
 
         nodes = []
         for record in response:
-            if "text" in record["properties"]:
-                text = record["properties"].pop("text")
+            # text indicates a chunk node
+            # none on the type indicates an implicit node, likely a chunk node
+            if "text" in record["properties"] or record["type"] is None:
+                text = record["properties"].pop("text", "")
                 nodes.append(
                     ChunkNode(
                         id_=record["name"],
                         text=text,
                         properties=remove_empty_values(record["properties"]),
                     )
                 )
```

### Comparing `llama_index_graph_stores_neo4j-0.2.0/pyproject.toml` & `llama_index_graph_stores_neo4j-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores neo4j integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-neo4j"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.40"
 neo4j = "^5.16.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_graph_stores_neo4j-0.2.0/PKG-INFO` & `llama_index_graph_stores_neo4j-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-neo4j
-Version: 0.2.0
+Version: 0.2.1
 Summary: llama-index graph stores neo4j integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

