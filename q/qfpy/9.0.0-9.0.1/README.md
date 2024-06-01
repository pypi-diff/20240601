# Comparing `tmp/qfpy-9.0.0.tar.gz` & `tmp/qfpy-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-9.0.0.tar", last modified: Sat Jun  1 17:11:23 2024, max compression
+gzip compressed data, was "qfpy-9.0.1.tar", last modified: Sat Jun  1 17:13:23 2024, max compression
```

## Comparing `qfpy-9.0.0.tar` & `qfpy-9.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.751454 qfpy-9.0.0/
--rw-rw-rw-   0        0        0      251 2024-06-01 17:11:23.749499 qfpy-9.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-06-01 17:11:02.000000 qfpy-9.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 17:11:23.751454 qfpy-9.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.715728 qfpy-9.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.736809 qfpy-9.0.0/src/qfpy/
--rw-rw-rw-   0        0        0      100 2024-06-01 17:10:50.000000 qfpy-9.0.0/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      212 2024-06-01 17:05:01.000000 qfpy-9.0.0/src/qfpy/character.py
--rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-9.0.0/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-9.0.0/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-9.0.0/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-9.0.0/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-9.0.0/src/qfpy/function.py
--rw-rw-rw-   0        0        0      329 2024-06-01 17:10:13.000000 qfpy-9.0.0/src/qfpy/output.py
--rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-9.0.0/src/qfpy/process.py
--rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-9.0.0/src/qfpy/system.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.748523 qfpy-9.0.0/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      251 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.823913 qfpy-9.0.1/
+-rw-rw-rw-   0        0        0      227 2024-06-01 17:13:23.822942 qfpy-9.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-06-01 17:13:06.000000 qfpy-9.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:13:23.823913 qfpy-9.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.779848 qfpy-9.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.810675 qfpy-9.0.1/src/qfpy/
+-rw-rw-rw-   0        0        0      100 2024-06-01 17:10:50.000000 qfpy-9.0.1/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-06-01 17:05:01.000000 qfpy-9.0.1/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-9.0.1/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-9.0.1/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     1992 2024-06-01 17:12:53.000000 qfpy-9.0.1/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-9.0.1/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-9.0.1/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      329 2024-06-01 17:10:13.000000 qfpy-9.0.1/src/qfpy/output.py
+-rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-9.0.1/src/qfpy/process.py
+-rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-9.0.1/src/qfpy/system.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.821960 qfpy-9.0.1/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-9.0.0/src/qfpy/crypto.py` & `qfpy-9.0.1/src/qfpy/crypto.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.0/src/qfpy/exif.py` & `qfpy-9.0.1/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.0/src/qfpy/ffmpeg.py` & `qfpy-9.0.1/src/qfpy/ffmpeg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-def concat_video(files: list[str], output_file: str)
-
 def is_hevc(file: Path) -> bool
 
 def is_not_hevc(file: Path) -> bool
 
 class FFprobe
     def duration
 
@@ -13,39 +11,14 @@
     def size
 """
 
 import json
 import subprocess as sp
 from pathlib import Path
 
-from moviepy.editor import VideoFileClip, concatenate_videoclips
-
-
-def concat_video(files: list[str], output_file: str):
-    """
-    合并视频文件列表中的所有视频成一个视频。
-
-    参数:
-    files: list[str] - 包含要合并的视频文件路径的列表。
-    output_file: str - 合并后的视频文件输出路径。
-
-    后处理：合并完成后，删除原始视频文件。
-
-    注意：该函数仅使用CPU进行视频合并，如果合并大量视频文件，可能会非常慢。
-    """
-    # 加载所有指定的视频文件为VideoFileClip对象
-    clips = [VideoFileClip(f) for f in files]
-    # 将所有VideoFileClip对象合并为一个final_clip
-    final_clip = concatenate_videoclips(clips)
-    # 将合并后的视频写入指定的输出文件
-    final_clip.write_videofile(output_file)
-    # 删除所有原始视频文件
-    for f in files:
-        f.unlink()
-
 
 class FFprobe:
     """
     方法
 
     duration：获取视频时长
```

### Comparing `qfpy-9.0.0/src/qfpy/folder.py` & `qfpy-9.0.1/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.0/src/qfpy/function.py` & `qfpy-9.0.1/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.0/src/qfpy/process.py` & `qfpy-9.0.1/src/qfpy/process.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.0/src/qfpy/system.py` & `qfpy-9.0.1/src/qfpy/system.py`

 * *Files identical despite different names*

