# Comparing `tmp/webull_options-0.6.3.tar.gz` & `tmp/webull_options-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_options-0.6.3.tar", last modified: Wed May 15 16:01:00 2024, max compression
+gzip compressed data, was "webull_options-0.6.4.tar", last modified: Sat Jun  1 18:46:29 2024, max compression
```

## Comparing `webull_options-0.6.3.tar` & `webull_options-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.265092 webull_options-0.6.3/
--rw-rw-rw-   0        0        0     7368 2024-05-15 16:01:00.265092 webull_options-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 16:01:00.265092 webull_options-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-05-15 16:00:43.000000 webull_options-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/__init__.py
--rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options/models/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.3/webull_options/models/__init__.py
--rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.3/webull_options/models/db_manager.py
--rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 webull_options-0.6.3/webull_options/models/options_data.py
--rw-rw-rw-   0        0        0    47390 2024-05-15 16:00:35.000000 webull_options-0.6.3/webull_options/webull_options.py
--rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.3/webull_options/webull_trader.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:01:00.255088 webull_options-0.6.3/webull_options.egg-info/
--rw-rw-rw-   0        0        0     7368 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3867 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 16:01:00.000000 webull_options-0.6.3/webull_options.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.367531 webull_options-0.6.4/
+-rw-rw-rw-   0        0        0     7366 2024-06-01 18:46:29.366531 webull_options-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 18:46:29.367531 webull_options-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-06-01 18:46:17.000000 webull_options-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.341023 webull_options-0.6.4/webull_options/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/__init__.py
+-rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.358531 webull_options-0.6.4/webull_options/models/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/models/__init__.py
+-rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.4/webull_options/models/db_manager.py
+-rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 webull_options-0.6.4/webull_options/models/options_data.py
+-rw-rw-rw-   0        0        0    47798 2024-06-01 18:46:08.000000 webull_options-0.6.4/webull_options/webull_options.py
+-rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.4/webull_options/webull_trader.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.356527 webull_options-0.6.4/webull_options.egg-info/
+-rw-rw-rw-   0        0        0     7366 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3865 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/top_level.txt
```

### Comparing `webull_options-0.6.3/PKG-INFO` & `webull_options-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: webull_options
-Version: 0.6.3
+Version: 0.6.4
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: asgiref==3.7.2
 Requires-Dist: astunparse==1.6.3
 Requires-Dist: async-timeout==4.0.3
-Requires-Dist: asyncio==3.4.3
+Requires-Dist: asyncio==3.9.3
 Requires-Dist: asyncpg==0.29.0
 Requires-Dist: attrs==23.1.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: bcrypt==4.0.1
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bidict==0.22.1
 Requires-Dist: blinker==1.7.0
@@ -114,27 +114,27 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.14.1
+Requires-Dist: openai==1.30.1
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: orjson==3.9.10
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: overrides==7.4.0
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.2.1
+Requires-Dist: pandas==2.2.2
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: plotly==5.20.0
 Requires-Dist: polygon==1.1.3
 Requires-Dist: polygon-api-client==1.13.3
 Requires-Dist: posthog==3.0.2
@@ -205,14 +205,14 @@
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.23.2
 Requires-Dist: waitress==2.1.2
 Requires-Dist: watchfiles==0.21.0
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
 Requires-Dist: websocket-client==1.6.4
-Requires-Dist: websockets==11.0.3
+Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: wsproto==1.2.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yfinance==0.2.32
 Requires-Dist: zipp==3.17.0
```

### Comparing `webull_options-0.6.3/webull_options/helpers.py` & `webull_options-0.6.4/webull_options/helpers.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.3/webull_options/models/db_manager.py` & `webull_options-0.6.4/webull_options/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.3/webull_options/models/options_data.py` & `webull_options-0.6.4/webull_options/models/options_data.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.3/webull_options/webull_options.py` & `webull_options-0.6.4/webull_options/webull_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,44 +143,45 @@
         # Calculate the nearest Friday
         today = datetime.now()
         nearest_friday = today + timedelta((4-today.weekday()) % 7)  # 4 represents Friday
         expireDate = nearest_friday.strftime('%Y-%m-%d')  # Format to YYYY-MM-DD
             
         ticker_id = await self.get_ticker_id(ticker)
 
-
-
         params = {
             "tickerId": f"{ticker_id}",
             "count": -1,
             "direction": direction,
             "type": 0,
             "quoteMultiplier": 100,
             "unSymbol": f"{ticker}",
             "expireDate": expireDate
         }
-        url=f"https://quotes-gw.webullfintech.com/api/quote/option/strategy/list"
-        async with httpx.AsyncClient(headers=self.headers) as client:
-            data = await client.post(url, data=json.dumps(params))
-            try:
-                data = data.json()
+        url = "https://quotes-gw.webullfintech.com/api/quote/option/strategy/list"
+        
+        try:
+            async with httpx.AsyncClient(headers=self.headers, timeout=60) as client:
+                response = await client.post(url, data=json.dumps(params))
+                response.raise_for_status()
+                data = response.json()
 
                 from_ = 0
                 base_data = OptionData(data)
-
-
-                underlying_price = base_data.close
-                vol1y = base_data.vol1y
-
                 option_data = OptionData(data)
 
                 return base_data, from_, option_data
-            except Exception as e:
-                print(e)
-                
+        except httpx.RequestError as exc:
+            print(f"An error occurred while requesting {exc.request.url!r}: {exc}")
+        except httpx.HTTPStatusError as exc:
+            print(f"Error response {exc.response.status_code} while requesting {exc.request.url!r}: {exc.response.text}")
+        except httpx.ReadTimeout:
+            print(f"ReadTimeout while requesting {url}")
+        except Exception as e:
+            print(f"An unexpected error occurred: {e}")
+        return None, None, None
     async def zeroDTE_options(self, ticker, direction='all'):
         
         ticker_id = await self.get_ticker_id(ticker)
  
 
 
         params = {
```

### Comparing `webull_options-0.6.3/webull_options/webull_trader.py` & `webull_options-0.6.4/webull_options/webull_trader.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.3/webull_options.egg-info/PKG-INFO` & `webull_options-0.6.4/webull_options.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: webull-options
-Version: 0.6.3
+Version: 0.6.4
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: asgiref==3.7.2
 Requires-Dist: astunparse==1.6.3
 Requires-Dist: async-timeout==4.0.3
-Requires-Dist: asyncio==3.4.3
+Requires-Dist: asyncio==3.9.3
 Requires-Dist: asyncpg==0.29.0
 Requires-Dist: attrs==23.1.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: bcrypt==4.0.1
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bidict==0.22.1
 Requires-Dist: blinker==1.7.0
@@ -114,27 +114,27 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.14.1
+Requires-Dist: openai==1.30.1
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: orjson==3.9.10
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: overrides==7.4.0
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.2.1
+Requires-Dist: pandas==2.2.2
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: plotly==5.20.0
 Requires-Dist: polygon==1.1.3
 Requires-Dist: polygon-api-client==1.13.3
 Requires-Dist: posthog==3.0.2
@@ -205,14 +205,14 @@
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.23.2
 Requires-Dist: waitress==2.1.2
 Requires-Dist: watchfiles==0.21.0
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
 Requires-Dist: websocket-client==1.6.4
-Requires-Dist: websockets==11.0.3
+Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: wsproto==1.2.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yfinance==0.2.32
 Requires-Dist: zipp==3.17.0
```

### Comparing `webull_options-0.6.3/webull_options.egg-info/requires.txt` & `webull_options-0.6.4/webull_options.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 aiosignal==1.3.1
 annotated-types==0.6.0
 anyio==3.7.1
 appdirs==1.4.4
 asgiref==3.7.2
 astunparse==1.6.3
 async-timeout==4.0.3
-asyncio==3.4.3
+asyncio==3.9.3
 asyncpg==0.29.0
 attrs==23.1.0
 backoff==2.2.1
 bcrypt==4.0.1
 beautifulsoup4==4.12.2
 bidict==0.22.1
 blinker==1.7.0
@@ -111,27 +111,27 @@
 mypy-extensions==1.0.0
 namex==0.0.7
 natsort==8.4.0
 nh3==0.2.14
 numpy==1.26.4
 oauthlib==3.2.2
 onnxruntime==1.16.1
-openai==1.14.1
+openai==1.30.1
 opentelemetry-api==1.20.0
 opentelemetry-exporter-otlp-proto-common==1.20.0
 opentelemetry-exporter-otlp-proto-grpc==1.20.0
 opentelemetry-proto==1.20.0
 opentelemetry-sdk==1.20.0
 opentelemetry-semantic-conventions==0.41b0
 opt-einsum==3.3.0
 orjson==3.9.10
 outcome==1.3.0.post0
 overrides==7.4.0
 packaging==23.2
-pandas==2.2.1
+pandas==2.2.2
 peewee==3.17.0
 Pillow==10.1.0
 pkginfo==1.9.6
 plotly==5.20.0
 polygon==1.1.3
 polygon-api-client==1.13.3
 posthog==3.0.2
@@ -202,14 +202,14 @@
 urllib3==1.26.18
 uvicorn==0.23.2
 waitress==2.1.2
 watchfiles==0.21.0
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.6.4
-websockets==11.0.3
+websockets==12.0
 Werkzeug==3.0.1
 wrapt==1.14.1
 wsproto==1.2.0
 yarl==1.9.4
 yfinance==0.2.32
 zipp==3.17.0
```

