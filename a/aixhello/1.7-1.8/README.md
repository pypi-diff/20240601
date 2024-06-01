# Comparing `tmp/aixhello-1.7.tar.gz` & `tmp/aixhello-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-1.7.tar", last modified: Fri May 31 19:12:23 2024, max compression
+gzip compressed data, was "aixhello-1.8.tar", last modified: Sat Jun  1 21:20:36 2024, max compression
```

## Comparing `aixhello-1.7.tar` & `aixhello-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 19:12:23.328455 aixhello-1.7/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.7/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      627 2024-05-31 19:12:23.328455 aixhello-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 19:12:23.307422 aixhello-1.7/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.7/aixhello/__init__.py
--rw-rw-rw-   0        0        0   404337 2024-05-31 19:12:15.000000 aixhello-1.7/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-05-31 19:12:23.326422 aixhello-1.7/aixhello.egg-info/
--rw-rw-rw-   0        0        0      627 2024-05-31 19:12:23.000000 aixhello-1.7/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-31 19:12:23.000000 aixhello-1.7/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 19:12:23.000000 aixhello-1.7/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-31 19:12:23.000000 aixhello-1.7/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 19:12:23.000000 aixhello-1.7/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-31 19:12:23.330788 aixhello-1.7/setup.cfg
--rw-rw-rw-   0        0        0      984 2024-05-31 18:59:59.000000 aixhello-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.355423 aixhello-1.8/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-1.8/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:20:36.354415 aixhello-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.339161 aixhello-1.8/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-1.8/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   423382 2024-06-01 21:17:13.000000 aixhello-1.8/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 21:20:36.353161 aixhello-1.8/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 21:20:36.000000 aixhello-1.8/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 21:20:36.357421 aixhello-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 21:19:18.000000 aixhello-1.8/setup.py
```

### Comparing `aixhello-1.7/LICENSE` & `aixhello-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-1.7/aixhello/xyello.c` & `aixhello-1.8/aixhello/xyello.c`

 * *Files 2% similar despite different names*

```diff
@@ -1856,14 +1856,44 @@
 
 /* SliceObject.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
         PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
+/* PyObjectSetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+#else
+#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
+#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#endif
+
+/* ListAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
+        Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
+        PyList_SET_ITEM(list, len, x);
+        #endif
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
+#endif
+
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* RaiseUnexpectedTypeError.proto */
@@ -2179,106 +2209,120 @@
 /* #### Code section: string_decls ### */
 static const char __pyx_k__2[] = ".";
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__16[] = "?";
+static const char __pyx_k__18[] = "?";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_post[] = "post";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
+static const char __pyx_k_chunk[] = "chunk";
+static const char __pyx_k_input[] = "input";
+static const char __pyx_k_model[] = "model";
 static const char __pyx_k_modes[] = "modes";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_Cipher[] = "Cipher";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_cipher[] = "cipher";
+static const char __pyx_k_create[] = "create";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_xyellw[] = "xyellw";
+static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
-static const char __pyx_k_decrypt[] = "decrypt";
 static const char __pyx_k_disable[] = "disable";
-static const char __pyx_k_encrypt[] = "encrypt";
 static const char __pyx_k_message[] = "message";
-static const char __pyx_k_say_msg[] = "say_msg";
 static const char __pyx_k_strText[] = "strText";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_requests[] = "requests";
 static const char __pyx_k_response[] = "response";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_text_key[] = "text_key";
+static const char __pyx_k_Decenigma[] = "Decenigma";
+static const char __pyx_k_Decipherx[] = "Decipherx";
+static const char __pyx_k_Encapseal[] = "Encapseal";
 static const char __pyx_k_b64decode[] = "b64decode";
 static const char __pyx_k_b64encode[] = "b64encode";
 static const char __pyx_k_decryptor[] = "decryptor";
+static const char __pyx_k_embedding[] = "embedding";
 static const char __pyx_k_encryptor[] = "encryptor";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_algorithms[] = "algorithms";
+static const char __pyx_k_embeddings[] = "embeddings";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_Embedshroud[] = "Embedshroud";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
+static const char __pyx_k_text_chunks[] = "text_chunks";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_decryptedText[] = "decryptedText";
 static const char __pyx_k_encryptedText[] = "encryptedText";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
-static const char __pyx_k_xyellw_decrypt[] = "xyellw.decrypt";
-static const char __pyx_k_xyellw_encrypt[] = "xyellw.encrypt";
-static const char __pyx_k_xyellw_say_msg[] = "xyellw.say_msg";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
 static const char __pyx_k_default_backend[] = "default_backend";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN=VKM";
+static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
+static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
+static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
+static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_xyellw_Embedshroud[] = "xyellw.Embedshroud";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
+static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
-static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z?U8rS5jN@PvE4W7F&J(=DhN";
+static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_say_msg(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2encrypt(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4decrypt(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2307,68 +2351,78 @@
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   PyTypeObject *__pyx_ptype_8aixhello_6xyello_xyellw;
   PyObject *__pyx_n_s_AES;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
+  PyObject *__pyx_n_s_Decenigma;
+  PyObject *__pyx_n_s_Decipherx;
+  PyObject *__pyx_n_s_Embedshroud;
+  PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
-  PyObject *__pyx_n_s__16;
+  PyObject *__pyx_n_s__18;
   PyObject *__pyx_kp_u__2;
   PyObject *__pyx_n_s__3;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
+  PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_n_s_api_url;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b64decode;
   PyObject *__pyx_n_s_b64encode;
   PyObject *__pyx_n_s_backend;
   PyObject *__pyx_n_s_base64;
   PyObject *__pyx_n_s_chr;
+  PyObject *__pyx_n_s_chunk;
   PyObject *__pyx_n_s_cipher;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_create;
   PyObject *__pyx_n_s_cryptography_hazmat_backends;
   PyObject *__pyx_n_s_cryptography_hazmat_primitives_c;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_decode;
   PyObject *__pyx_n_s_decoded_encryptedText;
-  PyObject *__pyx_n_s_decrypt;
   PyObject *__pyx_n_s_decryptedText;
   PyObject *__pyx_n_s_decrypted_padded_text;
   PyObject *__pyx_n_s_decryptor;
   PyObject *__pyx_n_s_default_backend;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_embedding;
+  PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encoded_url;
-  PyObject *__pyx_n_s_encrypt;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_input;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_iv;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_u_message;
+  PyObject *__pyx_n_s_model;
   PyObject *__pyx_n_s_modes;
   PyObject *__pyx_n_s_msg;
   PyObject *__pyx_n_s_mth;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
+  PyObject *__pyx_n_s_openai;
   PyObject *__pyx_n_s_pad_length;
   PyObject *__pyx_n_s_padded_text;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_post;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
@@ -2376,50 +2430,55 @@
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_xyellw;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_requests;
   PyObject *__pyx_n_s_response;
-  PyObject *__pyx_n_s_say_msg;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
+  PyObject *__pyx_n_s_text_chunks;
+  PyObject *__pyx_kp_u_text_embedding_ada_002;
+  PyObject *__pyx_n_s_text_key;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_xyellw;
+  PyObject *__pyx_n_s_xyellw_Decenigma;
+  PyObject *__pyx_n_s_xyellw_Decipherx;
+  PyObject *__pyx_n_s_xyellw_Embedshroud;
+  PyObject *__pyx_n_s_xyellw_Encapseal;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
-  PyObject *__pyx_n_s_xyellw_decrypt;
-  PyObject *__pyx_n_s_xyellw_encrypt;
-  PyObject *__pyx_n_s_xyellw_say_msg;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__12;
   PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__16;
   PyObject *__pyx_codeobj__5;
   PyObject *__pyx_codeobj__7;
   PyObject *__pyx_codeobj__9;
   PyObject *__pyx_codeobj__11;
   PyObject *__pyx_codeobj__13;
   PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__17;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2459,68 +2518,78 @@
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_AES);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decenigma);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__16);
+  Py_CLEAR(clear_module_state->__pyx_n_s__18);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
+  Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_base64);
   Py_CLEAR(clear_module_state->__pyx_n_s_chr);
+  Py_CLEAR(clear_module_state->__pyx_n_s_chunk);
   Py_CLEAR(clear_module_state->__pyx_n_s_cipher);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_decoded_encryptedText);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decrypt);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_padded_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
-  Py_CLEAR(clear_module_state->__pyx_n_s_encrypt);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_input);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_iv);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_u_message);
+  Py_CLEAR(clear_module_state->__pyx_n_s_model);
   Py_CLEAR(clear_module_state->__pyx_n_s_modes);
   Py_CLEAR(clear_module_state->__pyx_n_s_msg);
   Py_CLEAR(clear_module_state->__pyx_n_s_mth);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
+  Py_CLEAR(clear_module_state->__pyx_n_s_openai);
   Py_CLEAR(clear_module_state->__pyx_n_s_pad_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_padded_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_post);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
@@ -2528,50 +2597,55 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_requests);
   Py_CLEAR(clear_module_state->__pyx_n_s_response);
-  Py_CLEAR(clear_module_state->__pyx_n_s_say_msg);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_text_chunks);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_text_embedding_ada_002);
+  Py_CLEAR(clear_module_state->__pyx_n_s_text_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Embedshroud);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_decrypt);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_encrypt);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_say_msg);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__12);
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
   Py_CLEAR(clear_module_state->__pyx_codeobj__7);
   Py_CLEAR(clear_module_state->__pyx_codeobj__9);
   Py_CLEAR(clear_module_state->__pyx_codeobj__11);
   Py_CLEAR(clear_module_state->__pyx_codeobj__13);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2589,68 +2663,78 @@
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_AES);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decenigma);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__16);
+  Py_VISIT(traverse_module_state->__pyx_n_s__18);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
+  Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_base64);
   Py_VISIT(traverse_module_state->__pyx_n_s_chr);
+  Py_VISIT(traverse_module_state->__pyx_n_s_chunk);
   Py_VISIT(traverse_module_state->__pyx_n_s_cipher);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_decoded_encryptedText);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decrypt);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_padded_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
-  Py_VISIT(traverse_module_state->__pyx_n_s_encrypt);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_input);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_iv);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_u_message);
+  Py_VISIT(traverse_module_state->__pyx_n_s_model);
   Py_VISIT(traverse_module_state->__pyx_n_s_modes);
   Py_VISIT(traverse_module_state->__pyx_n_s_msg);
   Py_VISIT(traverse_module_state->__pyx_n_s_mth);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
+  Py_VISIT(traverse_module_state->__pyx_n_s_openai);
   Py_VISIT(traverse_module_state->__pyx_n_s_pad_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_padded_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_post);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
@@ -2658,50 +2742,55 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_requests);
   Py_VISIT(traverse_module_state->__pyx_n_s_response);
-  Py_VISIT(traverse_module_state->__pyx_n_s_say_msg);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_text_chunks);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_text_embedding_ada_002);
+  Py_VISIT(traverse_module_state->__pyx_n_s_text_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Embedshroud);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_decrypt);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_encrypt);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_say_msg);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__12);
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
   Py_VISIT(traverse_module_state->__pyx_codeobj__7);
   Py_VISIT(traverse_module_state->__pyx_codeobj__9);
   Py_VISIT(traverse_module_state->__pyx_codeobj__11);
   Py_VISIT(traverse_module_state->__pyx_codeobj__13);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2729,68 +2818,78 @@
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_type_8aixhello_6xyello_xyellw
 #endif
 #define __pyx_ptype_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello_xyellw
 #define __pyx_n_s_AES __pyx_mstate_global->__pyx_n_s_AES
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
+#define __pyx_n_s_Decenigma __pyx_mstate_global->__pyx_n_s_Decenigma
+#define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
+#define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
+#define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
-#define __pyx_n_s__16 __pyx_mstate_global->__pyx_n_s__16
+#define __pyx_n_s__18 __pyx_mstate_global->__pyx_n_s__18
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
+#define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b64decode __pyx_mstate_global->__pyx_n_s_b64decode
 #define __pyx_n_s_b64encode __pyx_mstate_global->__pyx_n_s_b64encode
 #define __pyx_n_s_backend __pyx_mstate_global->__pyx_n_s_backend
 #define __pyx_n_s_base64 __pyx_mstate_global->__pyx_n_s_base64
 #define __pyx_n_s_chr __pyx_mstate_global->__pyx_n_s_chr
+#define __pyx_n_s_chunk __pyx_mstate_global->__pyx_n_s_chunk
 #define __pyx_n_s_cipher __pyx_mstate_global->__pyx_n_s_cipher
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_create __pyx_mstate_global->__pyx_n_s_create
 #define __pyx_n_s_cryptography_hazmat_backends __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_backends
 #define __pyx_n_s_cryptography_hazmat_primitives_c __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_primitives_c
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
 #define __pyx_n_s_decoded_encryptedText __pyx_mstate_global->__pyx_n_s_decoded_encryptedText
-#define __pyx_n_s_decrypt __pyx_mstate_global->__pyx_n_s_decrypt
 #define __pyx_n_s_decryptedText __pyx_mstate_global->__pyx_n_s_decryptedText
 #define __pyx_n_s_decrypted_padded_text __pyx_mstate_global->__pyx_n_s_decrypted_padded_text
 #define __pyx_n_s_decryptor __pyx_mstate_global->__pyx_n_s_decryptor
 #define __pyx_n_s_default_backend __pyx_mstate_global->__pyx_n_s_default_backend
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
+#define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
-#define __pyx_n_s_encrypt __pyx_mstate_global->__pyx_n_s_encrypt
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_input __pyx_mstate_global->__pyx_n_s_input
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_iv __pyx_mstate_global->__pyx_n_s_iv
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_u_message __pyx_mstate_global->__pyx_n_u_message
+#define __pyx_n_s_model __pyx_mstate_global->__pyx_n_s_model
 #define __pyx_n_s_modes __pyx_mstate_global->__pyx_n_s_modes
 #define __pyx_n_s_msg __pyx_mstate_global->__pyx_n_s_msg
 #define __pyx_n_s_mth __pyx_mstate_global->__pyx_n_s_mth
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
+#define __pyx_n_s_openai __pyx_mstate_global->__pyx_n_s_openai
 #define __pyx_n_s_pad_length __pyx_mstate_global->__pyx_n_s_pad_length
 #define __pyx_n_s_padded_text __pyx_mstate_global->__pyx_n_s_padded_text
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_post __pyx_mstate_global->__pyx_n_s_post
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
@@ -2798,63 +2897,68 @@
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_xyellw __pyx_mstate_global->__pyx_n_s_pyx_unpickle_xyellw
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_requests __pyx_mstate_global->__pyx_n_s_requests
 #define __pyx_n_s_response __pyx_mstate_global->__pyx_n_s_response
-#define __pyx_n_s_say_msg __pyx_mstate_global->__pyx_n_s_say_msg
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
+#define __pyx_n_s_text_chunks __pyx_mstate_global->__pyx_n_s_text_chunks
+#define __pyx_kp_u_text_embedding_ada_002 __pyx_mstate_global->__pyx_kp_u_text_embedding_ada_002
+#define __pyx_n_s_text_key __pyx_mstate_global->__pyx_n_s_text_key
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
+#define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
+#define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
+#define __pyx_n_s_xyellw_Embedshroud __pyx_mstate_global->__pyx_n_s_xyellw_Embedshroud
+#define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
-#define __pyx_n_s_xyellw_decrypt __pyx_mstate_global->__pyx_n_s_xyellw_decrypt
-#define __pyx_n_s_xyellw_encrypt __pyx_mstate_global->__pyx_n_s_xyellw_encrypt
-#define __pyx_n_s_xyellw_say_msg __pyx_mstate_global->__pyx_n_s_xyellw_say_msg
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1say_msg(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_1say_msg = {"say_msg", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1say_msg, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1say_msg(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx = {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_msg = 0;
@@ -2864,15 +2968,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("say_msg (wrapper)", 0);
+  __Pyx_RefNannySetupContext("Decipherx (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -2890,46 +2994,46 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_msg)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 8, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "say_msg") < 0)) __PYX_ERR(0, 8, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decipherx") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_msg = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("say_msg", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 8, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Decipherx", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.say_msg", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Decipherx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), (&PyUnicode_Type), 1, "msg", 1))) __PYX_ERR(0, 8, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_say_msg(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_msg);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), (&PyUnicode_Type), 1, "msg", 1))) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_msg);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -2938,36 +3042,36 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_say_msg(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg) {
   PyObject *__pyx_v_encoded_url = NULL;
   PyObject *__pyx_v_api_url = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("say_msg", 1);
+  __Pyx_RefNannySetupContext("Decipherx", 1);
 
   __Pyx_INCREF(__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   __pyx_v_encoded_url = __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -2980,19 +3084,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_encoded_url};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
@@ -3005,82 +3109,82 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_api_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_api_url);
   __Pyx_GIVEREF(__pyx_v_api_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_api_url)) __PYX_ERR(0, 12, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_api_url)) __PYX_ERR(0, 13, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_message, __pyx_v_msg) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_3) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_message, __pyx_v_msg) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_response = __pyx_t_3;
   __pyx_t_3 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.say_msg", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Decipherx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_encoded_url);
   __Pyx_XDECREF(__pyx_v_api_url);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_3encrypt(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_3encrypt = {"encrypt", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3encrypt, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_3encrypt(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal = {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_strText = 0;
@@ -3090,15 +3194,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("encrypt (wrapper)", 0);
+  __Pyx_RefNannySetupContext("Encapseal (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -3116,46 +3220,46 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_strText)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encrypt") < 0)) __PYX_ERR(0, 15, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Encapseal") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_strText = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encrypt", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 15, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Encapseal", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 16, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.encrypt", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Encapseal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_strText), (&PyUnicode_Type), 1, "strText", 1))) __PYX_ERR(0, 15, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_2encrypt(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_strText);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_strText), (&PyUnicode_Type), 1, "strText", 1))) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_strText);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -3164,15 +3268,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2encrypt(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText) {
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_iv = NULL;
   PyObject *__pyx_v_mth = NULL;
   PyObject *__pyx_v_backend = NULL;
   PyObject *__pyx_v_cipher = NULL;
   PyObject *__pyx_v_encryptor = NULL;
   PyObject *__pyx_v_pad_length = NULL;
@@ -3186,25 +3290,25 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("encrypt", 1);
+  __Pyx_RefNannySetupContext("Encapseal", 1);
 
   __Pyx_INCREF(__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   __pyx_v_key = __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
 
   __Pyx_INCREF(__pyx_kp_b_y1c8_8BxP9XN_VKM);
   __pyx_v_iv = __pyx_kp_b_y1c8_8BxP9XN_VKM;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3217,22 +3321,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_key};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_mth = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -3244,26 +3348,26 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_backend = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -3276,38 +3380,38 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_iv};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_mth);
   __Pyx_GIVEREF(__pyx_v_mth);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 20, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 21, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cipher = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_encryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_encryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -3319,45 +3423,45 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_encryptor = __pyx_t_2;
   __pyx_t_2 = 0;
 
   if (unlikely(__pyx_v_strText == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 24, __pyx_L1_error)
+    __PYX_ERR(0, 25, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_strText); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t((16 - __Pyx_mod_Py_ssize_t(__pyx_t_6, 16))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_strText); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t((16 - __Pyx_mod_Py_ssize_t(__pyx_t_6, 16))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_pad_length = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_v_pad_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_v_pad_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_strText, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_strText, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_padded_text = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_padded_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_padded_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
@@ -3369,15 +3473,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
@@ -3392,19 +3496,19 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_5};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
@@ -3416,29 +3520,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_encryptedText = __pyx_t_5;
   __pyx_t_5 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
@@ -3451,19 +3555,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_encryptedText};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
@@ -3476,15 +3580,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
@@ -3492,15 +3596,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.encrypt", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Encapseal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_iv);
   __Pyx_XDECREF(__pyx_v_mth);
   __Pyx_XDECREF(__pyx_v_backend);
   __Pyx_XDECREF(__pyx_v_cipher);
@@ -3511,23 +3615,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_5decrypt(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_5decrypt = {"decrypt", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5decrypt, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_5decrypt(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma = {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_encryptedText = 0;
@@ -3537,15 +3641,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decrypt (wrapper)", 0);
+  __Pyx_RefNannySetupContext("Decenigma (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -3563,46 +3667,46 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_encryptedText)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decrypt") < 0)) __PYX_ERR(0, 30, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decenigma") < 0)) __PYX_ERR(0, 31, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_encryptedText = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decrypt", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 30, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Decenigma", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 31, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.decrypt", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Decenigma", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encryptedText), (&PyUnicode_Type), 1, "encryptedText", 1))) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_4decrypt(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_encryptedText);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encryptedText), (&PyUnicode_Type), 1, "encryptedText", 1))) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_encryptedText);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -3611,15 +3715,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4decrypt(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText) {
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_iv = NULL;
   PyObject *__pyx_v_mth = NULL;
   PyObject *__pyx_v_backend = NULL;
   PyObject *__pyx_v_cipher = NULL;
   PyObject *__pyx_v_decryptor = NULL;
   PyObject *__pyx_v_decoded_encryptedText = NULL;
@@ -3632,25 +3736,25 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decrypt", 1);
+  __Pyx_RefNannySetupContext("Decenigma", 1);
 
   __Pyx_INCREF(__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   __pyx_v_key = __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
 
   __Pyx_INCREF(__pyx_kp_b_y1c8_8BxP9XN_VKM);
   __pyx_v_iv = __pyx_kp_b_y1c8_8BxP9XN_VKM;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3663,22 +3767,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_key};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_mth = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -3690,26 +3794,26 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_backend = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -3722,38 +3826,38 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_iv};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_mth);
   __Pyx_GIVEREF(__pyx_v_mth);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 35, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 36, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cipher = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_decryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_decryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -3765,24 +3869,24 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_decryptor = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -3795,22 +3899,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_encryptedText};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_v_decoded_encryptedText = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
@@ -3822,19 +3926,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_decoded_encryptedText};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
@@ -3846,40 +3950,40 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_decrypted_padded_text = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_decrypted_padded_text, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_decrypted_padded_text, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_pad_length = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = PyNumber_Negative(__pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Negative(__pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_decrypted_padded_text, 0, 0, NULL, &__pyx_t_3, NULL, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_decrypted_padded_text, 0, 0, NULL, &__pyx_t_3, NULL, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_decryptedText = __pyx_t_5;
   __pyx_t_5 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptedText, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptedText, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -3891,30 +3995,30 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.decrypt", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Decenigma", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_iv);
   __Pyx_XDECREF(__pyx_v_mth);
   __Pyx_XDECREF(__pyx_v_backend);
   __Pyx_XDECREF(__pyx_v_cipher);
@@ -3926,23 +4030,272 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_text_chunks, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud = {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_text_chunks, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_text_key = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("Embedshroud (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text_key,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Embedshroud") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_text_key = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 48, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_text_chunks), __pyx_v_text_key);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
+  PyObject *__pyx_v_embeddings = NULL;
+  PyObject *__pyx_v_chunk = NULL;
+  PyObject *__pyx_v_response = NULL;
+  PyObject *__pyx_v_embedding = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("Embedshroud", 1);
+
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_api_key, __pyx_v_text_key) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_embeddings = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  if (likely(PyList_CheckExact(((PyObject *)__pyx_v_text_chunks))) || PyTuple_CheckExact(((PyObject *)__pyx_v_text_chunks))) {
+    __pyx_t_1 = ((PyObject *)__pyx_v_text_chunks); __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_text_chunks)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 51, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_create); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+
+    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_INCREF(__pyx_v_chunk);
+    __Pyx_GIVEREF(__pyx_v_chunk);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_input, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_6);
+    __pyx_t_6 = 0;
+
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_embedding); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_6);
+    __pyx_t_6 = 0;
+
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
+
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_embeddings);
+  __pyx_r = __pyx_v_embeddings;
+  goto __pyx_L0;
+
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_embeddings);
+  __Pyx_XDECREF(__pyx_v_chunk);
+  __Pyx_XDECREF(__pyx_v_response);
+  __Pyx_XDECREF(__pyx_v_embedding);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -3959,22 +4312,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -4092,23 +4445,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -4174,28 +4527,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
@@ -4570,19 +4923,20 @@
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
     if (tp_free) tp_free(o);
   }
   #endif
 }
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
-  {"say_msg", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1say_msg, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"encrypt", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3encrypt, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"decrypt", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5decrypt, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_8aixhello_6xyello_xyellw_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello_xyellw},
   {Py_tp_methods, (void *)__pyx_methods_8aixhello_6xyello_xyellw},
   {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello_xyellw},
@@ -4694,68 +5048,78 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_AES, __pyx_k_AES, sizeof(__pyx_k_AES), 0, 0, 1, 1},
     {&__pyx_n_s_CBC, __pyx_k_CBC, sizeof(__pyx_k_CBC), 0, 0, 1, 1},
     {&__pyx_n_s_Cipher, __pyx_k_Cipher, sizeof(__pyx_k_Cipher), 0, 0, 1, 1},
+    {&__pyx_n_s_Decenigma, __pyx_k_Decenigma, sizeof(__pyx_k_Decenigma), 0, 0, 1, 1},
+    {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
+    {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
+    {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 0, 1, 1},
+    {&__pyx_n_s__18, __pyx_k__18, sizeof(__pyx_k__18), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
+    {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
     {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
     {&__pyx_n_s_backend, __pyx_k_backend, sizeof(__pyx_k_backend), 0, 0, 1, 1},
     {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
     {&__pyx_n_s_chr, __pyx_k_chr, sizeof(__pyx_k_chr), 0, 0, 1, 1},
+    {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
     {&__pyx_n_s_cipher, __pyx_k_cipher, sizeof(__pyx_k_cipher), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_backends, __pyx_k_cryptography_hazmat_backends, sizeof(__pyx_k_cryptography_hazmat_backends), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_k_cryptography_hazmat_primitives_c, sizeof(__pyx_k_cryptography_hazmat_primitives_c), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
     {&__pyx_n_s_decoded_encryptedText, __pyx_k_decoded_encryptedText, sizeof(__pyx_k_decoded_encryptedText), 0, 0, 1, 1},
-    {&__pyx_n_s_decrypt, __pyx_k_decrypt, sizeof(__pyx_k_decrypt), 0, 0, 1, 1},
     {&__pyx_n_s_decryptedText, __pyx_k_decryptedText, sizeof(__pyx_k_decryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_decrypted_padded_text, __pyx_k_decrypted_padded_text, sizeof(__pyx_k_decrypted_padded_text), 0, 0, 1, 1},
     {&__pyx_n_s_decryptor, __pyx_k_decryptor, sizeof(__pyx_k_decryptor), 0, 0, 1, 1},
     {&__pyx_n_s_default_backend, __pyx_k_default_backend, sizeof(__pyx_k_default_backend), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
+    {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
-    {&__pyx_n_s_encrypt, __pyx_k_encrypt, sizeof(__pyx_k_encrypt), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_iv, __pyx_k_iv, sizeof(__pyx_k_iv), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_u_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 1, 0, 1},
+    {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
     {&__pyx_n_s_modes, __pyx_k_modes, sizeof(__pyx_k_modes), 0, 0, 1, 1},
     {&__pyx_n_s_msg, __pyx_k_msg, sizeof(__pyx_k_msg), 0, 0, 1, 1},
     {&__pyx_n_s_mth, __pyx_k_mth, sizeof(__pyx_k_mth), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
+    {&__pyx_n_s_openai, __pyx_k_openai, sizeof(__pyx_k_openai), 0, 0, 1, 1},
     {&__pyx_n_s_pad_length, __pyx_k_pad_length, sizeof(__pyx_k_pad_length), 0, 0, 1, 1},
     {&__pyx_n_s_padded_text, __pyx_k_padded_text, sizeof(__pyx_k_padded_text), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_post, __pyx_k_post, sizeof(__pyx_k_post), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
@@ -4763,84 +5127,92 @@
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_xyellw, __pyx_k_pyx_unpickle_xyellw, sizeof(__pyx_k_pyx_unpickle_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_requests, __pyx_k_requests, sizeof(__pyx_k_requests), 0, 0, 1, 1},
     {&__pyx_n_s_response, __pyx_k_response, sizeof(__pyx_k_response), 0, 0, 1, 1},
-    {&__pyx_n_s_say_msg, __pyx_k_say_msg, sizeof(__pyx_k_say_msg), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
+    {&__pyx_n_s_text_chunks, __pyx_k_text_chunks, sizeof(__pyx_k_text_chunks), 0, 0, 1, 1},
+    {&__pyx_kp_u_text_embedding_ada_002, __pyx_k_text_embedding_ada_002, sizeof(__pyx_k_text_embedding_ada_002), 0, 1, 0, 0},
+    {&__pyx_n_s_text_key, __pyx_k_text_key, sizeof(__pyx_k_text_key), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_Embedshroud, __pyx_k_xyellw_Embedshroud, sizeof(__pyx_k_xyellw_Embedshroud), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_decrypt, __pyx_k_xyellw_decrypt, sizeof(__pyx_k_xyellw_decrypt), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_encrypt, __pyx_k_xyellw_encrypt, sizeof(__pyx_k_xyellw_encrypt), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_say_msg, __pyx_k_xyellw_say_msg, sizeof(__pyx_k_xyellw_say_msg), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 26, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_say_msg, 8, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  __pyx_tuple__6 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_encrypt, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  __pyx_tuple__8 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_decrypt, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  __pyx_tuple__10 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(6, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 48, __pyx_L1_error)
 
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 16, __pyx_L1_error)
+
+  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -4897,35 +5269,35 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8aixhello_6xyello_xyellw = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello_xyellw_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello_xyellw)) __PYX_ERR(0, 6, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello_xyellw_spec, __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_ptype_8aixhello_6xyello_xyellw = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello_xyellw_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello_xyellw)) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello_xyellw_spec, __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   #else
   __pyx_ptype_8aixhello_6xyello_xyellw = &__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8aixhello_6xyello_xyellw->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8aixhello_6xyello_xyellw->tp_dictoffset && __pyx_ptype_8aixhello_6xyello_xyellw->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8aixhello_6xyello_xyellw->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_xyellw, (PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_xyellw, (PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -5281,45 +5653,56 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_backend, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1say_msg, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_say_msg, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_openai, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_say_msg, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openai, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3encrypt, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_encrypt, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_encrypt, __pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5decrypt, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_decrypt, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_decrypt, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Embedshroud, __pyx_t_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6529,14 +6912,28 @@
     PyErr_Format(PyExc_TypeError,
         "'" __Pyx_FMT_TYPENAME "' object is unsliceable", obj_type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
 bad:
     return NULL;
 }
 
+/* PyObjectSetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_setattro))
+        return tp->tp_setattro(obj, attr_name, value);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_setattr))
+        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
+#endif
+    return PyObject_SetAttr(obj, attr_name, value);
+}
+#endif
+
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
@@ -9458,15 +9855,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__16);
+        name = __Pyx_NewRef(__pyx_n_s__18);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
```

### Comparing `aixhello-1.7/setup.py` & `aixhello-1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,27 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='1.7',  # Increment the version number
+    version='1.8',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=[
         'requests',  
         'cryptography',
+        'openai',
     ],
     ext_modules=cythonize(extensions, **cythonize_options),
     packages=['aixhello'],
 )
```

