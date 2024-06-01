# Comparing `tmp/baidu_serp_api-0.6.tar.gz` & `tmp/baidu_serp_api-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.6.tar", last modified: Fri May 31 02:47:22 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.7.tar", last modified: Sat Jun  1 16:55:05 2024, max compression
```

## Comparing `baidu_serp_api-0.6.tar` & `baidu_serp_api-0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-31 02:47:22.000000 baidu_serp_api-0.6/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-31 02:47:22.000000 baidu_serp_api-0.6/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:47:22.000000 baidu_serp_api-0.6/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 02:47:22.000000 baidu_serp_api-0.6/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 02:47:22.000000 baidu_serp_api-0.6/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:47:22.244418 baidu_serp_api-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-31 02:47:17.000000 baidu_serp_api-0.6/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:55:05.098178 baidu_serp_api-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.6/LICENSE.txt` & `baidu_serp_api-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.6/PKG-INFO` & `baidu_serp_api-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.6
+Version: 0.7
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.6/README.md` & `baidu_serp_api-0.7/README.md`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.6/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.7/baidu_serp_api/baidu_mobile.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 class BaiduMobile:
     
     def __init__(self):
         self.random_params = gen_random_params()
         self.keyword = None
         self.recomment_list = []
+        self.date_range = None
+        self.pn = None
+        self.proxies = None
 
     def extract_baidum_data(self, html_content):
         search_data = []
         soup = BeautifulSoup(html_content, 'html.parser')
         search_results = soup.select('div[tpl="www_index"]')
         for result in search_results:
             title_element = result.find('p', class_='cu-title')
@@ -22,14 +25,18 @@
             if url:
                 url = json.loads(url)['mu']
 
             description = ""
             date_time = ""
             source = ""
 
+            order = int(result.get('order', 0))
+            pn = self.pn if self.pn is not None else 1
+            ranking = order + (pn - 1) * 10
+
             summary_element = result.select_one('div[class*=summary-]')
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
                 date_time_element = summary_element.find('span', class_='c-gap-right-small c-color-gray')
                 if date_time_element:
                     description = description.replace(date_time_element.get_text().strip(), '')
@@ -37,19 +44,19 @@
 
             source_element = result.select_one('div[class*=_text_]')
             if source_element:
                 source = source_element.get_text().strip()
 
             if title_element and url:
                 title_text = clean_html_tags(title_element.get_text().strip())
-                search_data.append({'title': title_text, 'url': url, 'description': description, 'date_time': date_time, "source": source})
+                search_data.append({'title': title_text, 'url': url, 'description': description, 'date_time': date_time, "source": source, "ranking": ranking})
 
         return search_data
 
-    def get_recommend(self, keyword, qid, proxies=None):
+    def get_recommend(self, keyword, qid):
         url = 'https://m.baidu.com/rec'
         params = {
             'word': keyword,
             'platform': 'wise',
             'ms': '1',
             'lsAble': '1',
             'rset': 'rcmd',
@@ -63,15 +70,15 @@
             'r': self.random_params['r'],
         }
         headers = {
             'Cookie': f'BAIDUID={self.random_params["baiduid"]}:FG=1; BAIDUID_BFESS={self.random_params["baiduid"]}:FG=1;BDUSS={self.random_params["bduss"]};',
             'User-Agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36 baiduboxapp/13.10.0.10',
         }
         try:
-            response = requests.get(url, headers=headers, params=params, proxies=proxies, timeout=10)
+            response = requests.get(url, headers=headers, params=params, proxies=self.proxies, timeout=10)
             response.raise_for_status()
             response.encoding = 'utf-8'
             json_data = response.json()
             # 获取所有键名为'up'和'down'的值
             up_values = []
             down_values = []
             if json_data['errcode'] != 0:
@@ -83,41 +90,41 @@
 
                 # 排重并合并为新的列表
                 recomment_list = list(set(up_values + down_values))
                 return recomment_list
         except requests.exceptions.RequestException as e:
             return []
 
-    def get_baidum_serp(self, keyword, date_range=None, pn=None, proxies=None):
+    def get_baidum_serp(self, keyword):
         url = 'https://m.baidu.com/s'
         params = {
             'word': keyword
         }
-        if date_range:
-            start_date, end_date = date_range.split(',')
+        if self.date_range:
+            start_date, end_date = self.date_range.split(',')
             start_timestamp = int(datetime.strptime(start_date, '%Y%m%d').timestamp())
             end_timestamp = int(datetime.strptime(end_date, '%Y%m%d').timestamp())
             params['gpc'] = f'stf={start_timestamp},{end_timestamp}|stftype=2'
-        if pn:
-            params['pn'] = str((int(pn) - 1) * 10)
+        if self.pn:
+            params['pn'] = str((int(self.pn) - 1) * 10)
         headers = {
             'Cookie': f'BAIDUID={self.random_params["baiduid"]}:FG=1; BAIDUID_BFESS={self.random_params["baiduid"]}:FG=1;BDUSS={self.random_params["bduss"]};',
             'User-Agent': 'Mozilla/5.0 (Linux; Android 13; SM-G981B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36 baiduboxapp/13.10.0.10'
         }
         try:
-            response = requests.get(url, headers=headers, params=params, proxies=proxies, timeout=10)
+            response = requests.get(url, headers=headers, params=params, proxies=self.proxies, timeout=10)
             response.raise_for_status()
             response.encoding = 'utf-8'
 
             # 如果没有传页码或者是第1页则获取相关搜索词
-            if pn is None or pn==1:
+            if self.pn is None or self.pn==1:
                 res_headers = response.headers
                 if 'qid' in res_headers:
                     qid = res_headers['qid']
-                self.recomment_list = self.get_recommend(keyword, qid=qid, proxies=proxies)
+                self.recomment_list = self.get_recommend(keyword, qid=qid)
 
                 soup = BeautifulSoup(response.text, 'html.parser')
                 page_rcmd = [elem.get_text() for elem in soup.select('a.c-fwb, span.c-fwb')]
                 
                 # 合并并排重
                 self.recomment_list = list(set(self.recomment_list + page_rcmd))
 
@@ -138,9 +145,12 @@
                 search_results = self.extract_baidum_data(response)
                 last_page = 'new-nextpage' not in response
                 return {'code': 200, 'msg': 'ok', 'data': {'results': search_results, 'recomment': self.recomment_list, 'last_page': last_page}}
         else:
             return response
 
     def search(self, keyword, date_range=None, pn=None, proxies=None):
-        html_content = self.get_baidum_serp(keyword, date_range, pn, proxies)
+        self.date_range = date_range
+        self.pn = pn
+        self.proxies = proxies
+        html_content = self.get_baidum_serp(keyword)
         return self.handle_response(html_content)
```

### Comparing `baidu_serp_api-0.6/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.7/baidu_serp_api/baidu_pc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import requests
 from bs4 import BeautifulSoup
 import json
-from urllib.parse import quote
 from datetime import datetime
 from .util import gen_random_params, clean_html_tags, logger
 import re
 
 class BaiduPc:
 
     def __init__(self):
         self.random_params = gen_random_params()
         self.keyword = None
+        self.date_range = None
+        self.pn = None
+        self.proxies = None
 
     def extract_baidupc_data(self, html_content):
         soup = BeautifulSoup(html_content, 'html.parser')
         search_results = soup.select('div[tpl="se_com_default"]')
         result_data = []
         for result in search_results:
             title_element = result.select_one('h3.c-title')
 
             url = result.get('mu')
 
             description = ""
             date_time = ""
             source = ""
 
+            ranking = result.get('id', 0)
+
             summary_element = result.select_one('span[class^="content-right_"]')
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
             date_time_element = result.select_one('span.c-color-gray2')
             if date_time_element:
                 date_time = date_time_element.get_text().strip()
 
             source_element = result.select_one('span.c-color-gray')
             if source_element:
                 source = source_element.get_text().strip()
 
             if title_element and url:
                 title_text = clean_html_tags(title_element.get_text().strip())
-                result_data.append({"title": title_text, "url": url, "description": description, "date_time": date_time, "source": source})
+                result_data.append({"title": title_text, "url": url, "description": description, "date_time": date_time, "source": source, "ranking": ranking})
 
         return result_data
 
     def get_recommend(self, html_content):
         # 找出所有 s-data 注释块
         pattern = r"<!--s-data:(.*?)-->"
         matches = re.findall(pattern, html_content, re.DOTALL)
@@ -62,15 +66,15 @@
                 for sublist in json_data['newList']:
                     for item in sublist:
                         keyword_set.add(item['word'])
 
         recomment_list = list(keyword_set)
         return recomment_list
 
-    def get_baidupc_serp(self, keyword, date_range=None, pn=None, proxies=None):
+    def get_baidupc_serp(self, keyword):
         url = 'http://www.baidu.com/s'
 
         params = {
             'wd': keyword,
             'ie':'utf-8',
             'f':'8',
             'rsv_bp':'1',
@@ -101,24 +105,23 @@
         # 搜索词为site:xxx时, 增加si和ct参数
         if 'site:' in keyword:
             site = keyword.split('site:')[1].strip()
             params['si'] = site
             params['ct'] = '2097152'
 
         # 搜索指定日期范围
-        if date_range:
-            start_date, end_date = date_range.split(',')
+        if self.date_range:
+            start_date, end_date = self.date_range.split(',')
             start_timestamp = int(datetime.strptime(start_date, '%Y%m%d').timestamp())
             end_timestamp = int(datetime.strptime(end_date, '%Y%m%d').timestamp())
-            # params['gpc'] = quote(f'stf={start_timestamp},{end_timestamp}|stftype=2')
             params['gpc'] = f'stf={start_timestamp},{end_timestamp}|stftype=2'
 
         # 搜索指定页码
-        if pn:
-            params['pn'] = str((int(pn) - 1) * 10)
+        if self.pn:
+            params['pn'] = str((int(self.pn) - 1) * 10)
 
         # logger.debug(params)
         headers = {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'Accept-Encoding': 'gzip, deflate, br, zstd',
             'Accept-Language': 'zh-CN,zh;q=0.9',
             'Cache-Control': 'no-cache',
@@ -135,15 +138,15 @@
             'sec-ch-ua-platform': '"macOS"',
             'Referer': 'http://www.baidu.com/',
             'cookie': f'BAIDUID={self.random_params["baiduid"]}:FG=1; BAIDUID_BFESS={self.random_params["baiduid"]}:FG=1; '\
                     f'BDUSS={self.random_params["bduss"]}; H_PS_645EC={self.random_params["rsv_t"]}; H_PS_PSSID={self.random_params["rsv_sid"]}',
             'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36'
         }
         try:
-            response = requests.get(url, headers=headers, params=params, proxies=proxies, timeout=10, allow_redirects=False)
+            response = requests.get(url, headers=headers, params=params, proxies=self.proxies, timeout=10, allow_redirects=False)
             # logger.debug(response.url)
             response.raise_for_status()
             response.encoding = 'utf-8'
             return response.text
         except requests.exceptions.RequestException as e:
             return {'code': 500, 'msg': '网络请求失败'}
 
@@ -161,9 +164,12 @@
                 last_page = '下一页' not in response
                 return {'code': 200, 'msg': 'ok', 'data': {'results': search_results, 'recommend':recomment_list, 'last_page': last_page}}
         else:
             return response
 
     def search(self, keyword, date_range=None, pn=None, proxies=None):
         self.keyword = keyword
-        html_content = self.get_baidupc_serp(keyword, date_range, pn, proxies)
+        self.date_range = date_range
+        self.pn = pn
+        self.proxies = proxies
+        html_content = self.get_baidupc_serp(keyword)
         return self.handle_response(html_content)
```

### Comparing `baidu_serp_api-0.6/baidu_serp_api/util.py` & `baidu_serp_api-0.7/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.6/baidu_serp_api.egg-info/PKG-INFO` & `baidu_serp_api-0.7/baidu_serp_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.6
+Version: 0.7
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.6/setup.py` & `baidu_serp_api-0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baidu-serp-api',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `baidu_serp_api-0.6/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.7/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

