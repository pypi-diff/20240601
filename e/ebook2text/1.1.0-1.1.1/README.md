# Comparing `tmp/ebook2text-1.1.0.tar.gz` & `tmp/ebook2text-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebook2text-1.1.0.tar", last modified: Fri May 31 15:52:27 2024, max compression
+gzip compressed data, was "ebook2text-1.1.1.tar", last modified: Sat Jun  1 05:33:47 2024, max compression
```

## Comparing `ebook2text-1.1.0.tar` & `ebook2text-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 15:52:27.005857 ebook2text-1.1.0/
--rw-rw-rw-   0        0        0     4542 2024-05-31 15:52:27.005857 ebook2text-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2555 2024-05-31 10:17:21.000000 ebook2text-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 15:52:26.983039 ebook2text-1.1.0/ebook2text/
--rw-rw-rw-   0        0        0       23 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/VERSION.py
--rw-rw-rw-   0        0        0      224 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/__init__.py
--rw-rw-rw-   0        0        0      457 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/_exceptions.py
--rw-rw-rw-   0        0        0      314 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/_namespaces.py
--rw-rw-rw-   0        0        0      471 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/_types.py
--rw-rw-rw-   0        0        0     2088 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/abstract_book.py
--rw-rw-rw-   0        0        0     5907 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/chapter_check.py
--rw-rw-rw-   0        0        0     1533 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/convert_file.py
--rw-rw-rw-   0        0        0    10889 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/docx_conversion.py
--rw-rw-rw-   0        0        0     5887 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/epub_conversion.py
--rw-rw-rw-   0        0        0      253 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/file_handling.py
--rw-rw-rw-   0        0        0     2758 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/ocr.py
--rw-rw-rw-   0        0        0    17533 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/pdf_conversion.py
--rw-rw-rw-   0        0        0     1583 2024-05-31 10:11:29.000000 ebook2text-1.1.0/ebook2text/text_conversion.py
-drwxrwxrwx   0        0        0        0 2024-05-31 15:52:27.004860 ebook2text-1.1.0/ebook2text.egg-info/
--rw-rw-rw-   0        0        0     4542 2024-05-31 15:52:26.000000 ebook2text-1.1.0/ebook2text.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-05-31 15:52:26.000000 ebook2text-1.1.0/ebook2text.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 15:52:26.000000 ebook2text-1.1.0/ebook2text.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      427 2024-05-31 15:52:26.000000 ebook2text-1.1.0/ebook2text.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 15:52:26.000000 ebook2text-1.1.0/ebook2text.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 15:52:27.002855 ebook2text-1.1.0/folder/
--rw-rw-rw-   0        0        0      430 2024-05-31 06:36:01.000000 ebook2text-1.1.0/folder/files.py
--rw-rw-rw-   0        0        0     1071 2024-05-31 10:11:29.000000 ebook2text-1.1.0/license.txt
--rw-rw-rw-   0        0        0     2060 2024-05-31 15:52:14.000000 ebook2text-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2024-05-31 15:52:27.010863 ebook2text-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-05-31 15:13:21.000000 ebook2text-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.217872 ebook2text-1.1.1/
+-rw-rw-rw-   0        0        0     4101 2024-06-01 05:33:47.217872 ebook2text-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-06-01 05:22:29.000000 ebook2text-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.202872 ebook2text-1.1.1/ebook2text/
+-rw-rw-rw-   0        0        0       23 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebook2text/VERSION.py
+-rw-rw-rw-   0        0        0      224 2024-06-01 05:33:33.000000 ebook2text-1.1.1/ebook2text/__init__.py
+-rw-rw-rw-   0        0        0      457 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/_exceptions.py
+-rw-rw-rw-   0        0        0      314 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/_namespaces.py
+-rw-rw-rw-   0        0        0      471 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/_types.py
+-rw-rw-rw-   0        0        0     2088 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/abstract_book.py
+-rw-rw-rw-   0        0        0     5907 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/chapter_check.py
+-rw-rw-rw-   0        0        0     1533 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/convert_file.py
+-rw-rw-rw-   0        0        0    10889 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/docx_conversion.py
+-rw-rw-rw-   0        0        0     5887 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/epub_conversion.py
+-rw-rw-rw-   0        0        0      253 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/file_handling.py
+-rw-rw-rw-   0        0        0     2758 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/ocr.py
+-rw-rw-rw-   0        0        0    17533 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/pdf_conversion.py
+-rw-rw-rw-   0        0        0     1583 2024-05-31 10:11:29.000000 ebook2text-1.1.1/ebook2text/text_conversion.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.216871 ebook2text-1.1.1/ebook2text.egg-info/
+-rw-rw-rw-   0        0        0     4101 2024-06-01 05:33:47.000000 ebook2text-1.1.1/ebook2text.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2024-06-01 05:33:47.000000 ebook2text-1.1.1/ebook2text.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 05:33:47.000000 ebook2text-1.1.1/ebook2text.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-06-01 05:33:47.000000 ebook2text-1.1.1/ebook2text.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-06-01 05:33:47.000000 ebook2text-1.1.1/ebook2text.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.210871 ebook2text-1.1.1/ebooklib/
+-rw-rw-rw-   0        0        0     1555 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/__init__.py
+-rw-rw-rw-   0        0        0    59997 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/epub.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.214872 ebook2text-1.1.1/ebooklib/plugins/
+-rw-rw-rw-   0        0        0        0 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1595 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/base.py
+-rw-rw-rw-   0        0        0     4478 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/booktype.py
+-rw-rw-rw-   0        0        0     2549 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/sourcecode.py
+-rw-rw-rw-   0        0        0    12764 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/standard.py
+-rw-rw-rw-   0        0        0     2399 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/plugins/tidyhtml.py
+-rw-rw-rw-   0        0        0     3327 2024-06-01 05:22:29.000000 ebook2text-1.1.1/ebooklib/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:33:47.215872 ebook2text-1.1.1/folder/
+-rw-rw-rw-   0        0        0      430 2024-05-31 06:36:01.000000 ebook2text-1.1.1/folder/files.py
+-rw-rw-rw-   0        0        0     1071 2024-05-31 10:11:29.000000 ebook2text-1.1.1/license.txt
+-rw-rw-rw-   0        0        0     1770 2024-06-01 05:22:29.000000 ebook2text-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      214 2024-06-01 05:33:47.220307 ebook2text-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2024-06-01 05:33:35.000000 ebook2text-1.1.1/setup.py
```

### Comparing `ebook2text-1.1.0/PKG-INFO` & `ebook2text-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,39 @@
 Metadata-Version: 2.1
 Name: ebook2text
-Version: 1.1.0
+Version: 1.1.1
 Summary: Convert common book file types to text for machine learning
 Author: Ashlynn Antrobus
 Author-email: Ashlynn Antrobus <ashlynn@prosepal.io>
 License: MIT
 Project-URL: Respository, https://github.com/ashrobertsdragon/Ebook-conversion-to-Text-for-Machine-Learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: anyio<5,>3.5
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: certifi>=2024.2.2
-Requires-Dist: cffi>=1.12
-Requires-Dist: colorama>=0.4.6
-Requires-Dist: cryptography>=42.0.7
-Requires-Dist: distro<2,>=1.7
-Requires-Dist: EbookLib==0.18
-Requires-Dist: h11<=0.15,>=0.13
-Requires-Dist: httpcore>1
-Requires-Dist: httpx<1,>=0.23.0
-Requires-Dist: idna<4,>2.8.0
-Requires-Dist: lxml>3.1.0
 Requires-Dist: openai>=1.30.1
 Requires-Dist: pillow>=10.2.0
-Requires-Dist: pycparser==2.22
-Requires-Dist: pydantic<3,>1.9
-Requires-Dist: pydantic-core==2.18.2
 Requires-Dist: python-docx>=1.1.0
 Requires-Dist: python-dotenv>=1.0.1
-Requires-Dist: six==1.16.0
-Requires-Dist: sniffio>=1.1.0
-Requires-Dist: soupsieve>1.2
-Requires-Dist: tqdm>=4.0.0
-Requires-Dist: typing-extensions>=4.9.0
+Requires-Dist: pdfminer.six>=0231228
 
 
 # Convert Ebook File
 
 ## Overview
 
 This Python script provides functionality for converting various ebook file formats (EPUB, DOCX, PDF, TXT) into a standardized text format. The script processes each file, identifying chapters, and replaces chapter headers with asterisks. It also performs OCR (Optical Character Recognition) for image-based text using GPT-4o and standardizes the text by desmartenizing punctuation.
@@ -123,7 +104,10 @@
   - setup.py and requirements.txt typo fixed
 
 - **v1.0.2** (Release date: May 17, 2024)
   - added tests, fixex minor typos
 
 - **v1.1.0** (Release date: May 30, 2024)
   - Change to abstract factory pattern
+
+- **v1.1.1** (Release date: May 31, 2024)
+  - Pulled current version of ebooklib from Github and folded it into library since package repo out of date
```

### Comparing `ebook2text-1.1.0/README.md` & `ebook2text-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,7 +71,10 @@
   - setup.py and requirements.txt typo fixed
 
 - **v1.0.2** (Release date: May 17, 2024)
   - added tests, fixex minor typos
 
 - **v1.1.0** (Release date: May 30, 2024)
   - Change to abstract factory pattern
+
+- **v1.1.1** (Release date: May 31, 2024)
+  - Pulled current version of ebooklib from Github and folded it into library since package repo out of date
```

### Comparing `ebook2text-1.1.0/ebook2text/abstract_book.py` & `ebook2text-1.1.1/ebook2text/abstract_book.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/chapter_check.py` & `ebook2text-1.1.1/ebook2text/chapter_check.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/convert_file.py` & `ebook2text-1.1.1/ebook2text/convert_file.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/docx_conversion.py` & `ebook2text-1.1.1/ebook2text/docx_conversion.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/epub_conversion.py` & `ebook2text-1.1.1/ebook2text/epub_conversion.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/ocr.py` & `ebook2text-1.1.1/ebook2text/ocr.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/pdf_conversion.py` & `ebook2text-1.1.1/ebook2text/pdf_conversion.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text/text_conversion.py` & `ebook2text-1.1.1/ebook2text/text_conversion.py`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/ebook2text.egg-info/PKG-INFO` & `ebook2text-1.1.1/ebook2text.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,39 @@
 Metadata-Version: 2.1
 Name: ebook2text
-Version: 1.1.0
+Version: 1.1.1
 Summary: Convert common book file types to text for machine learning
 Author: Ashlynn Antrobus
 Author-email: Ashlynn Antrobus <ashlynn@prosepal.io>
 License: MIT
 Project-URL: Respository, https://github.com/ashrobertsdragon/Ebook-conversion-to-Text-for-Machine-Learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: anyio<5,>3.5
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: certifi>=2024.2.2
-Requires-Dist: cffi>=1.12
-Requires-Dist: colorama>=0.4.6
-Requires-Dist: cryptography>=42.0.7
-Requires-Dist: distro<2,>=1.7
-Requires-Dist: EbookLib==0.18
-Requires-Dist: h11<=0.15,>=0.13
-Requires-Dist: httpcore>1
-Requires-Dist: httpx<1,>=0.23.0
-Requires-Dist: idna<4,>2.8.0
-Requires-Dist: lxml>3.1.0
 Requires-Dist: openai>=1.30.1
 Requires-Dist: pillow>=10.2.0
-Requires-Dist: pycparser==2.22
-Requires-Dist: pydantic<3,>1.9
-Requires-Dist: pydantic-core==2.18.2
 Requires-Dist: python-docx>=1.1.0
 Requires-Dist: python-dotenv>=1.0.1
-Requires-Dist: six==1.16.0
-Requires-Dist: sniffio>=1.1.0
-Requires-Dist: soupsieve>1.2
-Requires-Dist: tqdm>=4.0.0
-Requires-Dist: typing-extensions>=4.9.0
+Requires-Dist: pdfminer.six>=0231228
 
 
 # Convert Ebook File
 
 ## Overview
 
 This Python script provides functionality for converting various ebook file formats (EPUB, DOCX, PDF, TXT) into a standardized text format. The script processes each file, identifying chapters, and replaces chapter headers with asterisks. It also performs OCR (Optical Character Recognition) for image-based text using GPT-4o and standardizes the text by desmartenizing punctuation.
@@ -123,7 +104,10 @@
   - setup.py and requirements.txt typo fixed
 
 - **v1.0.2** (Release date: May 17, 2024)
   - added tests, fixex minor typos
 
 - **v1.1.0** (Release date: May 30, 2024)
   - Change to abstract factory pattern
+
+- **v1.1.1** (Release date: May 31, 2024)
+  - Pulled current version of ebooklib from Github and folded it into library since package repo out of date
```

### Comparing `ebook2text-1.1.0/ebook2text.egg-info/SOURCES.txt` & `ebook2text-1.1.1/ebook2text.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,8 +19,17 @@
 ebook2text/pdf_conversion.py
 ebook2text/text_conversion.py
 ebook2text.egg-info/PKG-INFO
 ebook2text.egg-info/SOURCES.txt
 ebook2text.egg-info/dependency_links.txt
 ebook2text.egg-info/requires.txt
 ebook2text.egg-info/top_level.txt
+ebooklib/__init__.py
+ebooklib/epub.py
+ebooklib/utils.py
+ebooklib/plugins/__init__.py
+ebooklib/plugins/base.py
+ebooklib/plugins/booktype.py
+ebooklib/plugins/sourcecode.py
+ebooklib/plugins/standard.py
+ebooklib/plugins/tidyhtml.py
 folder/files.py
```

### Comparing `ebook2text-1.1.0/license.txt` & `ebook2text-1.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `ebook2text-1.1.0/pyproject.toml` & `ebook2text-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,66 +8,49 @@
 readme = "README.md"
 authors = [{name = "Ashlynn Antrobus", email = "ashlynn@prosepal.io"}]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
+    "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Text Processing"
 ]
 requires-python = ">= 3.8"
 dependencies = [
-    "annotated-types>=0.4.0",
-    "anyio>3.5,<5",
     "beautifulsoup4>=4.12.3",
-    "certifi>=2024.2.2",
-    "cffi>=1.12",
-    "colorama>=0.4.6",
-    "cryptography>=42.0.7",
-    "distro>=1.7,<2",
-    "EbookLib==0.18",
-    "h11>=0.13,<=0.15",
-    "httpcore>1",
-    "httpx>=0.23.0,<1",
-    "idna>2.8.0,<4",
-    "lxml>3.1.0",
     "openai>=1.30.1",
     "pillow>=10.2.0",
-    "pycparser==2.22",
-    "pydantic>1.9,<3",
-    "pydantic-core==2.18.2",
     "python-docx>=1.1.0",
     "python-dotenv>=1.0.1",
-    "six==1.16.0",
-    "sniffio>=1.1.0",
-    "soupsieve>1.2",
-    "tqdm>=4.0.0",
-    "typing-extensions>=4.9.0"
+    "pdfminer.six>=0231228"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Respository = "https://github.com/ashrobertsdragon/Ebook-conversion-to-Text-for-Machine-Learning"
 
 [tool.ruff]
 line-length = 79
-exclude = [".git", "__pycache__",".venv"]
+force-exclude = true
+exclude = [".git", "__pycache__", ".venv", "ebooklib", "dist", "build", ".vscode", ".egg-info"]
 
 [tool.flake8]
 max_line_length = 79
-exclude = [".git", "__pycache__", ".venv"]
+exclude = [".git", "__pycache__", ".venv", "ebooklib", "dist", "build", ".vscode", ".egg-info"]
 
 [tool.isort]
 line_length = 79
 
 [tool.mypy]
 disable_error_code = "import-untyped"
+exclude = "ebooklib"
```

### Comparing `ebook2text-1.1.0/setup.py` & `ebook2text-1.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,13 @@
     long_description=long_description,
     author="Ashlynn Antrobus",
     author_email="ashlynn@prosepal.io",
     packages=find_packages(),
     install_requires=[
         "pdfminer.six",
         "pillow",
-        "EbookLib",
         "beautifulsoup4",
         "python-docx",
         "python-dotenv",
         "openai",
     ],
 )
```

