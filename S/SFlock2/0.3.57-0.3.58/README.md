# Comparing `tmp/SFlock2-0.3.57.tar.gz` & `tmp/SFlock2-0.3.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFlock2-0.3.57.tar", last modified: Tue Dec  5 10:40:21 2023, max compression
+gzip compressed data, was "sflock2-0.3.58.tar", last modified: Sat Jun  1 19:52:10 2024, max compression
```

## Comparing `SFlock2-0.3.57.tar` & `SFlock2-0.3.58.tar`

### file list

```diff
@@ -1,101 +1,95 @@
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.439592 SFlock2-0.3.57/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      370 2020-06-10 09:29:08.000000 SFlock2-0.3.57/MANIFEST.in
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1178 2023-12-05 10:40:21.439110 SFlock2-0.3.57/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2717 2023-11-01 12:01:00.000000 SFlock2-0.3.57/README.md
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.371881 SFlock2-0.3.57/SFlock2.egg-info/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1178 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1890 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/SOURCES.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/dependency_links.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       44 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/entry_points.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      132 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/requires.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        7 2023-12-05 10:40:21.000000 SFlock2-0.3.57/SFlock2.egg-info/top_level.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       38 2023-12-05 10:40:21.439697 SFlock2-0.3.57/setup.cfg
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1880 2023-02-01 06:49:14.000000 SFlock2-0.3.57/setup.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.379136 SFlock2-0.3.57/sflock/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2023-12-05 10:04:42.000000 SFlock2-0.3.57/sflock/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      335 2021-07-15 18:56:48.000000 SFlock2-0.3.57/sflock/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      100 2023-12-05 10:40:08.000000 SFlock2-0.3.57/sflock/__version__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15323 2023-12-05 10:40:08.000000 SFlock2-0.3.57/sflock/abstracts.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.381991 SFlock2-0.3.57/sflock/aux/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2023-11-01 11:37:40.000000 SFlock2-0.3.57/sflock/aux/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/aux/__init__.py
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)     7367 2023-06-22 07:41:53.000000 SFlock2-0.3.57/sflock/aux/decode_vbe_jse.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.383668 SFlock2-0.3.57/sflock/compat/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      152 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/compat/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1295 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/compat/magic.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      564 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/config.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.389893 SFlock2-0.3.57/sflock/data/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:22.000000 SFlock2-0.3.57/sflock/data/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      157 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       26 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/data/password.txt
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   668240 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/poweriso.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.399147 SFlock2-0.3.57/sflock/data/win32/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   536241 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win32/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   150016 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win32/magic1.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    79360 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win32/regex2.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    72192 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win32/zlib1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.408014 SFlock2-0.3.57/sflock/data/win64/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    67720 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win64/libgnurx-0.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)  2944752 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win64/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   717504 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/data/win64/magic1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.413752 SFlock2-0.3.57/sflock/data/yara/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      464 2022-09-02 19:41:32.000000 SFlock2-0.3.57/sflock/data/yara/archives.yar
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    11391 2022-02-19 08:23:06.000000 SFlock2-0.3.57/sflock/data/yara/shellcodes.yar
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   873032 2023-01-31 10:07:30.000000 SFlock2-0.3.57/sflock/data/zipjail.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.414932 SFlock2-0.3.57/sflock/decode/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      302 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/decode/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5967 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/decode/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      364 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/exception.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    16321 2023-12-05 10:40:08.000000 SFlock2-0.3.57/sflock/ident.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3271 2023-01-19 07:23:25.000000 SFlock2-0.3.57/sflock/main.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1328 2021-12-08 14:30:13.000000 SFlock2-0.3.57/sflock/misc.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4275 2023-11-01 10:58:23.000000 SFlock2-0.3.57/sflock/pick.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.422177 SFlock2-0.3.57/sflock/unpack/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      309 2020-06-10 09:29:08.000000 SFlock2-0.3.57/sflock/unpack/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1276 2023-01-31 10:07:51.000000 SFlock2-0.3.57/sflock/unpack/ace.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1570 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/bup.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      945 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/cab.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1065 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/daa.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2180 2021-12-29 11:09:37.000000 SFlock2-0.3.57/sflock/unpack/eml.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1838 2021-07-16 14:34:19.000000 SFlock2-0.3.57/sflock/unpack/lzip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2055 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/msg.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2225 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/mso.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      977 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2468 2021-12-08 17:07:57.000000 SFlock2-0.3.57/sflock/unpack/pdf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1489 2023-12-05 10:40:08.000000 SFlock2-0.3.57/sflock/unpack/pgp.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      932 2022-03-08 17:08:34.000000 SFlock2-0.3.57/sflock/unpack/rar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5029 2022-01-14 07:58:22.000000 SFlock2-0.3.57/sflock/unpack/tar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6399 2023-12-05 10:40:08.000000 SFlock2-0.3.57/sflock/unpack/zip7.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1805 2023-11-01 11:40:18.000000 SFlock2-0.3.57/sflock/unpack/zpaq.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-12-05 10:40:21.438132 SFlock2-0.3.57/tests/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5150 2022-10-27 10:16:35.000000 SFlock2-0.3.57/tests/test_7z.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3436 2023-12-05 10:14:12.000000 SFlock2-0.3.57/tests/test_ace.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1046 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_attr.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1414 2022-01-14 07:58:22.000000 SFlock2-0.3.57/tests/test_bup.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1991 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_cab.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      974 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_daa.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1066 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_decode.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      324 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_elf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3518 2022-12-14 17:01:41.000000 SFlock2-0.3.57/tests/test_eml.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      954 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_exts.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1599 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_file.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2833 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_ident.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      996 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_lzh.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1222 2021-07-16 14:54:32.000000 SFlock2-0.3.57/tests/test_lzip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      704 2021-07-16 12:01:23.000000 SFlock2-0.3.57/tests/test_magic.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1169 2023-12-05 10:40:08.000000 SFlock2-0.3.57/tests/test_main.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      459 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_misc.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3005 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_msg.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      506 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_mso.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1563 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6874 2023-10-17 10:02:41.000000 SFlock2-0.3.57/tests/test_package.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2093 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_pdf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1370 2021-12-08 14:59:59.000000 SFlock2-0.3.57/tests/test_pick.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4556 2022-01-14 07:58:22.000000 SFlock2-0.3.57/tests/test_rar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      524 2022-10-27 10:07:17.000000 SFlock2-0.3.57/tests/test_shellcode.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     7291 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_tar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    17695 2022-02-19 09:29:07.000000 SFlock2-0.3.57/tests/test_unpack.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1486 2021-07-16 16:51:56.000000 SFlock2-0.3.57/tests/test_win.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     8544 2022-01-14 07:58:22.000000 SFlock2-0.3.57/tests/test_zip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1689 2021-12-08 17:07:57.000000 SFlock2-0.3.57/tests/test_zipify.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      919 2023-12-05 10:40:08.000000 SFlock2-0.3.57/tests/test_zpaq.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.637338 sflock2-0.3.58/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      370 2023-06-26 09:04:21.000000 sflock2-0.3.58/MANIFEST.in
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1178 2024-06-01 19:52:10.636549 sflock2-0.3.58/PKG-INFO
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2723 2024-06-01 19:51:19.000000 sflock2-0.3.58/README.md
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.634741 sflock2-0.3.58/SFlock2.egg-info/
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1178 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/PKG-INFO
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1797 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/SOURCES.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)        1 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/dependency_links.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)       44 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/entry_points.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)      132 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/requires.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)        7 2024-06-01 19:52:10.000000 sflock2-0.3.58/SFlock2.egg-info/top_level.txt
+-rw-r--r--   0 doomedraven   (501) staff       (20)       38 2024-06-01 19:52:10.637485 sflock2-0.3.58/setup.cfg
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1984 2024-06-01 19:51:19.000000 sflock2-0.3.58/setup.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.508844 sflock2-0.3.58/sflock/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      316 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      100 2024-06-01 19:51:46.000000 sflock2-0.3.58/sflock/__version__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)    15304 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/abstracts.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.510748 sflock2-0.3.58/sflock/auxiliary/
+-rw-r--r--   0 doomedraven   (501) staff       (20)        1 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/auxiliary/__init__.py
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)     7367 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/auxiliary/decode_vbe_jse.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      564 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/config.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.523664 sflock2-0.3.58/sflock/data/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      157 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)       26 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/password.txt
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)   668240 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/poweriso.elf
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.567767 sflock2-0.3.58/sflock/data/win32/
+-rw-r--r--   0 doomedraven   (501) staff       (20)   367616 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/data/win32/libmagic.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)  8258464 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/data/win32/magic.mgc
+-rw-r--r--   0 doomedraven   (501) staff       (20)    79360 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/win32/regex2.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)    72192 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/win32/zlib1.dll
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.572156 sflock2-0.3.58/sflock/data/win64/
+-rw-r--r--   0 doomedraven   (501) staff       (20)    67720 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/win64/libgnurx-0.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)   396800 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/data/win64/libmagic.dll
+-rw-r--r--   0 doomedraven   (501) staff       (20)  8258464 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/data/win64/magic.mgc
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.595032 sflock2-0.3.58/sflock/data/yara/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      464 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/yara/archives.yar
+-rw-r--r--   0 doomedraven   (501) staff       (20)    11391 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/yara/shellcodes.yar
+-rwxr-xr-x   0 doomedraven   (501) staff       (20)   873032 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/data/zipjail.elf
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.596616 sflock2-0.3.58/sflock/decode/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      302 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/decode/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     5967 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/decode/office.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      364 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/exception.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)    16283 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/ident.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     3271 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/main.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1328 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/misc.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     4275 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/pick.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.608461 sflock2-0.3.58/sflock/unpack/
+-rw-r--r--   0 doomedraven   (501) staff       (20)      309 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/__init__.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1276 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/ace.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1570 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/bup.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      945 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/cab.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1065 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/daa.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2180 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/eml.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1838 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/lzip.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2055 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/msg.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2225 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/mso.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      977 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/office.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2468 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/pdf.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1489 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/unpack/pgp.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      932 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/rar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     5029 2023-06-26 09:04:21.000000 sflock2-0.3.58/sflock/unpack/tar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     6399 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/unpack/zip7.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1805 2024-06-01 19:51:19.000000 sflock2-0.3.58/sflock/unpack/zpaq.py
+drwxr-xr-x   0 doomedraven   (501) staff       (20)        0 2024-06-01 19:52:10.633810 sflock2-0.3.58/tests/
+-rw-r--r--   0 doomedraven   (501) staff       (20)     5150 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_7z.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     3436 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_ace.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1046 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_attr.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1414 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_bup.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1991 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_cab.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      974 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_daa.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1066 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_decode.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      324 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_elf.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     3518 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_eml.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      954 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_exts.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1599 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_file.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2833 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_ident.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      996 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_lzh.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1222 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_lzip.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      704 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_magic.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1169 2024-06-01 19:51:19.000000 sflock2-0.3.58/tests/test_main.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      459 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_misc.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     3005 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_msg.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      506 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_mso.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1563 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_office.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     6874 2023-09-28 13:51:02.000000 sflock2-0.3.58/tests/test_package.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     2093 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_pdf.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1370 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_pick.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     4556 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_rar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      524 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_shellcode.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     7291 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_tar.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)    17695 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_unpack.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1486 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_win.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     8544 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_zip.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)     1689 2023-06-26 09:04:21.000000 sflock2-0.3.58/tests/test_zipify.py
+-rw-r--r--   0 doomedraven   (501) staff       (20)      919 2024-06-01 19:51:19.000000 sflock2-0.3.58/tests/test_zpaq.py
```

### Comparing `SFlock2-0.3.57/PKG-INFO` & `sflock2-0.3.58/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.57
+Version: 0.3.58
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SFlock2-0.3.57/README.md` & `sflock2-0.3.58/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 As-is sflock has been designed to be used to its full extent on
 Ubuntu/Debian-like systems. For optimal usage it is recommended to install the
 following packages alongside sflock. It is currently not possible to run the
 unpackers that require native tooling support on non-Linux platforms.
 
 ```bash
-$ sudo apt-get install p7zip-full rar unace-nonfree cabextract lzip libjpeg8-dev zlib1g-dev zpaq
+$ sudo apt-get install p7zip-full rar unace-nonfree cabextract lzip libjpeg8-dev zlib1g-dev zpaq gnupg
 ```
 
 Installation of sflock itself may be done as follows.
 
 ```bash
 $ sudo pip install -U sflock2
 ```
```

### Comparing `SFlock2-0.3.57/SFlock2.egg-info/PKG-INFO` & `sflock2-0.3.58/SFlock2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.57
+Version: 0.3.58
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SFlock2-0.3.57/SFlock2.egg-info/SOURCES.txt` & `sflock2-0.3.58/SFlock2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,36 @@
 setup.py
 SFlock2.egg-info/PKG-INFO
 SFlock2.egg-info/SOURCES.txt
 SFlock2.egg-info/dependency_links.txt
 SFlock2.egg-info/entry_points.txt
 SFlock2.egg-info/requires.txt
 SFlock2.egg-info/top_level.txt
-sflock/.DS_Store
 sflock/__init__.py
 sflock/__version__.py
 sflock/abstracts.py
 sflock/config.py
 sflock/exception.py
 sflock/ident.py
 sflock/main.py
 sflock/misc.py
 sflock/pick.py
-sflock/aux/.DS_Store
-sflock/aux/__init__.py
-sflock/aux/decode_vbe_jse.py
-sflock/compat/__init__.py
-sflock/compat/magic.py
-sflock/data/.DS_Store
+sflock/auxiliary/__init__.py
+sflock/auxiliary/decode_vbe_jse.py
 sflock/data/__init__.py
 sflock/data/password.txt
 sflock/data/poweriso.elf
 sflock/data/zipjail.elf
+sflock/data/win32/libmagic.dll
 sflock/data/win32/magic.mgc
-sflock/data/win32/magic1.dll
 sflock/data/win32/regex2.dll
 sflock/data/win32/zlib1.dll
 sflock/data/win64/libgnurx-0.dll
+sflock/data/win64/libmagic.dll
 sflock/data/win64/magic.mgc
-sflock/data/win64/magic1.dll
 sflock/data/yara/archives.yar
 sflock/data/yara/shellcodes.yar
 sflock/decode/__init__.py
 sflock/decode/office.py
 sflock/unpack/__init__.py
 sflock/unpack/ace.py
 sflock/unpack/bup.py
```

### Comparing `SFlock2-0.3.57/setup.py` & `sflock2-0.3.58/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 # Copyright (C) 2015-2018 Jurriaan Bremer.
 # Copyright (C) 2018-2019 Hatching B.V.
 # This file is part of SFlock - http://www.sflock.org/.
 # See the file 'docs/LICENSE.txt' for copying permission.
 
+import sys
+
 from setuptools import setup, find_packages
 from distutils.util import convert_path
 
 ver_module_ns = {}
 ver_module = convert_path("sflock/__version__.py")
 with open(ver_module) as fh:
     exec(fh.read(), ver_module_ns)
 assert "__version__" in ver_module_ns
 version = ver_module_ns["__version__"]
 
+install_requires=[
+    "click",
+    "cryptography>=2.1",
+    "olefile>=0.43",
+    # "peepdf>=0.4.1",
+    "python-magic>=0.4.13",
+    "pefile",
+]
+
+if sys.platform == "win32":
+    install_requires.append("python-magic-bin>=0.4.14")
+
 setup(
     name="SFlock2",
     version=version,
     author="Hatching B.V.",
     author_email="jbr@hatching.io",
     packages=[
         "sflock",
@@ -43,20 +57,13 @@
         "Topic :: Security",
     ],
     keywords=("sflock unarchive"),
     url="https://github.com/doomedraven/sflock/",
     license="GPLv3",
     description="Sample staging and detonation utility",
     include_package_data=True,
-    install_requires=[
-        "click",
-        "cryptography>=2.1",
-        "olefile>=0.43",
-        # "peepdf>=0.4.1",
-        "python-magic>=0.4.13",
-        "pefile",
-    ],
+    install_requires=install_requires,
     extras_require={
         "dev": ["mock", "pytest"],
         "shellcode": ["unicorn>=2.0.0", "yara-python>=4.1.0"],
     }
 )
```

### Comparing `SFlock2-0.3.57/sflock/abstracts.py` & `sflock2-0.3.58/sflock/abstracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright (C) 2015-2018 Jurriaan Bremer.
 # Copyright (C) 2018 Hatching B.V.
 # This file is part of SFlock - http://www.sflock.org/.
 # See the file 'docs/LICENSE.txt' for copying permission.
 
 import hashlib
 import io
+import magic
 import ntpath
 import olefile
 import os.path
 import re
 import shutil
 import subprocess
 import tempfile
 
-from sflock.compat import magic
 from sflock.config import iter_passwords
 from sflock.exception import UnpackException
 from sflock.misc import data_file, make_list
 from sflock.pick import package, platform
 
 
 class Unpacker(object):
@@ -42,15 +42,15 @@
     def supported(self):
         return os.path.exists(self.exe)
 
     def zipjail(self, filepath, dirpath, *args):
         zipjail = data_file(b"zipjail.elf")
 
         p = subprocess.Popen(
-            (zipjail, filepath, dirpath, "-c=2", "--", self.exe) + args,
+            (zipjail, filepath, dirpath, "-c=3", "--", self.exe) + args,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
 
         return_code = p.wait()
         out, err = p.communicate()
```

### Comparing `SFlock2-0.3.57/sflock/aux/decode_vbe_jse.py` & `sflock2-0.3.58/sflock/auxiliary/decode_vbe_jse.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/config.py` & `sflock2-0.3.58/sflock/config.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/poweriso.elf` & `sflock2-0.3.58/sflock/data/poweriso.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/win32/regex2.dll` & `sflock2-0.3.58/sflock/data/win32/regex2.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/win32/zlib1.dll` & `sflock2-0.3.58/sflock/data/win32/zlib1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/win64/libgnurx-0.dll` & `sflock2-0.3.58/sflock/data/win64/libgnurx-0.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/yara/shellcodes.yar` & `sflock2-0.3.58/sflock/data/yara/shellcodes.yar`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/data/zipjail.elf` & `sflock2-0.3.58/sflock/data/zipjail.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/decode/office.py` & `sflock2-0.3.58/sflock/decode/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/ident.py` & `sflock2-0.3.58/sflock/ident.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is part of SFlock - http://www.sflock.org/.
 # See the file 'docs/LICENSE.txt' for copying permission.
 import os
 import re
 from collections import OrderedDict
 
 import pefile
-from sflock.aux.decode_vbe_jse import decode_file as vbe_decode_file
+from sflock.auxiliary.decode_vbe_jse import decode_file as vbe_decode_file
 
 
 try:
     import yara
 
     cur_dir = os.path.dirname(os.path.abspath(__file__))
     shellcode_rules = yara.compile(filepath=os.path.join(cur_dir, "data", "yara", "shellcodes.yar"))
@@ -192,14 +192,16 @@
         ("HTML", "html"),
         ("ZPAQ file", "zpaq"),
         # https://github.com/file/file/blob/master/magic/Magdir/pgp
         ("PGP ", "pgp"),
     ]
 )
 
+def is_executable(f):
+    return f.contents.startswith((b"MZ", b"\x7fELF"))
 
 def detect_shellcode(f):
 
     if f.contents[6:10] == b"JFIF":
         return
     """
     if HAVE_YARA:
@@ -263,15 +265,15 @@
         if re.search(rb"(?is)<\?XML.*?<scriptlet.*?<registration", f.contents):
             return "sct"
         else:
             return "hta"
 
 
 def xxe(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     STRINGS = [
         b"XXEncode",
         b"begin",
         b"+",
     ]
@@ -281,15 +283,15 @@
         found += f.contents.count(string)
 
     if found >= 300 and b"XXEncode" in f.contents and b"begin" in f.contents:
         return "xxe"
 
 
 def hta(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     STRINGS = [
         b"<head",
         b"<title",
         b"<body",
         b"SINGLEINSTANCE",
@@ -318,15 +320,15 @@
 
 def office_one(f):
     if f.contents.startswith(b"\xE4\x52\x5C\x7B\x8C\xD8\xA7\x4D\xAE\xB1\x53\x78\xD0\x29\x96\xD3"):
         return "one"
 
 
 def office_webarchive(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     STRINGS = [
         b"<o:Pages>",
         b"<o:DocumentProperties>",
         b"<o:Words>",
         b"<o:Characters>",
@@ -399,15 +401,15 @@
     if ["WordDocument"] in files:
         return "doc"
     if ["Workbook"] in files:
         return "xls"
 
 
 def powershell(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     POWERSHELL_STRS = [
         b"$PSHOME",
         b"Get-WmiObject",
         b"Write-",
         b"new-object",
@@ -424,15 +426,15 @@
             found += 1
 
     if found > 1:
         return "ps1"
 
 
 def javascript(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     JS_STRS = [
         b"var ",
         b"function ",
         b"eval",
         b" true",
@@ -452,24 +454,24 @@
             found += 1
 
     if found >= 5:
         return "js"
 
 
 def wsf(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     match = re.search(b'<script\\s+language="(J|VB|Perl)Script"', f.contents, re.I)
     if match:
         return "wsf"
 
 
 def pub(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     PUB_STRS = [
         b"Microsoft Publisher",
         b"MSPublisher",
     ]
     found = 0
@@ -478,15 +480,15 @@
             found += 1
 
     if found >= 1:
         return "pub"
 
 
 def visualbasic(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     VB_STRS = [
         b"Dim ",
         b"\x00D\x00i\x00m\x00 ",
         b"dim ",
         b"\s\x00d\x00i\x00m\x00 ",
@@ -530,15 +532,15 @@
 
 def dmg(f):
     if any([child.magic == "AppleDouble encoded Macintosh file" for child in f.children or []]):
         return "dmg"
 
 
 def vbe_jse(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     if b"#@~^" in f.contents[:100]:
         data = vbe_decode_file("", f.contents)
         if data:
             if re.findall(rb"\s?Dim\s", data, re.I) or re.findall(b"\s\x00D\x00i\x00m\x00\s", data, re.I):
                 return "vbs"
@@ -552,15 +554,15 @@
     if HAVE_YARA:
         matches = archives_rules.match(data=f.contents)
         if "archive_udf" in [rule.rule for rule in matches]:
             return "udf"
 
 
 def inf(f):
-    if f.contents.startswith(b"MZ"):
+    if is_executable(f):
         return None
 
     STRINGS = [
         # b"[version]",
         b"Signature=",
         b"AdvancedINF=",
         b"[DefaultInstall_SingleUser]",
```

### Comparing `SFlock2-0.3.57/sflock/main.py` & `sflock2-0.3.58/sflock/main.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/misc.py` & `sflock2-0.3.58/sflock/misc.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/pick.py` & `sflock2-0.3.58/sflock/pick.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/ace.py` & `sflock2-0.3.58/sflock/unpack/ace.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/bup.py` & `sflock2-0.3.58/sflock/unpack/bup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/cab.py` & `sflock2-0.3.58/sflock/unpack/cab.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/daa.py` & `sflock2-0.3.58/sflock/unpack/daa.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/eml.py` & `sflock2-0.3.58/sflock/unpack/eml.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/lzip.py` & `sflock2-0.3.58/sflock/unpack/lzip.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/msg.py` & `sflock2-0.3.58/sflock/unpack/msg.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/mso.py` & `sflock2-0.3.58/sflock/unpack/mso.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/office.py` & `sflock2-0.3.58/sflock/unpack/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/pdf.py` & `sflock2-0.3.58/sflock/unpack/pdf.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/pgp.py` & `sflock2-0.3.58/sflock/unpack/pgp.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/rar.py` & `sflock2-0.3.58/sflock/unpack/rar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/tar.py` & `sflock2-0.3.58/sflock/unpack/tar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/zip7.py` & `sflock2-0.3.58/sflock/unpack/zip7.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/sflock/unpack/zpaq.py` & `sflock2-0.3.58/sflock/unpack/zpaq.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_7z.py` & `sflock2-0.3.58/tests/test_7z.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_ace.py` & `sflock2-0.3.58/tests/test_ace.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_attr.py` & `sflock2-0.3.58/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_bup.py` & `sflock2-0.3.58/tests/test_bup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_cab.py` & `sflock2-0.3.58/tests/test_cab.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_daa.py` & `sflock2-0.3.58/tests/test_daa.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_decode.py` & `sflock2-0.3.58/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_eml.py` & `sflock2-0.3.58/tests/test_eml.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_exts.py` & `sflock2-0.3.58/tests/test_exts.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_file.py` & `sflock2-0.3.58/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_ident.py` & `sflock2-0.3.58/tests/test_ident.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_lzh.py` & `sflock2-0.3.58/tests/test_lzh.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_lzip.py` & `sflock2-0.3.58/tests/test_lzip.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_magic.py` & `sflock2-0.3.58/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_main.py` & `sflock2-0.3.58/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_msg.py` & `sflock2-0.3.58/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_office.py` & `sflock2-0.3.58/tests/test_office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_package.py` & `sflock2-0.3.58/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_pdf.py` & `sflock2-0.3.58/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_pick.py` & `sflock2-0.3.58/tests/test_pick.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_rar.py` & `sflock2-0.3.58/tests/test_rar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_shellcode.py` & `sflock2-0.3.58/tests/test_shellcode.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_tar.py` & `sflock2-0.3.58/tests/test_tar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_unpack.py` & `sflock2-0.3.58/tests/test_unpack.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_win.py` & `sflock2-0.3.58/tests/test_win.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_zip.py` & `sflock2-0.3.58/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_zipify.py` & `sflock2-0.3.58/tests/test_zipify.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.57/tests/test_zpaq.py` & `sflock2-0.3.58/tests/test_zpaq.py`

 * *Files identical despite different names*

