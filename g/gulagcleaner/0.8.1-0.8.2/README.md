# Comparing `tmp/gulagcleaner-0.8.1.tar.gz` & `tmp/gulagcleaner-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.8.1.tar", last modified: Thu Sep 21 16:25:44 2023, max compression
+gzip compressed data, was "gulagcleaner-0.8.2.tar", last modified: Thu Sep 21 16:45:55 2023, max compression
```

## Comparing `gulagcleaner-0.8.1.tar` & `gulagcleaner-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-21 16:25:44.965318 gulagcleaner-0.8.1/
--rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     3185 2023-09-21 16:25:44.965318 gulagcleaner-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2023-09-19 15:10:13.000000 gulagcleaner-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-09-21 16:25:44.939463 gulagcleaner-0.8.1/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.8.1/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     4166 2023-09-21 16:21:42.000000 gulagcleaner-0.8.1/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.8.1/gulagcleaner/decrypt.py
--rw-rw-rw-   0        0        0     8210 2023-09-19 16:08:52.000000 gulagcleaner-0.8.1/gulagcleaner/extract.py
--rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.8.1/gulagcleaner/metadata.py
-drwxrwxrwx   0        0        0        0 2023-09-21 16:25:44.963286 gulagcleaner-0.8.1/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     3185 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-09-21 16:25:44.000000 gulagcleaner-0.8.1/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0      834 2023-09-21 16:25:44.971834 gulagcleaner-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-09-21 16:45:55.754105 gulagcleaner-0.8.2/
+-rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0     3697 2023-09-21 16:45:55.752668 gulagcleaner-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3056 2023-09-21 16:45:37.000000 gulagcleaner-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-09-21 16:45:55.730759 gulagcleaner-0.8.2/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.8.2/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     4195 2023-09-21 16:39:01.000000 gulagcleaner-0.8.2/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.8.2/gulagcleaner/decrypt.py
+-rw-rw-rw-   0        0        0     8670 2023-09-21 16:36:54.000000 gulagcleaner-0.8.2/gulagcleaner/extract.py
+-rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.8.2/gulagcleaner/metadata.py
+drwxrwxrwx   0        0        0        0 2023-09-21 16:45:55.751668 gulagcleaner-0.8.2/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     3697 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-09-21 16:45:55.000000 gulagcleaner-0.8.2/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0      834 2023-09-21 16:45:55.760108 gulagcleaner-0.8.2/setup.cfg
```

### Comparing `gulagcleaner-0.8.1/LICENSE` & `gulagcleaner-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.8.1/PKG-INFO` & `gulagcleaner-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -76,7 +76,14 @@
 ```
 
 # License
 Gulag Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.
 
 # Contributing
 We're always looking for ways to improve Gulag Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.
+
+## TODO
+If you want to help, these are the top priorities right now:
+
+* Revamp the argument parsing. We should use some parsing library to allow for short "-v" and long "--version" arguments. Idealy it should support parameters for each argument.
+
+* Add the "Naive" cleaning method. This method is just a fallback that crops the Ads by zooming in and moving the MediaBox. This is not ideal, but there will always be edge cases not covered in the other methods and doing this better than giving an error.
```

### Comparing `gulagcleaner-0.8.1/README.md` & `gulagcleaner-0.8.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -58,7 +58,14 @@
 ```
 
 # License
 Gulag Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.
 
 # Contributing
 We're always looking for ways to improve Gulag Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.
+
+## TODO
+If you want to help, these are the top priorities right now:
+
+* Revamp the argument parsing. We should use some parsing library to allow for short "-v" and long "--version" arguments. Idealy it should support parameters for each argument.
+
+* Add the "Naive" cleaning method. This method is just a fallback that crops the Ads by zooming in and moving the MediaBox. This is not ideal, but there will always be edge cases not covered in the other methods and doing this better than giving an error.
```

### Comparing `gulagcleaner-0.8.1/gulagcleaner/command_line.py` & `gulagcleaner-0.8.2/gulagcleaner/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from gulagcleaner.extract import clean_pdf
 from gulagcleaner.decrypt import decrypt_pdf
 from gulagcleaner.metadata import extract_metadata
 from os.path import exists, isdir, join
-from os import listdir
+from os import listdir, remove
 
 def parseArgs():
     '''
     Function to parse arguments.
 
     Checks for any optional arguments passed to the program and activates
     the corresponding flags.
@@ -54,15 +54,15 @@
         print("  -r            Replace original files with their cleaned version.")
         print("  -s            Do not show metadata about cleaned files.")
         print("  -v            Show the version of the program.")
         return
 
     # Check for the -v argument
     if arguments["version"]:
-        print("Current version: 0.8.1")
+        print("Current version: 0.8.2")
         return
 
     # Get the pdf_path argument
     if len(arguments["files"]) == 0:
         print('Usage: gulagcleaner [-h] [-r] [-s] [-v] <pdf_path>...')
         return
     
@@ -87,15 +87,15 @@
         if replace:
             output_path = pdf_path
         else:
             output_path = pdf_path[:-4] + "_clean.pdf"
         
         # We decrypt the PDF file
         pdf_path = decrypt_pdf(pdf_path)
-
+        
         # If short mode is not active, extract metadata
         if not short:
             try:
                 metadict = extract_metadata(pdf_path)
                 print("Metadata:")
                 print("Archivo: " + metadict["Archivo"])
                 print("Autor: " + metadict["Autor"])
@@ -104,16 +104,16 @@
                 print("Facultad: " + metadict["Facultad"])
                 print("Universidad: " + metadict["Universidad"])
             except Exception as e:
                 print("Failed to extract metadata:", e)
 
         # Call the cleaning function
         return_msg = clean_pdf(pdf_path, output_path)
-
+        remove(pdf_path)
         if return_msg["Success"]:
-            print(pdf_path + "cleaning successful. File saved in " + 
+            print("Cleaning successful. File saved in " + 
                   return_msg["return_path"])
         else:
             print("Error cleaning " + pdf_path + ": " + return_msg["Error"])
 
 if __name__ == "__main__":
     print('Call from the "gulagcleaner" command.')
```

### Comparing `gulagcleaner-0.8.1/gulagcleaner/extract.py` & `gulagcleaner-0.8.2/gulagcleaner/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,17 @@
             newpages = []
             for i,page in enumerate([page for page in pdf.pages if len(page.Contents)>1]):
                 newpage = page.copy()
                 newpage.Contents = [pdf.indirect_objects[iobj] for iobj in new_contents[i]]
                 newpage.Annots = []
                 newpage.MediaBox = PdfArray([0,0,float(newpage.MediaBox[2])-float(newpage.MediaBox[0]),float(newpage.MediaBox[3])-float(newpage.MediaBox[1])])
                 newpage.BleedBox = PdfArray([0,0,float(newpage.BleedBox[2])-float(newpage.BleedBox[0]),float(newpage.BleedBox[3])-float(newpage.BleedBox[1])])
+                newpage.TrimBox = PdfArray([0,0,float(newpage.TrimBox[2])-float(newpage.TrimBox[0]),float(newpage.TrimBox[3])-float(newpage.TrimBox[1])])
+                newpage.ArtBox = PdfArray([0,0,float(newpage.ArtBox[2])-float(newpage.ArtBox[0]),float(newpage.ArtBox[3])-float(newpage.ArtBox[1])])
+                newpage.CropBox = PdfArray([0,0,float(newpage.CropBox[2])-float(newpage.CropBox[0]),float(newpage.CropBox[3])-float(newpage.CropBox[1])])
                 newpages.append(newpage)
 
         #Naive method. Just detects the pages with ads and crops them. THIS METHOD IS NOT RECOMENDED AT ALL. It is very unreliable and when copying text from the outputed pdf the ads and watermaks are copied as well, because we are just "hiding" them from the user, not truly removing them.
         elif method=="naive":
             #Not yet implemented.
             newpages = []
             for page in pdf.pages:
```

### Comparing `gulagcleaner-0.8.1/gulagcleaner/metadata.py` & `gulagcleaner-0.8.2/gulagcleaner/metadata.py`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.8.1/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.8.2/gulagcleaner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -76,7 +76,14 @@
 ```
 
 # License
 Gulag Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.
 
 # Contributing
 We're always looking for ways to improve Gulag Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.
+
+## TODO
+If you want to help, these are the top priorities right now:
+
+* Revamp the argument parsing. We should use some parsing library to allow for short "-v" and long "--version" arguments. Idealy it should support parameters for each argument.
+
+* Add the "Naive" cleaning method. This method is just a fallback that crops the Ads by zooming in and moving the MediaBox. This is not ideal, but there will always be edge cases not covered in the other methods and doing this better than giving an error.
```

### Comparing `gulagcleaner-0.8.1/setup.cfg` & `gulagcleaner-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e38 2e31  .version = 0.8.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e38 2e32  .version = 0.8.2
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2064 6176 6964 2e66 6f6e 7461 6e65 6461   david.fontaneda
 00000060: 3136 4067 6d61 696c 2e63 6f6d 0d0a 6465  16@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4164 2072  scription = Ad r
 00000080: 656d 6f76 616c 2074 6f6f 6c20 666f 7220  emoval tool for 
 00000090: 5044 4673 2077 7269 7474 656e 2069 6e20  PDFs written in
```

