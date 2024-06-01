# Comparing `tmp/astrospec-0.1.0.tar.gz` & `tmp/astrospec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrospec-0.1.0.tar", last modified: Sun May 26 14:26:51 2024, max compression
+gzip compressed data, was "astrospec-0.2.0.tar", last modified: Sat Jun  1 16:30:38 2024, max compression
```

## Comparing `astrospec-0.1.0.tar` & `astrospec-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-05-26 14:26:51.124323 astrospec-0.1.0/
--rw-r--r--   0 chenliang   (501) staff       (20)     1125 2024-05-26 13:44:14.000000 astrospec-0.1.0/LICENSE
--rw-r--r--   0 chenliang   (501) staff       (20)      493 2024-05-26 14:26:51.123271 astrospec-0.1.0/PKG-INFO
--rw-r--r--   0 chenliang   (501) staff       (20)     4443 2024-05-26 13:52:55.000000 astrospec-0.1.0/README.md
-drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-05-26 14:26:51.115085 astrospec-0.1.0/astrospec/
--rw-r--r--   0 chenliang   (501) staff       (20)     5926 2024-05-26 12:43:29.000000 astrospec-0.1.0/astrospec/__init__.py
--rw-r--r--   0 chenliang   (501) staff       (20)     2670 2024-05-25 16:02:50.000000 astrospec-0.1.0/astrospec/cli.py
--rw-r--r--   0 chenliang   (501) staff       (20)     6406 2024-05-26 13:29:03.000000 astrospec-0.1.0/astrospec/postproc.py
--rw-r--r--   0 chenliang   (501) staff       (20)     5512 2024-05-26 13:29:04.000000 astrospec-0.1.0/astrospec/shape_correction.py
--rw-r--r--   0 chenliang   (501) staff       (20)     4151 2024-05-26 11:46:27.000000 astrospec-0.1.0/astrospec/spectrum.py
--rw-r--r--   0 chenliang   (501) staff       (20)      118 2024-05-25 14:23:36.000000 astrospec-0.1.0/astrospec/utils.py
--rw-r--r--   0 chenliang   (501) staff       (20)     3504 2024-05-25 14:24:19.000000 astrospec-0.1.0/astrospec/video_reader.py
-drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-05-26 14:26:51.121961 astrospec-0.1.0/astrospec.egg-info/
--rw-r--r--   0 chenliang   (501) staff       (20)      493 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/PKG-INFO
--rw-r--r--   0 chenliang   (501) staff       (20)      384 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/SOURCES.txt
--rw-r--r--   0 chenliang   (501) staff       (20)        1 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/dependency_links.txt
--rw-r--r--   0 chenliang   (501) staff       (20)       45 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/entry_points.txt
--rw-r--r--   0 chenliang   (501) staff       (20)      132 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/requires.txt
--rw-r--r--   0 chenliang   (501) staff       (20)       10 2024-05-26 14:26:51.000000 astrospec-0.1.0/astrospec.egg-info/top_level.txt
--rw-r--r--   0 chenliang   (501) staff       (20)       38 2024-05-26 14:26:51.124512 astrospec-0.1.0/setup.cfg
--rw-r--r--   0 chenliang   (501) staff       (20)      707 2024-05-26 14:26:11.000000 astrospec-0.1.0/setup.py
+drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-06-01 16:30:38.957678 astrospec-0.2.0/
+-rw-r--r--   0 chenliang   (501) staff       (20)     1125 2024-05-26 13:44:14.000000 astrospec-0.2.0/LICENSE
+-rw-r--r--   0 chenliang   (501) staff       (20)      493 2024-06-01 16:30:38.956488 astrospec-0.2.0/PKG-INFO
+-rw-r--r--   0 chenliang   (501) staff       (20)     4755 2024-06-01 16:17:45.000000 astrospec-0.2.0/README.md
+drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-06-01 16:30:38.947505 astrospec-0.2.0/astrospec/
+-rw-r--r--   0 chenliang   (501) staff       (20)     6602 2024-06-01 15:38:47.000000 astrospec-0.2.0/astrospec/__init__.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     3395 2024-06-01 16:12:39.000000 astrospec-0.2.0/astrospec/cli.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     5322 2024-06-01 15:32:09.000000 astrospec-0.2.0/astrospec/light_correction.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     6438 2024-06-01 15:41:18.000000 astrospec-0.2.0/astrospec/postproc.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     5659 2024-06-01 14:41:15.000000 astrospec-0.2.0/astrospec/shape_correction.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     4151 2024-05-26 11:46:27.000000 astrospec-0.2.0/astrospec/spectrum.py
+-rw-r--r--   0 chenliang   (501) staff       (20)      118 2024-06-01 14:41:13.000000 astrospec-0.2.0/astrospec/utils.py
+-rw-r--r--   0 chenliang   (501) staff       (20)     3504 2024-05-25 14:24:19.000000 astrospec-0.2.0/astrospec/video_reader.py
+drwxr-xr-x   0 chenliang   (501) staff       (20)        0 2024-06-01 16:30:38.955031 astrospec-0.2.0/astrospec.egg-info/
+-rw-r--r--   0 chenliang   (501) staff       (20)      493 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/PKG-INFO
+-rw-r--r--   0 chenliang   (501) staff       (20)      414 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/SOURCES.txt
+-rw-r--r--   0 chenliang   (501) staff       (20)        1 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/dependency_links.txt
+-rw-r--r--   0 chenliang   (501) staff       (20)       45 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/entry_points.txt
+-rw-r--r--   0 chenliang   (501) staff       (20)      132 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/requires.txt
+-rw-r--r--   0 chenliang   (501) staff       (20)       10 2024-06-01 16:30:38.000000 astrospec-0.2.0/astrospec.egg-info/top_level.txt
+-rw-r--r--   0 chenliang   (501) staff       (20)       38 2024-06-01 16:30:38.957869 astrospec-0.2.0/setup.cfg
+-rw-r--r--   0 chenliang   (501) staff       (20)      707 2024-06-01 16:18:29.000000 astrospec-0.2.0/setup.py
```

### Comparing `astrospec-0.1.0/LICENSE` & `astrospec-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astrospec-0.1.0/README.md` & `astrospec-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,61 +4,65 @@
 
 This project is used to reconstruct image from raw video captured by the [spectroheliograph](https://en.wikipedia.org/wiki/Spectroheliograph)
 
 **Highlights**
 - Clear API interface
 - Algorithm with sub-pixel interpolation for wavelength correction 
 - Additional features such as color mapping
+- Advanced algorithm to remove stray light ([view comparison](#Stray-light-remove))
 
 ## Installation
 
 ```bash
 pip install astrospec
 ```
 
 ## Getting Started
 
 ### For end users
 
 ```bash
+# single file input, generate 16-bit png files at the sub-folder named "output/img", no normalization, no color mapping
+ascli -i "<SER file>" --raw
+
 # single file input, generate png files at the sub-folder named "output/img"
-ascli -i "<SER file>" [-c color_map_name]
+ascli -i "<SER file>" [-c color_map_name] [-nb brightness(default=1)]
 
 # process all .ser files in the folder, generate png files at the sub-folder named "output/img"
-ascli -f "<folder>" [-c color_map_name]
+ascli -f "<folder>" [-c color_map_name] [-nb brightness(default=1)]
 
 # color_map_name（optional）:
 # - orange-enhanced (default)
 # - enhanced
 # - linear
 
 ```
 
 ### For developers
 
 #### example 1
 
 ```py
-from astrospec import raw_file_to_raw_image, raw_file_to_image, raw_file_to_file
+import astrospec as ass
 import matplotlib.pyplot as plt
 
-img = raw_file_to_image('input.ser')
-plt.imshow(img)
+img = ass.raw_file_to_image('input.ser')
+plt.imshow(img[0])
 plt.show()
 ```
 ![2024-05-18 Hα solar image](docs/2024-05-18-070400_Ha.jpg)
 
 #### example 2
 
 ```py
-from astrospec import raw_file_to_raw_image, raw_file_to_image, raw_file_to_file
+import astrospec as ass
 import matplotlib.pyplot as plt
 
-img = raw_file_to_image('input.ser', color_map_name='linear')
-plt.imshow(img, cmap='gray')
+img = ass.raw_file_to_image('input.ser', color_map_name='linear')
+plt.imshow(img[0], cmap='gray')
 plt.show()
 ```
 ![2024-05-18 Hα solar image](docs/2024-05-18-070400_Ha_linear.jpg)
 
 #### API
 
 - Reconstruct image from the ser file, return the reconstructed image in the original value space, np.array(float64)
@@ -100,14 +104,18 @@
     :param shifts: the wavelength offsets in pixels, e.g. [-0.5, 0, 0.5] returns 3 images in corresponding wavelengths
     :param color_map_name: color map, values: orange-enhanced (default), enhanced, linear
     :param verbose: 0~3，log information level
     :return: None
     """ 
 ```
 
+## Stray light remove
+![correct stray light](docs/2024-05-28_1306.gif)
+![correct stray light](docs/2024-05-28-0549_3.gif)
+
 ## Reference
 1. [SolEx](http://www.astrosurf.com/solex/sol-ex-presentation-en.html) - The design of a DIY spectroheliograph by Valerie Desnoux, with very detailed introduction, which is worth reading carefully.
 2. [DIY迷你太阳光谱仪](https://www.bilibili.com/video/BV1um421j7co) by 阴天wnova酱 - The design of another DIY mini-spectroheliograph
 3. [Solex_ser_recon](https://github.com/Vdesnoux/Solex_ser_recon) - An open-source reconstruct software made by Valerie Desnoux
 4. [SHG](https://github.com/thelondonsmiths/Solex_ser_recon_EN) - Another open-source reconstruct software
 5. [又能看光谱又能拍摄太阳的太阳光谱仪](https://www.bilibili.com/video/BV1fw411W7HJ) by 摄日者天文
 6. [太阳光谱扫描成像](https://lcsky.org/3.0/2024/05/19/spectroheliograph-1/) by Harold Liang - My DIY and observation records
```

### Comparing `astrospec-0.1.0/astrospec/__init__.py` & `astrospec-0.2.0/astrospec/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 # filename -> float np.array: raw_file_to_raw_image
 # filename -> uint8 np.array: raw_file_to_image
 # filename -> filename:       raw_file_to_file
 
 from .video_reader import video_reader
 from .spectrum import reduce_mean, fit_line_with_poly, frame_to_line, reconstruct
 from .shape_correction import detect_edge_points, filter_out_invalid_points, fit_ellipse, warp_frame
+from .light_correction import correct_light
 from .postproc import normalize, color_map
 from .utils import print
 import cv2
 import numpy as np
+import matplotlib.pyplot as plt
 from einops import rearrange, reduce, repeat
 
-def raw_file_to_file(file, output_file, shifts = [0], color_map_name = 'orange-enhanced', verbose = 0):
+def raw_file_to_file(file, output_file, raw = False, shifts = [0], correct_light_axis = 2, normalize_brightness = 1.0, color_map_name = 'orange-enhanced', verbose = 0):
     """
     raw_file_to_file 从ser文件重建图像，输出重建图像文件
     raw_file_to_file reconstruct image from raw video (ser file), write reconstructed, normalized, color mapped image to file(s)
 
     :param file: 输入ser文件路径 
     :param file: input file path
     :param output_file: 输出文件路径。如果shifts有多个值，可通过参数{i:02d}、{shift:02d}指定文件名
@@ -30,28 +32,31 @@
     :param shifts: the wavelength offsets in pixels, e.g. [-0.5, 0, 0.5] returns 3 images in corresponding wavelengths
     :param color_map_name: 色彩映射，取值范围：orange-enhanced (默认), enhanced, linear (不进行任何映射)
     :param color_map_name: color map, values: orange-enhanced (default), enhanced, linear
     :param verbose: 0~3，输出调试信息
     :param verbose: 0~3，log information level
     :return: None
     """ 
-    imgs = raw_file_to_raw_image(file, shifts, verbose)
+    imgs = raw_file_to_raw_image(file, shifts, correct_light_axis, verbose)
 
     for i,img in enumerate(imgs):
-        img = normalize(img).astype(int)
-        img = color_map(img, color_map_name)
-        if len(img.shape) == 3:
-            img = img[:,:,::-1]
-
         _file = output_file.format(i=i, shift=shifts[i])
         if verbose > 1:
             print(f'write to {_file} (i={i}, shift={shifts[i]})')
-        cv2.imwrite(_file, img)
+        if raw:
+            cv2.imwrite(_file, np.clip(img, 0, 65535).astype(np.uint16))
+        else:
+            img = normalize(img, brightness=normalize_brightness, verbose=verbose).astype(int)
+            img = color_map(img, color_map_name)
+            if len(img.shape) == 3:
+                img = img[:,:,::-1]
+
+            cv2.imwrite(_file, img)
 
-def raw_file_to_image(file, shifts = [0], color_map_name = 'orange-enhanced', verbose = 0):
+def raw_file_to_image(file, shifts = [0], correct_light_axis = 2, normalize_brightness = 1.0, color_map_name = 'orange-enhanced', verbose = 0):
     """
     raw_file_to_image 从ser文件重建图像，返回色彩映射后的重建图像，np.array(uint8)
     raw_file_to_image reconstruct image from raw video (ser file), return the reconstructed, normalized, color mapped image, np.array(uint8)
 
     :param file: 输入ser文件路径 
     :param file: input file path
     :param shifts: 波长偏移，例如：[-0.5, 0, 0.5]将输出3张偏离谱线中心指定距离的图片，单位为像素
@@ -59,20 +64,20 @@
     :param color_map_name: 色彩映射，取值范围：orange-enhanced (默认), enhanced, linear (不进行任何映射)
     :param color_map_name: color map, values: orange-enhanced (default), enhanced, linear
     :param verbose: 0~3，输出调试信息
     :param verbose: 0~3，log information level
     :return: 色彩映射后的重建图像，np.array(uint8)
     :return: reconstructed, normalized, color mapped image, np.array(uint8)
     """ 
-    imgs = raw_file_to_raw_image(file, shifts, verbose)
-    imgs = [normalize(img).astype(int) for img in imgs]
+    imgs = raw_file_to_raw_image(file, shifts, correct_light_axis, verbose)
+    imgs = [normalize(img, brightness=normalize_brightness, verbose=verbose).astype(int) for img in imgs]
     imgs = [color_map(img, color_map_name) for img in imgs]
     return imgs
 
-def raw_file_to_raw_image(file, shifts = [0], verbose = 0, return_details = False):
+def raw_file_to_raw_image(file, shifts = [0], correct_light_axis = 2, verbose = 0, return_details = False):
     """
     raw_file_to_raw_image 从ser文件重建图像，返回原始值空间的重建图像，np.array(float64)
     raw_file_to_raw_image reconstruct image from raw video (ser file), return the reconstructed image, np.array(float64)
 
     :param file: 输入ser文件路径 
     :param file: input file path
     :param shifts: 波长偏移，例如：[-0.5, 0, 0.5]将输出3张偏离谱线中心指定距离的图片，单位为像素
@@ -100,17 +105,17 @@
     if verbose > 0:
         print(imgs.shape)
     if verbose > 1:
         plt.imshow(imgs[0,:,:])
         plt.show()
     
     # 椭圆拟合
-    edge_points, _ = detect_edge_points(reader, fit)
+    edge_points, raw_lines = detect_edge_points(reader, fit, verbose=verbose)
     edge_points = filter_out_invalid_points(edge_points, 10)
-    ellipse = fit_ellipse(edge_points, verbose=verbose)
+    ellipse = fit_ellipse(edge_points, raw_lines, verbose=verbose)
 
     ret = []
     sz = imgs.shape[1]
     # 图像变换
     for i in range(imgs.shape[0]):
         img = imgs[i,:,:].copy()
 
@@ -121,14 +126,19 @@
             print(f'stack: shape = {img.shape}, group_size = {group_size}')
         shape = img.shape
         img = reduce(img, f'h (w {group_size}) -> h w', 'mean')
         img = cv2.resize(img, shape[::-1])
 
         # 图像变换
         img = warp_frame(ellipse, img, sz)
+        
+        # 杂散光矫正
+        if correct_light_axis > 0:
+            img = correct_light(img, n_axis=correct_light_axis, verbose=verbose)
+        
         ret.append(img)
     
     if return_details:
         return {
             'result': np.array(ret),
             'uncalib': imgs,
             'edge_points': edge_points,
```

### Comparing `astrospec-0.1.0/astrospec/cli.py` & `astrospec-0.2.0/astrospec/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,51 +4,55 @@
 
 import os
 import argparse
 from tqdm import tqdm
 from glob import glob
 from pathlib import Path
 from astrospec import raw_file_to_file
+from .utils import print
 
 def files_to_mp4(folder, output_folder, frame_rate=30):
     os.system(f"""
         ffmpeg -framerate {frame_rate} -pattern_type glob -i '{folder}/*.png' -c:v libx264 -pix_fmt yuv420p '{output_folder}/output.mp4' -y
     """)
 
-def process_folder(input_folder, output_folder, color_map_name, output_video, verbose, **kwargs):
+def process_folder(input_folder, output_folder, raw, correct_light_axis, normalize_brightness, color_map_name, output_video, verbose, **kwargs):
     output_path = os.path.join(input_folder, output_folder)
     os.makedirs(output_path, exist_ok=True)
     for i, file in enumerate(tqdm(sorted(glob(os.path.join(input_folder, '*.SER'))), ncols=80)):
         file_out = os.path.join(output_path, Path(file).stem + '.png')
         if os.path.isfile(file_out):
             print(f'skipped: {file}, output file exists')
             continue
         # print(i, file, file_out)
         try:
-            raw_file_to_file(file, file_out, color_map_name = color_map_name, verbose = verbose)
+            raw_file_to_file(file, file_out, raw = raw, correct_light_axis = correct_light_axis, normalize_brightness = normalize_brightness, color_map_name = color_map_name, verbose = verbose)
         except Exception as e:
             print(e)
     
     if output_video:
         files_to_mp4(output_path, os.path.dirname(output_path))
 
-def process_single_file(input_file, output_folder, color_map_name, verbose, **kwargs):
+def process_single_file(input_file, output_folder, raw, correct_light_axis, normalize_brightness, color_map_name, verbose, **kwargs):
     output_path = os.path.join(os.path.dirname(input_file), output_folder)
     os.makedirs(output_path, exist_ok=True)
     file_out = os.path.join(output_path, Path(input_file).stem + '.png')
-    raw_file_to_file(input_file, file_out, color_map_name = color_map_name, verbose = verbose)
+    raw_file_to_file(input_file, file_out, raw = raw, correct_light_axis = correct_light_axis, normalize_brightness = normalize_brightness, color_map_name = color_map_name, verbose = verbose)
 
 def main():
     parser = argparse.ArgumentParser(description='astronomy spectroheliograph reconstruct tool')
     parser.add_argument('-i', '--input_file', help='Path to the input raw video file(.SER file)', default=None)
     parser.add_argument('-f', '--input_folder', help='Folder of the input raw video file(.SER file)', default=None)
     parser.add_argument('-o', '--output_folder', help='Output folder(relative to the input file)', default='output/img')
+    parser.add_argument('--raw', help='16-bit raw output, without normalization and color mapping', action='store_true', default=False)
+    parser.add_argument('-cr', '--correct_light_axis', help='Remove stray light, 1 for gradient in x-axis only, 2 for both axes', type=int, default=2)
     parser.add_argument('-ov', '--output_video', help='Whether to generate video', action='store_true', default=False)
     parser.add_argument('-c', '--color_map_name', help='Color map', default='orange-enhanced')
-    parser.add_argument('-v', '--verbose', help='verbose', default=0)
+    parser.add_argument('-v', '--verbose', help='verbose', type=int, default=0)
+    parser.add_argument('-nb', '--normalize_brightness', help='Relative target brightness', type=float, default=1)
     args = parser.parse_args()
     print(vars(args))
 
     if args.input_file is not None:
         process_single_file(**vars(args))
     elif args.input_folder is not None:
         process_folder(**vars(args))
```

### Comparing `astrospec-0.1.0/astrospec/postproc.py` & `astrospec-0.2.0/astrospec/postproc.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 from .utils import print
 
 color_maps = {
     'linear': [i for i in range(256)],
-    'orange-enhanced': [[0, 0, 0], [3, 1, 0], [9, 4, 0], [19, 7, 0], [32, 12, 0], [49, 18, 0], [70, 25, 0], [92, 33, 0], [114, 40, 0], [134, 48, 0], [154, 55, 0], [172, 63, 0], [189, 70, 0], [204, 77, 0], [218, 84, 0], [230, 91, 0], [240, 97, 0], [249, 104, 0], [255, 110, 0], [255, 116, 3], [255, 122, 6], [255, 128, 10], [255, 135, 14], [255, 141, 18], [255, 148, 22], [255, 154, 26], [255, 160, 31], [255, 166, 35], [255, 172, 39], [255, 178, 44], [255, 183, 47], [255, 188, 51], [255, 193, 55], [255, 197, 59], [255, 202, 62], [255, 206, 65], [255, 209, 68], [255, 213, 71], [255, 216, 73], [255, 219, 76], [255, 221, 78], [255, 224, 80], [255, 226, 81], [255, 228, 83], [255, 229, 84], [255, 231, 85], [255, 232, 86], [255, 233, 87], [255, 234, 88], [255, 235, 89], [255, 236, 89], [255, 236, 89], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 236, 90], [255, 236, 89], [255, 235, 89], [255, 235, 88], [255, 234, 88], [255, 233, 87], [255, 233, 87], [255, 232, 86], [255, 231, 85], [255, 229, 84], [255, 228, 83], [255, 227, 82], [255, 226, 81], [255, 224, 80], [255, 223, 79], [255, 221, 77], [255, 219, 76], [255, 218, 75], [255, 216, 73], [255, 214, 72], [255, 212, 70], [255, 210, 68], [255, 208, 67], [255, 205, 65], [255, 203, 63], [255, 201, 61], [255, 198, 59], [255, 196, 58], [255, 193, 56], [255, 191, 54], [255, 188, 52], [255, 186, 50], [255, 183, 48], [255, 180, 46], [255, 178, 44], [255, 175, 41], [255, 172, 39], [255, 169, 37], [255, 167, 35], [255, 164, 33], [255, 161, 31], [255, 158, 29], [255, 155, 27], [255, 153, 25], [255, 150, 24], [255, 147, 22], [255, 144, 20], [255, 142, 18], [255, 139, 16], [255, 136, 15], [255, 134, 13], [255, 131, 12], [255, 129, 10], [255, 126, 9], [255, 124, 7], [255, 121, 6], [255, 119, 5], [255, 117, 4], [255, 115, 2], [255, 112, 1], [255, 110, 1], [254, 108, 0], [252, 106, 0], [250, 104, 0], [248, 102, 0], [245, 101, 0], [242, 99, 0], [239, 97, 0], [237, 95, 0], [234, 93, 0], [230, 91, 0], [227, 89, 0], [224, 87, 0], [221, 86, 0], [217, 84, 0], [214, 82, 0], [211, 80, 0], [207, 79, 0], [204, 77, 0], [200, 75, 0], [197, 74, 0], [194, 72, 0], [190, 71, 0], [187, 69, 0], [183, 68, 0], [180, 66, 0], [177, 65, 0], [173, 63, 0], [170, 62, 0], [166, 60, 0], [163, 59, 0], [160, 58, 0], [157, 57, 0], [153, 55, 0], [150, 54, 0], [147, 53, 0], [144, 52, 0], [141, 50, 0], [138, 49, 0], [135, 48, 0], [132, 47, 0], [129, 46, 0], [126, 45, 0], [123, 44, 0], [121, 43, 0], [118, 42, 0], [115, 41, 0], [113, 40, 0], [110, 39, 0], [108, 38, 0], [105, 37, 0], [102, 36, 0], [100, 35, 0], [98, 35, 0], [95, 34, 0], [93, 33, 0], [91, 32, 0], [89, 31, 0], [86, 31, 0], [84, 30, 0], [82, 29, 0], [80, 28, 0], [78, 28, 0], [76, 27, 0], [74, 26, 0], [72, 26, 0], [70, 25, 0], [68, 24, 0], [67, 24, 0], [65, 23, 0], [63, 23, 0], [61, 22, 0], [60, 21, 0], [58, 21, 0], [57, 20, 0], [55, 20, 0], [53, 19, 0], [52, 19, 0], [51, 18, 0], [49, 18, 0], [48, 17, 0], [46, 17, 0], [45, 16, 0], [44, 16, 0], [42, 15, 0], [41, 15, 0], [40, 15, 0], [39, 14, 0], [37, 14, 0], [36, 13, 0], [35, 13, 0], [34, 12, 0], [33, 12, 0], [32, 12, 0], [31, 11, 0], [30, 11, 0], [29, 11, 0], [28, 10, 0], [27, 10, 0], [26, 10, 0], [25, 9, 0], [24, 9, 0], [23, 9, 0], [22, 8, 0], [21, 8, 0], [20, 8, 0], [19, 7, 0], [18, 7, 0], [18, 7, 0], [17, 7, 0], [16, 6, 0], [15, 6, 0], [15, 6, 0], [14, 5, 0], [13, 5, 0], [12, 5, 0], [12, 5, 0], [11, 4, 0], [10, 4, 0], [10, 4, 0], [9, 4, 0], [8, 3, 0], [8, 3, 0], [7, 3, 0], [7, 3, 0], [6, 2, 0], [6, 2, 0], [5, 2, 0], [4, 2, 0], [4, 2, 0], [3, 1, 0], [3, 1, 0], [2, 1, 0], [2, 1, 0], [1, 1, 0], [1, 0, 0], [0, 0, 0], [0, 0, 0]],
+    'orange-enhanced': [[53, 19, 0], [53, 19, 0], [61, 22, 0], [76, 27, 0], [93, 33, 0], [114, 41, 0], [137, 49, 0], [159, 57, 0], [179, 66, 0], [197, 74, 0], [212, 81, 0], [226, 88, 0], [238, 95, 0], [247, 102, 0], [255, 109, 0], [255, 115, 3], [255, 122, 6], [255, 128, 10], [255, 135, 14], [255, 142, 18], [255, 149, 23], [255, 155, 27], [255, 161, 32], [255, 168, 36], [255, 173, 40], [255, 179, 45], [255, 185, 49], [255, 190, 53], [255, 194, 56], [255, 199, 60], [255, 203, 63], [255, 207, 66], [255, 211, 69], [255, 214, 72], [255, 217, 74], [255, 220, 77], [255, 223, 79], [255, 225, 80], [255, 227, 82], [255, 229, 83], [255, 230, 85], [255, 232, 86], [255, 233, 87], [255, 234, 88], [255, 235, 88], [255, 235, 89], [255, 236, 89], [255, 236, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 237, 90], [255, 236, 90], [255, 236, 89], [255, 236, 89], [255, 235, 89], [255, 235, 88], [255, 234, 88], [255, 233, 87], [255, 232, 86], [255, 231, 85], [255, 230, 85], [255, 229, 84], [255, 228, 83], [255, 226, 82], [255, 225, 80], [255, 223, 79], [255, 222, 78], [255, 220, 77], [255, 219, 75], [255, 217, 74], [255, 215, 72], [255, 213, 71], [255, 211, 69], [255, 209, 68], [255, 207, 66], [255, 205, 64], [255, 202, 62], [255, 200, 61], [255, 198, 59], [255, 195, 57], [255, 193, 55], [255, 190, 53], [255, 188, 51], [255, 185, 49], [255, 182, 47], [255, 180, 45], [255, 177, 43], [255, 174, 41], [255, 172, 39], [255, 169, 37], [255, 166, 35], [255, 163, 33], [255, 161, 31], [255, 158, 29], [255, 155, 27], [255, 152, 25], [255, 150, 23], [255, 147, 22], [255, 144, 20], [255, 142, 18], [255, 139, 16], [255, 136, 15], [255, 134, 13], [255, 131, 12], [255, 129, 10], [255, 126, 9], [255, 124, 7], [255, 122, 6], [255, 119, 5], [255, 117, 4], [255, 115, 3], [255, 113, 2], [255, 111, 1], [255, 109, 0], [253, 107, 0], [251, 105, 0], [248, 103, 0], [246, 101, 0], [243, 99, 0], [240, 97, 0], [238, 95, 0], [235, 94, 0], [232, 92, 0], [229, 90, 0], [226, 88, 0], [222, 86, 0], [219, 85, 0], [216, 83, 0], [213, 81, 0], [209, 80, 0], [206, 78, 0], [203, 76, 0], [199, 75, 0], [196, 73, 0], [192, 72, 0], [189, 70, 0], [186, 69, 0], [182, 67, 0], [179, 66, 0], [176, 64, 0], [172, 63, 0], [169, 62, 0], [166, 60, 0], [163, 59, 0], [160, 58, 0], [156, 56, 0], [153, 55, 0], [150, 54, 0], [147, 53, 0], [144, 52, 0], [141, 50, 0], [138, 49, 0], [135, 48, 0], [132, 47, 0], [130, 46, 0], [127, 45, 0], [124, 44, 0], [121, 43, 0], [119, 42, 0], [116, 41, 0], [113, 40, 0], [111, 39, 0], [108, 38, 0], [106, 38, 0], [104, 37, 0], [101, 36, 0], [99, 35, 0], [97, 34, 0], [94, 33, 0], [92, 33, 0], [90, 32, 0], [88, 31, 0], [86, 30, 0], [84, 30, 0], [81, 29, 0], [79, 28, 0], [77, 28, 0], [76, 27, 0], [74, 26, 0], [72, 26, 0], [70, 25, 0], [68, 24, 0], [66, 24, 0], [65, 23, 0], [63, 23, 0], [61, 22, 0], [60, 21, 0], [58, 21, 0], [57, 20, 0], [55, 20, 0], [54, 19, 0], [52, 19, 0], [51, 18, 0], [49, 18, 0], [48, 17, 0], [47, 17, 0], [45, 16, 0], [44, 16, 0], [43, 16, 0], [41, 15, 0], [40, 15, 0], [39, 14, 0], [38, 14, 0], [37, 14, 0], [36, 13, 0], [34, 13, 0], [33, 12, 0], [32, 12, 0], [31, 12, 0], [30, 11, 0], [29, 11, 0], [28, 11, 0], [27, 10, 0], [26, 10, 0], [25, 10, 0], [24, 9, 0], [24, 9, 0], [23, 9, 0], [22, 8, 0], [21, 8, 0], [20, 8, 0], [19, 7, 0], [19, 7, 0], [18, 7, 0], [17, 7, 0], [16, 6, 0], [15, 6, 0], [15, 6, 0], [14, 5, 0], [13, 5, 0], [13, 5, 0], [12, 5, 0], [11, 4, 0], [11, 4, 0], [10, 4, 0], [9, 4, 0], [9, 4, 0], [8, 3, 0], [8, 3, 0], [7, 3, 0], [6, 3, 0], [6, 2, 0], [5, 2, 0], [5, 2, 0], [4, 2, 0], [4, 2, 0], [3, 1, 0], [3, 1, 0], [2, 1, 0], [2, 1, 0], [1, 1, 0], [1, 0, 0], [0, 0, 0], [0, 0, 0]],
     'enhanced': [0, 3, 8, 14, 22, 31, 40, 50, 58, 67, 75, 82, 89, 96, 103, 110, 116, 122, 128, 134, 140, 145, 151, 156, 161, 166, 170, 175, 179, 183, 187, 191, 194, 198, 201, 204, 207, 210, 213, 215, 217, 219, 221, 223, 225, 226, 227, 228, 229, 230, 231, 231, 232, 232, 232, 232, 232, 232, 231, 231, 230, 230, 229, 228, 228, 227, 226, 225, 224, 222, 221, 220, 219, 217, 216, 214, 213, 211, 209, 208, 206, 204, 202, 201, 199, 197, 195, 193, 191, 189, 187, 185, 183, 181, 179, 177, 175, 173, 171, 169, 167, 164, 162, 160, 158, 156, 154, 152, 150, 148, 146, 143, 141, 139, 137, 135, 133, 131, 129, 127, 125, 123, 121, 119, 117, 116, 114, 112, 110, 108, 106, 105, 103, 101, 100, 98, 96, 95, 93, 91, 90, 88, 87, 85, 84, 83, 81, 80, 78, 77, 76, 74, 73, 72, 71, 69, 68, 67, 66, 65, 63, 62, 61, 60, 59, 58, 57, 56, 55, 54, 53, 52, 51, 50, 49, 48, 47, 46, 45, 45, 44, 43, 42, 41, 40, 40, 39, 38, 37, 36, 36, 35, 34, 33, 33, 32, 31, 31, 30, 29, 29, 28, 27, 27, 26, 25, 25, 24, 24, 23, 22, 22, 21, 21, 20, 20, 19, 18, 18, 17, 17, 16, 16, 15, 15, 14, 14, 13, 13, 12, 12, 11, 11, 10, 10, 9, 9, 8, 8, 7, 7, 6, 6, 5, 5, 5, 4, 4, 3, 3, 2, 2, 1, 1, 0, 0],
 }
 
 def color_map(img, map_name = 'orange-enhanced', verbose = 0):
     _map = color_maps[map_name]
     if verbose > 1:
         plt.plot(_map)
@@ -22,15 +22,15 @@
     # _map = np.array(_map)
     # _func = np.vectorize(lambda x: _map[x], signature='()->(3)')
     # return _func(img)
 
     # faster
     return np.array([[_map[item] for item in row] for row in img])
 
-def normalize(img, verbose=0):
+def normalize(img, brightness=1.0, verbose=0):
     # 方法一：主体部分亮度均衡
     n, e = np.histogram(img, bins=100)
     if verbose > 1:
         plt.plot(n[20:])
         plt.show()
     med_idx = np.argsort(n[20:])[::-1] + 20
     # 直方图最高的3箱
@@ -38,15 +38,15 @@
     idx_b = min(max(med_idx[:3])+1, len(e)-1)
     med_val_a = e[idx_a]
     med_val_b = e[idx_b]
     # 直方图最高的3箱像素均值
     med_val = np.mean(img[(img>med_val_a) & (img<med_val_b)])
     # print(med_idx[:3], idx_a, idx_b)
     # print(med_val)
-    img = np.clip(img/med_val*152, 0, 255)
+    img = np.clip(img/med_val*152*brightness, 0, 255)
 
     # 方法二：按最亮的0.001部分归一化
     # val_max = np.quantile(img, 0.999) * 1.2
     # img = np.clip(img/val_max*255, 0, 255)
 
     if verbose > 0:
         print(f'overflow = {len(img[img==255]) / len(np.reshape(img, -1)) * 100:.3f}%')
```

### Comparing `astrospec-0.1.0/astrospec/shape_correction.py` & `astrospec-0.2.0/astrospec/shape_correction.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,35 +67,37 @@
     ret = []
     for idx in idxes:
         a, b = arr[idx], arr[idx+1]
         # print(a, b, thd)
         ret.append(idx + (thd-a)/(b-a))
     return ret
 
-def detect_edge_points(reader, fit, shifts=[10]):
+def detect_edge_points(reader, fit, shifts=[10], verbose=0):
     lines = []
     raw_lines = []
     line_maxval = []
     for i,img in enumerate(reader):
         # line = gaussian_filter(reduce(img.astype(float), 'h w -> h', 'mean'), sigma=3)
         # print(i)
         line = frame_to_line(img, fit, shifts=shifts)
         line = line.astype(float)[0,:]
         # line = gaussian_filter(line, sigma=3)
         raw_lines.append(line)
         # 变化最快
         # line = line[:-1] - line[1:]
-        # plt.plot(line, color='r')
-        # plt.show()
         # lines.append([np.argmin(line), np.argmax(line)])
         # 穿过1/4最大强度
-        thd_val = np.max(line)
+        _min = np.min(line)
+        thd_val = (np.max(line) - _min)
         line_maxval.append(thd_val)
-        thd_val = thd_val/4
+        thd_val = _min + thd_val/4
         lines.append(cross_points(line, thd_val))
+        if verbose > 3 and (i%50) == 0:
+            plt.plot(line, color='r')
+            plt.show()
 
     line_maxval = np.array(line_maxval)
     lines = np.array(lines)
     raw_lines = np.array(raw_lines)
     
     # 去除太暗的结果
     invalid = line_maxval < np.max(line_maxval) / 4
@@ -113,15 +115,15 @@
 
     invalid |= abs(x[:,0] - x[:,1]) < 10
 
     x[invalid,:] = np.nan
 
     return x
 
-def fit_ellipse(edge_points, verbose=0):
+def fit_ellipse(edge_points, raw_lines, verbose=0):
     points = []
     for x, ys in enumerate(edge_points):
         for y in ys:
             if not np.isnan(y):
                 points.append([x, y])
     points = np.array(points)
 
@@ -131,17 +133,18 @@
 
     if verbose > 0:
         print(center, width, height, phi)
         
     if verbose > 1:
         # fig = plt.figure(figsize=(6, 6))
         ax = plt.subplot()
-        # ax.axis('equal')
-        # ax.plot(X1, X2, 'ro', zorder=1)
-        ax.plot(edge_points)
+        print(raw_lines.shape)
+        ax.imshow(raw_lines.T)
+        
+        ax.scatter(points[:,0], points[:,1], marker='x', c='r')
         ellipse = Ellipse(
             xy=center, width=2*width, height=2*height, angle=phi,
             edgecolor='b', fc='None', lw=1, label='Fit', zorder=2
         )
         ax.add_patch(ellipse)
         plt.show()
```

### Comparing `astrospec-0.1.0/astrospec/spectrum.py` & `astrospec-0.2.0/astrospec/spectrum.py`

 * *Files identical despite different names*

### Comparing `astrospec-0.1.0/astrospec/video_reader.py` & `astrospec-0.2.0/astrospec/video_reader.py`

 * *Files identical despite different names*

### Comparing `astrospec-0.1.0/setup.py` & `astrospec-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="astrospec",
-    version="0.1.0",
+    version="0.2.0",
     author="liangchen",
     author_email="lcpcsky@gmail.com",
     description="astronomy spectroheliograph data processing tools",
     url="https://github.com/liangchen-harold/astrospec",
     packages=find_packages(),
     install_requires=[
         "einops~=0.8.0",
```

