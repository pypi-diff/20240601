# Comparing `tmp/wasmpy-build-0.5.1.tar.gz` & `tmp/wasmpy_build-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.5.1.tar", last modified: Fri Feb  9 18:49:19 2024, max compression
+gzip compressed data, was "wasmpy_build-0.5.2.tar", last modified: Sat Jun  1 01:25:59 2024, max compression
```

## Comparing `wasmpy-build-0.5.1.tar` & `wasmpy_build-0.5.2.tar`

### file list

```diff
@@ -1,1126 +1,1129 @@
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:19.041830 wasmpy-build-0.5.1/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       83 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/.gitignore
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       79 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/.gitmodules
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1068 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       27 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/MANIFEST.in
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2915 2024-02-09 18:49:19.037830 wasmpy-build-0.5.1/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      760 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/README.md
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      998 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/appveyor.yml
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      732 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/generate.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1135 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/pyproject.toml
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       38 2024-02-09 18:49:19.041830 wasmpy-build-0.5.1/setup.cfg
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.717821 wasmpy-build-0.5.1/wasmpy_build/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3039 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/__init__.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.713821 wasmpy-build-0.5.1/wasmpy_build/include/
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.745822 wasmpy-build-0.5.1/wasmpy_build/include/cp310/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3224 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      344 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/README.rst
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31405 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1224 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1484 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2593 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      720 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5703 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1657 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      318 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      520 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1806 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1962 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/context.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.753822 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14054 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      769 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4119 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1468 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7570 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2218 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3734 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      723 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4267 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3152 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1630 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7597 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      387 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1243 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1399 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19613 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3356 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/picklebufobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1093 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5476 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2095 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11914 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4811 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9196 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      506 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      404 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      975 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    44284 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9635 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3002 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3853 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1700 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      831 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/eval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/exports.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      508 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4360 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      337 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4257 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/genericaliasobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3347 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3026 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.769823 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2971 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28828 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6457 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_atomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5271 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      870 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_call.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3484 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      696 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1045 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      822 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      646 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1704 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_format.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6859 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_gc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_getopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3697 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5625 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9289 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_interp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      350 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_list.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2589 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1047 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5989 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      626 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_parser.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1981 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2314 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4940 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3211 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3938 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4902 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_runtime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      386 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5578 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      548 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2970 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      425 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_tuple.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      633 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      593 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1781 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8606 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2764 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4147 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10333 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2458 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/namespaceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28344 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8445 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5509 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1301 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2474 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12426 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4223 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2080 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8313 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3891 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31684 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5250 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystrhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1110 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5938 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3381 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2074 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1390 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2669 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      584 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1614 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2460 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    36148 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2863 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp310/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.789823 wasmpy-build-0.5.1/wasmpy_build/include/cp311/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2854 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      344 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/README.rst
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31404 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1212 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1462 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2617 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6255 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      520 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      724 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/complexobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.805824 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8229 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1305 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4568 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      723 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1239 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1656 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11484 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2218 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1248 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1959 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1642 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3324 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      818 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      702 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1108 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4424 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3279 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1526 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7817 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1769 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3817 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4532 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2556 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4303 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18305 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2998 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/picklebufobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3505 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1073 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4522 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      582 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2099 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14351 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4811 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1426 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12158 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1997 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      489 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1513 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    41910 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      560 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2103 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/weakrefobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9635 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1256 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3852 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1780 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/exports.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1570 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      507 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1530 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/genericaliasobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3025 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.825824 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3031 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29315 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6549 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_atomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6062 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1424 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3475 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_call.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4409 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15930 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1045 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2839 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1239 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5684 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_dict.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      704 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      842 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7403 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1307 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_format.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7567 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_frame.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      413 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_function.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6895 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_gc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1164 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_getopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1436 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12980 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3696 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      743 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5800 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6671 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_interp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1352 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_list.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3516 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1040 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      392 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_namespace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10037 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18986 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      626 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_parser.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2494 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3507 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9435 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3708 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4250 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5988 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_runtime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    49092 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_signal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_strhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      580 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5638 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      605 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3501 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2089 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_tuple.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1158 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1716 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      678 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      740 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      593 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1780 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3272 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      827 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2810 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5072 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6541 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2374 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29800 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8428 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11187 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2471 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5115 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pybuffer.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12782 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      551 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4154 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2249 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6064 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1979 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3890 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24452 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4635 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1189 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4833 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      851 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/pytypedefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1543 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2040 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1388 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1381 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2669 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      583 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1613 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2342 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    36032 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1129 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1226 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp311/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.845825 wasmpy-build-0.5.1/wasmpy_build/include/cp312/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2854 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      486 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/README.rst
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    32616 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1136 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1466 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2619 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6267 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      448 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      728 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/complexobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.861825 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7870 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1163 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4426 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1076 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1650 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2245 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16189 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2660 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1248 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1965 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1642 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4686 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      818 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      900 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1108 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7150 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3316 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1623 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7820 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      387 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1633 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4879 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4679 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2272 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2276 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4336 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21212 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3316 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1311 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      848 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/picklebufobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3505 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pthread_stubs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1413 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4276 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1479 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3423 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16921 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4903 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1426 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12375 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2146 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      489 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    34467 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      564 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2032 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/weakrefobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9769 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3080 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3860 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1779 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1267 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/exports.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1650 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      507 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1532 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/genericaliasobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3033 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.889826 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3035 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31288 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6749 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ast_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1149 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atexit.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atomic_funcs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6062 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bitutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_blocks_output_buffer.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1339 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3920 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_call.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5265 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ceval_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15835 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3453 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2839 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1301 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      499 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6384 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dict.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1095 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dict_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1626 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_emscripten_signal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      842 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_exceptions.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2220 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_faulthandler.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7910 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2724 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_fileutils_windows.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1578 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4630 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_flowgraph.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_format.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9256 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_frame.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_function.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7658 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_gc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1186 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_getopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3035 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_objects.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)   116175 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_objects_fini_generated.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    25665 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_strings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3742 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4286 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_hashtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6358 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5706 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2999 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_instruments.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9086 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_interp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1397 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_intrinsics.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1980 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_list.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7805 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      383 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1192 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      392 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_namespace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14429 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_object_state.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    27284 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_obmalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2085 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_obmalloc_init.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20081 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2686 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_opcode_utils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1358 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_parser.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pathconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2783 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      709 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3365 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8600 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3040 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2654 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymem_init.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4982 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2075 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_range.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8429 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6087 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime_init.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46045 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime_init_generated.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2611 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_signal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      414 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_strhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      923 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6828 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      734 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      388 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_time.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3050 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3501 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3075 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2197 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_tuple.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4669 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_typeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      763 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_typevarobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1966 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    91455 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unicodeobject_generated.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      682 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unionobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      740 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      333 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-02-09 18:49:08.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1782 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3275 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      827 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1081 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5076 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6515 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3559 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    37188 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9238 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12808 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2473 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5282 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pybuffer.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1727 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2404 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13017 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      551 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4154 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2249 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2810 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6318 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1688 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3914 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    25384 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4635 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2741 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystats.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1313 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4875 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      851 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/pytypedefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      630 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2518 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1645 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1398 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1729 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      585 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2192 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1615 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2342 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35164 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1129 2024-02-09 18:49:09.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1234 2024-02-09 18:49:10.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp312/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.917827 wasmpy-build-0.5.1/wasmpy_build/include/cp36/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12781 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22274 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/Python-ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3221 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    47451 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1016 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1213 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      477 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      792 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/bitset.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3191 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8363 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      701 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8524 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1666 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5945 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2164 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9414 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2964 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7178 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1497 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/eval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1651 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3524 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3530 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4079 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3583 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1966 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/graminit.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2074 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/grammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4233 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      513 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2900 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3761 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8471 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/metagrammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3847 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7317 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2285 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/namespaceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1007 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/node.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    40373 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14244 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1288 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5073 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      691 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2885 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/parsetok.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1130 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pgen.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1180 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pgenheaders.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4307 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8128 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyatomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1320 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      863 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1970 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17219 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8471 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      410 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pygetopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4139 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4078 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3500 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8557 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    27573 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11146 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      495 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystrhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6782 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2992 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7609 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3333 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2485 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2018 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1353 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4994 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1355 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1943 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3644 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2444 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    81779 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1693 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp36/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.949828 wasmpy-build-0.5.1/wasmpy_build/include/cp37/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12793 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21802 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/Python-ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3554 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    40798 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1016 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1213 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      641 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      810 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/bitset.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3301 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8493 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      713 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8717 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1679 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6065 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2946 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2014 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9848 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3135 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7323 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1695 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/eval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1811 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4534 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3318 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4178 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3646 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1992 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/graminit.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2319 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/grammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4977 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.953828 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1438 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2726 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      701 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1432 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3616 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      123 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/hash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      114 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6831 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/mem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/pygetopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4311 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      508 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2927 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8594 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/metagrammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4519 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8559 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2304 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/namespaceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1113 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/node.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    41842 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14474 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1280 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5109 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      691 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2905 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/parsetok.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pgen.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1222 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pgenheaders.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4062 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16121 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyatomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1320 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1214 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      969 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2285 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17369 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      341 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4139 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7780 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3535 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8993 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28235 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16324 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      495 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystrhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6204 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5332 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8926 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3362 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2480 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4928 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1511 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2480 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3644 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2471 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    82278 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp37/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.981829 wasmpy-build-0.5.1/wasmpy_build/include/cp38/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13937 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    26491 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/Python-ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3615 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30286 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1229 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      948 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      468 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/bitset.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3301 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8493 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      713 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8366 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1710 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7178 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3582 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2014 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/context.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.985829 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12294 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3845 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      721 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16028 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      456 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15691 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3600 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4717 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2263 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3511 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9810 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      547 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1036 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46308 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9260 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3019 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3716 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1695 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/eval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4352 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3317 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4200 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3720 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2118 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/graminit.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1821 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/grammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4926 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:18.993829 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16944 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_atomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      966 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      542 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      779 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1254 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_getopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1520 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3698 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5218 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2896 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2037 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1329 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3815 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8217 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9588 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3076 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      418 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      591 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2927 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9520 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4406 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9591 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2362 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/namespaceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1328 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/node.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29599 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10537 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1300 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5164 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2958 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/parsetok.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      847 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/picklebufobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2477 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1214 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12786 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      341 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4140 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2081 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3778 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5406 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30221 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4686 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystrhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7645 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5660 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8926 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3362 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2517 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5308 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2429 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      601 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1661 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35732 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp38/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:19.021830 wasmpy-build-0.5.1/wasmpy_build/include/cp39/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13937 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/LICENSE
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    26193 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/Python-ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3532 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/Python.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30476 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1224 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/asdl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      947 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/ast.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      468 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/bitset.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/bltinmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      885 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/boolobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1484 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3048 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      712 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cellobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5954 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1657 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/classobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      318 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/codecs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3778 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/compile.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1806 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/complexobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1962 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/context.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:19.029830 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14200 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      769 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4114 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/bytesobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1537 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6989 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3797 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      721 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4004 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3059 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1473 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      456 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1364 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1399 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19358 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4456 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5101 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2096 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3511 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10134 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      575 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1036 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46154 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9255 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/datetime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3019 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/descrobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3715 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/dictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/dynamic_annotations.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/enumobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1624 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/errcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/eval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/exports.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/fileobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4360 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/floatobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      337 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/frameobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4057 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/funcobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/genericaliasobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3525 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/genobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2118 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/graminit.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1821 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/grammar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3026 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/import.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:19.037830 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      953 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pegen_interface.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_abstract.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_accu.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16977 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_atomic.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2620 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      870 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_call.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3403 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_ceval.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      541 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_code.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_condvar.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      800 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_context.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      646 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1541 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6647 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_gc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_getopt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_gil.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3697 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_hamt.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_import.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5233 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5299 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_interp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_long.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4157 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1936 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2032 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3741 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3363 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3583 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4452 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_runtime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      548 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3056 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      442 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      633 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/interpreteridobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/intrcheck.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      521 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/iterobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1781 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/listobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/longintrepr.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9513 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/longobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/marshal.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2764 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/memoryobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3775 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/methodobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9959 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/modsupport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2361 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/moduleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/namespaceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1281 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/node.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24628 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/object.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8423 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/objimpl.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/odictobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4900 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/opcode.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/osdefs.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/osmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2958 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/parsetok.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/patchlevel.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/picklebufobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2474 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/py_curses.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyarena.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pycapsule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-02-09 18:47:11.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyctype.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1093 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydebug.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydtrace.d
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydtrace.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12427 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyerrors.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyexpat.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyfpe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyframe.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4263 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2136 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pylifecycle.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymacconfig.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymacro.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8580 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymath.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4406 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymem.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31273 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyport.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5250 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystate.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-02-09 18:49:01.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystrcmp.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystrhex.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystrtod.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7673 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pythonrun.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5938 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pythread.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8928 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/pytime.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/rangeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3324 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/setobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/sliceobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/structmember.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1390 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/structseq.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5307 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/symtable.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/sysmodule.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2642 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/token.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      584 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/traceback.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/tracemalloc.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1614 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/tupleobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2350 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/typeslots.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-02-09 18:49:05.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/ucnhash.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35426 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/unicodeobject.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-02-09 18:49:06.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/warnings.h
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2863 2024-02-09 18:49:07.000000 wasmpy-build-0.5.1/wasmpy_build/include/cp39/weakrefobject.h
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-02-09 18:49:19.037830 wasmpy-build-0.5.1/wasmpy_build.egg-info/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2915 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    47514 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/SOURCES.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/dependency_links.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       94 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/entry_points.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       22 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/requires.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)       13 2024-02-09 18:49:18.000000 wasmpy-build-0.5.1/wasmpy_build.egg-info/top_level.txt
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.279638 wasmpy_build-0.5.2/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       83 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/.gitignore
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       79 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/.gitmodules
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1068 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       27 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/MANIFEST.in
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3148 2024-06-01 01:25:59.279638 wasmpy_build-0.5.2/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      760 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/README.md
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      994 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/analyze.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      998 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/appveyor.yml
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      732 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/generate.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1374 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/pyproject.toml
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       38 2024-06-01 01:25:59.279638 wasmpy_build-0.5.2/setup.cfg
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:58.923620 wasmpy_build-0.5.2/wasmpy_build/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      124 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/cli.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2749 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/core.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:58.915619 wasmpy_build-0.5.2/wasmpy_build/include/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:58.951621 wasmpy_build-0.5.2/wasmpy_build/include/cp310/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3224 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      344 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/README.rst
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31405 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1224 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1484 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2593 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      720 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5703 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1657 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      318 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      520 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1806 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1962 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/context.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:58.963622 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14054 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      769 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4119 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1468 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7570 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2218 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3734 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      723 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4267 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3152 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1630 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7597 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      387 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1243 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1399 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19613 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3356 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/picklebufobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1093 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5476 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2095 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11914 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4811 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9196 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      506 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      404 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      975 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    44284 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9635 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3002 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3853 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1700 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      831 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/eval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/exports.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      508 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4360 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      337 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4257 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/genericaliasobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3347 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3026 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:58.979623 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2971 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28828 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6457 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_atomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5271 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      870 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_call.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3484 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      696 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1045 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      822 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      646 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1704 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_format.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6859 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_gc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_getopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3697 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5625 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9289 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_interp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      350 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_list.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2589 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1047 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5989 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      626 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_parser.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1981 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2314 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4940 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3211 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3938 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4902 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_runtime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      386 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5578 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      548 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2970 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      425 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_tuple.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      633 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      593 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1781 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8606 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2764 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4147 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10333 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2458 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/namespaceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28344 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8445 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5509 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1301 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2474 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12426 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4223 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2080 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8313 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3891 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31684 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5250 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystrhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1110 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5938 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3381 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2074 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1390 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2669 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      584 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1614 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2460 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    36148 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2863 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp310/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.003624 wasmpy_build-0.5.2/wasmpy_build/include/cp311/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2854 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      344 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/README.rst
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31404 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1212 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1462 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2617 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6255 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      520 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      724 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/complexobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.015625 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8229 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1305 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4568 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      723 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1239 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1656 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11484 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2218 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1248 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1959 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1642 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3324 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      818 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      702 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1108 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4424 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3279 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1526 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7817 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1769 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3817 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4532 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2556 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4303 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18305 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2998 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/picklebufobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3505 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1073 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4522 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      582 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2099 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14351 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4811 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1426 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12158 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1997 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      489 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1513 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    41910 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      560 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2103 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/weakrefobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9635 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1256 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3852 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1780 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/exports.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1570 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      507 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1530 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/genericaliasobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3025 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.043626 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3031 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29315 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6549 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_atomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6062 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1424 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3475 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_call.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4409 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15930 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1045 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2839 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1239 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5684 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_dict.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      704 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      842 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7403 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1307 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_format.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7567 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_frame.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      413 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_function.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6895 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_gc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1164 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_getopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1436 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12980 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3696 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      743 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5800 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6671 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_interp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1352 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_list.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3516 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1040 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      392 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_namespace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10037 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    18986 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      626 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_parser.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2494 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3507 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9435 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3708 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4250 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5988 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_runtime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    49092 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_signal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_strhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      580 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5638 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      605 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3501 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2089 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_tuple.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1158 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1716 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      678 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      740 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      593 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1780 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3272 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      827 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2810 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5072 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6541 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2374 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29800 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8428 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11187 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2471 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5115 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pybuffer.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12782 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      551 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4154 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2249 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6064 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1979 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3890 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24452 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4635 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1189 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4833 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      851 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/pytypedefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1543 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2040 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1388 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1381 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2669 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      583 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1613 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2342 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    36032 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1129 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1226 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp311/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.067627 wasmpy_build-0.5.2/wasmpy_build/include/cp312/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13936 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2854 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      486 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/README.rst
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    32616 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1136 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1466 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2619 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6267 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7071 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      448 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      728 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/complexobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.083628 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7870 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1163 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4426 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1076 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1650 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2245 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16189 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2660 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1248 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1965 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1642 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4686 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      818 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      232 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      900 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1108 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7150 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3316 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1623 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7820 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      387 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1633 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4879 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4679 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2272 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2276 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4336 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21212 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3316 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1311 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      848 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/picklebufobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3505 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pthread_stubs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1413 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4276 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1479 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3423 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3379 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16921 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4903 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1426 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12375 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2146 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      489 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    34467 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      564 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2032 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/weakrefobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9769 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3080 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3860 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22471 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1779 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1267 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/exports.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1650 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      507 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1532 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      336 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/genericaliasobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3033 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.111630 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3035 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31288 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6749 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ast_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1149 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atexit.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2438 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atomic_funcs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6062 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bitutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8688 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_blocks_output_buffer.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1339 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3920 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_call.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5265 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ceval_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15835 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3453 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2839 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1301 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      499 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6384 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dict.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1095 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dict_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1626 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      562 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_emscripten_signal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      842 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_exceptions.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2220 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_faulthandler.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7910 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2724 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_fileutils_windows.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1578 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4630 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_flowgraph.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      480 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_format.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9256 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_frame.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      611 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_function.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7658 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_gc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1186 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_getopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3035 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_objects.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)   116175 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_objects_fini_generated.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    25665 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_strings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3742 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4286 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_hashtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6358 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5706 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2999 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_instruments.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9086 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_interp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1397 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_intrinsics.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1980 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_list.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7805 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      383 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1192 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      392 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_namespace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14429 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_object_state.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    27284 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_obmalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2085 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_obmalloc_init.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    20081 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2686 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_opcode_utils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1358 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_parser.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      606 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pathconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2733 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2783 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      709 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3365 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8600 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3040 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2654 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymem_init.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4982 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2075 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      346 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_range.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8429 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6087 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime_init.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46045 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime_init_generated.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2611 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_signal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      414 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      937 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_strhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      923 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6828 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      734 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      388 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_time.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3050 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3501 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3075 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2197 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_tuple.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4669 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_typeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      763 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_typevarobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      898 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1966 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    91455 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unicodeobject_generated.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      682 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unionobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      740 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      333 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      772 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1782 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3275 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      827 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1081 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5076 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6515 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3559 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    37188 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9238 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12808 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2473 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5282 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pybuffer.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1727 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2404 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13017 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      551 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4154 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2249 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2810 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6318 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1688 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3914 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    25384 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4635 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2741 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystats.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1313 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4875 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      851 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/pytypedefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      630 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1557 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2518 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1645 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1398 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1729 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      585 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2192 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1615 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2342 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35164 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1129 2024-06-01 01:25:53.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1234 2024-06-01 01:25:54.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp312/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.147631 wasmpy_build-0.5.2/wasmpy_build/include/cp36/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12781 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22274 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/Python-ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3221 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    47451 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1016 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1213 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      477 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      792 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/bitset.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3191 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8363 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      701 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8524 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1666 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5945 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2164 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9414 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2964 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7178 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1497 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/eval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1651 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3524 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3530 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4079 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3583 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1966 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/graminit.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2074 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/grammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4233 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      513 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2900 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3761 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8471 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/metagrammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3847 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7317 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2285 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/namespaceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1007 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/node.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    40373 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14244 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1288 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5073 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      691 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2885 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/parsetok.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1130 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pgen.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1180 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pgenheaders.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4307 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8128 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyatomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1320 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      863 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1970 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17219 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8471 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      410 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pygetopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4139 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4078 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3500 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8557 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    27573 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    11146 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      495 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystrhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6782 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2992 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7609 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3333 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2485 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2018 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1353 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4994 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1355 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1943 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3644 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2444 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    81779 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1693 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp36/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.179633 wasmpy_build-0.5.2/wasmpy_build/include/cp37/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12793 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    21802 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/Python-ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3554 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    40798 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1016 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1213 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      641 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      810 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/bitset.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3301 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8493 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      713 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8717 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1679 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6065 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2946 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2014 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9848 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3135 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7323 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1695 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/eval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1811 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4534 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3318 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4178 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3646 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1992 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/graminit.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2319 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/grammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4977 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.183633 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1438 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2726 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      701 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1432 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3616 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      123 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/hash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      114 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6831 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/mem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/pygetopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4311 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      508 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2927 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8594 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/metagrammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4519 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8559 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2304 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/namespaceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1113 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/node.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    41842 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14474 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1280 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5109 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      691 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2905 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/parsetok.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pgen.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1222 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pgenheaders.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4062 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16121 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyatomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1320 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1214 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      969 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2285 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    17369 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      341 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4139 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7780 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3535 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8993 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    28235 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16324 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      495 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystrhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6204 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5332 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8926 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3362 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2480 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4928 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1511 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2480 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3644 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2471 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    82278 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp37/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.211635 wasmpy_build-0.5.2/wasmpy_build/include/cp38/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13937 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    26491 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/Python-ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3615 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30286 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1229 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      948 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      468 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/bitset.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      886 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2114 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3301 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8493 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      713 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8366 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1710 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7178 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3582 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1807 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2014 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/context.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.219635 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12294 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3845 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      721 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16028 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      456 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15691 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3600 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4717 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2263 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3511 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9810 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      547 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1036 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46308 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9260 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3019 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3716 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      458 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1695 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/eval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4352 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4794 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3317 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4200 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3720 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2118 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/graminit.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1821 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/grammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4926 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.227635 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16944 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_atomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      966 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      542 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      779 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1254 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_getopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1520 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3698 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5218 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2896 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2037 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1329 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3815 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8217 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9588 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3076 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      418 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      591 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      567 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2927 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9520 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2765 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4406 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9591 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2362 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/namespaceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1328 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/node.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    29599 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10537 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1300 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5164 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2958 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/parsetok.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      847 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/picklebufobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2477 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1726 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1214 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12786 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      341 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4140 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2081 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3778 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8312 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5406 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30221 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4686 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystrhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7645 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5660 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8926 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      629 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3362 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2517 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1377 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5308 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2429 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      601 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1661 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2253 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35732 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2866 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp38/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.259637 wasmpy_build-0.5.2/wasmpy_build/include/cp39/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13937 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    26193 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/Python-ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3532 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/Python.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    30476 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1224 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/asdl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      947 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/ast.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      468 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/bitset.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/bltinmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      885 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/boolobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1484 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3048 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      712 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cellobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5954 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1657 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/classobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      318 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6793 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/codecs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3778 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/compile.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1806 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/complexobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1962 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/context.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.267638 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14200 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      769 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4114 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/bytesobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1537 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6989 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3797 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      721 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4004 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3059 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1473 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16979 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      456 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1364 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1399 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19358 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4456 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5101 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2096 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3511 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10134 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      575 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1036 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    46154 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9255 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/datetime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3019 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/descrobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3715 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/dictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    22469 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/dynamic_annotations.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      253 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/enumobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1624 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/errcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/eval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1098 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/exports.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1571 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/fileobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      597 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4360 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/floatobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      337 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/frameobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4057 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/funcobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/genericaliasobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3525 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/genobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2118 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/graminit.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1821 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/grammar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3026 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/import.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.275638 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      953 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pegen_interface.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      479 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_abstract.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1126 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_accu.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16977 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_atomic.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3384 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2620 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      870 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_call.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3403 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_ceval.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      541 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_code.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2809 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_condvar.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      800 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_context.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      646 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1541 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6647 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_gc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      490 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_getopt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1565 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_gil.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3697 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_hamt.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4197 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      473 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_import.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5233 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5299 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_interp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1548 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_long.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4157 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1936 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2032 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      206 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3741 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3363 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3583 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4452 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_runtime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      548 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3056 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      442 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      633 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      334 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/interpreteridobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      861 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/intrcheck.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      521 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/iterobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1781 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/listobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3799 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/longintrepr.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9513 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/longobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      803 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/marshal.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2764 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/memoryobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3775 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/methodobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9959 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/modsupport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2361 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/moduleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      349 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/namespaceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1281 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/node.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24628 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/object.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8423 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/objimpl.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/odictobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4900 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/opcode.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      737 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/osdefs.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      291 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/osmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2958 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/parsetok.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1299 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/patchlevel.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      846 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/picklebufobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2474 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/py_curses.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2744 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyarena.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1725 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pycapsule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    48603 2024-06-01 01:23:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1387 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyctype.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1093 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydebug.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1008 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydtrace.d
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2413 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydtrace.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12427 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyerrors.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2450 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyexpat.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      444 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyfpe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      466 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyframe.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4263 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2136 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pylifecycle.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2989 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymacconfig.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4920 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymacro.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8580 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymath.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4406 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymem.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    31273 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyport.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5250 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystate.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      436 2024-06-01 01:25:44.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystrcmp.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      849 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystrhex.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1483 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystrtod.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     7673 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pythonrun.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5938 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pythread.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8928 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/pytime.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      628 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/rangeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3324 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/setobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2516 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/sliceobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2030 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/structmember.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1390 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/structseq.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5307 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/symtable.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1242 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/sysmodule.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2642 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/token.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      584 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/traceback.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1114 2024-06-01 01:25:51.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/tracemalloc.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1614 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/tupleobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2350 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/typeslots.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1056 2024-06-01 01:25:49.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/ucnhash.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    35426 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/unicodeobject.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1776 2024-06-01 01:25:50.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/warnings.h
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2863 2024-06-01 01:25:52.000000 wasmpy_build-0.5.2/wasmpy_build/include/cp39/weakrefobject.h
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2024-06-01 01:25:59.279638 wasmpy_build-0.5.2/wasmpy_build.egg-info/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3148 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    47566 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/SOURCES.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/dependency_links.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      145 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/entry_points.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       22 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/requires.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       13 2024-06-01 01:25:58.000000 wasmpy_build-0.5.2/wasmpy_build.egg-info/top_level.txt
```

### Comparing `wasmpy-build-0.5.1/LICENSE` & `wasmpy_build-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/PKG-INFO` & `wasmpy_build-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.5.1
+Version: 0.5.2
 Summary: WebAssembly build tool for CPython C/C++ extensions
 Author-email: Olivia Ryan <olivia.r.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Olivia Ryan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Issues, https://github.com/olivi-r/wasmpy-build/issues
+Project-URL: Repository, https://github.com/olivi-r/wasmpy-build
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: WebAssembly
```

### Comparing `wasmpy-build-0.5.1/README.md` & `wasmpy_build-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/appveyor.yml` & `wasmpy_build-0.5.2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/generate.py` & `wasmpy_build-0.5.2/generate.py`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/pyconfig.h` & `wasmpy_build-0.5.2/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/picklebufobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/cpython/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/eval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/exports.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_atomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_call.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_gc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_interp.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_parser.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_runtime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/internal/pycore_warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystrhex.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp310/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp310/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/picklebufobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pyframe.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/cpython/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/exports.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_atomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_call.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_dict.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_frame.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_gc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_interp.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_list.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_parser.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_runtime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_signal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_strhex.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_tuple.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/internal/pycore_warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pybuffer.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyframe.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/pytypedefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp311/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp311/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/picklebufobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pthread_stubs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pyframe.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/cpython/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/exports.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ast_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atexit.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atexit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_atomic_funcs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bitutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_blocks_output_buffer.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_call.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ceval_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ceval_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dict.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dict_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dict_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_dtoa.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_emscripten_signal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_exceptions.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_faulthandler.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_faulthandler.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_fileutils_windows.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_fileutils_windows.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_flowgraph.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_flowgraph.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_frame.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_function.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_function.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_gc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_objects.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_objects_fini_generated.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_objects_fini_generated.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_global_strings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_hashtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_instruments.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_instruments.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_interp.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_intrinsics.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_intrinsics.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_list.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_object_state.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_object_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_obmalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_obmalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_obmalloc_init.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_obmalloc_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_opcode_utils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_opcode_utils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_parser.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pathconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pymem_init.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pymem_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime_init.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_runtime_init_generated.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_runtime_init_generated.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_signal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_strhex.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_tuple.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_typeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_typevarobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_typevarobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unicodeobject_generated.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unicodeobject_generated.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_unionobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/internal/pycore_warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pybuffer.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyframe.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystats.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystats.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/pytypedefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp312/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp312/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/Python-ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/bitset.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/bitset.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/eval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/graminit.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/grammar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/node.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/parsetok.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pgenheaders.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pgenheaders.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyatomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyatomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyfpe.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyfpe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp36/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp36/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/Python-ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/bitset.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/bitset.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/eval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/graminit.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/grammar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/mem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/mem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/internal/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/internal/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/node.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/parsetok.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pgenheaders.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pgenheaders.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyatomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyatomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp37/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp37/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/Python-ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/cpython/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/eval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/graminit.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/grammar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_atomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/internal/pycore_warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/node.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/parsetok.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/picklebufobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystrhex.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp38/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp38/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/LICENSE` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/Python-ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/Python.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/asdl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/ast.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/boolobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cellobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/classobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/codecs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/compile.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/complexobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/abstract.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/bytesobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/frameobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/cpython/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/datetime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/descrobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/dictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/dynamic_annotations.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/errcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/eval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/exports.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/fileobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/floatobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/funcobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/genobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/graminit.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/grammar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/import.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pegen_interface.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pegen_interface.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_accu.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_atomic.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_call.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_ceval.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_code.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_condvar.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_context.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_gc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_gil.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_hamt.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_interp.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_long.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_runtime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/internal/pycore_warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/intrcheck.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/iterobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/listobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/longintrepr.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/longobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/marshal.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/memoryobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/methodobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/modsupport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/moduleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/node.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/object.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/objimpl.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/odictobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/opcode.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/osdefs.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/parsetok.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/patchlevel.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/picklebufobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/py_curses.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyarena.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pycapsule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyctype.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydebug.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydtrace.d` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pydtrace.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyerrors.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyexpat.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pylifecycle.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymacconfig.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymacro.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymath.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pymem.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pyport.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystate.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystrhex.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pystrtod.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pythonrun.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pythread.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/pytime.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/rangeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/setobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/sliceobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/structmember.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/structseq.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/symtable.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/sysmodule.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/token.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/traceback.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/tracemalloc.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/tupleobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/typeslots.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/ucnhash.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/unicodeobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/warnings.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build/include/cp39/weakrefobject.h` & `wasmpy_build-0.5.2/wasmpy_build/include/cp39/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.5.1/wasmpy_build.egg-info/PKG-INFO` & `wasmpy_build-0.5.2/wasmpy_build.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.5.1
+Version: 0.5.2
 Summary: WebAssembly build tool for CPython C/C++ extensions
 Author-email: Olivia Ryan <olivia.r.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Olivia Ryan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Issues, https://github.com/olivi-r/wasmpy-build/issues
+Project-URL: Repository, https://github.com/olivi-r/wasmpy-build
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: WebAssembly
```

### Comparing `wasmpy-build-0.5.1/wasmpy_build.egg-info/SOURCES.txt` & `wasmpy_build-0.5.2/wasmpy_build.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .gitignore
 .gitmodules
 LICENSE
 MANIFEST.in
 README.md
+analyze.py
 appveyor.yml
 generate.py
 pyconfig.h
 pyproject.toml
 wasmpy_build/__init__.py
+wasmpy_build/cli.py
+wasmpy_build/core.py
 wasmpy_build.egg-info/PKG-INFO
 wasmpy_build.egg-info/SOURCES.txt
 wasmpy_build.egg-info/dependency_links.txt
 wasmpy_build.egg-info/entry_points.txt
 wasmpy_build.egg-info/requires.txt
 wasmpy_build.egg-info/top_level.txt
 wasmpy_build/include/cp310/LICENSE
```

