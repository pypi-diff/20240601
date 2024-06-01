# Comparing `tmp/yomitandic-0.1.7.tar.gz` & `tmp/yomitandic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yomitandic-0.1.7.tar", last modified: Sun Mar 10 21:55:50 2024, max compression
+gzip compressed data, was "yomitandic-0.1.8.tar", last modified: Sun Mar 10 22:17:20 2024, max compression
```

## Comparing `yomitandic-0.1.7.tar` & `yomitandic-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 21:55:50.264026 yomitandic-0.1.7/
--rw-rw-rw-   0        0        0      211 2024-03-10 21:55:50.264026 yomitandic-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2913 2024-03-10 14:32:19.000000 yomitandic-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 21:55:50.260026 yomitandic-0.1.7/YomitanDic.egg-info/
--rw-rw-rw-   0        0        0      211 2024-03-10 21:55:50.000000 yomitandic-0.1.7/YomitanDic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-03-10 21:55:50.000000 yomitandic-0.1.7/YomitanDic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 21:55:50.000000 yomitandic-0.1.7/YomitanDic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-10 21:55:50.000000 yomitandic-0.1.7/YomitanDic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-10 21:55:50.264026 yomitandic-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-03-10 21:55:31.000000 yomitandic-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 21:55:50.262027 yomitandic-0.1.7/yomitandic/
--rw-rw-rw-   0        0        0       65 2024-03-10 21:16:48.000000 yomitandic-0.1.7/yomitandic/__init__.py
--rw-rw-rw-   0        0        0     5754 2024-03-10 21:55:20.000000 yomitandic-0.1.7/yomitandic/yomitandic.py
+drwxrwxrwx   0        0        0        0 2024-03-10 22:17:20.831691 yomitandic-0.1.8/
+-rw-rw-rw-   0        0        0      211 2024-03-10 22:17:20.831691 yomitandic-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2913 2024-03-10 14:32:19.000000 yomitandic-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-03-10 22:17:20.828693 yomitandic-0.1.8/YomitanDic.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-03-10 22:17:20.000000 yomitandic-0.1.8/YomitanDic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-03-10 22:17:20.000000 yomitandic-0.1.8/YomitanDic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-10 22:17:20.000000 yomitandic-0.1.8/YomitanDic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-03-10 22:17:20.000000 yomitandic-0.1.8/YomitanDic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-10 22:17:20.831691 yomitandic-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-03-10 22:16:48.000000 yomitandic-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-10 22:17:20.829692 yomitandic-0.1.8/yomitandic/
+-rw-rw-rw-   0        0        0       65 2024-03-10 21:16:48.000000 yomitandic-0.1.8/yomitandic/__init__.py
+-rw-rw-rw-   0        0        0     5993 2024-03-10 22:16:37.000000 yomitandic-0.1.8/yomitandic/yomitandic.py
```

### Comparing `yomitandic-0.1.7/README.md` & `yomitandic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `yomitandic-0.1.7/yomitandic/yomitandic.py` & `yomitandic-0.1.8/yomitandic/yomitandic.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,22 @@
                 create_html_element("li", [create_html_element("a", link, href=link)])
             ], style={"listStyleType": "\"⧉\""})
         ]
         self.structured_content = True
 
     def validate_element(self, element):
         allowed_elements = ["br", "ruby", "rt", "rp", "table", "thead", "tbody", "tfoot", "tr", "td", "th", "span", "div", "ol", "ul", "li", "img", "a"]
+        allowed_href_elements = ["a"]
+
         if element["tag"] not in allowed_elements:
             raise ValueError(f"Unsupported HTML element: {element['tag']}")
+
+        if "href" in element and element["tag"] not in allowed_href_elements:
+            raise ValueError(f"The 'href' attribute is not allowed in the '{element['tag']}' element, only <a>.")
+
         if "content" in element:
             if isinstance(element["content"], list):
                 for child_element in element["content"]:
                     self.validate_element(child_element)
             elif not isinstance(element["content"], str):
                 raise ValueError("Content must be a string or a list of elements")
```

