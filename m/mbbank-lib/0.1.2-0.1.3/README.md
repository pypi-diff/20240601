# Comparing `tmp/mbbank-lib-0.1.2.tar.gz` & `tmp/mbbank_lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank-lib-0.1.2.tar", last modified: Tue Mar 26 15:11:22 2024, max compression
+gzip compressed data, was "mbbank_lib-0.1.3.tar", last modified: Sat Jun  1 06:45:25 2024, max compression
```

## Comparing `mbbank-lib-0.1.2.tar` & `mbbank_lib-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:11:22.965321 mbbank-lib-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 15:11:16.000000 mbbank-lib-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-26 15:11:22.965321 mbbank-lib-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:11:22.965321 mbbank-lib-0.1.2/mbbank/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 15:11:16.000000 mbbank-lib-0.1.2/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-03-26 15:11:16.000000 mbbank-lib-0.1.2/mbbank/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-26 15:11:16.000000 mbbank-lib-0.1.2/mbbank/mbasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:11:22.965321 mbbank-lib-0.1.2/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-26 15:11:22.000000 mbbank-lib-0.1.2/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-26 15:11:22.000000 mbbank-lib-0.1.2/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 15:11:22.000000 mbbank-lib-0.1.2/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 15:11:22.000000 mbbank-lib-0.1.2/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 15:11:22.000000 mbbank-lib-0.1.2/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 15:11:22.965321 mbbank-lib-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-26 15:11:16.000000 mbbank-lib-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/mbasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/setup.py
```

### Comparing `mbbank-lib-0.1.2/LICENSE.txt` & `mbbank_lib-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank-lib-0.1.2/PKG-INFO` & `mbbank_lib-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.1.2
+Version: 0.1.3
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: Pillow
```

### Comparing `mbbank-lib-0.1.2/mbbank/main.py` & `mbbank_lib-0.1.3/mbbank/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,15 +21,33 @@
 
 def get_now_time():
     now = datetime.datetime.now()
     microsecond = int(now.strftime("%f")[:2])
     return now.strftime(f"%Y%m%d%H%M{microsecond}")
 
 
+class MBBankError(Exception):
+    def __init__(self, err_out):
+        self.code = err_out['responseCode']
+        self.message = err_out['message']
+        super().__init__(f"{err_out['responseCode']} | {err_out['message']}")
+
+
 class MBBank:
+    """Core class
+
+    Attributes:
+        deviceIdCommon (str): Device id common
+        sessionId (str or None): Current Session id
+
+    Args:
+        username (str): MBBank Account Username
+        password (str): MBBank Account Password
+        tesseract_path (str, optional): Tesseract path. Defaults to None.
+    """
     deviceIdCommon = f'i1vzyjp5-mbib-0000-0000-{get_now_time()}'
 
     def __init__(self, *, username, password, tesseract_path=None):
         self.__userid = username
         self.__password = password
         if tesseract_path is not None:
             pytesseract.pytesseract.tesseract_cmd = tesseract_path
@@ -40,15 +58,15 @@
     def _req(self, url, *, json=None, headers=None):
         if headers is None:
             headers = {}
         if json is None:
             json = {}
         while True:
             if self.sessionId is None:
-                self.authenticate()
+                self._authenticate()
             rid = f"{self.__userid}-{get_now_time()}"
             json_data = {
                 'sessionId': self.sessionId if self.sessionId is not None else "",
                 'refNo': rid,
                 'deviceIdCommon': self.deviceIdCommon,
             }
             json_data.update(json)
@@ -61,21 +79,21 @@
                     data_out = r.json()
             if data_out["result"] is None:
                 self.getBalance()
             elif data_out["result"]["ok"]:
                 data_out.pop("result", None)
                 break
             elif data_out["result"]["responseCode"] == "GW200":
-                self.authenticate()
+                self._authenticate()
             else:
                 err_out = data_out["result"]
-                raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
+                raise MBBankError(err_out)
         return data_out
 
-    def authenticate(self):
+    def _authenticate(self):
         while True:
             self._userinfo = None
             self.sessionId = None
             self._temp = {}
             rid = f"{self.__userid}-{get_now_time()}"
             json_data = {
                 'sessionId': "",
@@ -118,74 +136,188 @@
                 return
             elif data_out["result"]["responseCode"] == "GW283":
                 pass
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
 
-    def getTransactionAccountHistory(self, *, accountNo:str=None, from_date: datetime.datetime, to_date: datetime.datetime):
+    def getTransactionAccountHistory(self, *, accountNo: str = None, from_date: datetime.datetime,
+                                     to_date: datetime.datetime):
+        """
+        Get account transaction history
+
+        Args:
+            accountNo (str, optional): Sub account number Defaults to Main Account number.
+            from_date (datetime.datetime): transaction from date
+            to_date (datetime.datetime): transaction to date
+
+        Returns:
+            success (dict): account transaction history
+
+        Raises:
+            MBBankError: if api response not ok
+        """
+        if self._userinfo is None:
+            self._authenticate()
+        if accountNo is None:
+            accountNo = self._userinfo["result"]["data"]["accountNo"]
         json_data = {
             'accountNo': self.__userid if accountNo is None else accountNo,
             'fromDate': from_date.strftime("%d/%m/%Y"),
             'toDate': to_date.strftime("%d/%m/%Y"),  # max 3 months
         }
         data_out = self._req(
             "https://online.mbbank.com.vn/api/retail-transactionms/transactionms/get-account-transaction-history",
             json=json_data)
         return data_out
 
     def getBalance(self):
+        """
+        Get all main account and sub account balance
+
+        Returns:
+            success (dict): list account balance
+
+        Raises:
+            MBBankError: if api response not ok
+        """
+        if self._userinfo is None:
+            self._authenticate()
         data_out = self._req("https://online.mbbank.com.vn/api/retail-web-accountms/getBalance")
         return data_out
 
     def getBalanceLoyalty(self):
+        """
+        Get Account loyalty rank and Member loyalty point
+
+        Returns:
+            success (dict): loyalty point
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/loyalty/getBalanceLoyalty")
         return data_out
 
     def getInterestRate(self, currency: str = "VND"):
+        """
+        Get saving interest rate
+
+        Args:
+            currency (str, optional): currency ISO 4217 format. Defaults to "VND" (Viet Nam Dong).
+
+        Returns:
+            success (dict): interest rate
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
             "productCode": "TIENGUI.KHN.EMB",
             "currency": currency,
         }
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/saving/getInterestRate", json=json_data)
         return data_out
 
     def getFavorBeneficiaryList(self, *, transactionType: typing.Literal["TRANSFER", "PAYMENT"],
                                 searchType: typing.Literal["MOST", "LATEST"]):
+        """
+        Get all favor or most transfer beneficiary list from your account
+
+        Args:
+            transactionType (Literal["TRANSFER", "PAYMENT"]): transaction type
+            searchType (Literal["MOST", "LATEST"]): search type
+
+        Returns:
+            success (dict): favor beneficiary list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
             "transactionType": transactionType,
             "searchType": searchType
         }
         data_out = self._req(
             "https://online.mbbank.com.vn/api/retail_web/internetbanking/getFavorBeneficiaryList", json=json_data)
         return data_out
 
     def getCardList(self):
+        """
+        Get all card list from your account
+
+        Returns:
+            success (dict): card list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/card/getList")
         return data_out
 
     def getSavingList(self):
+        """
+        Get all saving list from your account
+
+        Returns:
+            success (dict): saving list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/saving/getList")
         return data_out
 
     def getLoanList(self):
+        """
+        Get all loan list from your account
+
+        Returns:
+            success (dict): loan list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/loan/getList")
         return data_out
 
-    def getCardTransactionHistory(self, cardNo:str, from_date: datetime.datetime, to_date: datetime.datetime):
+    def getCardTransactionHistory(self, cardNo: str, from_date: datetime.datetime, to_date: datetime.datetime):
+        """
+        Get card transaction history
+
+        Args:
+            cardNo (str): card number get from getCardList
+            from_date (datetime.datetime): from date
+            to_date (datetime.datetime): to date
+
+        Returns:
+            success (dict): card transaction history
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
-          "accountNo": cardNo,
-          "fromDate": from_date.strftime("%d/%m/%Y"),
-          "toDate": to_date.strftime("%d/%m/%Y"),  # max 3 months
-          "historyNumber": "",
-          "historyType": "DATE_RANGE",
-          "type": "CARD",
+            "accountNo": cardNo,
+            "fromDate": from_date.strftime("%d/%m/%Y"),
+            "toDate": to_date.strftime("%d/%m/%Y"),  # max 3 months
+            "historyNumber": "",
+            "historyType": "DATE_RANGE",
+            "type": "CARD",
         }
         data_out = self._req("https://online.mbbank.com.vn/api/retail_web/common/getTransactionHistory", json=json_data)
         return data_out
 
     def userinfo(self):
+        """
+        Get current user info
+
+        Returns:
+            success (dict): user info
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         if self._userinfo is None:
-            self.authenticate()
+            self._authenticate()
         else:
             self.getBalance()
         return self._userinfo
```

### Comparing `mbbank-lib-0.1.2/mbbank/mbasync.py` & `mbbank_lib-0.1.3/mbbank/mbasync.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 import base64
 import hashlib
 import typing
 import io
 import platform
 import aiohttp
+from .main import MBBankError
 
 headers_default = {
     'Cache-Control': 'no-cache',
     'Accept': 'application/json, text/plain, */*',
     'Authorization': 'Basic RU1CUkVUQUlMV0VCOlNEMjM0ZGZnMzQlI0BGR0AzNHNmc2RmNDU4NDNm',
     'User-Agent': f'Mozilla/5.0 (X11; {platform.system()} {platform.processor()})',
     "Origin": "https://online.mbbank.com.vn",
@@ -22,29 +23,40 @@
 def get_now_time():
     now = datetime.datetime.now()
     microsecond = int(now.strftime("%f")[:2])
     return now.strftime(f"%Y%m%d%H%M{microsecond}")
 
 
 class MBBankAsync:
+    """Core Async class
+
+    Attributes:
+        deviceIdCommon (str): Device id common
+        sessionId (str or None): Current Session id
+
+    Args:
+        username (str): MBBank Account Username
+        password (str): MBBank Account Password
+        tesseract_path (str, optional): Tesseract path. Defaults to None.
+    """
     deviceIdCommon = f'i1vzyjp5-mbib-0000-0000-{get_now_time()}'
 
     def __init__(self, *, username, password, tesseract_path=None):
         self.__userid = username
         self.__password = password
         if tesseract_path is not None:
             pytesseract.pytesseract.tesseract_cmd = tesseract_path
         self.sessionId = None
         self._userinfo = None
         self._temp = {}
 
     async def _req(self, url, *, json={}, headers={}):
         while True:
             if self.sessionId is None:
-                await self.authenticate()
+                await self._authenticate()
             rid = f"{self.__userid}-{get_now_time()}"
             json_data = {
                 'sessionId': self.sessionId if self.sessionId is not None else "",
                 'refNo': rid,
                 'deviceIdCommon': self.deviceIdCommon,
             }
             json_data.update(json)
@@ -57,21 +69,21 @@
                     data_out = await r.json()
             if data_out["result"] is None:
                 await self.getBalance()
             elif data_out["result"]["ok"]:
                 data_out.pop("result", None)
                 break
             elif data_out["result"]["responseCode"] == "GW200":
-                await self.authenticate()
+                await self._authenticate()
             else:
                 err_out = data_out["result"]
-                raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
+                raise MBBankError(err_out)
         return data_out
 
-    async def authenticate(self):
+    async def _authenticate(self):
         while True:
             self._userinfo = None
             self.sessionId = None
             self._temp = {}
             rid = f"{self.__userid}-{get_now_time()}"
             json_data = {
                 'sessionId': "",
@@ -116,69 +128,191 @@
                 pass
             else:
                 err_out = data_out["result"]
                 raise Exception(f"{err_out['responseCode']} | {err_out['message']}")
 
     async def getTransactionAccountHistory(self, *, accountNo: str = None, from_date: datetime.datetime,
                                            to_date: datetime.datetime):
+        """
+        Get account transaction history
+
+        Args:
+            accountNo (str, optional): Sub account number Defaults to Main Account number.
+            from_date (datetime.datetime): transaction from date
+            to_date (datetime.datetime): transaction to date
+
+        Returns:
+            success (dict): account transaction history
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
             'accountNo': self.__userid if accountNo is None else accountNo,
             'fromDate': from_date.strftime("%d/%m/%Y"),
             'toDate': to_date.strftime("%d/%m/%Y"),  # max 3 months
         }
         data_out = await self._req(
             "https://online.mbbank.com.vn/api/retail-transactionms/transactionms/get-account-transaction-history",
             json=json_data)
         return data_out
 
     async def getBalance(self):
+        """
+        Get all main account and sub account balance
+
+        Returns:
+            success (dict): list account balance
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = await self._req("https://online.mbbank.com.vn/api/retail-web-accountms/getBalance")
         return data_out
 
     async def getBalanceLoyalty(self):
+        """
+        Get Account loyalty rank and Member loyalty point
+
+        Returns:
+            success (dict): loyalty point
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/loyalty/getBalanceLoyalty")
         return data_out
 
     async def getInterestRate(self, currency: str = "VND"):
+        """
+        Get saving interest rate
+
+        Args:
+            currency (str, optional): currency ISO 4217 format. Defaults to "VND" (Viet Nam Dong).
+
+        Returns:
+            success (dict): interest rate
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
             "productCode": "TIENGUI.KHN.EMB",
-            "currency": currency,
+            "currency": currency
         }
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/saving/getInterestRate", json=json_data)
         return data_out
 
     async def getFavorBeneficiaryList(self, *, transactionType: typing.Literal["TRANSFER", "PAYMENT"],
                                       searchType: typing.Literal["MOST", "LATEST"]):
+        """
+        Get all favor or most transfer beneficiary list from your account
+
+        Args:
+            transactionType (Literal["TRANSFER", "PAYMENT"]): transaction type
+            searchType (Literal["MOST", "LATEST"]): search type
+
+        Returns:
+            success (dict): favor beneficiary list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         json_data = {
             "transactionType": transactionType,
             "searchType": searchType
         }
         data_out = await self._req(
             "https://online.mbbank.com.vn/api/retail_web/internetbanking/getFavorBeneficiaryList", json=json_data)
         return data_out
 
     async def getCardList(self):
+        """
+        Get all card list from your account
+
+        Returns:
+            success (dict): card list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/card/getList")
         return data_out
 
     async def getSavingList(self):
+        """
+        Get all saving list from your account
+
+        Returns:
+            success (dict): saving list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/saving/getList")
         return data_out
 
     async def getLoanList(self):
+        """
+        Get all loan list from your account
+
+        Returns:
+            success (dict): loan list
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/loan/getList")
         return data_out
 
+    async def getCardTransactionHistory(self, cardNo: str, from_date: datetime.datetime, to_date: datetime.datetime):
+        """
+        Get card transaction history
+
+        Args:
+            cardNo (str): card number get from getCardList
+            from_date (datetime.datetime): from date
+            to_date (datetime.datetime): to date
+
+        Returns:
+            success (dict): card transaction history
+
+        Raises:
+            MBBankError: if api response not ok
+        """
+        json_data = {
+            "accountNo": cardNo,
+            "fromDate": from_date.strftime("%d/%m/%Y"),
+            "toDate": to_date.strftime("%d/%m/%Y"),  # max 3 months
+            "historyNumber": "",
+            "historyType": "DATE_RANGE",
+            "type": "CARD",
+        }
+        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/common/getTransactionHistory",
+                                   json=json_data)
+        return data_out
+
     async def userinfo(self):
+        """
+        Get current user info
+
+        Returns:
+            success (dict): user info
+
+        Raises:
+            MBBankError: if api response not ok
+        """
         if self._userinfo is None:
-            await self.authenticate()
+            await self._authenticate()
         else:
             await self.getBalance()
         return self._userinfo
 
+    # working on beta
+
     async def getBankList(self):
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/common/getBankList")
         return data_out
 
     async def inquiryAccountName(self, *, typeTransfer: str = None, debitAccount: str, bankCode: str = None,
                                  creditAccount: str, creditAccountType: typing.Literal["ACCOUNT", "CARD"]):
         creditCardNo = None
@@ -234,20 +368,7 @@
     async def getAccountByPhone(self, phone: str):
         json_data = {
             "phone": phone
         }
         data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/common/getAccountByPhone",
                                    json=json_data)
         return data_out
-
-    async def getCardTransactionHistory(self, cardNo: str, from_date: datetime.datetime, to_date: datetime.datetime):
-        json_data = {
-            "accountNo": cardNo,
-            "fromDate": from_date.strftime("%d/%m/%Y"),
-            "toDate": to_date.strftime("%d/%m/%Y"),  # max 3 months
-            "historyNumber": "",
-            "historyType": "DATE_RANGE",
-            "type": "CARD",
-        }
-        data_out = await self._req("https://online.mbbank.com.vn/api/retail_web/common/getTransactionHistory",
-                                   json=json_data)
-        return data_out
```

### Comparing `mbbank-lib-0.1.2/mbbank_lib.egg-info/PKG-INFO` & `mbbank_lib-0.1.3/mbbank_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbbank-lib
-Version: 0.1.2
+Version: 0.1.3
 Summary: A unofficially light weight Python Api for the "Military Commercial Joint Stock Bank" accounts
 Home-page: https://github.com/thedtvn/MBBank
 Author: The DT
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: Pillow
```

### Comparing `mbbank-lib-0.1.2/setup.py` & `mbbank_lib-0.1.3/setup.py`

 * *Files identical despite different names*

