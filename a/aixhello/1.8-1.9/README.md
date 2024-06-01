# Comparing `tmp/aixhello-1.8.tar.gz` & `tmp/aixhello-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-1.8.tar", last modified: Sat Jun  1 21:20:36 2024, max compression
+gzip compressed data, was "aixhello-1.9.tar", last modified: Sat Jun  1 21:33:36 2024, max compression
```

## Comparing `aixhello-1.8.tar` & `aixhello-1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.355423 aixhello-1.8/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.8/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 21:20:36.354415 aixhello-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.339161 aixhello-1.8/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.8/aixhello/__init__.py
--rw-rw-rw-   0        0        0   423382 2024-06-01 21:17:13.000000 aixhello-1.8/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.353161 aixhello-1.8/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 21:20:36.357421 aixhello-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 21:19:18.000000 aixhello-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:33:36.018268 aixhello-1.9/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.9/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:33:36.018268 aixhello-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:33:35.994260 aixhello-1.9/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.9/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   423631 2024-06-01 21:33:30.000000 aixhello-1.9/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 21:33:36.016272 aixhello-1.9/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 21:33:35.000000 aixhello-1.9/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 21:33:36.022263 aixhello-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 21:32:43.000000 aixhello-1.9/setup.py
```

### Comparing `aixhello-1.8/LICENSE` & `aixhello-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-1.8/PKG-INFO` & `aixhello-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.8
+Version: 1.9
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.8/aixhello/xyello.c` & `aixhello-1.9/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -1865,14 +1865,18 @@
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
+/* unicode_iter.proto */
+static CYTHON_INLINE int __Pyx_init_unicode_iteration(
+    PyObject* ustring, Py_ssize_t *length, void** data, int *kind);
+
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -2312,15 +2316,15 @@
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -4030,35 +4034,36 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_text_chunks, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud = {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_text_chunks, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
+  PyObject *__pyx_v_text_chunks = 0;
   PyObject *__pyx_v_text_key = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[1] = {0};
+  PyObject* values[2] = {0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("Embedshroud (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
@@ -4066,87 +4071,112 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text_key,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text_chunks,&__pyx_n_s_text_key,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_chunks)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 2, 2, 1); __PYX_ERR(0, 48, __pyx_L3_error)
+        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Embedshroud") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 1)) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_text_key = values[0];
+    __pyx_v_text_chunks = ((PyObject*)values[0]);
+    __pyx_v_text_key = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 48, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 48, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_text_chunks), __pyx_v_text_key);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyUnicode_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
-  PyObject *__pyx_v_chunk = NULL;
+  Py_UCS4 __pyx_v_chunk;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  void *__pyx_t_5;
+  int __pyx_t_6;
   int __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Embedshroud", 1);
 
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -4154,130 +4184,87 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_embeddings = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  if (likely(PyList_CheckExact(((PyObject *)__pyx_v_text_chunks))) || PyTuple_CheckExact(((PyObject *)__pyx_v_text_chunks))) {
-    __pyx_t_1 = ((PyObject *)__pyx_v_text_chunks); __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_text_chunks)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-          #endif
-          if (__pyx_t_2 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-        #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-          #endif
-          if (__pyx_t_2 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-        #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 51, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_create); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-
-    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_INCREF(__pyx_v_chunk);
-    __Pyx_GIVEREF(__pyx_v_chunk);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_input, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(__pyx_v_text_chunks == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
+    __PYX_ERR(0, 51, __pyx_L1_error)
+  }
+  __Pyx_INCREF(__pyx_v_text_chunks);
+  __pyx_t_2 = __pyx_v_text_chunks;
+  __pyx_t_7 = __Pyx_init_unicode_iteration(__pyx_t_2, (&__pyx_t_4), (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
+  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_4; __pyx_t_8++) {
+    __pyx_t_3 = __pyx_t_8;
+    __pyx_v_chunk = __Pyx_PyUnicode_READ(__pyx_t_6, __pyx_t_5, __pyx_t_3);
 
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_embedding); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __pyx_t_9 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+
+    __pyx_t_10 = __Pyx_PyUnicode_FromOrdinal(__pyx_v_chunk); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = PyList_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_GIVEREF(__pyx_t_10);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_11, 0, __pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error);
+    __pyx_t_10 = 0;
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_input, __pyx_t_11) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_11);
+    __pyx_t_11 = 0;
+
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_11, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_embedding); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_11);
+    __pyx_t_11 = 0;
 
+    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_embeddings);
   __pyx_r = __pyx_v_embeddings;
   goto __pyx_L0;
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
-  __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5186,18 +5173,18 @@
   __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   __pyx_tuple__8 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  __pyx_tuple__10 = PyTuple_Pack(6, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 48, __pyx_L1_error)
 
   __pyx_tuple__12 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
   __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 16, __pyx_L1_error)
@@ -6926,14 +6913,34 @@
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
+/* unicode_iter */
+static CYTHON_INLINE int __Pyx_init_unicode_iteration(
+    PyObject* ustring, Py_ssize_t *length, void** data, int *kind) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    *kind   = 0;
+    *length = PyUnicode_GetLength(ustring);
+    *data   = (void*)ustring;
+#elif CYTHON_PEP393_ENABLED
+    if (unlikely(__Pyx_PyUnicode_READY(ustring) < 0)) return -1;
+    *kind   = PyUnicode_KIND(ustring);
+    *length = PyUnicode_GET_LENGTH(ustring);
+    *data   = PyUnicode_DATA(ustring);
+#else
+    *kind   = 0;
+    *length = PyUnicode_GET_SIZE(ustring);
+    *data   = (void*)PyUnicode_AS_UNICODE(ustring);
+#endif
+    return 0;
+}
+
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
```

### Comparing `aixhello-1.8/aixhello.egg-info/PKG-INFO` & `aixhello-1.9/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 1.8
+Version: 1.9
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-1.8/setup.py` & `aixhello-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='1.8',  # Increment the version number
+    version='1.9',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

