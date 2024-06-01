# Comparing `tmp/cyhole-0.0.1a0.tar.gz` & `tmp/cyhole-0.0.1a1.tar.gz`

## Comparing `cyhole-0.0.1a0.tar` & `cyhole-0.0.1a1.tar`

### file list

```diff
@@ -1,38 +1,60 @@
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/mkdocs.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/.github/workflows/publish-doc.yml
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/.github/workflows/publish-version.yml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/index.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/requirements.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/config/css/mkdocstrings.css
--rw-r--r--   0        0        0    35043 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/config/images/logo.png
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/config/overrides/partials/toc-item.html
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/development/index.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/development/core/api.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/development/core/exception.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/development/core/index.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/development/core/param.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/interactions/birdeye/api.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/interactions/birdeye/exception.md
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/interactions/birdeye/index.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/interactions/birdeye/param.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/docs/interactions/birdeye/schema.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/__init__.py
--rw-r--r--   0        0        0    30054 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/birdeye/Birdeye.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/birdeye/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/birdeye/exception.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/birdeye/param.py
--rw-r--r--   0        0        0    29953 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/birdeye/schema.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/core/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/core/api.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/core/exception.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/src/cyhole/core/param.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/tests/config.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/tests/requirements.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/tests/test.default.ini
--rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/tests/test_birdeye.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/README.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 cyhole-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/mkdocs.yml
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/.github/workflows/execute-tests.yml
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/.github/workflows/publish-doc.yml
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/.github/workflows/publish-version.yml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/index.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/requirements.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/config/css/mkdocstrings.css
+-rw-r--r--   0        0        0    35043 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/config/images/logo.png
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/config/overrides/partials/toc-item.html
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/development/index.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/development/core/api.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/development/core/exception.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/development/core/index.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/development/core/param.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/interactions/birdeye/api.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/interactions/birdeye/exception.md
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/interactions/birdeye/index.md
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/interactions/birdeye/param.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/docs/interactions/birdeye/schema.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/__init__.py
+-rw-r--r--   0        0        0    29189 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/birdeye/Birdeye.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/birdeye/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/birdeye/exception.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/birdeye/param.py
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/birdeye/schema.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/api.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/exception.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/param.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/address/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/address/ethereum.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/src/cyhole/core/address/solana.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/config.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/requirements.txt
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/test.default.ini
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/test_birdeye.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/test_core.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_history.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_ohlcv_base_quote.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_ohlcv_pair.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_ohlcv_token.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_price.json
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_price_historical.json
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_price_multiple.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_creation_info.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_list.json
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_overview_ethereum.json
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_overview_solana.json
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_security_other.json
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_token_security_solana.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_trades_pair.json
+-rw-r--r--   0        0        0    54140 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_trades_token.json
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/tests/resources/mock/birdeye/get_wallet_supported_networks.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/README.md
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 cyhole-0.0.1a1/PKG-INFO
```

### Comparing `cyhole-0.0.1a0/mkdocs.yml` & `cyhole-0.0.1a1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/.github/workflows/publish-doc.yml` & `cyhole-0.0.1a1/.github/workflows/publish-doc.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 jobs:
   deploy:
     name: deploy a new version of cyhole library documentation
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
+        with:
+          token: ${{ secrets.GITHUB_TOKEN }}
 
       # set up environment
       - name: setup python
         uses: actions/setup-python@v3
         with:
           python-version: 3.12
       - name: install pip
```

### Comparing `cyhole-0.0.1a0/.github/workflows/publish-version.yml` & `cyhole-0.0.1a1/.github/workflows/publish-version.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - name: install dependencies
         run: pip install -r src/requirements.txt
       - name: install build
         run: python -m pip install --upgrade build
 
       # update library version equals release
       - name: update version in pyproject.toml
-        run: sed -i "s/{{PROJET_VERSION}}/${{ github.event.release.tag_name }}/g" pyproject.toml
+        run: sed -i "s/{{PROJECT_VERSION}}/${{ github.event.release.tag_name }}/g" pyproject.toml
 
       # build package
       - name: build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/
 
       # publish on pypi
       - name: publish package
```

### Comparing `cyhole-0.0.1a0/docs/config/images/logo.png` & `cyhole-0.0.1a1/docs/config/images/logo.png`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/docs/config/overrides/partials/toc-item.html` & `cyhole-0.0.1a1/docs/config/overrides/partials/toc-item.html`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/docs/development/index.md` & `cyhole-0.0.1a1/docs/development/index.md`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/docs/interactions/birdeye/index.md` & `cyhole-0.0.1a1/docs/interactions/birdeye/index.md`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/docs/interactions/birdeye/schema.md` & `cyhole-0.0.1a1/docs/interactions/birdeye/schema.md`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/src/cyhole/birdeye/Birdeye.py` & `cyhole-0.0.1a1/src/cyhole/birdeye/Birdeye.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import requests
+from typing import Any
 from datetime import datetime
 
 from ..core.api import APICaller
 from ..core.param import RequestType
 from ..core.exception import MissingAPIKeyError, AuthorizationAPIKeyError
 from ..birdeye.exception import BirdeyeTimeRangeError, BirdeyeAuthorisationError
 from ..birdeye.param import (
@@ -70,14 +72,21 @@
         super().__init__(header)
 
         self.url_api_public = "https://public-api.birdeye.so/defi/"
         self.url_api_private = "https://public-api.birdeye.so/defi/"
         self.url_api_private_wallet = "https://public-api.birdeye.so/v1/wallet"
         return
 
+    def api(self, type: str, url: str, *args: tuple, **kwargs: dict[str, Any]) -> requests.Response:
+        # overide function to manage client specific exceptions
+        try:
+            return super().api(type, url, *args, **kwargs)
+        except AuthorizationAPIKeyError:
+            raise BirdeyeAuthorisationError
+
     def get_token_list(
         self,
         chain: str = BirdeyeChain.SOLANA.value,
         sort_by: str = BirdeyeSort.SORT_V24HUSD.value,
         order_by: str = BirdeyeOrder.DESCENDING.value,
         offset: int | None = None,
         limit: int | None = None
@@ -120,18 +129,15 @@
             "sort_by" : sort_by,
             "sort_type" : order_by,
             "offset" : offset,
             "limit": limit
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetTokenListResponse(**content_raw.json())
 
         return content
 
     def get_token_creation_info(
@@ -163,18 +169,15 @@
         url = self.url_api_public + "token_creation_info"
         params = {
             "x-chain" : chain,
             "address" : address
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetTokenCreationInfoResponse(**content_raw.json())
 
         return content
 
     def get_token_security(
@@ -208,18 +211,15 @@
         url = self.url_api_public + "token_security"
         params = {
             "x-chain" : chain,
             "address" : address
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetTokenSecurityResponse(**content_raw.json())
 
         return content
 
     def get_token_overview(
@@ -295,18 +295,15 @@
         params = {
             "x-chain" : chain,
             "address" : address,
             "include_liquidity" : str(include_liquidity).lower() if include_liquidity else None
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetPriceResponse(**content_raw.json())
 
         return content
 
     def get_price_multiple(
@@ -342,18 +339,15 @@
         params = {
             "x-chain" : chain,
             "list_address" : ",".join(list_address),
             "include_liquidity" : str(include_liquidity).lower() if include_liquidity else None
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetPriceMultipleResponse(**content_raw.json())
 
         return content
 
     def get_price_historical(
@@ -400,32 +394,29 @@
 
         # set default
         if dt_to is None:
             dt_to = datetime.now()
 
         # check consistency
         if dt_from > dt_to:
-            raise BirdeyeTimeRangeError(f"Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
+            raise BirdeyeTimeRangeError("Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
 
         # set params
         url = self.url_api_public + "history_price"
         params = {
             "x-chain" : chain,
             "address" : address,
             "address_type" : address_type,
             "type" : timeframe,
             "time_from" : int(dt_from.timestamp()),
             "time_to" : int(dt_to.timestamp())
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetPriceHistoricalResponse(**content_raw.json())
 
         return content
 
     def get_history(self, chain: str = BirdeyeChain.SOLANA.value) -> GetHistoryResponse:
@@ -451,18 +442,15 @@
         # set params
         url = self.url_api_public + "history"
         params = {
             "x-chain" : chain
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetHistoryResponse(**content_raw.json())
 
         return content
 
     def get_trades_token(
@@ -506,18 +494,15 @@
             "tx_type" : trade_type,
             "x-chain" : chain,
             "offset" : offset,
             "limit": limit
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetTradesTokenResponse(**content_raw.json())
 
         return content
 
     def get_trades_pair(
@@ -569,18 +554,15 @@
             "x-chain" : chain,
             "sort_type": order_by,
             "offset" : offset,
             "limit": limit
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetTradesPairResponse(**content_raw.json())
 
         return content
 
     def get_ohlcv(
@@ -627,33 +609,30 @@
 
         # set default
         if dt_to is None:
             dt_to = datetime.now()
 
         # check consistency
         if dt_from > dt_to:
-            raise BirdeyeTimeRangeError(f"Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
+            raise BirdeyeTimeRangeError("Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
 
         # set params
         url = self.url_api_public + "ohlcv"
         if address_type == BirdeyeAddressType.PAIR.value:
             url = url + "/" + BirdeyeAddressType.PAIR.value
         params = {
             "x-chain" : chain,
             "address" : address,
             "type" : timeframe,
             "time_from" : int(dt_from.timestamp()),
             "time_to" : int(dt_to.timestamp())
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetOHLCVTokenPairResponse(**content_raw.json())
 
         return content
 
     def get_ohlcv_base_quote(
@@ -697,32 +676,29 @@
 
         # set default
         if dt_to is None:
             dt_to = datetime.now()
 
         # check consistency
         if dt_from > dt_to:
-            raise BirdeyeTimeRangeError(f"Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
+            raise BirdeyeTimeRangeError("Inconsistent timewindow provided: 'dt_from' > 'dt_to'")
 
         # set params
         url = self.url_api_public + "ohlcv/base_quote"
         params = {
             "x-chain" : chain,
             "base_address" : base_address,
             "quote_address" : quote_address,
             "type" : timeframe,
             "time_from" : int(dt_from.timestamp()),
             "time_to" : int(dt_to.timestamp())
         }
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url, params = params)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url, params = params)
 
         # parse response
         content = GetOHLCVBaseQuoteResponse(**content_raw.json())
 
         return content
 
     def get_wallet_supported_networks(self) -> GetWalletSupportedNetworksResponse:
@@ -735,16 +711,13 @@
 
             Raises:
                 BirdeyeAuthorisationError: if the API key provided does not give access to related endpoint.
         """
         url = self.url_api_private_wallet + "/list_supported_chain"
 
         # execute request
-        try:
-            content_raw = self.api(RequestType.GET.value, url)
-        except AuthorizationAPIKeyError:
-            raise BirdeyeAuthorisationError
+        content_raw = self.api(RequestType.GET.value, url)
 
         # parse response
         content = GetWalletSupportedNetworksResponse(**content_raw.json())
 
         return content
```

### Comparing `cyhole-0.0.1a0/src/cyhole/birdeye/param.py` & `cyhole-0.0.1a1/src/cyhole/birdeye/param.py`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/src/cyhole/birdeye/schema.py` & `cyhole-0.0.1a1/src/cyhole/birdeye/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
     type: str
     type_swap: str = Field(alias = "typeSwap")
     ui_amount: float = Field(alias = "uiAmount")
     price: float | None = None
     nearest_price: float = Field(alias = "nearestPrice")
     change_amount: float = Field(alias = "changeAmount")
     ui_change_amount: float = Field(alias = "uiChangeAmount")
-    icon: str
+    icon: str | None = None
 
 class GetTradesTokenTrade(BaseModel):
     volume: float
     volume_usd: float = Field(alias = "volumeUSD")
     trade_hash: str = Field(alias = "txHash")
     slot: int
     source: str
```

### Comparing `cyhole-0.0.1a0/src/cyhole/core/api.py` & `cyhole-0.0.1a1/src/cyhole/core/api.py`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/src/cyhole/core/exception.py` & `cyhole-0.0.1a1/src/cyhole/core/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         General exception of Cyhole library
     """
     def __init__(self, description):
         self.description = description
 
     def __str__(self):
         return self.description
-    
+
 class RequestTypeNotSupported(CyholeException):
     pass
 
 class AuthorizationAPIKeyError(CyholeException):
     pass
 
 class MissingAPIKeyError(CyholeException):
```

### Comparing `cyhole-0.0.1a0/src/cyhole/core/param.py` & `cyhole-0.0.1a1/src/cyhole/core/param.py`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/tests/config.py` & `cyhole-0.0.1a1/tests/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,24 +19,26 @@
     disabled, the process automatically stores the response in a JSON file into the 
     proper resources folder.
 
 """
 import json
 import configparser
 from pathlib import Path
+from requests import Response
 from typing import TypeVar, Type
 from pydantic import BaseModel
 
 ResponseModel = TypeVar('ResponseModel', bound = BaseModel)
 
 class BirdeyeConfiguration(BaseModel):
     """
         Model in charge to manage the birdeye APIs.
     """
-    mock_response: bool = True
+    mock_response_public: bool = False
+    mock_response_private: bool = True
     mock_folder: str = "birdeye"
     api_key: str = ""
 
 class TestConfiguration(BaseModel):
     """
         Model in charge to manage the tests' configuration.
     """
@@ -49,86 +51,99 @@
         This function is used to load the test configuration file.
 
         It is strongly suggested to leave the default 'path' and 'file' 
         name for the test configuration file. However, if a dedicated file 
         is used, then is possible to load another file by providing the 
         necesary information in the input variables.
 
-        Args:
-
-        - path (str) [optional] : path of the configuration file. \\
-            By default is the same test folder 'tests'.
+        Parameters:
+            path: path of the configuration file.
+            file: name of the configuration file (with extension).
 
-        - file (str) [optional] : name of the configuration file (with extension). \\
-            By default is 'test.ini'.
+        Returns:
+            pydantic model of the test's configuration.
     """
     config_path_file = f"{path}/{file}"
     config = configparser.ConfigParser()
 
     # load config
     config.read(config_path_file)
     test_config = TestConfiguration()
     
     # global
     test_config.mock_response = config.getboolean("global", "mock_response", fallback = test_config.mock_response)
     test_config.mock_folder = config.get("global", "mock_folder", fallback = test_config.mock_folder)
 
     # birdeye
-    test_config.birdeye.mock_response = config.getboolean("birdeye", "mock_response", fallback = test_config.birdeye.mock_response)
+    test_config.birdeye.mock_response_public = config.getboolean("birdeye", "mock_response_public", fallback = test_config.birdeye.mock_response_public)
+    test_config.birdeye.mock_response_private = config.getboolean("birdeye", "mock_response_private", fallback = test_config.birdeye.mock_response_private)
     test_config.birdeye.mock_folder = config.get("birdeye", "mock_folder", fallback = test_config.birdeye.mock_folder)
     test_config.birdeye.api_key = config.get("birdeye", "api_key", fallback = test_config.birdeye.api_key)
 
     return test_config
 
-class TestMocker:
+class MockerManager:
     """
         Class used to manage the mock responses.
     """
 
     def __init__(self, mock_path: Path) -> None:
         # set/create resources folder
         self.mock_path = mock_path
         mock_path.mkdir(parents = True, exist_ok = True)
     
-    def load_mock_response(self, file_name: str, response_model: Type[ResponseModel]) -> ResponseModel:
+    def load_mock_model(self, file_name: str, response_model: Type[ResponseModel]) -> ResponseModel:
         """
             Use this function to load mock response model from a file.
 
-            Args:
-
-            - file_name (str) [mandatory] : file name containing the response to load.
-                By assumption, the file must be a JSON file and the file name should not contain the extension.
-
-            - response_model (Type[ResponseModel]) [mandatory] : objects that inherit from 
-                    pydantic.BaseModel and describe the response object element.
+            Parameters:
+                file_name: file name containing the response to load.
+                    By assumption, the file must be a JSON file and the file name should not contain the extension.
+                response_model: objects that inherit from `pydantic.BaseModel` and describe the response object element.
         """
         mock_file = f"{file_name}.json"
         mock_path_file = self.mock_path / mock_file
 
         if not mock_path_file.exists():
             raise Exception(f"mock file '{mock_file}' does not exist in '{self.mock_path}'.")
-        
+
         with open(mock_path_file, "r") as file:
             data = json.loads(file.read())
             mock_response = response_model(**data)
-        
+
         return mock_response
 
-    def store_mock_response(self, file_name: str, response: BaseModel) -> None:
+    def store_mock_model(self, file_name: str, response: BaseModel) -> None:
         """
             Use this function to store the mock response model into a file.
 
-            Args:
-
-            - file_name (str) [mandatory] : file name containing the response to load.
-                By assumption, the file must be a JSON file and the file name should not contain the extension.
-
-            - response (ResponseModel) [mandatory] : objects that inherit from 
-                    pydantic.BaseModel and describe the response object element.
+            Parameters:
+                file_name: file name containing the response to load.
+                    By assumption, the file must be a JSON file and the file name should not contain the extension.
+                response: objects that inherit from `pydantic.BaseModel` and describe the response object element.
         """
         mock_file = f"{file_name}.json"
         mock_path_file = self.mock_path / mock_file
 
         with open(mock_path_file, "w") as file:
             file.write(response.model_dump_json(indent = 4, by_alias = True))
-        
-        return
+
+        return
+
+    def load_mock_response(self, file_name: str, response_model: Type[ResponseModel]) -> Response:
+        """
+            Use this function to load mock response model from a file and return a dummy `Response` object.
+
+            Parameters:
+                file_name: file name containing the response to load.
+                    By assumption, the file must be a JSON file and the file name should not contain the extension.
+                response_model: objects that inherit from `pydantic.BaseModel` and describe the response object element.
+        """
+        mock_model = self.load_mock_model(file_name, response_model)
+
+        # create dummy response
+        mock_response = Response()
+        mock_response._content = mock_model.model_dump_json(by_alias = True).encode()
+        mock_response.status_code = 200
+        mock_response.encoding = "utf-8"
+
+        return mock_response
```

### Comparing `cyhole-0.0.1a0/tests/test_birdeye.py` & `cyhole-0.0.1a1/tests/test_birdeye.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,459 +17,497 @@
     GetHistoryResponse,
     GetTradesTokenResponse,
     GetTradesPairResponse,
     GetOHLCVTokenPairResponse,
     GetOHLCVBaseQuoteResponse,
     GetWalletSupportedNetworksResponse
 )
+from cyhole.birdeye.exception import BirdeyeAuthorisationError, BirdeyeTimeRangeError
 from cyhole.core.exception import MissingAPIKeyError
+from cyhole.core.address.solana import SOL, USDC
+from cyhole.core.address.ethereum import WETH
 
 # load test config
-from tests.config import load_config, TestMocker
+from .config import load_config, MockerManager
 config = load_config()
 
+# constant address
+TOM_SOL = "842NwDnKYcfMRWAYqsD3hoTWXKKMi28gVABtmaupFcnS"
+JRK = "JRKXwVpdyQbF3A4pvQvKYj22syubbEwfwUiobDzSPtJ"
+
 # create resources folder
 mock_path = Path(config.mock_folder) / config.birdeye.mock_folder
 mock_path.mkdir(parents = True, exist_ok = True)
 
+# set client, mocker
+_client = Birdeye(api_key = config.birdeye.api_key)
+_mocker = MockerManager(mock_path = Path(config.mock_folder) / config.birdeye.mock_folder)
+
 class TestBirdeyePublic:
     """
         Class grouping all unit test associate to PUBLIC endpoints
     """
-    mocker = TestMocker(
-        mock_path = Path(config.mock_folder) / config.birdeye.mock_folder
-    )
+    client = _client
+    mocker = _mocker
 
     def test_missing_api_key(self) -> None:
         """
             Unit Test to correcty identify a missing/wrong API Key
         """
         with pytest.raises(MissingAPIKeyError):
             Birdeye()
 
     def test_get_token_list(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - List".
 
             Mock Response File: get_token_list.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
-
+    
         # load mock response
         mock_file_name = "get_token_list"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_public:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenListResponse)
-            mocker.patch.object(client, "get_token_list", return_value = mock_response)
-            
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
+
         # execute request
-        response = client.get_token_list(limit = 1)
+        response = self.client.get_token_list(limit = 1)
 
         # actual test
-        assert isinstance(response, GetTokenListResponse)   
+        assert isinstance(response, GetTokenListResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_public:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_price(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Price".
 
             Mock Response File: get_price.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_price"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_public:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetPriceResponse)
-            mocker.patch.object(client, "get_price", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_price(address = "So11111111111111111111111111111111111111112")
+        response = self.client.get_price(address = SOL)
 
         # actual test
         assert isinstance(response, GetPriceResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_public:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_price_multiple(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Price - Multiple".
 
             Mock Response File: get_price_multiple.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_price_multiple"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_public:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetPriceMultipleResponse)
-            mocker.patch.object(client, "get_price_multiple", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        tokens_ca = ["So11111111111111111111111111111111111111112", "mSoLzYCxHdYgdzU16g5QSh3i5K3z3KZK7ytfqcJm7So"]
-        response = client.get_price_multiple(list_address = tokens_ca)
+        tokens_ca = [SOL, USDC]
+        response = self.client.get_price_multiple(list_address = tokens_ca)
 
         # actual test
         assert isinstance(response, GetPriceMultipleResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_public:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_price_historical(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Price - Historical".
 
             Mock Response File: get_price_historical.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_price_historical"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_public:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetPriceHistoricalResponse)
-            mocker.patch.object(client, "get_price_historical", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_price_historical(
-            address = "So11111111111111111111111111111111111111112",
+        response = self.client.get_price_historical(
+            address = SOL,
             address_type = BirdeyeAddressType.TOKEN.value,
             timeframe = BirdeyeTimeFrame.MIN15.value,
-            dt_from = datetime.now() - timedelta(hours = 1),
-            dt_to = datetime.now()
+            dt_from = datetime.now() - timedelta(hours = 1)
         )
 
         # actual test
         assert isinstance(response, GetPriceHistoricalResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_public:
+            self.mocker.store_mock_model(mock_file_name, response)
+
+    def test_get_price_historical_incorrect_input_dates(self, mocker: MockerFixture) -> None:
+        """
+            Unit Test used to check the incorrect dates inputs (dt_from > dt_to).
+        """
+
+        with pytest.raises(BirdeyeTimeRangeError):
+            # execute request
+            self.client.get_price_historical(
+                address = SOL,
+                address_type = BirdeyeAddressType.TOKEN.value,
+                timeframe = BirdeyeTimeFrame.MIN15.value,
+                dt_from = datetime.now() + timedelta(hours = 1)
+            )
 
     def test_get_history(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "History".
 
             Mock Response File: get_history.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_history"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_public:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetHistoryResponse)
-            mocker.patch.object(client, "get_history", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_history()
+        response = self.client.get_history()
 
         # actual test
         assert isinstance(response, GetHistoryResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_public:
+            self.mocker.store_mock_model(mock_file_name, response)
 
 class TestBirdeyePrivate:
     """
         Class grouping all unit test associate to PRIVATE endpoints
     """
-    mocker = TestMocker(
-        mock_path = Path(config.mock_folder) / config.birdeye.mock_folder
-    )
+    client = _client
+    mocker = _mocker
+
+    def test_not_authorised_api(self) -> None:
+        """
+            Unit Test to correcty identify a not Authorised API Key
+        """
+        client = Birdeye(api_key = "xxx-xxx-xxx")
+        with pytest.raises(BirdeyeAuthorisationError):
+            client.get_token_creation_info(address = SOL)
 
     def test_get_token_creation_info(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - Creation Token Info".
 
             Mock Response File: get_token_creation_info.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_token_creation_info"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenCreationInfoResponse)
-            mocker.patch.object(client, "get_token_creation_info", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_token_creation_info(address = "So11111111111111111111111111111111111111112")
+        response = self.client.get_token_creation_info(address = SOL)
 
         # actual test
         assert isinstance(response, GetTokenCreationInfoResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_token_security_solana(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - Security" specifically for Solana chain.
 
             Mock Response File: get_token_security_solana.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_token_security_solana"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenSecurityResponse)
-            mocker.patch.object(client, "get_token_security", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_token_security(
-            address = "JRKXwVpdyQbF3A4pvQvKYj22syubbEwfwUiobDzSPtJ"
-        )
+        response = self.client.get_token_security(JRK)
 
         # actual test
         assert isinstance(response, GetTokenSecurityResponse)
         assert isinstance(response.data, GetTokenSecurityDataSolana)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_token_security_other(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - Security" specifically for other chains.
 
             Mock Response File: get_token_security_other.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_token_security_other"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenSecurityResponse)
-            mocker.patch.object(client, "get_token_security", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_token_security(
-            address = "JRKXwVpdyQbF3A4pvQvKYj22syubbEwfwUiobDzSPtJ", 
+        response = self.client.get_token_security(
+            address = JRK, 
             chain = BirdeyeChain.ETHEREUM.value
         )
 
         # actual test
         assert isinstance(response, GetTokenSecurityResponse)
         assert isinstance(response.data, dict)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_token_overview_solana(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - Overview" specifically for Solana chain.
 
             Mock Response File: get_token_overview_solana.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
-        token_address = "So11111111111111111111111111111111111111112"
+        token_address = SOL
 
         # load mock response
         mock_file_name = "get_token_overview_solana"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenOverviewResponse)
-            mocker.patch.object(client, "get_token_overview", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_token_overview(token_address)
+        response = self.client.get_token_overview(token_address)
 
         # actual test
         assert isinstance(response, GetTokenOverviewResponse)
         assert response.data.address == token_address
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_token_overview_ethereum(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Token - Overview" specifically for Ethereum chain.
 
             Mock Response File: get_token_overview_ethereum.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
-        token_address = "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
+        token_address = WETH
 
         # load mock response
         mock_file_name = "get_token_overview_ethereum"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTokenOverviewResponse)
-            mocker.patch.object(client, "get_token_overview", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_token_overview(token_address, BirdeyeChain.ETHEREUM.value)
+        response = self.client.get_token_overview(token_address, BirdeyeChain.ETHEREUM.value)
 
         # actual test
         assert isinstance(response, GetTokenOverviewResponse)
         assert response.data.address == token_address
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_trades_token(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Trades - Token".
 
             Mock Response File: get_trades_token.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_trades_token"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTradesTokenResponse)
-            mocker.patch.object(client, "get_trades_token", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_trades_token(address = "SMMzJzseLTFb6pxacL8r5mZMEqjTTGWjNPk4q3JQHTu")
-
+        response = self.client.get_trades_token(SOL)
         # actual test
         assert isinstance(response, GetTradesTokenResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
     
     def test_get_trades_pair(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Trades - Pair".
 
             Mock Response File: get_trades_pair.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
-
         # load mock response
         mock_file_name = "get_trades_pair"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetTradesPairResponse)
-            mocker.patch.object(client, "get_trades_pair", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_trades_pair(address = "842NwDnKYcfMRWAYqsD3hoTWXKKMi28gVABtmaupFcnS")
+        response = self.client.get_trades_pair(address = TOM_SOL)
 
         # actual test
         assert isinstance(response, GetTradesPairResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
+
+    def test_get_ohlcv_incorrect_input_dates(self, mocker: MockerFixture) -> None:
+        """
+            Unit Test used to check the incorrect dates inputs (dt_from > dt_to).
+        """
+
+        with pytest.raises(BirdeyeTimeRangeError):
+            # execute request
+            self.client.get_ohlcv(
+                address = SOL,
+                address_type = BirdeyeAddressType.TOKEN.value,
+                timeframe = BirdeyeTimeFrame.MIN15.value,
+                dt_from = datetime.now() + timedelta(hours = 1)
+            )
 
     def test_get_ohlcv_token(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "OHLCV - Token".
 
             Mock Response File: get_ohlcv_token.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_ohlcv_token"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetOHLCVTokenPairResponse)
-            mocker.patch.object(client, "get_ohlcv", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_ohlcv(
-            address = "So11111111111111111111111111111111111111112",
+        response = self.client.get_ohlcv(
+            address = SOL,
             address_type = BirdeyeAddressType.TOKEN.value,
             timeframe = BirdeyeTimeFrame.MIN15.value,
             dt_from = datetime.now() - timedelta(hours = 1),
             dt_to = datetime.now()
         )
 
         # actual test
         assert isinstance(response, GetOHLCVTokenPairResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_ohlcv_pair(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "OHLCV - Pair".
 
             Mock Response File: get_ohlcv_pair.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_ohlcv_pair"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetOHLCVTokenPairResponse)
-            mocker.patch.object(client, "get_ohlcv", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_ohlcv(
-            address = "9wFFyRfZBsuAha4YcuxcXLKwMxJR43S7fPfQLusDBzvT",
+        response = self.client.get_ohlcv(
+            address = SOL,
             address_type = BirdeyeAddressType.PAIR.value,
             timeframe = BirdeyeTimeFrame.MIN15.value,
             dt_from = datetime.now() - timedelta(hours = 1),
             dt_to = datetime.now()
         )
 
         # actual test
         assert isinstance(response, GetOHLCVTokenPairResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
+
+    def test_get_ohlcv_base_quote_incorrect_input_dates(self, mocker: MockerFixture) -> None:
+        """
+            Unit Test used to check the incorrect dates inputs (dt_from > dt_to).
+        """
+
+        with pytest.raises(BirdeyeTimeRangeError):
+            # execute request
+            self.client.get_ohlcv_base_quote(
+                base_address = SOL,
+                quote_address = USDC,
+                timeframe = BirdeyeTimeFrame.MIN15.value,
+                dt_from = datetime.now() + timedelta(hours = 1)
+            )
 
     def test_get_ohlcv_base_quote(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "OHLCV - Base/Quote".
 
             Mock Response File: get_ohlcv_base_quote.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_ohlcv_base_quote"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetOHLCVBaseQuoteResponse)
-            mocker.patch.object(client, "get_ohlcv_base_quote", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_ohlcv_base_quote(
-            base_address = "So11111111111111111111111111111111111111112",
-            quote_address = "EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v",
+        response = self.client.get_ohlcv_base_quote(
+            base_address = SOL,
+            quote_address = USDC,
             timeframe = BirdeyeTimeFrame.MIN15.value,
             dt_from = datetime.now() - timedelta(hours = 1),
             dt_to = datetime.now()
         )
 
         # actual test
         assert isinstance(response, GetOHLCVBaseQuoteResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
 
     def test_get_wallet_supported_networks(self, mocker: MockerFixture) -> None:
         """
             Unit Test used to check the response schema of endpoint "Wallet - Supported Networks".
 
             Mock Response File: get_wallet_supported_networks.json
         """
-        client = Birdeye(api_key = config.birdeye.api_key)
 
         # load mock response
         mock_file_name = "get_wallet_supported_networks"
-        if config.birdeye.mock_response:
+        if config.mock_response or config.birdeye.mock_response_private:
             mock_response = self.mocker.load_mock_response(mock_file_name, GetWalletSupportedNetworksResponse)
-            mocker.patch.object(client, "get_wallet_supported_networks", return_value = mock_response)
+            mocker.patch("cyhole.core.api.APICaller.api", return_value = mock_response)
             
         # execute request
-        response = client.get_wallet_supported_networks()
+        response = self.client.get_wallet_supported_networks()
 
         # actual test
         assert isinstance(response, GetWalletSupportedNetworksResponse)
 
         # store request (only not mock)
-        if not config.birdeye.mock_response:
-            self.mocker.store_mock_response(mock_file_name, response)
+        if not config.birdeye.mock_response_private:
+            self.mocker.store_mock_model(mock_file_name, response)
```

### Comparing `cyhole-0.0.1a0/LICENSE` & `cyhole-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyhole-0.0.1a0/README.md` & `cyhole-0.0.1a1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,126 @@
 00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-00000020: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000030: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000040: 2f7a 617a 7a61 3132 332f 6379 686f 6c65  /zazza123/cyhole
-00000050: 2f6d 6169 6e2f 646f 6373 2f63 6f6e 6669  /main/docs/confi
-00000060: 672f 696d 6167 6573 2f6c 6f67 6f2e 706e  g/images/logo.pn
-00000070: 6722 2061 6c74 3d22 6379 686f 6c65 2220  g" alt="cyhole" 
-00000080: 636c 6173 733d 2269 6d67 2d6c 6f67 6f22  class="img-logo"
-00000090: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a2a 2a63  >.</p>..---..**c
-000000a0: 7968 6f6c 652a 2a20 6973 2064 6573 6967  yhole** is desig
-000000b0: 6e65 6420 746f 2068 656c 7020 7079 7468  ned to help pyth
-000000c0: 6f6e 2773 2064 6576 656c 6f70 6572 7320  on's developers 
-000000d0: 746f 2069 6e74 6572 6163 7420 746f 2074  to interact to t
-000000e0: 6865 206d 6f73 7420 706f 7075 6c61 7220  he most popular 
-000000f0: 6578 7465 726e 616c 2041 5049 2073 6572  external API ser
-00000100: 7669 6365 7320 696e 2063 7279 7074 6f20  vices in crypto 
-00000110: 776f 726c 6420 616e 6420 6372 6561 7465  world and create
-00000120: 2061 7574 6f6d 6174 696f 6e20 7072 6f63   automation proc
-00000130: 6573 7365 732e 0a0a 4561 6368 2065 7874  esses...Each ext
-00000140: 6572 6e61 6c20 4150 4920 696e 7465 6772  ernal API integr
-00000150: 6174 6564 2069 6e74 6f20 7468 6520 6c69  ated into the li
-00000160: 6272 6172 7920 6973 2072 6566 6572 7265  brary is referre
-00000170: 6420 746f 2061 7320 616e 202a 496e 7465  d to as an *Inte
-00000180: 7261 6374 696f 6e2a 2c20 7072 6f76 6964  raction*, provid
-00000190: 696e 6720 6465 7665 6c6f 7065 7273 2077  ing developers w
-000001a0: 6974 6820 6120 636f 6d70 7265 6865 6e73  ith a comprehens
-000001b0: 6976 6520 746f 6f6c 6b69 7420 666f 7220  ive toolkit for 
-000001c0: 7265 7472 6965 7669 6e67 2072 6561 6c2d  retrieving real-
-000001d0: 7469 6d65 206d 6172 6b65 7420 6461 7461  time market data
-000001e0: 2c20 6869 7374 6f72 6963 616c 2074 7265  , historical tre
-000001f0: 6e64 732c 2061 6363 6f75 6e74 2069 6e66  nds, account inf
-00000200: 6f72 6d61 7469 6f6e 2c20 616e 6420 6d6f  ormation, and mo
-00000210: 7265 2e0a 0a3c 753e 4b65 7920 4665 6174  re...<u>Key Feat
-00000220: 7572 6573 3c2f 753e 0a0a 2020 2d20 2a43  ures</u>..  - *C
-00000230: 656e 7472 616c 697a 6564 2041 6363 6573  entralized Acces
-00000240: 732a 3a20 6163 6365 7373 206d 756c 7469  s*: access multi
-00000250: 706c 6520 6372 7970 746f 6375 7272 656e  ple cryptocurren
-00000260: 6379 2041 5049 7320 7468 726f 7567 6820  cy APIs through 
-00000270: 6120 7369 6e67 6c65 2069 6e74 6572 6661  a single interfa
-00000280: 6365 2e0a 2020 2d20 2a43 6f6d 7072 6568  ce..  - *Compreh
-00000290: 656e 7369 7665 2043 6f76 6572 6167 652a  ensive Coverage*
-000002a0: 3a20 6578 706c 6f72 6520 6120 7769 6465  : explore a wide
-000002b0: 2072 616e 6765 206f 6620 6372 7970 746f   range of crypto
-000002c0: 6375 7272 656e 6379 2064 6174 612c 2069  currency data, i
-000002d0: 6e63 6c75 6469 6e67 206d 6172 6b65 7420  ncluding market 
-000002e0: 7072 6963 6573 2c20 7472 6164 696e 6720  prices, trading 
-000002f0: 766f 6c75 6d65 732c 2061 6e64 2062 6c6f  volumes, and blo
-00000300: 636b 6368 6169 6e20 7374 6174 6973 7469  ckchain statisti
-00000310: 6373 2e0a 2020 2d20 2a53 696d 706c 6966  cs..  - *Simplif
-00000320: 6965 6420 4465 7665 6c6f 706d 656e 742a  ied Development*
-00000330: 3a20 6163 6365 6c65 7261 7465 2074 6865  : accelerate the
-00000340: 2064 6576 656c 6f70 6d65 6e74 2070 726f   development pro
-00000350: 6365 7373 2062 7920 6c65 7665 7261 6769  cess by leveragi
-00000360: 6e67 2070 7265 2d62 7569 6c74 2041 5049  ng pre-built API
-00000370: 2069 6e74 6567 7261 7469 6f6e 732e 0a20   integrations.. 
-00000380: 202d 202a 466c 6578 6962 6c65 2049 6e74   - *Flexible Int
-00000390: 6567 7261 7469 6f6e 2a3a 2073 6561 6d6c  egration*: seaml
-000003a0: 6573 736c 7920 696e 636f 7270 6f72 6174  essly incorporat
-000003b0: 6520 6379 686f 6c65 2069 6e74 6f20 5079  e cyhole into Py
-000003c0: 7468 6f6e 2070 726f 6a65 6374 732c 2077  thon projects, w
-000003d0: 6865 7468 6572 2062 7569 6c64 696e 6720  hether building 
-000003e0: 6175 746f 6d61 7465 6420 7472 6164 696e  automated tradin
-000003f0: 6720 616c 676f 7269 7468 6d73 206f 7220  g algorithms or 
-00000400: 6d6f 6e69 746f 7269 6e67 2063 7279 7074  monitoring crypt
-00000410: 6f63 7572 7265 6e63 7920 706f 7274 666f  ocurrency portfo
-00000420: 6c69 6f73 2e0a 0a54 6865 2069 6e73 7461  lios...The insta
-00000430: 6c6c 6174 696f 6e20 6973 2070 6572 666f  llation is perfo
-00000440: 726d 6564 2076 6961 2060 7069 7060 2062  rmed via `pip` b
-00000450: 7920 7275 6e6e 696e 673a 0a0a 6060 6073  y running:..```s
-00000460: 680a 7069 7020 696e 7374 616c 6c20 6379  h.pip install cy
-00000470: 686f 6c65 0a60 6060 0a0a 2323 2049 6e74  hole.```..## Int
-00000480: 6572 6163 7469 6f6e 730a 0a49 6e20 2a2a  eractions..In **
-00000490: 6379 686f 6c65 2a2a 2c20 496e 7465 7261  cyhole**, Intera
-000004a0: 6374 696f 6e73 2073 6572 7665 2061 7320  ctions serve as 
-000004b0: 7468 6520 6675 6e64 616d 656e 7461 6c20  the fundamental 
-000004c0: 636f 6d70 6f6e 656e 7473 2c20 616b 696e  components, akin
-000004d0: 2074 6f20 7468 6520 6275 696c 6469 6e67   to the building
-000004e0: 2062 6c6f 636b 7320 6f66 2061 2073 6369   blocks of a sci
-000004f0: 656e 7469 6669 6320 6d6f 6465 6c2e 2045  entific model. E
-00000500: 6163 6820 696e 7465 7261 6374 696f 6e20  ach interaction 
-00000510: 7265 7072 6573 656e 7473 2061 2064 6973  represents a dis
-00000520: 7469 6e63 7420 6372 7970 746f 6375 7272  tinct cryptocurr
-00000530: 656e 6379 2041 5049 2c20 7072 6f76 6964  ency API, provid
-00000540: 696e 6720 6465 7665 6c6f 7065 7273 2077  ing developers w
-00000550: 6974 6820 6163 6365 7373 2074 6f20 6573  ith access to es
-00000560: 7365 6e74 6961 6c20 6461 7461 2061 6e64  sential data and
-00000570: 206d 6574 7269 6373 2e0a 0a54 6865 2063   metrics...The c
-00000580: 7572 7265 6e74 2073 7570 706f 7274 6564  urrent supported
-00000590: 2065 7874 6572 6e61 6c2f 696e 7465 7261   external/intera
-000005a0: 6374 696f 6e73 2041 5049 7320 6172 653a  ctions APIs are:
-000005b0: 0a0a 7c53 6974 6520 2020 2020 2020 2020  ..|Site         
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 2020 7c50 6174 6820 2020 2020 2020      |Path       
-000005e0: 2020 2020 2020 7c43 6f6e 6e65 6374 6f72        |Connector
-000005f0: 7c0a 7c2d 2d2d 2d20 2020 2020 2020 2020  |.|----         
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 2020 7c2d 2d2d 2d20 2020 2020 2020      |----       
-00000620: 2020 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d        |---------
-00000630: 7c0a 7c5b 6269 7264 6579 652e 736f 5d28  |.|[birdeye.so](
-00000640: 6874 7470 733a 2f2f 6269 7264 6579 652e  https://birdeye.
-00000650: 736f 2920 7c60 6379 686f 6c65 2e62 6972  so) |`cyhole.bir
-00000660: 6465 7965 6020 7c60 4269 7264 6579 6560  deye` |`Birdeye`
-00000670: 7c0a                                     |.
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000020: 7470 733a 2f2f 7a61 7a7a 6131 3233 2e67  tps://zazza123.g
+00000030: 6974 6875 622e 696f 2f63 7968 6f6c 6522  ithub.io/cyhole"
+00000040: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000050: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00000060: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000070: 6d2f 7a61 7a7a 6131 3233 2f63 7968 6f6c  m/zazza123/cyhol
+00000080: 652f 6d61 696e 2f64 6f63 732f 636f 6e66  e/main/docs/conf
+00000090: 6967 2f69 6d61 6765 732f 6c6f 676f 2e70  ig/images/logo.p
+000000a0: 6e67 2220 616c 743d 2263 7968 6f6c 6522  ng" alt="cyhole"
+000000b0: 2068 6569 6768 743d 2231 3530 7078 2220   height="150px" 
+000000c0: 636c 6173 733d 2269 6d67 2d6c 6f67 6f22  class="img-logo"
+000000d0: 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a 3c70  >.  </a>.</p>.<p
+000000e0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000000f0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000100: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000110: 6a65 6374 2f63 7968 6f6c 6522 3e3c 696d  ject/cyhole"><im
+00000120: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000130: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000140: 7069 2f76 2f63 7968 6f6c 653f 636f 6c6f  pi/v/cyhole?colo
+00000150: 723d 2532 3333 3444 3035 3826 6c61 6265  r=%2334D058&labe
+00000160: 6c3d 7079 7069 2532 3070 6163 6b61 6765  l=pypi%20package
+00000170: 2220 616c 743d 2250 7950 4920 7665 7273  " alt="PyPI vers
+00000180: 696f 6e22 2068 6569 6768 743d 2231 3822  ion" height="18"
+00000190: 3e3c 2f61 3e0a 3c2f 703e 0a0a 0a2d 2d2d  ></a>.</p>...---
+000001a0: 0a0a 2a2a 6379 686f 6c65 2a2a 2069 7320  ..**cyhole** is 
+000001b0: 6465 7369 676e 6564 2074 6f20 6865 6c70  designed to help
+000001c0: 2070 7974 686f 6e27 7320 6465 7665 6c6f   python's develo
+000001d0: 7065 7273 2074 6f20 696e 7465 7261 6374  pers to interact
+000001e0: 2074 6f20 7468 6520 6d6f 7374 2070 6f70   to the most pop
+000001f0: 756c 6172 2065 7874 6572 6e61 6c20 4150  ular external AP
+00000200: 4920 7365 7276 6963 6573 2069 6e20 6372  I services in cr
+00000210: 7970 746f 2077 6f72 6c64 2061 6e64 2063  ypto world and c
+00000220: 7265 6174 6520 6175 746f 6d61 7469 6f6e  reate automation
+00000230: 2070 726f 6365 7373 6573 2e0a 0a45 6163   processes...Eac
+00000240: 6820 6578 7465 726e 616c 2041 5049 2069  h external API i
+00000250: 6e74 6567 7261 7465 6420 696e 746f 2074  ntegrated into t
+00000260: 6865 206c 6962 7261 7279 2069 7320 7265  he library is re
+00000270: 6665 7272 6564 2074 6f20 6173 2061 6e20  ferred to as an 
+00000280: 2a49 6e74 6572 6163 7469 6f6e 2a2c 2070  *Interaction*, p
+00000290: 726f 7669 6469 6e67 2064 6576 656c 6f70  roviding develop
+000002a0: 6572 7320 7769 7468 2061 2063 6f6d 7072  ers with a compr
+000002b0: 6568 656e 7369 7665 2074 6f6f 6c6b 6974  ehensive toolkit
+000002c0: 2066 6f72 2072 6574 7269 6576 696e 6720   for retrieving 
+000002d0: 7265 616c 2d74 696d 6520 6d61 726b 6574  real-time market
+000002e0: 2064 6174 612c 2068 6973 746f 7269 6361   data, historica
+000002f0: 6c20 7472 656e 6473 2c20 6163 636f 756e  l trends, accoun
+00000300: 7420 696e 666f 726d 6174 696f 6e2c 2061  t information, a
+00000310: 6e64 206d 6f72 652e 0a0a 3c75 3e4b 6579  nd more...<u>Key
+00000320: 2046 6561 7475 7265 733c 2f75 3e0a 0a20   Features</u>.. 
+00000330: 202d 202a 4365 6e74 7261 6c69 7a65 6420   - *Centralized 
+00000340: 4163 6365 7373 2a3a 2061 6363 6573 7320  Access*: access 
+00000350: 6d75 6c74 6970 6c65 2063 7279 7074 6f63  multiple cryptoc
+00000360: 7572 7265 6e63 7920 4150 4973 2074 6872  urrency APIs thr
+00000370: 6f75 6768 2061 2073 696e 676c 6520 696e  ough a single in
+00000380: 7465 7266 6163 652e 0a20 202d 202a 436f  terface..  - *Co
+00000390: 6d70 7265 6865 6e73 6976 6520 436f 7665  mprehensive Cove
+000003a0: 7261 6765 2a3a 2065 7870 6c6f 7265 2061  rage*: explore a
+000003b0: 2077 6964 6520 7261 6e67 6520 6f66 2063   wide range of c
+000003c0: 7279 7074 6f63 7572 7265 6e63 7920 6461  ryptocurrency da
+000003d0: 7461 2c20 696e 636c 7564 696e 6720 6d61  ta, including ma
+000003e0: 726b 6574 2070 7269 6365 732c 2074 7261  rket prices, tra
+000003f0: 6469 6e67 2076 6f6c 756d 6573 2c20 616e  ding volumes, an
+00000400: 6420 626c 6f63 6b63 6861 696e 2073 7461  d blockchain sta
+00000410: 7469 7374 6963 732e 0a20 202d 202a 5369  tistics..  - *Si
+00000420: 6d70 6c69 6669 6564 2044 6576 656c 6f70  mplified Develop
+00000430: 6d65 6e74 2a3a 2061 6363 656c 6572 6174  ment*: accelerat
+00000440: 6520 7468 6520 6465 7665 6c6f 706d 656e  e the developmen
+00000450: 7420 7072 6f63 6573 7320 6279 206c 6576  t process by lev
+00000460: 6572 6167 696e 6720 7072 652d 6275 696c  eraging pre-buil
+00000470: 7420 4150 4920 696e 7465 6772 6174 696f  t API integratio
+00000480: 6e73 2e0a 2020 2d20 2a46 6c65 7869 626c  ns..  - *Flexibl
+00000490: 6520 496e 7465 6772 6174 696f 6e2a 3a20  e Integration*: 
+000004a0: 7365 616d 6c65 7373 6c79 2069 6e63 6f72  seamlessly incor
+000004b0: 706f 7261 7465 2063 7968 6f6c 6520 696e  porate cyhole in
+000004c0: 746f 2050 7974 686f 6e20 7072 6f6a 6563  to Python projec
+000004d0: 7473 2c20 7768 6574 6865 7220 6275 696c  ts, whether buil
+000004e0: 6469 6e67 2061 7574 6f6d 6174 6564 2074  ding automated t
+000004f0: 7261 6469 6e67 2061 6c67 6f72 6974 686d  rading algorithm
+00000500: 7320 6f72 206d 6f6e 6974 6f72 696e 6720  s or monitoring 
+00000510: 6372 7970 746f 6375 7272 656e 6379 2070  cryptocurrency p
+00000520: 6f72 7466 6f6c 696f 732e 0a0a 5468 6520  ortfolios...The 
+00000530: 696e 7374 616c 6c61 7469 6f6e 2069 7320  installation is 
+00000540: 7065 7266 6f72 6d65 6420 7669 6120 6070  performed via `p
+00000550: 6970 6020 6279 2072 756e 6e69 6e67 3a0a  ip` by running:.
+00000560: 0a60 6060 7368 0a70 6970 2069 6e73 7461  .```sh.pip insta
+00000570: 6c6c 2063 7968 6f6c 650a 6060 600a 0a2d  ll cyhole.```..-
+00000580: 2d2d 0a0a 2a2a 446f 6375 6d65 6e74 6174  --..**Documentat
+00000590: 696f 6e2a 2a3a 205b 6874 7470 733a 2f2f  ion**: [https://
+000005a0: 7a61 7a7a 6131 3233 2e67 6974 6875 622e  zazza123.github.
+000005b0: 696f 2f63 7968 6f6c 655d 2868 7474 7073  io/cyhole](https
+000005c0: 3a2f 2f7a 617a 7a61 3132 332e 6769 7468  ://zazza123.gith
+000005d0: 7562 2e69 6f2f 6379 686f 6c65 290a 0a23  ub.io/cyhole)..#
+000005e0: 2320 496e 7465 7261 6374 696f 6e73 0a0a  # Interactions..
+000005f0: 496e 202a 2a63 7968 6f6c 652a 2a2c 2049  In **cyhole**, I
+00000600: 6e74 6572 6163 7469 6f6e 7320 7365 7276  nteractions serv
+00000610: 6520 6173 2074 6865 2066 756e 6461 6d65  e as the fundame
+00000620: 6e74 616c 2063 6f6d 706f 6e65 6e74 732c  ntal components,
+00000630: 2061 6b69 6e20 746f 2074 6865 2062 7569   akin to the bui
+00000640: 6c64 696e 6720 626c 6f63 6b73 206f 6620  lding blocks of 
+00000650: 6120 7363 6965 6e74 6966 6963 206d 6f64  a scientific mod
+00000660: 656c 2e20 4561 6368 2069 6e74 6572 6163  el. Each interac
+00000670: 7469 6f6e 2072 6570 7265 7365 6e74 7320  tion represents 
+00000680: 6120 6469 7374 696e 6374 2063 7279 7074  a distinct crypt
+00000690: 6f63 7572 7265 6e63 7920 4150 492c 2070  ocurrency API, p
+000006a0: 726f 7669 6469 6e67 2064 6576 656c 6f70  roviding develop
+000006b0: 6572 7320 7769 7468 2061 6363 6573 7320  ers with access 
+000006c0: 746f 2065 7373 656e 7469 616c 2064 6174  to essential dat
+000006d0: 6120 616e 6420 6d65 7472 6963 732e 0a0a  a and metrics...
+000006e0: 5468 6520 6375 7272 656e 7420 7375 7070  The current supp
+000006f0: 6f72 7465 6420 6578 7465 726e 616c 2f69  orted external/i
+00000700: 6e74 6572 6163 7469 6f6e 7320 4150 4973  nteractions APIs
+00000710: 2061 7265 3a0a 0a7c 5369 7465 2020 2020   are:..|Site    
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 2020 2020 2020 2020 207c 5061 7468 2020           |Path  
+00000740: 2020 2020 2020 2020 2020 207c 436f 6e6e             |Conn
+00000750: 6563 746f 727c 0a7c 2d2d 2d2d 2020 2020  ector|.|----    
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 2020 2020 2020 2020 207c 2d2d 2d2d 2020           |----  
+00000780: 2020 2020 2020 2020 2020 207c 2d2d 2d2d             |----
+00000790: 2d2d 2d2d 2d7c 0a7c 5b62 6972 6465 7965  -----|.|[birdeye
+000007a0: 2e73 6f5d 2868 7474 7073 3a2f 2f62 6972  .so](https://bir
+000007b0: 6465 7965 2e73 6f29 207c 6063 7968 6f6c  deye.so) |`cyhol
+000007c0: 652e 6269 7264 6579 6560 207c 6042 6972  e.birdeye` |`Bir
+000007d0: 6465 7965 607c 0a                        deye`|.
```

### Comparing `cyhole-0.0.1a0/pyproject.toml` & `cyhole-0.0.1a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cyhole"
-version = "0.0.1-alpha"
+version = "0.0.1-alpha-1"
 description = "cyhole, designed to help python's developers to interact to the most popular external API services in crypto and create automation processes."
 readme = "README.md"
 requires-python = ">=3.12"
 authors = [
     { name = "Andrea Zanini", email= "" },
 ]
 classifiers = [
@@ -20,16 +20,30 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Financial and Insurance Industry"
 ]
+dependencies = [
+    "requests>=2.31.0",
+    "pydantic>=2.7.0"
+]
 
 [project.urls]
 Homepage = "https://github.com/zazza123/cyhole"
 Repository = "https://github.com/zazza123/cyhole"
+Documentation = "https://zazza123.github.io/cyhole"
 
 [tool.pytest.ini_options]
 addopts = [
-    "--import-mode=importlib",
+    "--import-mode=importlib"
+]
+
+[tool.coverage.run]
+source = [
+    "src"
+]
+context = '${CONTEXT}'
+omit = [
+    "tests/config.py"
 ]
```

### Comparing `cyhole-0.0.1a0/PKG-INFO` & `cyhole-0.0.1a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 6379 686f  : 2.3.Name: cyho
 00000020: 6c65 0a56 6572 7369 6f6e 3a20 302e 302e  le.Version: 0.0.
-00000030: 3161 300a 5375 6d6d 6172 793a 2063 7968  1a0.Summary: cyh
+00000030: 3161 310a 5375 6d6d 6172 793a 2063 7968  1a1.Summary: cyh
 00000040: 6f6c 652c 2064 6573 6967 6e65 6420 746f  ole, designed to
 00000050: 2068 656c 7020 7079 7468 6f6e 2773 2064   help python's d
 00000060: 6576 656c 6f70 6572 7320 746f 2069 6e74  evelopers to int
 00000070: 6572 6163 7420 746f 2074 6865 206d 6f73  eract to the mos
 00000080: 7420 706f 7075 6c61 7220 6578 7465 726e  t popular extern
 00000090: 616c 2041 5049 2073 6572 7669 6365 7320  al API services 
 000000a0: 696e 2063 7279 7074 6f20 616e 6420 6372  in crypto and cr
@@ -14,151 +14,181 @@
 000000d0: 6374 2d55 524c 3a20 486f 6d65 7061 6765  ct-URL: Homepage
 000000e0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
 000000f0: 2e63 6f6d 2f7a 617a 7a61 3132 332f 6379  .com/zazza123/cy
 00000100: 686f 6c65 0a50 726f 6a65 6374 2d55 524c  hole.Project-URL
 00000110: 3a20 5265 706f 7369 746f 7279 2c20 6874  : Repository, ht
 00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000130: 2f7a 617a 7a61 3132 332f 6379 686f 6c65  /zazza123/cyhole
-00000140: 0a41 7574 686f 723a 2041 6e64 7265 6120  .Author: Andrea 
-00000150: 5a61 6e69 6e69 0a4c 6963 656e 7365 2d46  Zanini.License-F
-00000160: 696c 653a 204c 4943 454e 5345 0a43 6c61  ile: LICENSE.Cla
-00000170: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
-00000180: 6d65 6e74 2053 7461 7475 7320 3a3a 2031  ment Status :: 1
-00000190: 202d 2050 6c61 6e6e 696e 670a 436c 6173   - Planning.Clas
-000001a0: 7369 6669 6572 3a20 456e 7669 726f 6e6d  sifier: Environm
-000001b0: 656e 7420 3a3a 2057 6562 2045 6e76 6972  ent :: Web Envir
-000001c0: 6f6e 6d65 6e74 0a43 6c61 7373 6966 6965  onment.Classifie
-000001d0: 723a 2046 7261 6d65 776f 726b 203a 3a20  r: Framework :: 
-000001e0: 5079 6461 6e74 6963 0a43 6c61 7373 6966  Pydantic.Classif
-000001f0: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000200: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000210: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
-00000220: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-00000230: 6365 203a 3a20 4669 6e61 6e63 6961 6c20  ce :: Financial 
-00000240: 616e 6420 496e 7375 7261 6e63 6520 496e  and Insurance In
-00000250: 6475 7374 7279 0a43 6c61 7373 6966 6965  dustry.Classifie
-00000260: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000270: 656e 6365 203a 3a20 496e 666f 726d 6174  ence :: Informat
-00000280: 696f 6e20 5465 6368 6e6f 6c6f 6779 0a43  ion Technology.C
-00000290: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-000002a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000002b0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000002c0: 650a 436c 6173 7369 6669 6572 3a20 4f70  e.Classifier: Op
-000002d0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000002e0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000002f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000310: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
-00000320: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000330: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000340: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
-00000350: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000360: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000370: 5079 7468 6f6e 203a 3a20 332e 3132 0a52  Python :: 3.12.R
-00000380: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00000390: 3e3d 332e 3132 0a44 6573 6372 6970 7469  >=3.12.Descripti
-000003a0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003b0: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-000003c0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000003d0: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
-000003e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000003f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000400: 2f7a 617a 7a61 3132 332f 6379 686f 6c65  /zazza123/cyhole
-00000410: 2f6d 6169 6e2f 646f 6373 2f63 6f6e 6669  /main/docs/confi
-00000420: 672f 696d 6167 6573 2f6c 6f67 6f2e 706e  g/images/logo.pn
-00000430: 6722 2061 6c74 3d22 6379 686f 6c65 2220  g" alt="cyhole" 
-00000440: 636c 6173 733d 2269 6d67 2d6c 6f67 6f22  class="img-logo"
-00000450: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a2a 2a63  >.</p>..---..**c
-00000460: 7968 6f6c 652a 2a20 6973 2064 6573 6967  yhole** is desig
-00000470: 6e65 6420 746f 2068 656c 7020 7079 7468  ned to help pyth
-00000480: 6f6e 2773 2064 6576 656c 6f70 6572 7320  on's developers 
-00000490: 746f 2069 6e74 6572 6163 7420 746f 2074  to interact to t
-000004a0: 6865 206d 6f73 7420 706f 7075 6c61 7220  he most popular 
-000004b0: 6578 7465 726e 616c 2041 5049 2073 6572  external API ser
-000004c0: 7669 6365 7320 696e 2063 7279 7074 6f20  vices in crypto 
-000004d0: 776f 726c 6420 616e 6420 6372 6561 7465  world and create
-000004e0: 2061 7574 6f6d 6174 696f 6e20 7072 6f63   automation proc
-000004f0: 6573 7365 732e 0a0a 4561 6368 2065 7874  esses...Each ext
-00000500: 6572 6e61 6c20 4150 4920 696e 7465 6772  ernal API integr
-00000510: 6174 6564 2069 6e74 6f20 7468 6520 6c69  ated into the li
-00000520: 6272 6172 7920 6973 2072 6566 6572 7265  brary is referre
-00000530: 6420 746f 2061 7320 616e 202a 496e 7465  d to as an *Inte
-00000540: 7261 6374 696f 6e2a 2c20 7072 6f76 6964  raction*, provid
-00000550: 696e 6720 6465 7665 6c6f 7065 7273 2077  ing developers w
-00000560: 6974 6820 6120 636f 6d70 7265 6865 6e73  ith a comprehens
-00000570: 6976 6520 746f 6f6c 6b69 7420 666f 7220  ive toolkit for 
-00000580: 7265 7472 6965 7669 6e67 2072 6561 6c2d  retrieving real-
-00000590: 7469 6d65 206d 6172 6b65 7420 6461 7461  time market data
-000005a0: 2c20 6869 7374 6f72 6963 616c 2074 7265  , historical tre
-000005b0: 6e64 732c 2061 6363 6f75 6e74 2069 6e66  nds, account inf
-000005c0: 6f72 6d61 7469 6f6e 2c20 616e 6420 6d6f  ormation, and mo
-000005d0: 7265 2e0a 0a3c 753e 4b65 7920 4665 6174  re...<u>Key Feat
-000005e0: 7572 6573 3c2f 753e 0a0a 2020 2d20 2a43  ures</u>..  - *C
-000005f0: 656e 7472 616c 697a 6564 2041 6363 6573  entralized Acces
-00000600: 732a 3a20 6163 6365 7373 206d 756c 7469  s*: access multi
-00000610: 706c 6520 6372 7970 746f 6375 7272 656e  ple cryptocurren
-00000620: 6379 2041 5049 7320 7468 726f 7567 6820  cy APIs through 
-00000630: 6120 7369 6e67 6c65 2069 6e74 6572 6661  a single interfa
-00000640: 6365 2e0a 2020 2d20 2a43 6f6d 7072 6568  ce..  - *Compreh
-00000650: 656e 7369 7665 2043 6f76 6572 6167 652a  ensive Coverage*
-00000660: 3a20 6578 706c 6f72 6520 6120 7769 6465  : explore a wide
-00000670: 2072 616e 6765 206f 6620 6372 7970 746f   range of crypto
-00000680: 6375 7272 656e 6379 2064 6174 612c 2069  currency data, i
-00000690: 6e63 6c75 6469 6e67 206d 6172 6b65 7420  ncluding market 
-000006a0: 7072 6963 6573 2c20 7472 6164 696e 6720  prices, trading 
-000006b0: 766f 6c75 6d65 732c 2061 6e64 2062 6c6f  volumes, and blo
-000006c0: 636b 6368 6169 6e20 7374 6174 6973 7469  ckchain statisti
-000006d0: 6373 2e0a 2020 2d20 2a53 696d 706c 6966  cs..  - *Simplif
-000006e0: 6965 6420 4465 7665 6c6f 706d 656e 742a  ied Development*
-000006f0: 3a20 6163 6365 6c65 7261 7465 2074 6865  : accelerate the
-00000700: 2064 6576 656c 6f70 6d65 6e74 2070 726f   development pro
-00000710: 6365 7373 2062 7920 6c65 7665 7261 6769  cess by leveragi
-00000720: 6e67 2070 7265 2d62 7569 6c74 2041 5049  ng pre-built API
-00000730: 2069 6e74 6567 7261 7469 6f6e 732e 0a20   integrations.. 
-00000740: 202d 202a 466c 6578 6962 6c65 2049 6e74   - *Flexible Int
-00000750: 6567 7261 7469 6f6e 2a3a 2073 6561 6d6c  egration*: seaml
-00000760: 6573 736c 7920 696e 636f 7270 6f72 6174  essly incorporat
-00000770: 6520 6379 686f 6c65 2069 6e74 6f20 5079  e cyhole into Py
-00000780: 7468 6f6e 2070 726f 6a65 6374 732c 2077  thon projects, w
-00000790: 6865 7468 6572 2062 7569 6c64 696e 6720  hether building 
-000007a0: 6175 746f 6d61 7465 6420 7472 6164 696e  automated tradin
-000007b0: 6720 616c 676f 7269 7468 6d73 206f 7220  g algorithms or 
-000007c0: 6d6f 6e69 746f 7269 6e67 2063 7279 7074  monitoring crypt
-000007d0: 6f63 7572 7265 6e63 7920 706f 7274 666f  ocurrency portfo
-000007e0: 6c69 6f73 2e0a 0a54 6865 2069 6e73 7461  lios...The insta
-000007f0: 6c6c 6174 696f 6e20 6973 2070 6572 666f  llation is perfo
-00000800: 726d 6564 2076 6961 2060 7069 7060 2062  rmed via `pip` b
-00000810: 7920 7275 6e6e 696e 673a 0a0a 6060 6073  y running:..```s
-00000820: 680a 7069 7020 696e 7374 616c 6c20 6379  h.pip install cy
-00000830: 686f 6c65 0a60 6060 0a0a 2323 2049 6e74  hole.```..## Int
-00000840: 6572 6163 7469 6f6e 730a 0a49 6e20 2a2a  eractions..In **
-00000850: 6379 686f 6c65 2a2a 2c20 496e 7465 7261  cyhole**, Intera
-00000860: 6374 696f 6e73 2073 6572 7665 2061 7320  ctions serve as 
-00000870: 7468 6520 6675 6e64 616d 656e 7461 6c20  the fundamental 
-00000880: 636f 6d70 6f6e 656e 7473 2c20 616b 696e  components, akin
-00000890: 2074 6f20 7468 6520 6275 696c 6469 6e67   to the building
-000008a0: 2062 6c6f 636b 7320 6f66 2061 2073 6369   blocks of a sci
-000008b0: 656e 7469 6669 6320 6d6f 6465 6c2e 2045  entific model. E
-000008c0: 6163 6820 696e 7465 7261 6374 696f 6e20  ach interaction 
-000008d0: 7265 7072 6573 656e 7473 2061 2064 6973  represents a dis
-000008e0: 7469 6e63 7420 6372 7970 746f 6375 7272  tinct cryptocurr
-000008f0: 656e 6379 2041 5049 2c20 7072 6f76 6964  ency API, provid
-00000900: 696e 6720 6465 7665 6c6f 7065 7273 2077  ing developers w
-00000910: 6974 6820 6163 6365 7373 2074 6f20 6573  ith access to es
-00000920: 7365 6e74 6961 6c20 6461 7461 2061 6e64  sential data and
-00000930: 206d 6574 7269 6373 2e0a 0a54 6865 2063   metrics...The c
-00000940: 7572 7265 6e74 2073 7570 706f 7274 6564  urrent supported
-00000950: 2065 7874 6572 6e61 6c2f 696e 7465 7261   external/intera
-00000960: 6374 696f 6e73 2041 5049 7320 6172 653a  ctions APIs are:
-00000970: 0a0a 7c53 6974 6520 2020 2020 2020 2020  ..|Site         
-00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000990: 2020 2020 7c50 6174 6820 2020 2020 2020      |Path       
-000009a0: 2020 2020 2020 7c43 6f6e 6e65 6374 6f72        |Connector
-000009b0: 7c0a 7c2d 2d2d 2d20 2020 2020 2020 2020  |.|----         
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 2020 7c2d 2d2d 2d20 2020 2020 2020      |----       
-000009e0: 2020 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d        |---------
-000009f0: 7c0a 7c5b 6269 7264 6579 652e 736f 5d28  |.|[birdeye.so](
-00000a00: 6874 7470 733a 2f2f 6269 7264 6579 652e  https://birdeye.
-00000a10: 736f 2920 7c60 6379 686f 6c65 2e62 6972  so) |`cyhole.bir
-00000a20: 6465 7965 6020 7c60 4269 7264 6579 6560  deye` |`Birdeye`
-00000a30: 7c0a                                     |.
+00000140: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+00000150: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+00000160: 7073 3a2f 2f7a 617a 7a61 3132 332e 6769  ps://zazza123.gi
+00000170: 7468 7562 2e69 6f2f 6379 686f 6c65 0a41  thub.io/cyhole.A
+00000180: 7574 686f 723a 2041 6e64 7265 6120 5a61  uthor: Andrea Za
+00000190: 6e69 6e69 0a4c 6963 656e 7365 2d46 696c  nini.License-Fil
+000001a0: 653a 204c 4943 454e 5345 0a43 6c61 7373  e: LICENSE.Class
+000001b0: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+000001c0: 6e74 2053 7461 7475 7320 3a3a 2031 202d  nt Status :: 1 -
+000001d0: 2050 6c61 6e6e 696e 670a 436c 6173 7369   Planning.Classi
+000001e0: 6669 6572 3a20 456e 7669 726f 6e6d 656e  fier: Environmen
+000001f0: 7420 3a3a 2057 6562 2045 6e76 6972 6f6e  t :: Web Environ
+00000200: 6d65 6e74 0a43 6c61 7373 6966 6965 723a  ment.Classifier:
+00000210: 2046 7261 6d65 776f 726b 203a 3a20 5079   Framework :: Py
+00000220: 6461 6e74 6963 0a43 6c61 7373 6966 6965  dantic.Classifie
+00000230: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000240: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000250: 7273 0a43 6c61 7373 6966 6965 723a 2049  rs.Classifier: I
+00000260: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000270: 203a 3a20 4669 6e61 6e63 6961 6c20 616e   :: Financial an
+00000280: 6420 496e 7375 7261 6e63 6520 496e 6475  d Insurance Indu
+00000290: 7374 7279 0a43 6c61 7373 6966 6965 723a  stry.Classifier:
+000002a0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
+000002b0: 6365 203a 3a20 496e 666f 726d 6174 696f  ce :: Informatio
+000002c0: 6e20 5465 6368 6e6f 6c6f 6779 0a43 6c61  n Technology.Cla
+000002d0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+000002e0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000002f0: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+00000300: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000310: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000320: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+00000330: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000350: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00000360: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000380: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003b0: 7468 6f6e 203a 3a20 332e 3132 0a52 6571  thon :: 3.12.Req
+000003c0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000003d0: 332e 3132 0a52 6571 7569 7265 732d 4469  3.12.Requires-Di
+000003e0: 7374 3a20 7079 6461 6e74 6963 3e3d 322e  st: pydantic>=2.
+000003f0: 372e 300a 5265 7175 6972 6573 2d44 6973  7.0.Requires-Dis
+00000400: 743a 2072 6571 7565 7374 733e 3d32 2e33  t: requests>=2.3
+00000410: 312e 300a 4465 7363 7269 7074 696f 6e2d  1.0.Description-
+00000420: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000430: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 7020  xt/markdown..<p 
+00000440: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000450: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000460: 3a2f 2f7a 617a 7a61 3132 332e 6769 7468  ://zazza123.gith
+00000470: 7562 2e69 6f2f 6379 686f 6c65 223e 0a20  ub.io/cyhole">. 
+00000480: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000490: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000004a0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f7a  sercontent.com/z
+000004b0: 617a 7a61 3132 332f 6379 686f 6c65 2f6d  azza123/cyhole/m
+000004c0: 6169 6e2f 646f 6373 2f63 6f6e 6669 672f  ain/docs/config/
+000004d0: 696d 6167 6573 2f6c 6f67 6f2e 706e 6722  images/logo.png"
+000004e0: 2061 6c74 3d22 6379 686f 6c65 2220 6865   alt="cyhole" he
+000004f0: 6967 6874 3d22 3135 3070 7822 2063 6c61  ight="150px" cla
+00000500: 7373 3d22 696d 672d 6c6f 676f 223e 0a20  ss="img-logo">. 
+00000510: 203c 2f61 3e0a 3c2f 703e 0a3c 7020 616c   </a>.</p>.<p al
+00000520: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000530: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000540: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000550: 742f 6379 686f 6c65 223e 3c69 6d67 2073  t/cyhole"><img s
+00000560: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000570: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000580: 762f 6379 686f 6c65 3f63 6f6c 6f72 3d25  v/cyhole?color=%
+00000590: 3233 3334 4430 3538 266c 6162 656c 3d70  2334D058&label=p
+000005a0: 7970 6925 3230 7061 636b 6167 6522 2061  ypi%20package" a
+000005b0: 6c74 3d22 5079 5049 2076 6572 7369 6f6e  lt="PyPI version
+000005c0: 2220 6865 6967 6874 3d22 3138 223e 3c2f  " height="18"></
+000005d0: 613e 0a3c 2f70 3e0a 0a0a 2d2d 2d0a 0a2a  a>.</p>...---..*
+000005e0: 2a63 7968 6f6c 652a 2a20 6973 2064 6573  *cyhole** is des
+000005f0: 6967 6e65 6420 746f 2068 656c 7020 7079  igned to help py
+00000600: 7468 6f6e 2773 2064 6576 656c 6f70 6572  thon's developer
+00000610: 7320 746f 2069 6e74 6572 6163 7420 746f  s to interact to
+00000620: 2074 6865 206d 6f73 7420 706f 7075 6c61   the most popula
+00000630: 7220 6578 7465 726e 616c 2041 5049 2073  r external API s
+00000640: 6572 7669 6365 7320 696e 2063 7279 7074  ervices in crypt
+00000650: 6f20 776f 726c 6420 616e 6420 6372 6561  o world and crea
+00000660: 7465 2061 7574 6f6d 6174 696f 6e20 7072  te automation pr
+00000670: 6f63 6573 7365 732e 0a0a 4561 6368 2065  ocesses...Each e
+00000680: 7874 6572 6e61 6c20 4150 4920 696e 7465  xternal API inte
+00000690: 6772 6174 6564 2069 6e74 6f20 7468 6520  grated into the 
+000006a0: 6c69 6272 6172 7920 6973 2072 6566 6572  library is refer
+000006b0: 7265 6420 746f 2061 7320 616e 202a 496e  red to as an *In
+000006c0: 7465 7261 6374 696f 6e2a 2c20 7072 6f76  teraction*, prov
+000006d0: 6964 696e 6720 6465 7665 6c6f 7065 7273  iding developers
+000006e0: 2077 6974 6820 6120 636f 6d70 7265 6865   with a comprehe
+000006f0: 6e73 6976 6520 746f 6f6c 6b69 7420 666f  nsive toolkit fo
+00000700: 7220 7265 7472 6965 7669 6e67 2072 6561  r retrieving rea
+00000710: 6c2d 7469 6d65 206d 6172 6b65 7420 6461  l-time market da
+00000720: 7461 2c20 6869 7374 6f72 6963 616c 2074  ta, historical t
+00000730: 7265 6e64 732c 2061 6363 6f75 6e74 2069  rends, account i
+00000740: 6e66 6f72 6d61 7469 6f6e 2c20 616e 6420  nformation, and 
+00000750: 6d6f 7265 2e0a 0a3c 753e 4b65 7920 4665  more...<u>Key Fe
+00000760: 6174 7572 6573 3c2f 753e 0a0a 2020 2d20  atures</u>..  - 
+00000770: 2a43 656e 7472 616c 697a 6564 2041 6363  *Centralized Acc
+00000780: 6573 732a 3a20 6163 6365 7373 206d 756c  ess*: access mul
+00000790: 7469 706c 6520 6372 7970 746f 6375 7272  tiple cryptocurr
+000007a0: 656e 6379 2041 5049 7320 7468 726f 7567  ency APIs throug
+000007b0: 6820 6120 7369 6e67 6c65 2069 6e74 6572  h a single inter
+000007c0: 6661 6365 2e0a 2020 2d20 2a43 6f6d 7072  face..  - *Compr
+000007d0: 6568 656e 7369 7665 2043 6f76 6572 6167  ehensive Coverag
+000007e0: 652a 3a20 6578 706c 6f72 6520 6120 7769  e*: explore a wi
+000007f0: 6465 2072 616e 6765 206f 6620 6372 7970  de range of cryp
+00000800: 746f 6375 7272 656e 6379 2064 6174 612c  tocurrency data,
+00000810: 2069 6e63 6c75 6469 6e67 206d 6172 6b65   including marke
+00000820: 7420 7072 6963 6573 2c20 7472 6164 696e  t prices, tradin
+00000830: 6720 766f 6c75 6d65 732c 2061 6e64 2062  g volumes, and b
+00000840: 6c6f 636b 6368 6169 6e20 7374 6174 6973  lockchain statis
+00000850: 7469 6373 2e0a 2020 2d20 2a53 696d 706c  tics..  - *Simpl
+00000860: 6966 6965 6420 4465 7665 6c6f 706d 656e  ified Developmen
+00000870: 742a 3a20 6163 6365 6c65 7261 7465 2074  t*: accelerate t
+00000880: 6865 2064 6576 656c 6f70 6d65 6e74 2070  he development p
+00000890: 726f 6365 7373 2062 7920 6c65 7665 7261  rocess by levera
+000008a0: 6769 6e67 2070 7265 2d62 7569 6c74 2041  ging pre-built A
+000008b0: 5049 2069 6e74 6567 7261 7469 6f6e 732e  PI integrations.
+000008c0: 0a20 202d 202a 466c 6578 6962 6c65 2049  .  - *Flexible I
+000008d0: 6e74 6567 7261 7469 6f6e 2a3a 2073 6561  ntegration*: sea
+000008e0: 6d6c 6573 736c 7920 696e 636f 7270 6f72  mlessly incorpor
+000008f0: 6174 6520 6379 686f 6c65 2069 6e74 6f20  ate cyhole into 
+00000900: 5079 7468 6f6e 2070 726f 6a65 6374 732c  Python projects,
+00000910: 2077 6865 7468 6572 2062 7569 6c64 696e   whether buildin
+00000920: 6720 6175 746f 6d61 7465 6420 7472 6164  g automated trad
+00000930: 696e 6720 616c 676f 7269 7468 6d73 206f  ing algorithms o
+00000940: 7220 6d6f 6e69 746f 7269 6e67 2063 7279  r monitoring cry
+00000950: 7074 6f63 7572 7265 6e63 7920 706f 7274  ptocurrency port
+00000960: 666f 6c69 6f73 2e0a 0a54 6865 2069 6e73  folios...The ins
+00000970: 7461 6c6c 6174 696f 6e20 6973 2070 6572  tallation is per
+00000980: 666f 726d 6564 2076 6961 2060 7069 7060  formed via `pip`
+00000990: 2062 7920 7275 6e6e 696e 673a 0a0a 6060   by running:..``
+000009a0: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
+000009b0: 6379 686f 6c65 0a60 6060 0a0a 2d2d 2d0a  cyhole.```..---.
+000009c0: 0a2a 2a44 6f63 756d 656e 7461 7469 6f6e  .**Documentation
+000009d0: 2a2a 3a20 5b68 7474 7073 3a2f 2f7a 617a  **: [https://zaz
+000009e0: 7a61 3132 332e 6769 7468 7562 2e69 6f2f  za123.github.io/
+000009f0: 6379 686f 6c65 5d28 6874 7470 733a 2f2f  cyhole](https://
+00000a00: 7a61 7a7a 6131 3233 2e67 6974 6875 622e  zazza123.github.
+00000a10: 696f 2f63 7968 6f6c 6529 0a0a 2323 2049  io/cyhole)..## I
+00000a20: 6e74 6572 6163 7469 6f6e 730a 0a49 6e20  nteractions..In 
+00000a30: 2a2a 6379 686f 6c65 2a2a 2c20 496e 7465  **cyhole**, Inte
+00000a40: 7261 6374 696f 6e73 2073 6572 7665 2061  ractions serve a
+00000a50: 7320 7468 6520 6675 6e64 616d 656e 7461  s the fundamenta
+00000a60: 6c20 636f 6d70 6f6e 656e 7473 2c20 616b  l components, ak
+00000a70: 696e 2074 6f20 7468 6520 6275 696c 6469  in to the buildi
+00000a80: 6e67 2062 6c6f 636b 7320 6f66 2061 2073  ng blocks of a s
+00000a90: 6369 656e 7469 6669 6320 6d6f 6465 6c2e  cientific model.
+00000aa0: 2045 6163 6820 696e 7465 7261 6374 696f   Each interactio
+00000ab0: 6e20 7265 7072 6573 656e 7473 2061 2064  n represents a d
+00000ac0: 6973 7469 6e63 7420 6372 7970 746f 6375  istinct cryptocu
+00000ad0: 7272 656e 6379 2041 5049 2c20 7072 6f76  rrency API, prov
+00000ae0: 6964 696e 6720 6465 7665 6c6f 7065 7273  iding developers
+00000af0: 2077 6974 6820 6163 6365 7373 2074 6f20   with access to 
+00000b00: 6573 7365 6e74 6961 6c20 6461 7461 2061  essential data a
+00000b10: 6e64 206d 6574 7269 6373 2e0a 0a54 6865  nd metrics...The
+00000b20: 2063 7572 7265 6e74 2073 7570 706f 7274   current support
+00000b30: 6564 2065 7874 6572 6e61 6c2f 696e 7465  ed external/inte
+00000b40: 7261 6374 696f 6e73 2041 5049 7320 6172  ractions APIs ar
+00000b50: 653a 0a0a 7c53 6974 6520 2020 2020 2020  e:..|Site       
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 2020 2020 2020 7c50 6174 6820 2020 2020        |Path     
+00000b80: 2020 2020 2020 2020 7c43 6f6e 6e65 6374          |Connect
+00000b90: 6f72 7c0a 7c2d 2d2d 2d20 2020 2020 2020  or|.|----       
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2020 2020 7c2d 2d2d 2d20 2020 2020        |----     
+00000bc0: 2020 2020 2020 2020 7c2d 2d2d 2d2d 2d2d          |-------
+00000bd0: 2d2d 7c0a 7c5b 6269 7264 6579 652e 736f  --|.|[birdeye.so
+00000be0: 5d28 6874 7470 733a 2f2f 6269 7264 6579  ](https://birdey
+00000bf0: 652e 736f 2920 7c60 6379 686f 6c65 2e62  e.so) |`cyhole.b
+00000c00: 6972 6465 7965 6020 7c60 4269 7264 6579  irdeye` |`Birdey
+00000c10: 6560 7c0a                                e`|.
```

