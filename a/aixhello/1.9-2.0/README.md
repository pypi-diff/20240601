# Comparing `tmp/aixhello-1.9.tar.gz` & `tmp/aixhello-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-1.9.tar", last modified: Sat Jun  1 21:33:36 2024, max compression
+gzip compressed data, was "aixhello-2.0.tar", last modified: Sat Jun  1 21:39:51 2024, max compression
```

## Comparing `aixhello-1.9.tar` & `aixhello-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:33:36.018268 aixhello-1.9/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.9/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 21:33:36.018268 aixhello-1.9/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:33:35.994260 aixhello-1.9/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.9/aixhello/__init__.py
--rw-rw-rw-   0        0        0   423631 2024-06-01 21:33:30.000000 aixhello-1.9/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 21:33:36.016272 aixhello-1.9/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 21:33:36.022263 aixhello-1.9/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 21:32:43.000000 aixhello-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.544172 aixhello-2.0/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.0/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:39:51.543169 aixhello-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.525078 aixhello-2.0/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.0/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   422971 2024-06-01 21:39:43.000000 aixhello-2.0/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.542168 aixhello-2.0/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 21:39:51.545168 aixhello-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 21:39:18.000000 aixhello-2.0/setup.py
```

### Comparing `aixhello-1.9/LICENSE` & `aixhello-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-1.9/PKG-INFO` & `aixhello-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.9
+Version: 2.0
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.9/aixhello/xyello.c` & `aixhello-2.0/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -1865,18 +1865,14 @@
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
-/* unicode_iter.proto */
-static CYTHON_INLINE int __Pyx_init_unicode_iteration(
-    PyObject* ustring, Py_ssize_t *length, void** data, int *kind);
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -4131,15 +4127,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyUnicode_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyList_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
@@ -4152,31 +4148,25 @@
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
-  Py_UCS4 __pyx_v_chunk;
+  PyObject *__pyx_v_chunk = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  void *__pyx_t_5;
+  Py_ssize_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  int __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Embedshroud", 1);
 
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -4185,86 +4175,97 @@
 
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_embeddings = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   if (unlikely(__pyx_v_text_chunks == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 51, __pyx_L1_error)
   }
-  __Pyx_INCREF(__pyx_v_text_chunks);
-  __pyx_t_2 = __pyx_v_text_chunks;
-  __pyx_t_7 = __Pyx_init_unicode_iteration(__pyx_t_2, (&__pyx_t_4), (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
-  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_4; __pyx_t_8++) {
-    __pyx_t_3 = __pyx_t_8;
-    __pyx_v_chunk = __Pyx_PyUnicode_READ(__pyx_t_6, __pyx_t_5, __pyx_t_3);
+  __pyx_t_1 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  for (;;) {
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+      #endif
+      if (__pyx_t_2 >= __pyx_temp) break;
+    }
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+    #else
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    #endif
+    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_3);
+    __pyx_t_3 = 0;
 
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_openai); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_create); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    __pyx_t_9 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-
-    __pyx_t_10 = __Pyx_PyUnicode_FromOrdinal(__pyx_v_chunk); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_11 = PyList_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_GIVEREF(__pyx_t_10);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_11, 0, __pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error);
-    __pyx_t_10 = 0;
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_input, __pyx_t_11) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
 
-    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_11);
-    __pyx_t_11 = 0;
-
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_11, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_embedding); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_11);
-    __pyx_t_11 = 0;
+    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_INCREF(__pyx_v_chunk);
+    __Pyx_GIVEREF(__pyx_v_chunk);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_input, __pyx_t_5) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_5);
+    __pyx_t_5 = 0;
+
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embedding); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_5);
+    __pyx_t_5 = 0;
+
+    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
 
-    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_embeddings);
   __pyx_r = __pyx_v_embeddings;
   goto __pyx_L0;
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
+  __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6913,34 +6914,14 @@
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
-/* unicode_iter */
-static CYTHON_INLINE int __Pyx_init_unicode_iteration(
-    PyObject* ustring, Py_ssize_t *length, void** data, int *kind) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-    *kind   = 0;
-    *length = PyUnicode_GetLength(ustring);
-    *data   = (void*)ustring;
-#elif CYTHON_PEP393_ENABLED
-    if (unlikely(__Pyx_PyUnicode_READY(ustring) < 0)) return -1;
-    *kind   = PyUnicode_KIND(ustring);
-    *length = PyUnicode_GET_LENGTH(ustring);
-    *data   = PyUnicode_DATA(ustring);
-#else
-    *kind   = 0;
-    *length = PyUnicode_GET_SIZE(ustring);
-    *data   = (void*)PyUnicode_AS_UNICODE(ustring);
-#endif
-    return 0;
-}
-
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
```

### Comparing `aixhello-1.9/aixhello.egg-info/PKG-INFO` & `aixhello-2.0/aixhello.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.9
+Version: 2.0
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.9/setup.py` & `aixhello-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='1.9',  # Increment the version number
+    version='2.0',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

