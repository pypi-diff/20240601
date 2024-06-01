# Comparing `tmp/worldnewsapi-1.0.9.tar.gz` & `tmp/worldnewsapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worldnewsapi-1.0.9.tar", last modified: Thu Mar  7 22:53:40 2024, max compression
+gzip compressed data, was "worldnewsapi-1.1.1.tar", last modified: Sat Jun  1 00:46:46 2024, max compression
```

## Comparing `worldnewsapi-1.0.9.tar` & `worldnewsapi-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.406098 worldnewsapi-1.0.9/
--rw-rw-rw-   0        0        0     2054 2024-03-07 22:53:40.406098 worldnewsapi-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/README.md
--rw-rw-rw-   0        0        0     1113 2024-03-07 13:36:21.000000 worldnewsapi-1.0.9/README_pypi.md
--rw-rw-rw-   0        0        0     2671 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       76 2024-03-07 22:53:40.407096 worldnewsapi-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1234 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.375962 worldnewsapi-1.0.9/test/
--rw-rw-rw-   0        0        0     1477 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/test/test_extract_links_response.py
--rw-rw-rw-   0        0        0     1629 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/test/test_extract_news_response.py
--rw-rw-rw-   0        0        0     1589 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_geo_coordinates_response.py
--rw-rw-rw-   0        0        0     1537 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_news.py
--rw-rw-rw-   0        0        0     1283 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/test/test_news_api.py
--rw-rw-rw-   0        0        0     1622 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_news_article.py
--rw-rw-rw-   0        0        0     2646 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/test/test_search_news_response.py
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.380962 worldnewsapi-1.0.9/worldnewsapi/
--rw-rw-rw-   0        0        0     1317 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.399414 worldnewsapi-1.0.9/worldnewsapi/api/
--rw-rw-rw-   0        0        0       93 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/api/__init__.py
--rw-rw-rw-   0        0        0    79356 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/api/news_api.py
--rw-rw-rw-   0        0        0    26009 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/api_client.py
--rw-rw-rw-   0        0        0      688 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/api_response.py
--rw-rw-rw-   0        0        0    15674 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/configuration.py
--rw-rw-rw-   0        0        0     6213 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.403924 worldnewsapi-1.0.9/worldnewsapi/models/
--rw-rw-rw-   0        0        0      745 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/models/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/worldnewsapi/models/extract_links_response.py
--rw-rw-rw-   0        0        0     3412 2024-03-07 22:53:11.000000 worldnewsapi-1.0.9/worldnewsapi/models/extract_news_response.py
--rw-rw-rw-   0        0        0     2723 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/geo_coordinates_response.py
--rw-rw-rw-   0        0        0     3643 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/news.py
--rw-rw-rw-   0        0        0     3662 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/news_article.py
--rw-rw-rw-   0        0        0     3188 2024-03-07 22:53:12.000000 worldnewsapi-1.0.9/worldnewsapi/models/search_news_response.py
--rw-rw-rw-   0        0        0        0 2024-03-07 22:53:15.000000 worldnewsapi-1.0.9/worldnewsapi/py.typed
--rw-rw-rw-   0        0        0     9642 2024-03-07 22:53:16.000000 worldnewsapi-1.0.9/worldnewsapi/rest.py
-drwxrwxrwx   0        0        0        0 2024-03-07 22:53:40.405097 worldnewsapi-1.0.9/worldnewsapi.egg-info/
--rw-rw-rw-   0        0        0     2054 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-07 22:53:40.000000 worldnewsapi-1.0.9/worldnewsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.381311 worldnewsapi-1.1.1/
+-rw-rw-rw-   0        0        0     2054 2024-06-01 00:46:46.381311 worldnewsapi-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4752 2024-06-01 00:45:18.000000 worldnewsapi-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1113 2024-03-07 13:36:21.000000 worldnewsapi-1.1.1/README_pypi.md
+-rw-rw-rw-   0        0        0     2671 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2024-06-01 00:46:46.385824 worldnewsapi-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.343783 worldnewsapi-1.1.1/test/
+-rw-rw-rw-   0        0        0     1702 2024-06-01 00:45:12.000000 worldnewsapi-1.1.1/test/test_extract_news200_response.py
+-rw-rw-rw-   0        0        0     1564 2024-06-01 00:45:12.000000 worldnewsapi-1.1.1/test/test_extract_news_links200_response.py
+-rw-rw-rw-   0        0        0     1595 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/test/test_get_geo_coordinates200_response.py
+-rw-rw-rw-   0        0        0     1408 2024-06-01 00:45:18.000000 worldnewsapi-1.1.1/test/test_news_api.py
+-rw-rw-rw-   0        0        0     2156 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/test/test_search_news200_response.py
+-rw-rw-rw-   0        0        0     1922 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/test/test_search_news200_response_news_inner.py
+-rw-rw-rw-   0        0        0     2257 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/test/test_top_news200_response.py
+-rw-rw-rw-   0        0        0     2093 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/test/test_top_news200_response_top_news_inner.py
+-rw-rw-rw-   0        0        0     1921 2024-06-01 00:45:14.000000 worldnewsapi-1.1.1/test/test_top_news200_response_top_news_inner_news_inner.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.348785 worldnewsapi-1.1.1/worldnewsapi/
+-rw-rw-rw-   0        0        0     1648 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.370800 worldnewsapi-1.1.1/worldnewsapi/api/
+-rw-rw-rw-   0        0        0       93 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/api/__init__.py
+-rw-rw-rw-   0        0        0    98495 2024-06-01 00:45:18.000000 worldnewsapi-1.1.1/worldnewsapi/api/news_api.py
+-rw-rw-rw-   0        0        0    26657 2024-06-01 00:45:20.000000 worldnewsapi-1.1.1/worldnewsapi/api_client.py
+-rw-rw-rw-   0        0        0      688 2024-06-01 00:45:20.000000 worldnewsapi-1.1.1/worldnewsapi/api_response.py
+-rw-rw-rw-   0        0        0    15678 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/configuration.py
+-rw-rw-rw-   0        0        0     6215 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.379311 worldnewsapi-1.1.1/worldnewsapi/models/
+-rw-rw-rw-   0        0        0     1076 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/models/__init__.py
+-rw-rw-rw-   0        0        0     5042 2024-06-01 00:45:12.000000 worldnewsapi-1.1.1/worldnewsapi/models/extract_news200_response.py
+-rw-rw-rw-   0        0        0     2539 2024-06-01 00:45:12.000000 worldnewsapi-1.1.1/worldnewsapi/models/extract_news_links200_response.py
+-rw-rw-rw-   0        0        0     2995 2024-06-01 00:45:12.000000 worldnewsapi-1.1.1/worldnewsapi/models/get_geo_coordinates200_response.py
+-rw-rw-rw-   0        0        0     3393 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/worldnewsapi/models/search_news200_response.py
+-rw-rw-rw-   0        0        0     5266 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/worldnewsapi/models/search_news200_response_news_inner.py
+-rw-rw-rw-   0        0        0     3728 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/worldnewsapi/models/top_news200_response.py
+-rw-rw-rw-   0        0        0     3125 2024-06-01 00:45:13.000000 worldnewsapi-1.1.1/worldnewsapi/models/top_news200_response_top_news_inner.py
+-rw-rw-rw-   0        0        0     4486 2024-06-01 00:45:14.000000 worldnewsapi-1.1.1/worldnewsapi/models/top_news200_response_top_news_inner_news_inner.py
+-rw-rw-rw-   0        0        0        0 2024-06-01 00:45:19.000000 worldnewsapi-1.1.1/worldnewsapi/py.typed
+-rw-rw-rw-   0        0        0     9891 2024-06-01 00:45:20.000000 worldnewsapi-1.1.1/worldnewsapi/rest.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:46:46.380311 worldnewsapi-1.1.1/worldnewsapi.egg-info/
+-rw-rw-rw-   0        0        0     2054 2024-06-01 00:46:46.000000 worldnewsapi-1.1.1/worldnewsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2024-06-01 00:46:46.000000 worldnewsapi-1.1.1/worldnewsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:46:46.000000 worldnewsapi-1.1.1/worldnewsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-06-01 00:46:46.000000 worldnewsapi-1.1.1/worldnewsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 00:46:46.000000 worldnewsapi-1.1.1/worldnewsapi.egg-info/top_level.txt
```

### Comparing `worldnewsapi-1.0.9/PKG-INFO` & `worldnewsapi-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldnewsapi
-Version: 1.0.9
+Version: 1.1.1
 Summary: The world's news wrapped into a single API.
 Home-page: 
 Author: David Urbansky
 Author-email: David Urbansky <mail@worldnewsapi.com>
 Project-URL: Homepage, https://worldnewsapi.com
 Project-URL: Documentation, https://worldnewsapi.com/docs
 Project-URL: Repository, https://github.com/ddsky/world-news-api-clients/tree/main/python
```

### Comparing `worldnewsapi-1.0.9/README.md` & `worldnewsapi-1.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # worldnewsapi
 
 The World News API gives you access to thousands of news sources in over 50 languages from over 150 countries. News are semantically tagged allowing for semantic news search like never before.
 
 This is the python-package for easy acccess to the api.
 
-- API version: 1.1
-- Package version: 1.0.9
+- API version: 1.1.1
+- Package version: 1.1.1
 
 ## Resources
 
 - [Homepage](https://worldnewsapi.com/)
 - [Tutorial](https://worldnewsapi.com/docs/#Tutorial-Getting-Started) 
 
 ## Requirements
@@ -84,15 +84,15 @@
 
 
 # Enter a context with an instance of the API client
 with worldnewsapi.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = worldnewsapi.NewsApi(api_client)
     url = 'https://www.bbc.com/news/world-us-canada-59340789' # str | The url of the news.
-    analyze = False # bool | Whether to analyze the news (extract entities etc.) (default to False)
+    analyze = true # bool | Whether to analyze the news (extract entities etc.)
 
     try:
         # Extract News
         api_response = api_instance.extract_news(url, analyze)
         print("The response of NewsApi->extract_news:\n")
         pprint(api_response)
     except ApiException as e:
@@ -104,27 +104,30 @@
 
 All URIs are relative to *https://api.worldnewsapi.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *NewsApi* | [**extract_news**](docs/NewsApi.md#extract_news) | **GET** /extract-news | Extract News
 *NewsApi* | [**extract_news_links**](docs/NewsApi.md#extract_news_links) | **GET** /extract-news-links | Extract News Links
-*NewsApi* | [**geo_coordinates**](docs/NewsApi.md#geo_coordinates) | **GET** /geo-coordinates | Get Geo Coordinates
+*NewsApi* | [**get_geo_coordinates**](docs/NewsApi.md#get_geo_coordinates) | **GET** /geo-coordinates | Get Geo Coordinates
 *NewsApi* | [**news_website_to_rss_feed**](docs/NewsApi.md#news_website_to_rss_feed) | **GET** /feed.rss | News Website to RSS Feed
 *NewsApi* | [**search_news**](docs/NewsApi.md#search_news) | **GET** /search-news | Search News
+*NewsApi* | [**top_news**](docs/NewsApi.md#top_news) | **GET** /top-news | Top News
 
 
 ## Documentation For Models
 
- - [ExtractLinksResponse](docs/ExtractLinksResponse.md)
- - [ExtractNewsResponse](docs/ExtractNewsResponse.md)
- - [GeoCoordinatesResponse](docs/GeoCoordinatesResponse.md)
- - [News](docs/News.md)
- - [NewsArticle](docs/NewsArticle.md)
- - [SearchNewsResponse](docs/SearchNewsResponse.md)
+ - [ExtractNews200Response](docs/ExtractNews200Response.md)
+ - [ExtractNewsLinks200Response](docs/ExtractNewsLinks200Response.md)
+ - [GetGeoCoordinates200Response](docs/GetGeoCoordinates200Response.md)
+ - [SearchNews200Response](docs/SearchNews200Response.md)
+ - [SearchNews200ResponseNewsInner](docs/SearchNews200ResponseNewsInner.md)
+ - [TopNews200Response](docs/TopNews200Response.md)
+ - [TopNews200ResponseTopNewsInner](docs/TopNews200ResponseTopNewsInner.md)
+ - [TopNews200ResponseTopNewsInnerNewsInner](docs/TopNews200ResponseTopNewsInnerNewsInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
```

### Comparing `worldnewsapi-1.0.9/README_pypi.md` & `worldnewsapi-1.1.1/README_pypi.md`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.9/pyproject.toml` & `worldnewsapi-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "worldnewsapi"
-version = "1.0.9"
+version = "1.1.1"
 description = "World News API"
 authors = ["David Urbansky <mail@worldnewsapi.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/ddsky/world-news-api-clients/tree/main/python/"
 keywords = ["OpenAPI", "OpenAPI-Generator", "World News API"]
 include = ["worldnewsapi/py.typed"]
@@ -69,15 +69,15 @@
 #
 ### This one can be tricky to get passing if you use a lot of untyped libraries
 #warn_return_any = true
 
 # The following section is used by PiPy
 [project]
 name = "worldnewsapi"
-version = "1.0.9"
+version = "1.1.1"
 authors = [
   { name="David Urbansky", email="mail@worldnewsapi.com" },
 ]
 description = "The world's news wrapped into a single API."
 readme = "README_pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `worldnewsapi-1.0.9/setup.py` & `worldnewsapi-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from setuptools import setup, find_packages  # noqa: H301
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "worldnewsapi"
-VERSION = "1.0.9"
+VERSION = "1.1.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `worldnewsapi-1.0.9/test/test_extract_links_response.py` & `worldnewsapi-1.1.1/test/test_extract_news_links200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import unittest
 
-from worldnewsapi.models.extract_links_response import ExtractLinksResponse
+from worldnewsapi.models.extract_news_links200_response import ExtractNewsLinks200Response
 
 
-class TestExtractLinksResponse(unittest.TestCase):
-    """ExtractLinksResponse unit test stubs"""
+class TestExtractNewsLinks200Response(unittest.TestCase):
+    """ExtractNewsLinks200Response unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ExtractLinksResponse:
-        """Test ExtractLinksResponse
+    def make_instance(self, include_optional) -> ExtractNewsLinks200Response:
+        """Test ExtractNewsLinks200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ExtractLinksResponse`
+        # uncomment below to create an instance of `ExtractNewsLinks200Response`
         """
-        model = ExtractLinksResponse()
+        model = ExtractNewsLinks200Response()
         if include_optional:
-            return ExtractLinksResponse(
+            return ExtractNewsLinks200Response(
                 news_links = [
                     ''
                     ]
             )
         else:
-            return ExtractLinksResponse(
+            return ExtractNewsLinks200Response(
         )
         """
 
-    def testExtractLinksResponse(self):
-        """Test ExtractLinksResponse"""
+    def testExtractNewsLinks200Response(self):
+        """Test ExtractNewsLinks200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `worldnewsapi-1.0.9/test/test_extract_news_response.py` & `worldnewsapi-1.1.1/test/test_extract_news200_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import unittest
 
-from worldnewsapi.models.extract_news_response import ExtractNewsResponse
+from worldnewsapi.models.extract_news200_response import ExtractNews200Response
 
 
-class TestExtractNewsResponse(unittest.TestCase):
-    """ExtractNewsResponse unit test stubs"""
+class TestExtractNews200Response(unittest.TestCase):
+    """ExtractNews200Response unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ExtractNewsResponse:
-        """Test ExtractNewsResponse
+    def make_instance(self, include_optional) -> ExtractNews200Response:
+        """Test ExtractNews200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ExtractNewsResponse`
+        # uncomment below to create an instance of `ExtractNews200Response`
         """
-        model = ExtractNewsResponse()
+        model = ExtractNews200Response()
         if include_optional:
-            return ExtractNewsResponse(
+            return ExtractNews200Response(
                 title = '',
                 text = '',
                 url = '',
                 image = '',
+                publish_date = '',
                 author = '',
                 language = '',
                 source_country = '',
                 sentiment = 1.337
             )
         else:
-            return ExtractNewsResponse(
+            return ExtractNews200Response(
         )
         """
 
-    def testExtractNewsResponse(self):
-        """Test ExtractNewsResponse"""
+    def testExtractNews200Response(self):
+        """Test ExtractNews200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `worldnewsapi-1.0.9/test/test_news_api.py` & `worldnewsapi-1.1.1/test/test_news_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import unittest
@@ -35,16 +35,16 @@
     def test_extract_news_links(self) -> None:
         """Test case for extract_news_links
 
         Extract News Links
         """
         pass
 
-    def test_geo_coordinates(self) -> None:
-        """Test case for geo_coordinates
+    def test_get_geo_coordinates(self) -> None:
+        """Test case for get_geo_coordinates
 
         Get Geo Coordinates
         """
         pass
 
     def test_news_website_to_rss_feed(self) -> None:
         """Test case for news_website_to_rss_feed
@@ -56,10 +56,17 @@
     def test_search_news(self) -> None:
         """Test case for search_news
 
         Search News
         """
         pass
 
+    def test_top_news(self) -> None:
+        """Test case for top_news
+
+        Top News
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `worldnewsapi-1.0.9/test/test_search_news_response.py` & `worldnewsapi-1.1.1/test/test_search_news200_response_news_inner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,65 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import unittest
 
-from worldnewsapi.models.search_news_response import SearchNewsResponse
+from worldnewsapi.models.search_news200_response_news_inner import SearchNews200ResponseNewsInner
 
 
-class TestSearchNewsResponse(unittest.TestCase):
-    """SearchNewsResponse unit test stubs"""
+class TestSearchNews200ResponseNewsInner(unittest.TestCase):
+    """SearchNews200ResponseNewsInner unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SearchNewsResponse:
-        """Test SearchNewsResponse
+    def make_instance(self,
+                      include_optional) -> SearchNews200ResponseNewsInner:
+        """Test SearchNews200ResponseNewsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SearchNewsResponse`
+        # uncomment below to create an instance of `SearchNews200ResponseNewsInner`
         """
-        model = SearchNewsResponse()
+        model = SearchNews200ResponseNewsInner()
         if include_optional:
-            return SearchNewsResponse(
-                offset = 56,
-                number = 56,
-                available = 56,
-                news = [
-                    worldnewsapi.models.news_article.NewsArticle(
-                        id = 56, 
-                        title = '', 
-                        text = '', 
-                        summary = '', 
-                        url = '', 
-                        image = '', 
-                        publish_date = '', 
-                        author = '', 
-                        language = '', 
-                        source_country = '', 
-                        sentiment = 1.337, )
+            return SearchNews200ResponseNewsInner(
+                summary = '',
+                image = '',
+                sentiment = 1.337,
+                source_country = '',
+                language = '',
+                id = 56,
+                text = '',
+                title = '',
+                publish_date = '',
+                url = '',
+                authors = [
+                    ''
                     ]
             )
         else:
-            return SearchNewsResponse(
-                offset = 56,
-                number = 56,
-                available = 56,
-                news = [
-                    worldnewsapi.models.news_article.NewsArticle(
-                        id = 56, 
-                        title = '', 
-                        text = '', 
-                        summary = '', 
-                        url = '', 
-                        image = '', 
-                        publish_date = '', 
-                        author = '', 
-                        language = '', 
-                        source_country = '', 
-                        sentiment = 1.337, )
-                    ],
+            return SearchNews200ResponseNewsInner(
         )
         """
 
-    def testSearchNewsResponse(self):
-        """Test SearchNewsResponse"""
+    def testSearchNews200ResponseNewsInner(self):
+        """Test SearchNews200ResponseNewsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/__init__.py` & `worldnewsapi-1.1.1/worldnewsapi/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-__version__ = "1.0.9"
+__version__ = "1.1.1"
 
 # import apis into sdk package
 from worldnewsapi.api.news_api import NewsApi
 
 # import ApiClient
 from worldnewsapi.api_response import ApiResponse
 from worldnewsapi.api_client import ApiClient
@@ -27,13 +27,15 @@
 from worldnewsapi.exceptions import ApiTypeError
 from worldnewsapi.exceptions import ApiValueError
 from worldnewsapi.exceptions import ApiKeyError
 from worldnewsapi.exceptions import ApiAttributeError
 from worldnewsapi.exceptions import ApiException
 
 # import models into sdk package
-from worldnewsapi.models.extract_links_response import ExtractLinksResponse
-from worldnewsapi.models.extract_news_response import ExtractNewsResponse
-from worldnewsapi.models.geo_coordinates_response import GeoCoordinatesResponse
-from worldnewsapi.models.news import News
-from worldnewsapi.models.news_article import NewsArticle
-from worldnewsapi.models.search_news_response import SearchNewsResponse
+from worldnewsapi.models.extract_news200_response import ExtractNews200Response
+from worldnewsapi.models.extract_news_links200_response import ExtractNewsLinks200Response
+from worldnewsapi.models.get_geo_coordinates200_response import GetGeoCoordinates200Response
+from worldnewsapi.models.search_news200_response import SearchNews200Response
+from worldnewsapi.models.search_news200_response_news_inner import SearchNews200ResponseNewsInner
+from worldnewsapi.models.top_news200_response import TopNews200Response
+from worldnewsapi.models.top_news200_response_top_news_inner import TopNews200ResponseTopNewsInner
+from worldnewsapi.models.top_news200_response_top_news_inner_news_inner import TopNews200ResponseTopNewsInnerNewsInner
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/api/news_api.py` & `worldnewsapi-1.1.1/worldnewsapi/api/news_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictStr, field_validator
-from typing import Optional, Union
+from pydantic import Field, StrictBool, field_validator
+from typing import Any, Dict, Optional, Union
 from typing_extensions import Annotated
-from worldnewsapi.models.extract_links_response import ExtractLinksResponse
-from worldnewsapi.models.extract_news_response import ExtractNewsResponse
-from worldnewsapi.models.geo_coordinates_response import GeoCoordinatesResponse
-from worldnewsapi.models.search_news_response import SearchNewsResponse
+from worldnewsapi.models.extract_news200_response import ExtractNews200Response
+from worldnewsapi.models.extract_news_links200_response import ExtractNewsLinks200Response
+from worldnewsapi.models.get_geo_coordinates200_response import GetGeoCoordinates200Response
+from worldnewsapi.models.search_news200_response import SearchNews200Response
+from worldnewsapi.models.top_news200_response import TopNews200Response
 
 from worldnewsapi.api_client import ApiClient, RequestSerialized
 from worldnewsapi.api_response import ApiResponse
 from worldnewsapi.rest import RESTResponseType
 
 
 class NewsApi:
@@ -40,34 +41,36 @@
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_call
     def extract_news(
         self,
-        url: Annotated[StrictStr,
-                       Field(description="The url of the news.")],
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
         analyze: Annotated[
             StrictBool,
             Field(description=
                   "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ExtractNewsResponse:
+    ) -> ExtractNews200Response:
         """Extract News
 
-        Extract a news entry from a news site.
+        Extract a news article from a website to a well structure JSON object. The API will return the title, text, URL, image, publish date, author, language, source country, and sentiment of the news article.
 
         :param url: The url of the news. (required)
         :type url: str
         :param analyze: Whether to analyze the news (extract entities etc.) (required)
         :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -95,47 +98,55 @@
                                               analyze=analyze,
                                               _request_auth=_request_auth,
                                               _content_type=_content_type,
                                               _headers=_headers,
                                               _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractNewsResponse",
+            '200': "ExtractNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
     @validate_call
     def extract_news_with_http_info(
         self,
-        url: Annotated[StrictStr,
-                       Field(description="The url of the news.")],
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
         analyze: Annotated[
             StrictBool,
             Field(description=
                   "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ExtractNewsResponse]:
+    ) -> ApiResponse[ExtractNews200Response]:
         """Extract News
 
-        Extract a news entry from a news site.
+        Extract a news article from a website to a well structure JSON object. The API will return the title, text, URL, image, publish date, author, language, source country, and sentiment of the news article.
 
         :param url: The url of the news. (required)
         :type url: str
         :param analyze: Whether to analyze the news (extract entities etc.) (required)
         :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -163,29 +174,37 @@
                                               analyze=analyze,
                                               _request_auth=_request_auth,
                                               _content_type=_content_type,
                                               _headers=_headers,
                                               _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractNewsResponse",
+            '200': "ExtractNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
     @validate_call
     def extract_news_without_preload_content(
         self,
-        url: Annotated[StrictStr,
-                       Field(description="The url of the news.")],
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
         analyze: Annotated[
             StrictBool,
             Field(description=
                   "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
@@ -195,15 +214,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Extract News
 
-        Extract a news entry from a news site.
+        Extract a news article from a website to a well structure JSON object. The API will return the title, text, URL, image, publish date, author, language, source country, and sentiment of the news article.
 
         :param url: The url of the news. (required)
         :type url: str
         :param analyze: Whether to analyze the news (extract entities etc.) (required)
         :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -231,15 +250,21 @@
                                               analyze=analyze,
                                               _request_auth=_request_auth,
                                               _content_type=_content_type,
                                               _headers=_headers,
                                               _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractNewsResponse",
+            '200': "ExtractNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         return response_data.response
 
     def _extract_news_serialize(
         self,
@@ -255,15 +280,15 @@
 
         _collection_formats: Dict[str, str] = {}
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if url is not None:
 
             _query_params.append(('url', url))
@@ -296,52 +321,41 @@
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth)
 
     @validate_call
     def extract_news_links(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        prefix: Annotated[
-            Optional[StrictStr],
-            Field(description="The prefix the news links must start with."
-                  )] = None,
-        sub_domain: Annotated[
-            Optional[StrictBool],
-            Field(
-                description="Whether to include links to news on sub-domains."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ExtractLinksResponse:
+    ) -> ExtractNewsLinks200Response:
         """Extract News Links
 
-        Extract a news links from a news website. 
+        Extract news links from a news website.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param prefix: The prefix the news links must start with.
-        :type prefix: str
-        :param sub_domain: Whether to include links to news on sub-domains.
-        :type sub_domain: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -358,79 +372,67 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._extract_news_links_serialize(
             url=url,
-            api_key=api_key,
-            prefix=prefix,
-            sub_domain=sub_domain,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractLinksResponse",
+            '200': "ExtractNewsLinks200Response",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
     @validate_call
     def extract_news_links_with_http_info(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        prefix: Annotated[
-            Optional[StrictStr],
-            Field(description="The prefix the news links must start with."
-                  )] = None,
-        sub_domain: Annotated[
-            Optional[StrictBool],
-            Field(
-                description="Whether to include links to news on sub-domains."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ExtractLinksResponse]:
+    ) -> ApiResponse[ExtractNewsLinks200Response]:
         """Extract News Links
 
-        Extract a news links from a news website. 
+        Extract news links from a news website.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param prefix: The prefix the news links must start with.
-        :type prefix: str
-        :param sub_domain: Whether to include links to news on sub-domains.
-        :type sub_domain: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -447,79 +449,67 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._extract_news_links_serialize(
             url=url,
-            api_key=api_key,
-            prefix=prefix,
-            sub_domain=sub_domain,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractLinksResponse",
+            '200': "ExtractNewsLinks200Response",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
     @validate_call
     def extract_news_links_without_preload_content(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        prefix: Annotated[
-            Optional[StrictStr],
-            Field(description="The prefix the news links must start with."
-                  )] = None,
-        sub_domain: Annotated[
-            Optional[StrictBool],
-            Field(
-                description="Whether to include links to news on sub-domains."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Extract News Links
 
-        Extract a news links from a news website. 
+        Extract news links from a news website.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param prefix: The prefix the news links must start with.
-        :type prefix: str
-        :param sub_domain: Whether to include links to news on sub-domains.
-        :type sub_domain: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -536,74 +526,63 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._extract_news_links_serialize(
             url=url,
-            api_key=api_key,
-            prefix=prefix,
-            sub_domain=sub_domain,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ExtractLinksResponse",
+            '200': "ExtractNewsLinks200Response",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         return response_data.response
 
     def _extract_news_links_serialize(
         self,
         url,
-        api_key,
-        prefix,
-        sub_domain,
+        analyze,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {}
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if url is not None:
 
             _query_params.append(('url', url))
 
-        if prefix is not None:
-
-            _query_params.append(('prefix', prefix))
-
-        if sub_domain is not None:
-
-            _query_params.append(('sub-domain', sub_domain))
-
-        if api_key is not None:
+        if analyze is not None:
 
-            _query_params.append(('api-key', api_key))
+            _query_params.append(('analyze', analyze))
 
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -623,36 +602,37 @@
             files=_files,
             auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth)
 
     @validate_call
-    def geo_coordinates(
+    def get_geo_coordinates(
         self,
         location: Annotated[
-            StrictStr,
-            Field(description=
-                  "The address or name of the location, e.g. Tokyo, Japan.")],
+            str,
+            Field(strict=True,
+                  max_length=1000,
+                  description="The address or name of the location.")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GeoCoordinatesResponse:
+    ) -> GetGeoCoordinates200Response:
         """Get Geo Coordinates
 
-        Get the geo coordinates for a location. The location can be an exact address but also just the name of a city or country.
+        Retrieve the latitude and longitude of a location name. Given this information you can fill the location-filter parameter in the news search endpoint.
 
-        :param location: The address or name of the location, e.g. Tokyo, Japan. (required)
+        :param location: The address or name of the location. (required)
         :type location: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -668,55 +648,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._geo_coordinates_serialize(location=location,
-                                                 _request_auth=_request_auth,
-                                                 _content_type=_content_type,
-                                                 _headers=_headers,
-                                                 _host_index=_host_index)
+        _param = self._get_geo_coordinates_serialize(
+            location=location,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GeoCoordinatesResponse",
+            '200': "GetGeoCoordinates200Response",
+            '401': None,
+            '402': None,
+            '403': None,
             '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
     @validate_call
-    def geo_coordinates_with_http_info(
+    def get_geo_coordinates_with_http_info(
         self,
         location: Annotated[
-            StrictStr,
-            Field(description=
-                  "The address or name of the location, e.g. Tokyo, Japan.")],
+            str,
+            Field(strict=True,
+                  max_length=1000,
+                  description="The address or name of the location.")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GeoCoordinatesResponse]:
+    ) -> ApiResponse[GetGeoCoordinates200Response]:
         """Get Geo Coordinates
 
-        Get the geo coordinates for a location. The location can be an exact address but also just the name of a city or country.
+        Retrieve the latitude and longitude of a location name. Given this information you can fill the location-filter parameter in the news search endpoint.
 
-        :param location: The address or name of the location, e.g. Tokyo, Japan. (required)
+        :param location: The address or name of the location. (required)
         :type location: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -732,55 +719,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._geo_coordinates_serialize(location=location,
-                                                 _request_auth=_request_auth,
-                                                 _content_type=_content_type,
-                                                 _headers=_headers,
-                                                 _host_index=_host_index)
+        _param = self._get_geo_coordinates_serialize(
+            location=location,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GeoCoordinatesResponse",
+            '200': "GetGeoCoordinates200Response",
+            '401': None,
+            '402': None,
+            '403': None,
             '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
     @validate_call
-    def geo_coordinates_without_preload_content(
+    def get_geo_coordinates_without_preload_content(
         self,
         location: Annotated[
-            StrictStr,
-            Field(description=
-                  "The address or name of the location, e.g. Tokyo, Japan.")],
+            str,
+            Field(strict=True,
+                  max_length=1000,
+                  description="The address or name of the location.")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Geo Coordinates
 
-        Get the geo coordinates for a location. The location can be an exact address but also just the name of a city or country.
+        Retrieve the latitude and longitude of a location name. Given this information you can fill the location-filter parameter in the news search endpoint.
 
-        :param location: The address or name of the location, e.g. Tokyo, Japan. (required)
+        :param location: The address or name of the location. (required)
         :type location: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -796,29 +790,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._geo_coordinates_serialize(location=location,
-                                                 _request_auth=_request_auth,
-                                                 _content_type=_content_type,
-                                                 _headers=_headers,
-                                                 _host_index=_host_index)
+        _param = self._get_geo_coordinates_serialize(
+            location=location,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GeoCoordinatesResponse",
+            '200': "GetGeoCoordinates200Response",
+            '401': None,
+            '402': None,
+            '403': None,
             '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         return response_data.response
 
-    def _geo_coordinates_serialize(
+    def _get_geo_coordinates_serialize(
         self,
         location,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
@@ -827,15 +827,15 @@
 
         _collection_formats: Dict[str, str] = {}
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if location is not None:
 
             _query_params.append(('location', location))
@@ -864,47 +864,41 @@
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth)
 
     @validate_call
     def news_website_to_rss_feed(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        extract_news: Annotated[
-            Optional[StrictBool],
-            Field(
-                description=
-                "Whether extract news and add information such as description, publish date, and image to each item."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> object:
         """News Website to RSS Feed
 
-        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page. 
+        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param extract_news: Whether extract news and add information such as description, publish date, and image to each item.
-        :type extract_news: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -921,73 +915,67 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._news_website_to_rss_feed_serialize(
             url=url,
-            api_key=api_key,
-            extract_news=extract_news,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "object",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
     @validate_call
     def news_website_to_rss_feed_with_http_info(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        extract_news: Annotated[
-            Optional[StrictBool],
-            Field(
-                description=
-                "Whether extract news and add information such as description, publish date, and image to each item."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[object]:
         """News Website to RSS Feed
 
-        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page. 
+        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param extract_news: Whether extract news and add information such as description, publish date, and image to each item.
-        :type extract_news: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1004,73 +992,67 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._news_website_to_rss_feed_serialize(
             url=url,
-            api_key=api_key,
-            extract_news=extract_news,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "object",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
     @validate_call
     def news_website_to_rss_feed_without_preload_content(
         self,
-        url: Annotated[
-            StrictStr,
-            Field(
-                description="The url from which links should be extracted.")],
-        api_key: Annotated[StrictStr,
-                           Field(description="Your API key.")],
-        extract_news: Annotated[
-            Optional[StrictBool],
-            Field(
-                description=
-                "Whether extract news and add information such as description, publish date, and image to each item."
-            )] = None,
+        url: Annotated[str,
+                       Field(strict=True,
+                             max_length=1000,
+                             description="The url of the news.")],
+        analyze: Annotated[
+            StrictBool,
+            Field(description=
+                  "Whether to analyze the news (extract entities etc.)")],
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """News Website to RSS Feed
 
-        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page. 
+        Turn a news website into an RSS feed. Any page of a news website can be turned into an RSS feed. Provide the URL to the page and the API will return an RSS feed with the latest news from that page.
 
-        :param url: The url from which links should be extracted. (required)
+        :param url: The url of the news. (required)
         :type url: str
-        :param api_key: Your API key. (required)
-        :type api_key: str
-        :param extract_news: Whether extract news and add information such as description, publish date, and image to each item.
-        :type extract_news: bool
+        :param analyze: Whether to analyze the news (extract entities etc.) (required)
+        :type analyze: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1087,68 +1069,63 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._news_website_to_rss_feed_serialize(
             url=url,
-            api_key=api_key,
-            extract_news=extract_news,
+            analyze=analyze,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "object",
             '401': None,
             '402': None,
             '403': None,
             '404': None,
+            '406': None,
             '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         return response_data.response
 
     def _news_website_to_rss_feed_serialize(
         self,
         url,
-        api_key,
-        extract_news,
+        analyze,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {}
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if url is not None:
 
             _query_params.append(('url', url))
 
-        if extract_news is not None:
-
-            _query_params.append(('extract-news', extract_news))
-
-        if api_key is not None:
+        if analyze is not None:
 
-            _query_params.append(('api-key', api_key))
+            _query_params.append(('analyze', analyze))
 
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1171,29 +1148,29 @@
             _host=_host,
             _request_auth=_request_auth)
 
     @validate_call
     def search_news(
         self,
         text: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
-                description="The text to match in the news content.")] = None,
+                description=
+                "The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford"
+            )] = None,
         source_countries: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us."
+                "A comma-separated list of ISO 3166 country codes from which the news should originate."
             )] = None,
         language: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=2)]],
             Field(
-                description=
-                "The ISO 6391 language code of the news, e.g. \"en\" for English."
-            )] = None,
+                description="The ISO 6391 language code of the news.")] = None,
         min_sentiment: Annotated[
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The minimal sentiment of the news in range [-1,1]."
             )] = None,
@@ -1201,104 +1178,108 @@
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The maximal sentiment of the news in range [-1,1]."
             )] = None,
         earliest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description="The news must have been published after this date."
             )] = None,
         latest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description=
                 "The news must have been published before this date.")] = None,
         news_sources: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
             Field(
                 description=
-                "A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk"
+                "A comma-separated list of news sources from which the news should originate."
             )] = None,
         authors: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
                 description=
                 "A comma-separated list of author names. Only news from any of the given authors will be returned."
             )] = None,
         entities: Annotated[
-            Optional[StrictStr],
-            Field(description="Filter news by entities, e.g. ORG:Tesla."
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
+            Field(description="Filter news by entities (see semantic types)."
                   )] = None,
         location_filter: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100"
+                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers."
             )] = None,
+        sort: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
+            Field(
+                description="The sorting criteria (publish-time or sentiment)."
+            )] = None,
+        sort_direction: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=4)]],
+            Field(description=
+                  "Whether to sort ascending or descending (ASC or DESC)."
+                  )] = None,
         offset: Annotated[
-            Optional[Annotated[int, Field(le=1000, strict=True, ge=0)]],
-            Field(description="The number of news to skip in range [0,1000]"
+            Optional[Annotated[int, Field(le=10000, strict=True, ge=0)]],
+            Field(description="The number of news to skip in range [0,10000]"
                   )] = None,
         number: Annotated[
             Optional[Annotated[int, Field(le=100, strict=True, ge=1)]],
             Field(description="The number of news to return in range [1,100]"
                   )] = None,
-        sort: Annotated[Optional[StrictStr],
-                        Field(description="The sorting criteria.")] = None,
-        sort_direction: Annotated[
-            Optional[StrictStr],
-            Field(description="Whether to sort ascending or descending."
-                  )] = None,
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> SearchNewsResponse:
+    ) -> SearchNews200Response:
         """Search News
 
-        Search for news.
+        Search and filter news by text, date, location, language, and more. The API returns a list of news articles matching the given criteria. You can set as many filtering parameters as you like, but you have to set at least one, e.g. text or language.
 
-        :param text: The text to match in the news content.
+        :param text: The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford
         :type text: str
-        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us.
+        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate.
         :type source_countries: str
-        :param language: The ISO 6391 language code of the news, e.g. \"en\" for English.
+        :param language: The ISO 6391 language code of the news.
         :type language: str
         :param min_sentiment: The minimal sentiment of the news in range [-1,1].
         :type min_sentiment: float
         :param max_sentiment: The maximal sentiment of the news in range [-1,1].
         :type max_sentiment: float
         :param earliest_publish_date: The news must have been published after this date.
         :type earliest_publish_date: str
         :param latest_publish_date: The news must have been published before this date.
         :type latest_publish_date: str
-        :param news_sources: A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk
+        :param news_sources: A comma-separated list of news sources from which the news should originate.
         :type news_sources: str
         :param authors: A comma-separated list of author names. Only news from any of the given authors will be returned.
         :type authors: str
-        :param entities: Filter news by entities, e.g. ORG:Tesla.
+        :param entities: Filter news by entities (see semantic types).
         :type entities: str
-        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100
+        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers.
         :type location_filter: str
-        :param offset: The number of news to skip in range [0,1000]
+        :param sort: The sorting criteria (publish-time or sentiment).
+        :type sort: str
+        :param sort_direction: Whether to sort ascending or descending (ASC or DESC).
+        :type sort_direction: str
+        :param offset: The number of news to skip in range [0,10000]
         :type offset: int
         :param number: The number of news to return in range [1,100]
         :type number: int
-        :param sort: The sorting criteria.
-        :type sort: str
-        :param sort_direction: Whether to sort ascending or descending.
-        :type sort_direction: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1325,53 +1306,59 @@
             max_sentiment=max_sentiment,
             earliest_publish_date=earliest_publish_date,
             latest_publish_date=latest_publish_date,
             news_sources=news_sources,
             authors=authors,
             entities=entities,
             location_filter=location_filter,
-            offset=offset,
-            number=number,
             sort=sort,
             sort_direction=sort_direction,
+            offset=offset,
+            number=number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SearchNewsResponse",
+            '200': "SearchNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
     @validate_call
     def search_news_with_http_info(
         self,
         text: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
-                description="The text to match in the news content.")] = None,
+                description=
+                "The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford"
+            )] = None,
         source_countries: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us."
+                "A comma-separated list of ISO 3166 country codes from which the news should originate."
             )] = None,
         language: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=2)]],
             Field(
-                description=
-                "The ISO 6391 language code of the news, e.g. \"en\" for English."
-            )] = None,
+                description="The ISO 6391 language code of the news.")] = None,
         min_sentiment: Annotated[
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The minimal sentiment of the news in range [-1,1]."
             )] = None,
@@ -1379,104 +1366,108 @@
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The maximal sentiment of the news in range [-1,1]."
             )] = None,
         earliest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description="The news must have been published after this date."
             )] = None,
         latest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description=
                 "The news must have been published before this date.")] = None,
         news_sources: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
             Field(
                 description=
-                "A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk"
+                "A comma-separated list of news sources from which the news should originate."
             )] = None,
         authors: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
                 description=
                 "A comma-separated list of author names. Only news from any of the given authors will be returned."
             )] = None,
         entities: Annotated[
-            Optional[StrictStr],
-            Field(description="Filter news by entities, e.g. ORG:Tesla."
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
+            Field(description="Filter news by entities (see semantic types)."
                   )] = None,
         location_filter: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100"
+                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers."
             )] = None,
+        sort: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
+            Field(
+                description="The sorting criteria (publish-time or sentiment)."
+            )] = None,
+        sort_direction: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=4)]],
+            Field(description=
+                  "Whether to sort ascending or descending (ASC or DESC)."
+                  )] = None,
         offset: Annotated[
-            Optional[Annotated[int, Field(le=1000, strict=True, ge=0)]],
-            Field(description="The number of news to skip in range [0,1000]"
+            Optional[Annotated[int, Field(le=10000, strict=True, ge=0)]],
+            Field(description="The number of news to skip in range [0,10000]"
                   )] = None,
         number: Annotated[
             Optional[Annotated[int, Field(le=100, strict=True, ge=1)]],
             Field(description="The number of news to return in range [1,100]"
                   )] = None,
-        sort: Annotated[Optional[StrictStr],
-                        Field(description="The sorting criteria.")] = None,
-        sort_direction: Annotated[
-            Optional[StrictStr],
-            Field(description="Whether to sort ascending or descending."
-                  )] = None,
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[SearchNewsResponse]:
+    ) -> ApiResponse[SearchNews200Response]:
         """Search News
 
-        Search for news.
+        Search and filter news by text, date, location, language, and more. The API returns a list of news articles matching the given criteria. You can set as many filtering parameters as you like, but you have to set at least one, e.g. text or language.
 
-        :param text: The text to match in the news content.
+        :param text: The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford
         :type text: str
-        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us.
+        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate.
         :type source_countries: str
-        :param language: The ISO 6391 language code of the news, e.g. \"en\" for English.
+        :param language: The ISO 6391 language code of the news.
         :type language: str
         :param min_sentiment: The minimal sentiment of the news in range [-1,1].
         :type min_sentiment: float
         :param max_sentiment: The maximal sentiment of the news in range [-1,1].
         :type max_sentiment: float
         :param earliest_publish_date: The news must have been published after this date.
         :type earliest_publish_date: str
         :param latest_publish_date: The news must have been published before this date.
         :type latest_publish_date: str
-        :param news_sources: A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk
+        :param news_sources: A comma-separated list of news sources from which the news should originate.
         :type news_sources: str
         :param authors: A comma-separated list of author names. Only news from any of the given authors will be returned.
         :type authors: str
-        :param entities: Filter news by entities, e.g. ORG:Tesla.
+        :param entities: Filter news by entities (see semantic types).
         :type entities: str
-        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100
+        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers.
         :type location_filter: str
-        :param offset: The number of news to skip in range [0,1000]
+        :param sort: The sorting criteria (publish-time or sentiment).
+        :type sort: str
+        :param sort_direction: Whether to sort ascending or descending (ASC or DESC).
+        :type sort_direction: str
+        :param offset: The number of news to skip in range [0,10000]
         :type offset: int
         :param number: The number of news to return in range [1,100]
         :type number: int
-        :param sort: The sorting criteria.
-        :type sort: str
-        :param sort_direction: Whether to sort ascending or descending.
-        :type sort_direction: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1503,53 +1494,59 @@
             max_sentiment=max_sentiment,
             earliest_publish_date=earliest_publish_date,
             latest_publish_date=latest_publish_date,
             news_sources=news_sources,
             authors=authors,
             entities=entities,
             location_filter=location_filter,
-            offset=offset,
-            number=number,
             sort=sort,
             sort_direction=sort_direction,
+            offset=offset,
+            number=number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SearchNewsResponse",
+            '200': "SearchNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
     @validate_call
     def search_news_without_preload_content(
         self,
         text: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
-                description="The text to match in the news content.")] = None,
+                description=
+                "The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford"
+            )] = None,
         source_countries: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us."
+                "A comma-separated list of ISO 3166 country codes from which the news should originate."
             )] = None,
         language: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=2)]],
             Field(
-                description=
-                "The ISO 6391 language code of the news, e.g. \"en\" for English."
-            )] = None,
+                description="The ISO 6391 language code of the news.")] = None,
         min_sentiment: Annotated[
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The minimal sentiment of the news in range [-1,1]."
             )] = None,
@@ -1557,104 +1554,108 @@
             Optional[Union[Annotated[float,
                                      Field(le=1, strict=True, ge=-1)],
                            Annotated[int, Field(le=1, strict=True, ge=-1)]]],
             Field(
                 description="The maximal sentiment of the news in range [-1,1]."
             )] = None,
         earliest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description="The news must have been published after this date."
             )] = None,
         latest_publish_date: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=19)]],
             Field(
                 description=
                 "The news must have been published before this date.")] = None,
         news_sources: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
             Field(
                 description=
-                "A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk"
+                "A comma-separated list of news sources from which the news should originate."
             )] = None,
         authors: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=300)]],
             Field(
                 description=
                 "A comma-separated list of author names. Only news from any of the given authors will be returned."
             )] = None,
         entities: Annotated[
-            Optional[StrictStr],
-            Field(description="Filter news by entities, e.g. ORG:Tesla."
+            Optional[Annotated[str, Field(strict=True, max_length=10000)]],
+            Field(description="Filter news by entities (see semantic types)."
                   )] = None,
         location_filter: Annotated[
-            Optional[StrictStr],
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
             Field(
                 description=
-                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100"
+                "Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers."
+            )] = None,
+        sort: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=100)]],
+            Field(
+                description="The sorting criteria (publish-time or sentiment)."
             )] = None,
+        sort_direction: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=4)]],
+            Field(description=
+                  "Whether to sort ascending or descending (ASC or DESC)."
+                  )] = None,
         offset: Annotated[
-            Optional[Annotated[int, Field(le=1000, strict=True, ge=0)]],
-            Field(description="The number of news to skip in range [0,1000]"
+            Optional[Annotated[int, Field(le=10000, strict=True, ge=0)]],
+            Field(description="The number of news to skip in range [0,10000]"
                   )] = None,
         number: Annotated[
             Optional[Annotated[int, Field(le=100, strict=True, ge=1)]],
             Field(description="The number of news to return in range [1,100]"
                   )] = None,
-        sort: Annotated[Optional[StrictStr],
-                        Field(description="The sorting criteria.")] = None,
-        sort_direction: Annotated[
-            Optional[StrictStr],
-            Field(description="Whether to sort ascending or descending."
-                  )] = None,
         _request_timeout: Union[None, Annotated[StrictFloat,
                                                 Field(gt=0)],
                                 Tuple[Annotated[StrictFloat,
                                                 Field(gt=0)],
                                       Annotated[StrictFloat,
                                                 Field(gt=0)]]] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Search News
 
-        Search for news.
+        Search and filter news by text, date, location, language, and more. The API returns a list of news articles matching the given criteria. You can set as many filtering parameters as you like, but you have to set at least one, e.g. text or language.
 
-        :param text: The text to match in the news content.
+        :param text: The text to match in the news content (at least 3 characters). By default all query terms are expected, you can use an uppercase OR to search for any terms, e.g. tesla OR ford
         :type text: str
-        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate, e.g. gb,us.
+        :param source_countries: A comma-separated list of ISO 3166 country codes from which the news should originate.
         :type source_countries: str
-        :param language: The ISO 6391 language code of the news, e.g. \"en\" for English.
+        :param language: The ISO 6391 language code of the news.
         :type language: str
         :param min_sentiment: The minimal sentiment of the news in range [-1,1].
         :type min_sentiment: float
         :param max_sentiment: The maximal sentiment of the news in range [-1,1].
         :type max_sentiment: float
         :param earliest_publish_date: The news must have been published after this date.
         :type earliest_publish_date: str
         :param latest_publish_date: The news must have been published before this date.
         :type latest_publish_date: str
-        :param news_sources: A comma-separated list of news sources from which the news should originate, e.g. https://www.bbc.co.uk
+        :param news_sources: A comma-separated list of news sources from which the news should originate.
         :type news_sources: str
         :param authors: A comma-separated list of author names. Only news from any of the given authors will be returned.
         :type authors: str
-        :param entities: Filter news by entities, e.g. ORG:Tesla.
+        :param entities: Filter news by entities (see semantic types).
         :type entities: str
-        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\", e.g. 51.050407, 13.737262, 100
+        :param location_filter: Filter news by radius around a certain location. Format is \"latitude,longitude,radius in kilometers\". Radius must be between 1 and 100 kilometers.
         :type location_filter: str
-        :param offset: The number of news to skip in range [0,1000]
+        :param sort: The sorting criteria (publish-time or sentiment).
+        :type sort: str
+        :param sort_direction: Whether to sort ascending or descending (ASC or DESC).
+        :type sort_direction: str
+        :param offset: The number of news to skip in range [0,10000]
         :type offset: int
         :param number: The number of news to return in range [1,100]
         :type number: int
-        :param sort: The sorting criteria.
-        :type sort: str
-        :param sort_direction: Whether to sort ascending or descending.
-        :type sort_direction: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1681,25 +1682,31 @@
             max_sentiment=max_sentiment,
             earliest_publish_date=earliest_publish_date,
             latest_publish_date=latest_publish_date,
             news_sources=news_sources,
             authors=authors,
             entities=entities,
             location_filter=location_filter,
-            offset=offset,
-            number=number,
             sort=sort,
             sort_direction=sort_direction,
+            offset=offset,
+            number=number,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index)
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SearchNewsResponse",
+            '200': "SearchNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
         }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout)
         return response_data.response
 
     def _search_news_serialize(
         self,
@@ -1710,33 +1717,33 @@
         max_sentiment,
         earliest_publish_date,
         latest_publish_date,
         news_sources,
         authors,
         entities,
         location_filter,
-        offset,
-        number,
         sort,
         sort_direction,
+        offset,
+        number,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {}
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if text is not None:
 
             _query_params.append(('text', text))
@@ -1778,44 +1785,412 @@
 
             _query_params.append(('entities', entities))
 
         if location_filter is not None:
 
             _query_params.append(('location-filter', location_filter))
 
+        if sort is not None:
+
+            _query_params.append(('sort', sort))
+
+        if sort_direction is not None:
+
+            _query_params.append(('sort-direction', sort_direction))
+
         if offset is not None:
 
             _query_params.append(('offset', offset))
 
         if number is not None:
 
             _query_params.append(('number', number))
 
-        if sort is not None:
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
 
-            _query_params.append(('sort', sort))
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])
 
-        if sort_direction is not None:
+        # authentication setting
+        _auth_settings: List[str] = ['apiKey', 'headerApiKey']
 
-            _query_params.append(('sort-direction', sort_direction))
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/search-news',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth)
+
+    @validate_call
+    def top_news(
+        self,
+        source_country: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 3166 country code of the country for which top news should be retrieved."
+            )],
+        language: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 6391 language code of the top news. The language must be one spoken in the source-country."
+            )],
+        var_date: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=10)]],
+            Field(
+                description=
+                "The date for which the top news should be retrieved. If no date is given, the current day is assumed."
+            )] = None,
+        headlines_only: Annotated[
+            Optional[StrictBool],
+            Field(
+                description=
+                "Whether to only return basic information such as id, title, and url of the news."
+            )] = None,
+        _request_timeout: Union[None, Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                Tuple[Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                      Annotated[StrictFloat,
+                                                Field(gt=0)]]] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> TopNews200Response:
+        """Top News
+
+        Get the top news from a country in a language for a specific date. The top news are clustered from multiple sources in the given country. The more news in a cluster the higher the cluster is ranked.
+
+        :param source_country: The ISO 3166 country code of the country for which top news should be retrieved. (required)
+        :type source_country: str
+        :param language: The ISO 6391 language code of the top news. The language must be one spoken in the source-country. (required)
+        :type language: str
+        :param var_date: The date for which the top news should be retrieved. If no date is given, the current day is assumed.
+        :type var_date: str
+        :param headlines_only: Whether to only return basic information such as id, title, and url of the news.
+        :type headlines_only: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._top_news_serialize(source_country=source_country,
+                                          language=language,
+                                          var_date=var_date,
+                                          headlines_only=headlines_only,
+                                          _request_auth=_request_auth,
+                                          _content_type=_content_type,
+                                          _headers=_headers,
+                                          _host_index=_host_index)
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TopNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param, _request_timeout=_request_timeout)
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+    @validate_call
+    def top_news_with_http_info(
+        self,
+        source_country: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 3166 country code of the country for which top news should be retrieved."
+            )],
+        language: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 6391 language code of the top news. The language must be one spoken in the source-country."
+            )],
+        var_date: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=10)]],
+            Field(
+                description=
+                "The date for which the top news should be retrieved. If no date is given, the current day is assumed."
+            )] = None,
+        headlines_only: Annotated[
+            Optional[StrictBool],
+            Field(
+                description=
+                "Whether to only return basic information such as id, title, and url of the news."
+            )] = None,
+        _request_timeout: Union[None, Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                Tuple[Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                      Annotated[StrictFloat,
+                                                Field(gt=0)]]] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[TopNews200Response]:
+        """Top News
+
+        Get the top news from a country in a language for a specific date. The top news are clustered from multiple sources in the given country. The more news in a cluster the higher the cluster is ranked.
+
+        :param source_country: The ISO 3166 country code of the country for which top news should be retrieved. (required)
+        :type source_country: str
+        :param language: The ISO 6391 language code of the top news. The language must be one spoken in the source-country. (required)
+        :type language: str
+        :param var_date: The date for which the top news should be retrieved. If no date is given, the current day is assumed.
+        :type var_date: str
+        :param headlines_only: Whether to only return basic information such as id, title, and url of the news.
+        :type headlines_only: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._top_news_serialize(source_country=source_country,
+                                          language=language,
+                                          var_date=var_date,
+                                          headlines_only=headlines_only,
+                                          _request_auth=_request_auth,
+                                          _content_type=_content_type,
+                                          _headers=_headers,
+                                          _host_index=_host_index)
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TopNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param, _request_timeout=_request_timeout)
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+    @validate_call
+    def top_news_without_preload_content(
+        self,
+        source_country: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 3166 country code of the country for which top news should be retrieved."
+            )],
+        language: Annotated[
+            str,
+            Field(
+                strict=True,
+                max_length=2,
+                description=
+                "The ISO 6391 language code of the top news. The language must be one spoken in the source-country."
+            )],
+        var_date: Annotated[
+            Optional[Annotated[str, Field(strict=True, max_length=10)]],
+            Field(
+                description=
+                "The date for which the top news should be retrieved. If no date is given, the current day is assumed."
+            )] = None,
+        headlines_only: Annotated[
+            Optional[StrictBool],
+            Field(
+                description=
+                "Whether to only return basic information such as id, title, and url of the news."
+            )] = None,
+        _request_timeout: Union[None, Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                Tuple[Annotated[StrictFloat,
+                                                Field(gt=0)],
+                                      Annotated[StrictFloat,
+                                                Field(gt=0)]]] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Top News
+
+        Get the top news from a country in a language for a specific date. The top news are clustered from multiple sources in the given country. The more news in a cluster the higher the cluster is ranked.
+
+        :param source_country: The ISO 3166 country code of the country for which top news should be retrieved. (required)
+        :type source_country: str
+        :param language: The ISO 6391 language code of the top news. The language must be one spoken in the source-country. (required)
+        :type language: str
+        :param var_date: The date for which the top news should be retrieved. If no date is given, the current day is assumed.
+        :type var_date: str
+        :param headlines_only: Whether to only return basic information such as id, title, and url of the news.
+        :type headlines_only: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._top_news_serialize(source_country=source_country,
+                                          language=language,
+                                          var_date=var_date,
+                                          headlines_only=headlines_only,
+                                          _request_auth=_request_auth,
+                                          _content_type=_content_type,
+                                          _headers=_headers,
+                                          _host_index=_host_index)
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TopNews200Response",
+            '401': None,
+            '402': None,
+            '403': None,
+            '404': None,
+            '406': None,
+            '429': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param, _request_timeout=_request_timeout)
+        return response_data.response
+
+    def _top_news_serialize(
+        self,
+        source_country,
+        language,
+        var_date,
+        headlines_only,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {}
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if source_country is not None:
+
+            _query_params.append(('source-country', source_country))
+
+        if language is not None:
+
+            _query_params.append(('language', language))
+
+        if var_date is not None:
+
+            _query_params.append(('date', var_date))
+
+        if headlines_only is not None:
+
+            _query_params.append(('headlines-only', headlines_only))
 
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])
 
         # authentication setting
         _auth_settings: List[str] = ['apiKey', 'headerApiKey']
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/search-news',
+            resource_path='/top-news',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/api_client.py` & `worldnewsapi-1.1.1/worldnewsapi/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import datetime
@@ -18,15 +18,16 @@
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List, Dict
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from worldnewsapi.configuration import Configuration
 from worldnewsapi.api_response import ApiResponse, T as ApiResponseT
 import worldnewsapi.models
 from worldnewsapi import rest
 from worldnewsapi.exceptions import (ApiValueError, ApiException,
                                      BadRequestException,
@@ -77,15 +78,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
+        self.user_agent = 'OpenAPI-Generator/1.1.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -188,15 +189,16 @@
 
         # post parameters
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(header_params,
                                     query_params,
                                     auth_settings,
                                     resource_path,
                                     method,
@@ -291,15 +293,20 @@
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?",
                                       content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(
+                        response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text,
+                                                   response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -309,26 +316,31 @@
                            headers=response_data.getheaders(),
                            raw_data=response_data.data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -341,15 +353,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -482,36 +497,34 @@
                     new_params.append(
                         (k, delimiter.join(quote(str(value)) for value in v)))
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (mimetypes.guess_type(filename)[0]
-                                    or 'application/octet-stream')
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])]))
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (mimetypes.guess_type(filename)[0]
+                        or 'application/octet-stream')
+            params.append(tuple([k, tuple([filename, filedata, mimetype])]))
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/api_response.py` & `worldnewsapi-1.1.1/worldnewsapi/api_response.py`

 * *Files identical despite different names*

### Comparing `worldnewsapi-1.0.9/worldnewsapi/configuration.py` & `worldnewsapi-1.1.1/worldnewsapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import copy
@@ -406,16 +406,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.1\n"\
-               "SDK Package Version: 1.0.9".\
+               "Version of the API: 1.1.1\n"\
+               "SDK Package Version: 1.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/exceptions.py` & `worldnewsapi-1.1.1/worldnewsapi/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/models/extract_links_response.py` & `worldnewsapi-1.1.1/worldnewsapi/models/extract_news_links200_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 
-class ExtractLinksResponse(BaseModel):
+class ExtractNewsLinks200Response(BaseModel):
     """
-    ExtractLinksResponse
+    ExtractNewsLinks200Response
     """
 
   # noqa: E501
-    news_links: Optional[List[StrictStr]] = None
+    news_links: Optional[List[Optional[StrictStr]]] = None
     __properties: ClassVar[List[str]] = ["news_links"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExtractLinksResponse from a JSON string"""
+        """Create an instance of ExtractNewsLinks200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExtractLinksResponse from a dict"""
+        """Create an instance of ExtractNewsLinks200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({"news_links": obj.get("news_links")})
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/models/extract_news_response.py` & `worldnewsapi-1.1.1/worldnewsapi/models/search_news200_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, StrictInt
+from typing import Any, ClassVar, Dict, List, Optional
+from worldnewsapi.models.search_news200_response_news_inner import SearchNews200ResponseNewsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 
-class ExtractNewsResponse(BaseModel):
+class SearchNews200Response(BaseModel):
     """
-    ExtractNewsResponse
+    SearchNews200Response
     """
 
   # noqa: E501
-    title: Optional[StrictStr] = None
-    text: Optional[StrictStr] = None
-    url: Optional[StrictStr] = None
-    image: Optional[StrictStr] = None
-    author: Optional[StrictStr] = None
-    language: Optional[StrictStr] = None
-    source_country: Optional[StrictStr] = None
-    sentiment: Optional[Union[StrictFloat, StrictInt]] = None
+    offset: Optional[StrictInt] = None
+    number: Optional[StrictInt] = None
+    available: Optional[StrictInt] = None
+    news: Optional[List[SearchNews200ResponseNewsInner]] = None
     __properties: ClassVar[List[str]] = [
-        "title", "text", "url", "image", "author", "language",
-        "source_country", "sentiment"
+        "offset", "number", "available", "news"
     ]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExtractNewsResponse from a JSON string"""
+        """Create an instance of SearchNews200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,34 +71,38 @@
         excluded_fields: Set[str] = set([])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if image (nullable) is None
-        # and model_fields_set contains the field
-        if self.image is None and "image" in self.model_fields_set:
-            _dict['image'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of each item in news (list)
+        _items = []
+        if self.news:
+            for _item in self.news:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['news'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExtractNewsResponse from a dict"""
+        """Create an instance of SearchNews200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "title": obj.get("title"),
-            "text": obj.get("text"),
-            "url": obj.get("url"),
-            "image": obj.get("image"),
-            "author": obj.get("author"),
-            "language": obj.get("language"),
-            "source_country": obj.get("source_country"),
-            "sentiment": obj.get("sentiment")
+            "offset":
+            obj.get("offset"),
+            "number":
+            obj.get("number"),
+            "available":
+            obj.get("available"),
+            "news": [
+                SearchNews200ResponseNewsInner.from_dict(_item)
+                for _item in obj["news"]
+            ] if obj.get("news") is not None else None
         })
         return _obj
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/models/geo_coordinates_response.py` & `worldnewsapi-1.1.1/worldnewsapi/models/get_geo_coordinates200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
 
-class GeoCoordinatesResponse(BaseModel):
+class GetGeoCoordinates200Response(BaseModel):
     """
-    GeoCoordinatesResponse
+    GetGeoCoordinates200Response
     """
 
   # noqa: E501
-    latitude: Union[StrictFloat, StrictInt]
-    longitude: Union[StrictFloat, StrictInt]
+    latitude: Optional[Union[StrictFloat, StrictInt]] = None
+    longitude: Optional[Union[StrictFloat, StrictInt]] = None
     city: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["latitude", "longitude", "city"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GeoCoordinatesResponse from a JSON string"""
+        """Create an instance of GetGeoCoordinates200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,19 +67,24 @@
         excluded_fields: Set[str] = set([])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if city (nullable) is None
+        # and model_fields_set contains the field
+        if self.city is None and "city" in self.model_fields_set:
+            _dict['city'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GeoCoordinatesResponse from a dict"""
+        """Create an instance of GetGeoCoordinates200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/models/news.py` & `worldnewsapi-1.1.1/worldnewsapi/models/top_news200_response_top_news_inner_news_inner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 
-class News(BaseModel):
+class TopNews200ResponseTopNewsInnerNewsInner(BaseModel):
     """
-    A news entry.
+    TopNews200ResponseTopNewsInnerNewsInner
     """
 
   # noqa: E501
-    id: Optional[StrictInt] = None
-    title: Optional[StrictStr] = None
-    text: Optional[StrictStr] = None
     summary: Optional[StrictStr] = None
-    url: Optional[StrictStr] = None
     image: Optional[StrictStr] = None
+    id: Optional[StrictInt] = None
+    text: Optional[StrictStr] = None
+    title: Optional[StrictStr] = None
     publish_date: Optional[StrictStr] = None
-    author: Optional[StrictStr] = None
-    language: Optional[StrictStr] = None
-    source_country: Optional[StrictStr] = None
-    sentiment: Optional[Union[StrictFloat, StrictInt]] = None
+    url: Optional[StrictStr] = None
+    authors: Optional[List[Optional[StrictStr]]] = None
     __properties: ClassVar[List[str]] = [
-        "id", "title", "text", "summary", "url", "image", "publish_date",
-        "author", "language", "source_country", "sentiment"
+        "summary", "image", "id", "text", "title", "publish_date", "url",
+        "authors"
     ]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of News from a JSON string"""
+        """Create an instance of TopNews200ResponseTopNewsInnerNewsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,37 +75,59 @@
         excluded_fields: Set[str] = set([])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if summary (nullable) is None
+        # and model_fields_set contains the field
+        if self.summary is None and "summary" in self.model_fields_set:
+            _dict['summary'] = None
+
         # set to None if image (nullable) is None
         # and model_fields_set contains the field
         if self.image is None and "image" in self.model_fields_set:
             _dict['image'] = None
 
+        # set to None if text (nullable) is None
+        # and model_fields_set contains the field
+        if self.text is None and "text" in self.model_fields_set:
+            _dict['text'] = None
+
+        # set to None if title (nullable) is None
+        # and model_fields_set contains the field
+        if self.title is None and "title" in self.model_fields_set:
+            _dict['title'] = None
+
+        # set to None if publish_date (nullable) is None
+        # and model_fields_set contains the field
+        if self.publish_date is None and "publish_date" in self.model_fields_set:
+            _dict['publish_date'] = None
+
+        # set to None if url (nullable) is None
+        # and model_fields_set contains the field
+        if self.url is None and "url" in self.model_fields_set:
+            _dict['url'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of News from a dict"""
+        """Create an instance of TopNews200ResponseTopNewsInnerNewsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "title": obj.get("title"),
-            "text": obj.get("text"),
             "summary": obj.get("summary"),
-            "url": obj.get("url"),
             "image": obj.get("image"),
+            "id": obj.get("id"),
+            "text": obj.get("text"),
+            "title": obj.get("title"),
             "publish_date": obj.get("publish_date"),
-            "author": obj.get("author"),
-            "language": obj.get("language"),
-            "source_country": obj.get("source_country"),
-            "sentiment": obj.get("sentiment")
+            "url": obj.get("url"),
+            "authors": obj.get("authors")
         })
         return _obj
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/models/news_article.py` & `worldnewsapi-1.1.1/worldnewsapi/models/top_news200_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,62 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from worldnewsapi.models.top_news200_response_top_news_inner import TopNews200ResponseTopNewsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 
-class NewsArticle(BaseModel):
+class TopNews200Response(BaseModel):
     """
-    NewsArticle
+    TopNews200Response
     """
 
   # noqa: E501
-    id: Optional[StrictInt] = None
-    title: Optional[StrictStr] = None
-    text: Optional[StrictStr] = None
-    summary: Optional[StrictStr] = None
-    url: Optional[StrictStr] = None
-    image: Optional[StrictStr] = None
-    publish_date: Optional[StrictStr] = None
-    author: Optional[StrictStr] = None
+    top_news: Optional[List[TopNews200ResponseTopNewsInner]] = None
     language: Optional[StrictStr] = None
-    source_country: Optional[StrictStr] = None
-    sentiment: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = [
-        "id", "title", "text", "summary", "url", "image", "publish_date",
-        "author", "language", "source_country", "sentiment"
-    ]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    country: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["top_news", "language", "country"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NewsArticle from a JSON string"""
+        """Create an instance of TopNews200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,37 +68,46 @@
         excluded_fields: Set[str] = set([])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if image (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of each item in top_news (list)
+        _items = []
+        if self.top_news:
+            for _item in self.top_news:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['top_news'] = _items
+        # set to None if language (nullable) is None
+        # and model_fields_set contains the field
+        if self.language is None and "language" in self.model_fields_set:
+            _dict['language'] = None
+
+        # set to None if country (nullable) is None
         # and model_fields_set contains the field
-        if self.image is None and "image" in self.model_fields_set:
-            _dict['image'] = None
+        if self.country is None and "country" in self.model_fields_set:
+            _dict['country'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NewsArticle from a dict"""
+        """Create an instance of TopNews200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "title": obj.get("title"),
-            "text": obj.get("text"),
-            "summary": obj.get("summary"),
-            "url": obj.get("url"),
-            "image": obj.get("image"),
-            "publish_date": obj.get("publish_date"),
-            "author": obj.get("author"),
-            "language": obj.get("language"),
-            "source_country": obj.get("source_country"),
-            "sentiment": obj.get("sentiment")
+            "top_news": [
+                TopNews200ResponseTopNewsInner.from_dict(_item)
+                for _item in obj["top_news"]
+            ] if obj.get("top_news") is not None else None,
+            "language":
+            obj.get("language"),
+            "country":
+            obj.get("country")
         })
         return _obj
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi/rest.py` & `worldnewsapi-1.1.1/worldnewsapi/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     World News API
 
     The world's news wrapped into a single API.
 
-    The version of the OpenAPI document: 1.1
+    The version of the OpenAPI document: 1.1.1
     Contact: mail@worldnewsapi.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import io
@@ -174,14 +174,19 @@
                                                   headers=headers,
                                                   preload_content=False)
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [
+                        (a, json.dumps(b)) if isinstance(b, dict) else (a, b)
+                        for a, b in post_params
+                    ]
                     r = self.pool_manager.request(method,
                                                   url,
                                                   fields=post_params,
                                                   encode_multipart=True,
                                                   timeout=timeout,
                                                   headers=headers,
                                                   preload_content=False)
```

### Comparing `worldnewsapi-1.0.9/worldnewsapi.egg-info/PKG-INFO` & `worldnewsapi-1.1.1/worldnewsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldnewsapi
-Version: 1.0.9
+Version: 1.1.1
 Summary: The world's news wrapped into a single API.
 Home-page: 
 Author: David Urbansky
 Author-email: David Urbansky <mail@worldnewsapi.com>
 Project-URL: Homepage, https://worldnewsapi.com
 Project-URL: Documentation, https://worldnewsapi.com/docs
 Project-URL: Repository, https://github.com/ddsky/world-news-api-clients/tree/main/python
```

