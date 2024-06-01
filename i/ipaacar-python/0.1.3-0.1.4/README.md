# Comparing `tmp/ipaacar_python-0.1.3.tar.gz` & `tmp/ipaacar_python-0.1.4.tar.gz`

## Comparing `ipaacar_python-0.1.3.tar` & `ipaacar_python-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,61 @@
--rw-rw-rw-   0        0        0      737 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/Cargo.toml
--rw-rw-rw-   0        0        0        8 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/.gitignore
--rw-rw-rw-   0        0        0      198 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/README.md
--rw-rw-rw-   0        0        0     1483 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/examples/bad_ping.rs
--rw-rw-rw-   0        0        0     1319 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/examples/bad_pong.rs
--rw-rw-rw-   0        0        0     1304 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/backend/mod.rs
--rw-rw-rw-   0        0        0     5093 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/backend/mqtt.rs
--rw-rw-rw-   0        0        0     3310 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/async_utils.rs
--rw-rw-rw-   0        0        0     1925 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/buffer_iu_cb_manager.rs
--rw-rw-rw-   0        0        0     7810 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/input.rs
--rw-rw-rw-   0        0        0      872 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/mod.rs
--rw-rw-rw-   0        0        0     4478 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/output.rs
--rw-rw-rw-   0        0        0     1999 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/callback_list.rs
--rw-rw-rw-   0        0        0     4922 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/iu/core.rs
--rw-rw-rw-   0        0        0     3329 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/iu/links.rs
--rw-rw-rw-   0        0        0     9866 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/iu/mod.rs
--rw-rw-rw-   0        0        0       75 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/components/mod.rs
--rw-rw-rw-   0        0        0      766 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-core/src/lib.rs
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 ipaacar_python-0.1.3/ipaacar-python/Cargo.toml
--rw-rw-rw-   0        0        0      689 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/.gitignore
--rw-rw-rw-   0        0        0    14755 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/example.py
--rw-rw-rw-   0        0        0     7305 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/ipaaca_interface.py
--rw-rw-rw-   0        0        0      711 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/iu_new_perf.py
--rw-rw-rw-   0        0        0      711 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/iu_update_perf.py
--rw-rw-rw-   0        0        0      713 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/msg_perf.py
--rw-rw-rw-   0        0        0     1333 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/port/dummyPerception.py
--rw-rw-rw-   0        0        0      396 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/legacy/port/dummyReceiver.py
--rw-rw-rw-   0        0        0      850 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/messages/simple.py
--rw-rw-rw-   0        0        0      935 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_iu.py
--rw-rw-rw-   0        0        0     1014 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_msg_json.py
--rw-rw-rw-   0        0        0      950 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_msg_value.py
--rw-rw-rw-   0        0        0     1133 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_new_iu.py
--rw-rw-rw-   0        0        0     1987 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/multiple_buffer.py
--rw-rw-rw-   0        0        0     1529 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/parallel_ius.py
--rw-rw-rw-   0        0        0     2975 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/pingpong/ping.py
--rw-rw-rw-   0        0        0     1390 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/examples/pingpong/pong.py
--rw-rw-rw-   0        0        0     5895 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/components.pyi
--rw-rw-rw-   0        0        0      968 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/examples/__init__.py
--rw-rw-rw-   0        0        0      689 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/handler.py
--rw-rw-rw-   0        0        0     5949 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/legacy.py
--rw-rw-rw-   0        0        0     5117 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/performance_comparison/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/porting_old_code/__init__.py
--rw-rw-rw-   0        0        0        0 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/py.typed
--rw-rw-rw-   0        0        0     9443 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/src/input_buffer.rs
--rw-rw-rw-   0        0        0    16732 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/src/iu.rs
--rw-rw-rw-   0        0        0     3337 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/src/lib.rs
--rw-rw-rw-   0        0        0     6318 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/src/output_buffer.rs
--rw-rw-rw-   0        0        0     1174 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/ipaacar-python/test/run_doctests.py
--rw-rw-rw-   0        0        0    30160 2024-04-10 09:47:20.000000 ipaacar_python-0.1.3/Cargo.lock
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 ipaacar_python-0.1.3/Cargo.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 ipaacar_python-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     2189 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/python/ipaacar/components.pyi
--rw-rw-rw-   0        0        0      689 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/python/ipaacar/handler.py
--rw-rw-rw-   0        0        0     5949 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/python/ipaacar/legacy.py
--rw-rw-rw-   0        0        0        0 2023-09-19 08:50:58.000000 ipaacar_python-0.1.3/python/ipaacar/py.typed
--rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 ipaacar_python-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-06-01 14:34:44.000000 ipaacar_python-0.1.4/ipaacar-core/Cargo.toml
+-rw-rw-rw-   0        0        0        8 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/.gitignore
+-rw-rw-rw-   0        0        0      121 2024-06-01 14:34:44.000000 ipaacar_python-0.1.4/ipaacar-core/README.md
+-rw-rw-rw-   0        0        0     1483 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/examples/bad_ping.rs
+-rw-rw-rw-   0        0        0     1319 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/examples/bad_pong.rs
+-rw-rw-rw-   0        0        0     1304 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/backend/mod.rs
+-rw-rw-rw-   0        0        0     5093 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/backend/mqtt.rs
+-rw-rw-rw-   0        0        0     3310 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/async_utils.rs
+-rw-rw-rw-   0        0        0     1925 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/buffer_iu_cb_manager.rs
+-rw-rw-rw-   0        0        0     7810 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/input.rs
+-rw-rw-rw-   0        0        0      872 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/mod.rs
+-rw-rw-rw-   0        0        0     4478 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/output.rs
+-rw-rw-rw-   0        0        0     1999 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/callback_list.rs
+-rw-rw-rw-   0        0        0     4922 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/iu/core.rs
+-rw-rw-rw-   0        0        0     3329 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/iu/links.rs
+-rw-rw-rw-   0        0        0     9866 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/iu/mod.rs
+-rw-rw-rw-   0        0        0       75 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/components/mod.rs
+-rw-rw-rw-   0        0        0      766 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-core/src/lib.rs
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 ipaacar_python-0.1.4/ipaacar-python/Cargo.toml
+-rw-rw-rw-   0        0        0      689 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/.gitignore
+-rw-r--r--   0        0        0    35073 2024-06-01 15:24:35.000000 ipaacar_python-0.1.4/ipaacar-python/LICENSE
+-rw-r--r--   0        0        0     3265 2024-06-01 15:24:35.000000 ipaacar_python-0.1.4/ipaacar-python/README.md
+-rw-rw-rw-   0        0        0    14755 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/example.py
+-rw-rw-rw-   0        0        0     7305 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/ipaaca_interface.py
+-rw-rw-rw-   0        0        0      711 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/iu_new_perf.py
+-rw-rw-rw-   0        0        0      711 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/iu_update_perf.py
+-rw-rw-rw-   0        0        0      713 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/msg_perf.py
+-rw-rw-rw-   0        0        0     1333 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/port/dummyPerception.py
+-rw-rw-rw-   0        0        0      396 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/legacy/port/dummyReceiver.py
+-rw-rw-rw-   0        0        0      850 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/messages/simple.py
+-rw-rw-rw-   0        0        0      935 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_iu.py
+-rw-rw-rw-   0        0        0     1014 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_msg_json.py
+-rw-rw-rw-   0        0        0      950 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_msg_value.py
+-rw-rw-rw-   0        0        0     1133 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_new_iu.py
+-rw-rw-rw-   0        0        0     1987 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/multiple_buffer.py
+-rw-rw-rw-   0        0        0     1529 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/parallel_ius.py
+-rw-rw-rw-   0        0        0     2975 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/pingpong/ping.py
+-rw-rw-rw-   0        0        0     1390 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/examples/pingpong/pong.py
+-rw-rw-rw-   0        0        0     5895 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/components.pyi
+-rw-rw-rw-   0        0        0      968 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/examples/__init__.py
+-rw-rw-rw-   0        0        0      689 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/handler.py
+-rw-rw-rw-   0        0        0     5949 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/legacy.py
+-rw-rw-rw-   0        0        0     5117 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/performance_comparison/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/porting_old_code/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/py.typed
+-rw-rw-rw-   0        0        0     9443 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/src/input_buffer.rs
+-rw-rw-rw-   0        0        0    16732 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/src/iu.rs
+-rw-rw-rw-   0        0        0     3337 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/src/lib.rs
+-rw-rw-rw-   0        0        0     6318 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/src/output_buffer.rs
+-rw-rw-rw-   0        0        0     1174 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/ipaacar-python/test/run_doctests.py
+-rw-rw-rw-   0        0        0    30160 2024-06-01 15:24:36.000000 ipaacar_python-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 ipaacar_python-0.1.4/Cargo.toml
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 ipaacar_python-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     2189 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/python/ipaacar/components.pyi
+-rw-rw-rw-   0        0        0      689 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/python/ipaacar/handler.py
+-rw-rw-rw-   0        0        0     5949 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/python/ipaacar/legacy.py
+-rw-rw-rw-   0        0        0        0 2023-09-19 08:50:59.000000 ipaacar_python-0.1.4/python/ipaacar/py.typed
+-rw-r--r--   0        0        0     3265 2024-06-01 15:24:35.000000 ipaacar_python-0.1.4/README.md
+-rw-r--r--   0        0        0    35073 2024-06-01 15:24:35.000000 ipaacar_python-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 ipaacar_python-0.1.4/PKG-INFO
```

### Comparing `ipaacar_python-0.1.3/ipaacar-core/Cargo.toml` & `ipaacar_python-0.1.4/ipaacar-core/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ipaacar-core"
-version = "0.1.2"
+version = "0.1.4"
 edition = "2021"
 authors = ["David Schwab <david-schwab@uni-bielefeld.de>"]
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "ipaacar_core"
 path = "src/lib.rs"
```

### Comparing `ipaacar_python-0.1.3/ipaacar-core/examples/bad_ping.rs` & `ipaacar_python-0.1.4/ipaacar-core/examples/bad_ping.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/examples/bad_pong.rs` & `ipaacar_python-0.1.4/ipaacar-core/examples/bad_pong.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/backend/mod.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/backend/mqtt.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/backend/mqtt.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/async_utils.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/async_utils.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/buffer_iu_cb_manager.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/buffer_iu_cb_manager.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/input.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/input.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/mod.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/mod.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/buffer/output.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/buffer/output.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/callback_list.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/callback_list.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/iu/core.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/iu/core.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/iu/links.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/iu/links.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/components/iu/mod.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/components/iu/mod.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-core/src/lib.rs` & `ipaacar_python-0.1.4/ipaacar-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/Cargo.toml` & `ipaacar_python-0.1.4/ipaacar-python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ipaacar-python"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 authors = ["AG-SCS"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 # this needs to match the function name in lib.rs
 name = "ipaacar"
```

### Comparing `ipaacar_python-0.1.3/ipaacar-python/.gitignore` & `ipaacar_python-0.1.4/ipaacar-python/.gitignore`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/example.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/example.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/ipaaca_interface.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/ipaaca_interface.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/iu_new_perf.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/iu_new_perf.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/iu_update_perf.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/iu_update_perf.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/msg_perf.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/msg_perf.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/legacy/port/dummyPerception.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/legacy/port/dummyPerception.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/messages/simple.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/messages/simple.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_iu.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_iu.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_msg_json.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_msg_json.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_msg_value.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_msg_value.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/comp_new_iu.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/comp_new_iu.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/multiple_buffer.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/multiple_buffer.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/performance_tests/parallel_ius.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/performance_tests/parallel_ius.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/pingpong/ping.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/pingpong/ping.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/examples/pingpong/pong.py` & `ipaacar_python-0.1.4/ipaacar-python/examples/pingpong/pong.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/__init__.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/__init__.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/components.pyi` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/components.pyi`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/examples/__init__.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/handler.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/handler.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/legacy.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/legacy.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/performance_comparison/__init__.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/performance_comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/python/ipaacar/porting_old_code/__init__.py` & `ipaacar_python-0.1.4/ipaacar-python/python/ipaacar/porting_old_code/__init__.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/src/input_buffer.rs` & `ipaacar_python-0.1.4/ipaacar-python/src/input_buffer.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/src/iu.rs` & `ipaacar_python-0.1.4/ipaacar-python/src/iu.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/src/lib.rs` & `ipaacar_python-0.1.4/ipaacar-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/src/output_buffer.rs` & `ipaacar_python-0.1.4/ipaacar-python/src/output_buffer.rs`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/ipaacar-python/test/run_doctests.py` & `ipaacar_python-0.1.4/ipaacar-python/test/run_doctests.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/Cargo.lock` & `ipaacar_python-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipaacar-core"
-version = "0.1.2"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "async-trait",
  "bytes",
  "env_logger",
  "futures",
  "log",
@@ -380,15 +380,15 @@
  "tokio",
  "tokio-util",
  "uuid",
 ]
 
 [[package]]
 name = "ipaacar-python"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "ipaacar-core",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "serde_json",
```

### Comparing `ipaacar_python-0.1.3/python/ipaacar/components.pyi` & `ipaacar_python-0.1.4/python/ipaacar/components.pyi`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/python/ipaacar/handler.py` & `ipaacar_python-0.1.4/python/ipaacar/handler.py`

 * *Files identical despite different names*

### Comparing `ipaacar_python-0.1.3/python/ipaacar/legacy.py` & `ipaacar_python-0.1.4/python/ipaacar/legacy.py`

 * *Files identical despite different names*

