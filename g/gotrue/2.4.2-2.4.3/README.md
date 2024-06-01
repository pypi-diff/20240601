# Comparing `tmp/gotrue-2.4.2.tar.gz` & `tmp/gotrue-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrue-2.4.2.tar", max compression
+gzip compressed data, was "gotrue-2.4.3.tar", max compression
```

## Comparing `gotrue-2.4.2.tar` & `gotrue-2.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1065 2023-08-23 17:46:45.779051 gotrue-2.4.2/LICENSE
--rw-r--r--   0        0        0     5155 2024-03-26 11:23:49.849634 gotrue-2.4.2/README.md
--rw-r--r--   0        0        0      751 2024-03-26 11:23:49.851106 gotrue-2.4.2/gotrue/__init__.py
--rw-r--r--   0        0        0       35 2024-03-26 11:23:49.851224 gotrue-2.4.2/gotrue/_async/__init__.py
--rw-r--r--   0        0        0     5549 2024-03-26 11:23:49.851381 gotrue-2.4.2/gotrue/_async/gotrue_admin_api.py
--rw-r--r--   0        0        0      947 2024-03-26 11:23:49.851491 gotrue-2.4.2/gotrue/_async/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3735 2024-03-26 11:23:49.851709 gotrue-2.4.2/gotrue/_async/gotrue_base_api.py
--rw-r--r--   0        0        0    36273 2024-03-26 11:23:49.851872 gotrue-2.4.2/gotrue/_async/gotrue_client.py
--rw-r--r--   0        0        0     3956 2024-03-26 11:23:49.851961 gotrue-2.4.2/gotrue/_async/gotrue_mfa_api.py
--rw-r--r--   0        0        0      925 2024-03-26 11:23:49.852030 gotrue-2.4.2/gotrue/_async/storage.py
--rw-r--r--   0        0        0       35 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/__init__.py
--rw-r--r--   0        0        0    19216 2024-03-26 11:23:49.000000 gotrue-2.4.2/gotrue/_sync/api.py
--rw-r--r--   0        0        0    22195 2024-03-26 11:23:49.000000 gotrue-2.4.2/gotrue/_sync/client.py
--rw-r--r--   0        0        0     5421 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/gotrue_admin_api.py
--rw-r--r--   0        0        0      934 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/gotrue_admin_mfa_api.py
--rw-r--r--   0        0        0     3669 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/gotrue_base_api.py
--rw-r--r--   0        0        0    35599 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/gotrue_client.py
--rw-r--r--   0        0        0     3913 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/gotrue_mfa_api.py
--rw-r--r--   0        0        0      886 2024-03-26 11:31:15.000000 gotrue-2.4.2/gotrue/_sync/storage.py
--rw-r--r--   0        0        0      329 2024-03-26 11:23:49.853222 gotrue-2.4.2/gotrue/constants.py
--rw-r--r--   0        0        0     2893 2024-03-26 11:23:49.853294 gotrue-2.4.2/gotrue/errors.py
--rw-r--r--   0        0        0     5189 2024-03-26 11:23:49.853376 gotrue-2.4.2/gotrue/helpers.py
--rw-r--r--   0        0        0      202 2024-03-26 11:23:49.853441 gotrue-2.4.2/gotrue/http_clients.py
--rw-r--r--   0        0        0     1366 2024-03-26 11:23:49.853501 gotrue-2.4.2/gotrue/timer.py
--rw-r--r--   0        0        0    16819 2024-03-26 11:23:49.853623 gotrue-2.4.2/gotrue/types.py
--rw-r--r--   0        0        0     1565 2024-03-26 11:30:41.690903 gotrue-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 gotrue-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-06-01 20:07:39.799145 gotrue-2.4.3/LICENSE
+-rw-r--r--   0        0        0     5120 2024-06-01 20:07:39.871145 gotrue-2.4.3/README.md
+-rw-r--r--   0        0        0      751 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/__init__.py
+-rw-r--r--   0        0        0     5645 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/gotrue_admin_api.py
+-rw-r--r--   0        0        0      947 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3759 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/gotrue_base_api.py
+-rw-r--r--   0        0        0    36329 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/gotrue_client.py
+-rw-r--r--   0        0        0     3956 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      901 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_async/storage.py
+-rw-r--r--   0        0        0       35 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/__init__.py
+-rw-r--r--   0        0        0    19288 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/api.py
+-rw-r--r--   0        0        0    22345 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/client.py
+-rw-r--r--   0        0        0     5517 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/gotrue_admin_api.py
+-rw-r--r--   0        0        0      934 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/gotrue_admin_mfa_api.py
+-rw-r--r--   0        0        0     3693 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/gotrue_base_api.py
+-rw-r--r--   0        0        0    35611 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/gotrue_client.py
+-rw-r--r--   0        0        0     3913 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/gotrue_mfa_api.py
+-rw-r--r--   0        0        0      862 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/_sync/storage.py
+-rw-r--r--   0        0        0      329 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/constants.py
+-rw-r--r--   0        0        0     2893 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/errors.py
+-rw-r--r--   0        0        0     5193 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/helpers.py
+-rw-r--r--   0        0        0      202 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/http_clients.py
+-rw-r--r--   0        0        0     1366 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/timer.py
+-rw-r--r--   0        0        0    16819 2024-06-01 20:07:39.803145 gotrue-2.4.3/gotrue/types.py
+-rw-r--r--   0        0        0     1565 2024-06-01 20:07:39.871145 gotrue-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 gotrue-2.4.3/PKG-INFO
```

### Comparing `gotrue-2.4.2/LICENSE` & `gotrue-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/README.md` & `gotrue-2.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 [![Github Watchers](https://img.shields.io/github/watchers/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py)
 [![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/graphs/contributors)
 
 This is a Python port of the [supabase js gotrue client](https://github.com/supabase/gotrue-js). The current state is that there is a features parity but with small differences that are mentioned in the section **Differences to the JS client**. As of December 14th, we renamed to repo from `gotrue-py` to `auth-py` to mirror the changes in the JavaScript library.
 
 ## Installation
 
-We are still working on making the `supabase_auth` python library more user-friendly. For now here are some sparse notes on how to install the module.
+We are still working on making the `gotrue` python library more user-friendly. For now here are some sparse notes on how to install the module.
 
 ### Poetry
 
 ```bash
-poetry add supabase_auth
+poetry add gotrue
 ```
 
 ### Pip
 
 ```bash
-pip install supabase_auth
+pip install gotrue
 ```
 
 ## Differences to the JS client
 
 It should be noted there are differences to the [JS client](https://github.com/supabase/gotrue-js). If you feel particulaly strongly about them and want to motivate a change, feel free to make a GitHub issue and we can discuss it there.
 
 Firstly, feature pairity is not 100% with the [JS client](https://github.com/supabase/gotrue-js). In most cases we match the methods and attributes of the [JS client](https://github.com/supabase/gotrue-js) and api classes, but is some places (e.g for browser specific code) it didn't make sense to port the code line for line.
@@ -42,24 +42,24 @@
 
 ```js
 const { data, error } = client.sign_up(...)
 ```
 
 The other key difference is we do not use pascalCase to encode variable and method names. Instead we use the snake_case convention adopted in the Python language.
 
-Also, the `supabase_auth` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.
+Also, the `gotrue` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.
 
 ## Usage (outdated)
 
 **Important:** This section is outdated, you can be guided by the [JS client documentation](https://supabase.github.io/gotrue-js) because this Python client has a lot of parity with the JS client.
 
 To instantiate the client, you'll need the URL and any request headers at a minimum.
 
 ```python
-from supabase_auth import SyncGoTrueClient
+from gotrue import SyncGoTrueClient
 
 headers = {
     "apiKey": "my-mega-awesome-api-key",
     # ... any other headers you might need.
 }
 client: SyncGoTrueClient = SyncGoTrueClient(url="www.genericauthwebsite.com", headers=headers)
 ```
```

### Comparing `gotrue-2.4.2/gotrue/__init__.py` & `gotrue-2.4.3/gotrue/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "2.4.2"
+__version__ = "2.4.3"
 
 from ._async.gotrue_admin_api import AsyncGoTrueAdminAPI  # type: ignore # noqa: F401
 from ._async.gotrue_client import AsyncGoTrueClient  # type: ignore # noqa: F401
 from ._async.storage import AsyncMemoryStorage  # type: ignore # noqa: F401
 from ._async.storage import AsyncSupportedStorage  # type: ignore # noqa: F401
 from ._sync.gotrue_admin_api import SyncGoTrueAdminAPI  # type: ignore # noqa: F401
 from ._sync.gotrue_client import SyncGoTrueClient  # type: ignore # noqa: F401
```

### Comparing `gotrue-2.4.2/gotrue/_async/gotrue_admin_api.py` & `gotrue-2.4.3/gotrue/_async/gotrue_admin_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 class AsyncGoTrueAdminAPI(AsyncGoTrueBaseAPI):
     def __init__(
         self,
         *,
         url: str = "",
         headers: Dict[str, str] = {},
         http_client: Union[AsyncClient, None] = None,
+        verify: bool = True,
     ) -> None:
         AsyncGoTrueBaseAPI.__init__(
             self,
             url=url,
             headers=headers,
             http_client=http_client,
+            verify=verify,
         )
         self.mfa = AsyncGoTrueAdminMFAAPI()
         self.mfa.list_factors = self._list_factors
         self.mfa.delete_factor = self._delete_factor
 
     async def sign_out(self, jwt: str, scope: SignOutScope = "global") -> None:
         """
@@ -109,17 +111,19 @@
         This function should only be called on a server.
         Never expose your `service_role` key in the browser.
         """
         return await self._request(
             "GET",
             "admin/users",
             query={"page": page, "per_page": per_page},
-            xform=lambda data: [model_validate(User, user) for user in data["users"]]
-            if "users" in data
-            else [],
+            xform=lambda data: (
+                [model_validate(User, user) for user in data["users"]]
+                if "users" in data
+                else []
+            ),
         )
 
     async def get_user_by_id(self, uid: str) -> UserResponse:
         """
         Get user by id.
 
         This function should only be called on a server.
```

### Comparing `gotrue-2.4.2/gotrue/_async/gotrue_admin_mfa_api.py` & `gotrue-2.4.3/gotrue/_async/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/_async/gotrue_base_api.py` & `gotrue-2.4.3/gotrue/_async/gotrue_base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 class AsyncGoTrueBaseAPI:
     def __init__(
         self,
         *,
         url: str,
         headers: Dict[str, str],
         http_client: Union[AsyncClient, None],
+        verify: bool = True,
     ):
         self._url = url
         self._headers = headers
-        self._http_client = http_client or AsyncClient()
+        self._http_client = http_client or AsyncClient(verify=bool(verify))
 
     async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(self, exc_t, exc_v, exc_tb) -> None:
         await self.close()
 
@@ -42,47 +43,44 @@
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: Literal[False] = False,
         xform: Callable[[Any], T],
-    ) -> T:
-        ...  # pragma: no cover
+    ) -> T: ...  # pragma: no cover
 
     @overload
     async def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: Literal[True],
         xform: Callable[[Response], T],
-    ) -> T:
-        ...  # pragma: no cover
+    ) -> T: ...  # pragma: no cover
 
     @overload
     async def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: bool = False,
-    ) -> None:
-        ...  # pragma: no cover
+    ) -> None: ...  # pragma: no cover
 
     async def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
```

### Comparing `gotrue-2.4.2/gotrue/_async/gotrue_client.py` & `gotrue-2.4.3/gotrue/_async/gotrue_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,20 +85,22 @@
         headers: Union[Dict[str, str], None] = None,
         storage_key: Union[str, None] = None,
         auto_refresh_token: bool = True,
         persist_session: bool = True,
         storage: Union[AsyncSupportedStorage, None] = None,
         http_client: Union[AsyncClient, None] = None,
         flow_type: AuthFlowType = "implicit",
+        verify: bool = True,
     ) -> None:
         AsyncGoTrueBaseAPI.__init__(
             self,
             url=url or GOTRUE_URL,
             headers=headers or DEFAULT_HEADERS,
             http_client=http_client,
+            verify=verify,
         )
         self._storage_key = storage_key or STORAGE_KEY
         self._auto_refresh_token = auto_refresh_token
         self._persist_session = persist_session
         self._storage = storage or AsyncMemoryStorage()
         self._in_memory_session: Union[Session, None] = None
         self._refresh_token_timer: Union[Timer, None] = None
```

### Comparing `gotrue-2.4.2/gotrue/_async/gotrue_mfa_api.py` & `gotrue-2.4.3/gotrue/_async/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/_async/storage.py` & `gotrue-2.4.3/gotrue/_async/storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 
 from abc import ABC, abstractmethod
 from typing import Dict, Optional
 
 
 class AsyncSupportedStorage(ABC):
     @abstractmethod
-    async def get_item(self, key: str) -> Optional[str]:
-        ...  # pragma: no cover
+    async def get_item(self, key: str) -> Optional[str]: ...  # pragma: no cover
 
     @abstractmethod
-    async def set_item(self, key: str, value: str) -> None:
-        ...  # pragma: no cover
+    async def set_item(self, key: str, value: str) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    async def remove_item(self, key: str) -> None:
-        ...  # pragma: no cover
+    async def remove_item(self, key: str) -> None: ...  # pragma: no cover
 
 
 class AsyncMemoryStorage(AsyncSupportedStorage):
     def __init__(self):
         self.storage: Dict[str, str] = {}
 
     async def get_item(self, key: str) -> Optional[str]:
```

### Comparing `gotrue-2.4.2/gotrue/_sync/api.py` & `gotrue-2.4.3/gotrue/_sync/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     def __init__(
         self,
         *,
         url: str,
         headers: Dict[str, str],
         cookie_options: CookieOptions,
         http_client: Optional[SyncClient] = None,
+        verify: bool = True,
     ) -> None:
         """Initialise API class."""
         self.url = url
         self.headers = headers
         self.cookie_options = cookie_options
-        self.http_client = http_client or SyncClient()
+        self.http_client = http_client or SyncClient(verify=bool(verify))
 
     def __enter__(self) -> SyncGoTrueAPI:
         return self
 
     def __exit__(self, exc_t, exc_v, exc_tb) -> None:
         self.close()
 
@@ -132,16 +133,16 @@
         query_string = ""
         if redirect_to:
             redirect_to_encoded = encode_uri_component(redirect_to)
             query_string = f"?redirect_to={redirect_to_encoded}"
         data = {"email": email, "password": password, "data": data}
         url = f"{self.url}/signup{query_string}"
         response = self.http_client.post(url, json=data, headers=headers)
-        SessionOrUserModel = determine_session_or_user_model_from_response(response)
-        return SessionOrUserModel.parse_response(response)
+        session_or_user_model = determine_session_or_user_model_from_response(response)
+        return session_or_user_model.parse_response(response)
 
     def sign_in_with_email(
         self,
         *,
         email: str,
         password: str,
         redirect_to: Optional[str] = None,
@@ -207,16 +208,16 @@
         APIError
             If an error occurs.
         """
         headers = self.headers
         data = {"phone": phone, "password": password, "data": data}
         url = f"{self.url}/signup"
         response = self.http_client.post(url, json=data, headers=headers)
-        SessionOrUserModel = determine_session_or_user_model_from_response(response)
-        return SessionOrUserModel.parse_response(response)
+        session_or_user_model = determine_session_or_user_model_from_response(response)
+        return session_or_user_model.parse_response(response)
 
     def sign_in_with_phone(
         self,
         *,
         phone: str,
         password: str,
     ) -> Session:
@@ -331,16 +332,16 @@
             "type": "sms",
         }
         if redirect_to:
             redirect_to_encoded = encode_uri_component(redirect_to)
             data["redirect_to"] = redirect_to_encoded
         url = f"{self.url}/verify"
         response = self.http_client.post(url, json=data, headers=headers)
-        SessionOrUserModel = determine_session_or_user_model_from_response(response)
-        return SessionOrUserModel.parse_response(response)
+        session_or_user_model = determine_session_or_user_model_from_response(response)
+        return session_or_user_model.parse_response(response)
 
     def invite_user_by_email(
         self,
         *,
         email: str,
         redirect_to: Optional[str] = None,
         data: Optional[Dict[str, Any]] = None,
@@ -633,16 +634,16 @@
         if password:
             data["password"] = password
         if redirect_to:
             redirect_to_encoded = encode_uri_component(redirect_to)
             data["redirect_to"] = redirect_to_encoded
         url = f"{self.url}/admin/generate_link"
         response = self.http_client.post(url, json=data, headers=headers)
-        SessionOrUserModel = determine_session_or_user_model_from_response(response)
-        return SessionOrUserModel.parse_response(response)
+        session_or_user_model = determine_session_or_user_model_from_response(response)
+        return session_or_user_model.parse_response(response)
 
     def set_auth_cookie(self, *, req, res):
         """Stub for parity with JS api."""
         raise NotImplementedError("set_auth_cookie not implemented.")
 
     def get_user_by_cookie(self, *, req):
         """Stub for parity with JS api."""
```

### Comparing `gotrue-2.4.2/gotrue/_sync/client.py` & `gotrue-2.4.3/gotrue/_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         headers: Dict[str, str] = {},
         auto_refresh_token: bool = True,
         persist_session: bool = True,
         local_storage: SyncSupportedStorage = SyncMemoryStorage(),
         cookie_options: CookieOptions = CookieOptions.parse_obj(COOKIE_OPTIONS),
         api: Optional[SyncGoTrueAPI] = None,
         replace_default_headers: bool = False,
+        verify: bool = True,
     ) -> None:
         """Create a new client
 
         url : str
             The URL of the GoTrue server.
         headers : Dict[str, str]
             Any additional headers to send to the GoTrue server.
@@ -50,14 +51,16 @@
         persist_session : bool
             Set to "true" if you want to automatically save the user session
             into local storage.
         local_storage : SupportedStorage
             The storage engine to use for persisting the session.
         cookie_options : CookieOptions
             The options for the cookie.
+        verify: bool
+            Verify SSL, True by default, False disables verification.
         """
         if url.startswith("http://"):
             print(
                 "Warning:\n\nDO NOT USE HTTP IN PRODUCTION FOR GOTRUE EVER!\n"
                 "GoTrue REQUIRES HTTPS to work securely."
             )
         self.state_change_emitters: Dict[str, Subscription] = {}
@@ -68,14 +71,15 @@
         self.persist_session = persist_session
         self.local_storage = local_storage
         empty_or_default_headers = {} if replace_default_headers else DEFAULT_HEADERS
         args = {
             "url": url,
             "headers": {**empty_or_default_headers, **headers},
             "cookie_options": cookie_options,
+            "verify": verify,
         }
         self.api = api or SyncGoTrueAPI(**args)
 
     def __enter__(self) -> SyncGoTrueClient:
         return self
 
     def __exit__(self, exc_t, exc_v, exc_tb) -> None:
```

### Comparing `gotrue-2.4.2/gotrue/_sync/gotrue_admin_api.py` & `gotrue-2.4.3/gotrue/_sync/gotrue_admin_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 class SyncGoTrueAdminAPI(SyncGoTrueBaseAPI):
     def __init__(
         self,
         *,
         url: str = "",
         headers: Dict[str, str] = {},
         http_client: Union[SyncClient, None] = None,
+        verify: bool = True,
     ) -> None:
         SyncGoTrueBaseAPI.__init__(
             self,
             url=url,
             headers=headers,
             http_client=http_client,
+            verify=verify,
         )
         self.mfa = SyncGoTrueAdminMFAAPI()
         self.mfa.list_factors = self._list_factors
         self.mfa.delete_factor = self._delete_factor
 
     def sign_out(self, jwt: str, scope: SignOutScope = "global") -> None:
         """
@@ -109,17 +111,19 @@
         This function should only be called on a server.
         Never expose your `service_role` key in the browser.
         """
         return self._request(
             "GET",
             "admin/users",
             query={"page": page, "per_page": per_page},
-            xform=lambda data: [model_validate(User, user) for user in data["users"]]
-            if "users" in data
-            else [],
+            xform=lambda data: (
+                [model_validate(User, user) for user in data["users"]]
+                if "users" in data
+                else []
+            ),
         )
 
     def get_user_by_id(self, uid: str) -> UserResponse:
         """
         Get user by id.
 
         This function should only be called on a server.
```

### Comparing `gotrue-2.4.2/gotrue/_sync/gotrue_admin_mfa_api.py` & `gotrue-2.4.3/gotrue/_sync/gotrue_admin_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/_sync/gotrue_base_api.py` & `gotrue-2.4.3/gotrue/_sync/gotrue_base_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 class SyncGoTrueBaseAPI:
     def __init__(
         self,
         *,
         url: str,
         headers: Dict[str, str],
         http_client: Union[SyncClient, None],
+        verify: bool = True,
     ):
         self._url = url
         self._headers = headers
-        self._http_client = http_client or SyncClient()
+        self._http_client = http_client or SyncClient(verify=bool(verify))
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(self, exc_t, exc_v, exc_tb) -> None:
         self.close()
 
@@ -42,47 +43,44 @@
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: Literal[False] = False,
         xform: Callable[[Any], T],
-    ) -> T:
-        ...  # pragma: no cover
+    ) -> T: ...  # pragma: no cover
 
     @overload
     def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: Literal[True],
         xform: Callable[[Response], T],
-    ) -> T:
-        ...  # pragma: no cover
+    ) -> T: ...  # pragma: no cover
 
     @overload
     def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
         redirect_to: Union[str, None] = None,
         headers: Union[Dict[str, str], None] = None,
         query: Union[Dict[str, str], None] = None,
         body: Union[Any, None] = None,
         no_resolve_json: bool = False,
-    ) -> None:
-        ...  # pragma: no cover
+    ) -> None: ...  # pragma: no cover
 
     def _request(
         self,
         method: Literal["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         *,
         jwt: Union[str, None] = None,
```

### Comparing `gotrue-2.4.2/gotrue/_sync/gotrue_client.py` & `gotrue-2.4.3/gotrue/_sync/gotrue_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,20 +85,22 @@
         headers: Union[Dict[str, str], None] = None,
         storage_key: Union[str, None] = None,
         auto_refresh_token: bool = True,
         persist_session: bool = True,
         storage: Union[SyncSupportedStorage, None] = None,
         http_client: Union[SyncClient, None] = None,
         flow_type: AuthFlowType = "implicit",
+        verify: bool = True,
     ) -> None:
         SyncGoTrueBaseAPI.__init__(
             self,
             url=url or GOTRUE_URL,
             headers=headers or DEFAULT_HEADERS,
             http_client=http_client,
+            verify=verify,
         )
         self._storage_key = storage_key or STORAGE_KEY
         self._auto_refresh_token = auto_refresh_token
         self._persist_session = persist_session
         self._storage = storage or SyncMemoryStorage()
         self._in_memory_session: Union[Session, None] = None
         self._refresh_token_timer: Union[Timer, None] = None
@@ -548,17 +550,15 @@
                 expires_in=expires_at - time_now,
                 expires_at=expires_at,
             )
         self._save_session(session)
         self._notify_all_subscribers("TOKEN_REFRESHED", session)
         return AuthResponse(session=session, user=response.user)
 
-    def refresh_session(
-        self, refresh_token: Union[str, None] = None
-    ) -> AuthResponse:
+    def refresh_session(self, refresh_token: Union[str, None] = None) -> AuthResponse:
         """
         Returns a new session, regardless of expiry status.
 
         Takes in an optional current session. If not passed in, then refreshSession()
         will attempt to retrieve it from getSession(). If the current session's
         refresh token is invalid, an error will be thrown.
         """
@@ -941,17 +941,15 @@
         self,
         provider: Provider,
         params: Dict[str, str],
     ) -> str:
         if self._flow_type == "pkce":
             code_verifier = generate_pkce_verifier()
             code_challenge = generate_pkce_challenge(code_verifier)
-            self._storage.set_item(
-                f"{self._storage_key}-code-verifier", code_verifier
-            )
+            self._storage.set_item(f"{self._storage_key}-code-verifier", code_verifier)
             code_challenge_method = (
                 "plain" if code_verifier == code_challenge else "s256"
             )
             params["code_challenge"] = code_challenge
             params["code_challenge_method"] = code_challenge_method
 
         params["provider"] = provider
```

### Comparing `gotrue-2.4.2/gotrue/_sync/gotrue_mfa_api.py` & `gotrue-2.4.3/gotrue/_sync/gotrue_mfa_api.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/_sync/storage.py` & `gotrue-2.4.3/gotrue/_sync/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 
 from abc import ABC, abstractmethod
 from typing import Dict, Optional
 
 
 class SyncSupportedStorage(ABC):
     @abstractmethod
-    def get_item(self, key: str) -> Optional[str]:
-        ...  # pragma: no cover
+    def get_item(self, key: str) -> Optional[str]: ...  # pragma: no cover
 
     @abstractmethod
-    def set_item(self, key: str, value: str) -> None:
-        ...  # pragma: no cover
+    def set_item(self, key: str, value: str) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    def remove_item(self, key: str) -> None:
-        ...  # pragma: no cover
+    def remove_item(self, key: str) -> None: ...  # pragma: no cover
 
 
 class SyncMemoryStorage(SyncSupportedStorage):
     def __init__(self):
         self.storage: Dict[str, str] = {}
 
     def get_item(self, key: str) -> Optional[str]:
```

### Comparing `gotrue-2.4.2/gotrue/errors.py` & `gotrue-2.4.3/gotrue/errors.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/helpers.py` & `gotrue-2.4.3/gotrue/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 
 def parse_sso_response(data: Any) -> SSOResponse:
     return model_validate(SSOResponse, data)
 
 
 def get_error_message(error: Any) -> str:
     props = ["msg", "message", "error_description", "error"]
-    filter = (
-        lambda prop: prop in error if isinstance(error, dict) else hasattr(error, prop)
+    filter = lambda prop: (
+        prop in error if isinstance(error, dict) else hasattr(error, prop)
     )
     return next((error[prop] for prop in props if filter(prop)), str(error))
 
 
 def looks_like_http_status_error(exception: Exception) -> bool:
     return isinstance(exception, HTTPStatusError)
 
@@ -129,19 +129,19 @@
         return AuthUnknownError(get_error_message(error), e)
 
 
 def decode_jwt_payload(token: str) -> Any:
     parts = token.split(".")
     if len(parts) != 3:
         raise ValueError("JWT is not valid: not a JWT structure")
-    base64Url = parts[1]
+    base64url = parts[1]
     # Addding padding otherwise the following error happens:
     # binascii.Error: Incorrect padding
-    base64UrlWithPadding = base64Url + "=" * (-len(base64Url) % 4)
-    return loads(urlsafe_b64decode(base64UrlWithPadding).decode("utf-8"))
+    base64url_with_padding = base64url + "=" * (-len(base64url) % 4)
+    return loads(urlsafe_b64decode(base64url_with_padding).decode("utf-8"))
 
 
 def generate_pkce_verifier(length=64):
     """Generate a random PKCE verifier of the specified length."""
     if length < 43 or length > 128:
         raise ValueError("PKCE verifier length must be between 43 and 128 characters")
```

### Comparing `gotrue-2.4.2/gotrue/timer.py` & `gotrue-2.4.3/gotrue/timer.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/gotrue/types.py` & `gotrue-2.4.3/gotrue/types.py`

 * *Files identical despite different names*

### Comparing `gotrue-2.4.2/pyproject.toml` & `gotrue-2.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gotrue"
-version = "2.4.2"
+version = "2.4.3"
 description = "Python Client Library for Supabase Auth"
 authors = ["Joel Lee <joel@joellee.org>"]
 homepage = "https://github.com/supabase-community/auth-py"
 repository = "https://github.com/supabase-community/auth-py"
 documentation = "https://github.com/supabase-community/auth-py"
 readme = "README.md"
 license = "MIT"
@@ -16,25 +16,25 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.23,<0.28"
 pydantic = ">=1.10,<3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.1.0"
+pytest = "^8.2.1"
 flake8 = "^5.0.4"
-black = "^24.3.0"
+black = "^24.4.2"
 isort = "^5.12.0"
 pre-commit = "^3.4.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-depends = "^1.0.1"
-pytest-asyncio = "^0.23.5"
-Faker = "^24.4.0"
+pytest-asyncio = "^0.23.7"
+Faker = "^25.2.0"
 unasync-cli = "^0.0.9"
-python-semantic-release = "^9.1.1"
+python-semantic-release = "^9.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pygithub = ">=1.57,<3.0"
 
 [tool.semantic_release]
 version_variables = ["gotrue/__init__.py:__version__"]
 version_toml = ["pyproject.toml:tool.poetry.version"]
```

### Comparing `gotrue-2.4.2/PKG-INFO` & `gotrue-2.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrue
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Client Library for Supabase Auth
 Home-page: https://github.com/supabase-community/auth-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,26 +35,26 @@
 [![Github Watchers](https://img.shields.io/github/watchers/supabase-community/gotrue-py?style=flat&logo=github)](https://github.com/supabase-community/gotrue-py)
 [![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/gotrue-py)](https://github.com/supabase-community/gotrue-py/graphs/contributors)
 
 This is a Python port of the [supabase js gotrue client](https://github.com/supabase/gotrue-js). The current state is that there is a features parity but with small differences that are mentioned in the section **Differences to the JS client**. As of December 14th, we renamed to repo from `gotrue-py` to `auth-py` to mirror the changes in the JavaScript library.
 
 ## Installation
 
-We are still working on making the `supabase_auth` python library more user-friendly. For now here are some sparse notes on how to install the module.
+We are still working on making the `gotrue` python library more user-friendly. For now here are some sparse notes on how to install the module.
 
 ### Poetry
 
 ```bash
-poetry add supabase_auth
+poetry add gotrue
 ```
 
 ### Pip
 
 ```bash
-pip install supabase_auth
+pip install gotrue
 ```
 
 ## Differences to the JS client
 
 It should be noted there are differences to the [JS client](https://github.com/supabase/gotrue-js). If you feel particulaly strongly about them and want to motivate a change, feel free to make a GitHub issue and we can discuss it there.
 
 Firstly, feature pairity is not 100% with the [JS client](https://github.com/supabase/gotrue-js). In most cases we match the methods and attributes of the [JS client](https://github.com/supabase/gotrue-js) and api classes, but is some places (e.g for browser specific code) it didn't make sense to port the code line for line.
@@ -65,24 +65,24 @@
 
 ```js
 const { data, error } = client.sign_up(...)
 ```
 
 The other key difference is we do not use pascalCase to encode variable and method names. Instead we use the snake_case convention adopted in the Python language.
 
-Also, the `supabase_auth` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.
+Also, the `gotrue` library for Python parses the date-time string into `datetime` Python objects. The [JS client](https://github.com/supabase/gotrue-js) keeps the date-time as strings.
 
 ## Usage (outdated)
 
 **Important:** This section is outdated, you can be guided by the [JS client documentation](https://supabase.github.io/gotrue-js) because this Python client has a lot of parity with the JS client.
 
 To instantiate the client, you'll need the URL and any request headers at a minimum.
 
 ```python
-from supabase_auth import SyncGoTrueClient
+from gotrue import SyncGoTrueClient
 
 headers = {
     "apiKey": "my-mega-awesome-api-key",
     # ... any other headers you might need.
 }
 client: SyncGoTrueClient = SyncGoTrueClient(url="www.genericauthwebsite.com", headers=headers)
 ```
```

