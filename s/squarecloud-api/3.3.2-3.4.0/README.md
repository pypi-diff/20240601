# Comparing `tmp/squarecloud_api-3.3.2.tar.gz` & `tmp/squarecloud_api-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squarecloud_api-3.3.2.tar", max compression
+gzip compressed data, was "squarecloud_api-3.4.0.tar", max compression
```

## Comparing `squarecloud_api-3.3.2.tar` & `squarecloud_api-3.4.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1100 2022-09-15 10:56:20.000000 squarecloud_api-3.3.2/LICENSE
--rw-r--r--   0        0        0      949 2024-01-17 23:33:35.165329 squarecloud_api-3.3.2/README.md
--rw-r--r--   0        0        0     1637 2024-02-18 21:45:05.486891 squarecloud_api-3.3.2/pyproject.toml
--rw-r--r--   0        0        0      346 2024-01-19 12:32:31.486852 squarecloud_api-3.3.2/squarecloud/__init__.py
--rw-r--r--   0        0        0    19503 2024-02-18 21:14:52.933249 squarecloud_api-3.3.2/squarecloud/app.py
--rw-r--r--   0        0        0      364 2024-01-17 23:33:35.168663 squarecloud_api-3.3.2/squarecloud/cli/__init__.py
--rw-r--r--   0        0        0    12306 2024-01-17 23:33:35.168663 squarecloud_api-3.3.2/squarecloud/cli/app.py
--rw-r--r--   0        0        0     5169 2023-12-25 17:15:24.000000 squarecloud_api-3.3.2/squarecloud/cli/files.py
--rw-r--r--   0        0        0     5280 2024-01-17 23:33:35.168663 squarecloud_api-3.3.2/squarecloud/cli/main.py
--rw-r--r--   0        0        0    23365 2024-02-18 21:14:52.933249 squarecloud_api-3.3.2/squarecloud/client.py
--rw-r--r--   0        0        0     7605 2024-02-18 21:14:52.933249 squarecloud_api-3.3.2/squarecloud/data.py
--rw-r--r--   0        0        0     5975 2024-01-19 12:32:31.493518 squarecloud_api-3.3.2/squarecloud/errors.py
--rw-r--r--   0        0        0     1929 2023-12-25 17:15:24.000000 squarecloud_api-3.3.2/squarecloud/file.py
--rw-r--r--   0        0        0       80 2023-01-15 11:59:16.000000 squarecloud_api-3.3.2/squarecloud/http/__init__.py
--rw-r--r--   0        0        0    10607 2023-12-26 14:07:08.000000 squarecloud_api-3.3.2/squarecloud/http/endpoints.py
--rw-r--r--   0        0        0    16146 2024-01-17 23:33:35.171996 squarecloud_api-3.3.2/squarecloud/http/http_client.py
--rw-r--r--   0        0        0     6420 2024-02-18 21:14:52.936583 squarecloud_api-3.3.2/squarecloud/listeners.py
--rw-r--r--   0        0        0     1651 2023-12-25 17:15:24.000000 squarecloud_api-3.3.2/squarecloud/logs.py
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 squarecloud_api-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-09-15 10:56:20.000000 squarecloud_api-3.4.0/LICENSE
+-rw-r--r--   0        0        0     1444 2024-03-29 23:53:51.466530 squarecloud_api-3.4.0/README.md
+-rw-r--r--   0        0        0     1858 2024-06-01 00:50:51.839948 squarecloud_api-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0      333 2024-06-01 08:16:19.250187 squarecloud_api-3.4.0/squarecloud/__init__.py
+-rw-r--r--   0        0        0    19002 2024-06-01 01:21:35.366963 squarecloud_api-3.4.0/squarecloud/app.py
+-rw-r--r--   0        0        0      364 2024-01-17 23:33:35.168663 squarecloud_api-3.4.0/squarecloud/cli/__init__.py
+-rw-r--r--   0        0        0    12335 2024-04-08 04:53:28.148104 squarecloud_api-3.4.0/squarecloud/cli/app.py
+-rw-r--r--   0        0        0     5169 2023-12-25 17:15:24.000000 squarecloud_api-3.4.0/squarecloud/cli/files.py
+-rw-r--r--   0        0        0     4195 2024-05-31 15:33:21.711374 squarecloud_api-3.4.0/squarecloud/cli/main.py
+-rw-r--r--   0        0        0    27682 2024-06-01 00:44:54.025379 squarecloud_api-3.4.0/squarecloud/client.py
+-rw-r--r--   0        0        0     7001 2024-05-31 15:33:53.491451 squarecloud_api-3.4.0/squarecloud/data.py
+-rw-r--r--   0        0        0     6226 2024-04-08 04:59:22.424754 squarecloud_api-3.4.0/squarecloud/errors.py
+-rw-r--r--   0        0        0     1929 2024-02-22 10:50:09.328482 squarecloud_api-3.4.0/squarecloud/file.py
+-rw-r--r--   0        0        0       80 2023-01-15 11:59:16.000000 squarecloud_api-3.4.0/squarecloud/http/__init__.py
+-rw-r--r--   0        0        0     9668 2024-06-01 07:58:58.723877 squarecloud_api-3.4.0/squarecloud/http/endpoints.py
+-rw-r--r--   0        0        0    25503 2024-05-31 15:33:09.668012 squarecloud_api-3.4.0/squarecloud/http/http_client.py
+-rw-r--r--   0        0        0     5440 2024-06-01 07:18:59.499250 squarecloud_api-3.4.0/squarecloud/listeners/__init__.py
+-rw-r--r--   0        0        0     5169 2024-06-01 07:05:56.133894 squarecloud_api-3.4.0/squarecloud/listeners/capture_listener.py
+-rw-r--r--   0        0        0     3765 2024-06-01 07:25:35.527017 squarecloud_api-3.4.0/squarecloud/listeners/request_listener.py
+-rw-r--r--   0        0        0     1718 2024-04-10 20:08:42.511271 squarecloud_api-3.4.0/squarecloud/logging.py
+-rw-r--r--   0        0        0     2438 2024-05-31 15:18:01.459097 squarecloud_api-3.4.0/squarecloud/utils.py
+-rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 squarecloud_api-3.4.0/PKG-INFO
```

### Comparing `squarecloud_api-3.3.2/LICENSE` & `squarecloud_api-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squarecloud_api-3.3.2/pyproject.toml` & `squarecloud_api-3.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 [tool.poetry]
-name = "squarecloud-api"
-version = "3.3.2"
-description = "SquareCloud API wrapper"
-authors = ["Robert Nogueira <robertlucasnogueira@gmail.com>"]
-repository = "https://github.com/squarecloudofc/wrapper-api-py"
-documentation = "https://docs.squarecloud.app/sdks/py"
-license = "MIT License"
-readme = "README.md"
-packages = [{ include = "squarecloud" }]
+name = 'squarecloud-api'
+version = '3.4.0'
+description = 'SquareCloud API wrapper'
+authors = ['Robert Nogueira <robertlucasnogueira@gmail.com>']
+repository = 'https://github.com/squarecloudofc/wrapper-api-py'
+documentation = 'https://docs.squarecloud.app/sdks/py'
+license = 'MIT License'
+readme = 'README.md'
+packages = [{ include = 'squarecloud' }]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-aiohttp = "3.9.3"
-click = "^8.1.6"
-rich = "^13.5.2"
-pydantic = "^2.5.2"
-python-dotenv = "^1.0.0"
+python = '^3.9'
+aiohttp = '3.9.3'
+click = '^8.1.6'
+rich = '^13.5.2'
+pydantic = '^2.5.2'
+python-dotenv = '^1.0.0'
+pypi = "^2.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
-blue = "^0.9.1"
-isort = "^5.12.0"
-taskipy = "^1.12.0"
-pytest-asyncio = "^0.21.1"
-pre-commit = "^3.3.3"
-ruff = "^0.0.289"
-memory-profiler = "^0.61.0"
-requests = "^2.31.0"
+pytest = '^7.4.3'
+pytest-cov = '^4.1.0'
+blue = '^0.9.1'
+isort = '^5.12.0'
+taskipy = '^1.12.0'
+pytest-asyncio = '^0.21.1'
+pre-commit = '^3.3.3'
+ruff = '^0.0.289'
+memory-profiler = '^0.61.0'
+requests = '^2.31.0'
+pytest-rerunfailures = "^13.0"
 
 
 [[tool.poetry.source]]
-name = "pypi-test"
-url = "https://test.pypi.org/simple/"
-priority = "primary"
+name = 'pypi-test'
+url = 'https://test.pypi.org/simple/'
+priority = 'primary'
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ['poetry-core']
+build-backend = 'poetry.core.masonry.api'
 
 [tool.pytest.ini_options]
-python_path = "tests"
-addopts = "--doctest-modules"
+asyncio_mode = 'auto'
+markers = [
+    'app',
+    'app_data',
+    'listeners',
+    'capture_listener',
+    'request_listener',
+    'files',
+    'upload',
+]
 
 [tool.isort]
-profile = "black"
+profile = 'black'
 line_length = 79
 
 [tool.taskipy.tasks]
-lint = "isort . && blue . && ruff ."
-pre_test = "task lint"
-test = "pytest -s -x --cov=tests -vv tests"
-post_test = "coverage html"
-cli = "poetry run squarecloud"
-publish-test = "poetry publish -r pypi-test --build"
-install-test = "pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple --upgrade squarecloud-api"
-docs = "mkdocs serve"
+lint = 'isort . && blue . && ruff .'
+pre_test = 'task lint'
+test = 'pytest -vv -s --reruns 5 --only-rerun TooManyRequests --reruns-delay 60 -x --cov=tests tests'
+post_test = 'coverage html'
+cli = 'python -m squarecloud.cli.main'
+publish-test = 'poetry publish -r pypi-test --build'
+install-test = 'pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple --upgrade squarecloud-api'
+docs = 'mkdocs serve'
 
 [tool.poetry.scripts]
-squarecloud = "squarecloud.cli.main:safe_entry_point"
+clear-test-apps = 'scripts.clear_test_apps:delete_test_apps'
 
 [tool.ruff]
 line-length = 79
 exclude = ['env']
 
 [tool.ruff.per-file-ignores]
 '__init__.py' = ['F401']
```

### Comparing `squarecloud_api-3.3.2/squarecloud/app.py` & `squarecloud_api-3.4.0/squarecloud/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
-from abc import ABC
+from functools import wraps
 from io import BytesIO
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Any, Callable
 
 from pydantic import PositiveInt
 
+from squarecloud import errors
+
 from .data import (
     AppData,
     BackupData,
     DeployData,
     DomainAnalytics,
     FileInfo,
     LogsData,
     StatusData,
 )
-from .errors import SquareException
 from .file import File
 from .http import Endpoint, HTTPClient, Response
-from .listeners import CaptureListenerManager
+from .listeners import Listener, ListenerConfig
+from .listeners.capture_listener import CaptureListenerManager
 
 # avoid circular imports
 if TYPE_CHECKING:
     from .client import Client
 
 
 class AppCache:
@@ -36,89 +38,89 @@
     def __init__(self) -> None:
         """
         The `__init__` function is called when the class is instantiated.
         It sets up the instance of the class, and defines all of its
         attributes.
 
 
-        :return: The instance of the class
-        :rtype: None
+        :return: None
         """
         self._status: StatusData | None = None
         self._logs: LogsData | None = None
         self._backup: BackupData | None = None
         self._app_data: AppData | None = None
 
     @property
     def status(self) -> StatusData:
         """
-        The status function returns the status of the application.
+        The status method is a property that returns the cached StatusData of
+        the application.
 
-        :return: The status of the application.
+        :return: A StatusData object.
         :rtype: StatusData
         """
         return self._status
 
     @property
     def logs(self) -> LogsData:
         """
-        The logs function the logs of the application.
+        The logs method is a property that returns the cached LogsData of
+        the application.
 
         :return: The logs of your application
         :rtype: LogsData
         """
         return self._logs
 
     @property
     def backup(self) -> BackupData:
         """
-        The backup function is used to create a backup of the application.
+        The backup method is a property that returns the cached BackupData of
+        the application.
 
         :return: The value of the _backup attribute
         :rtype: BackupData
         """
         return self._backup
 
     @property
     def app_data(self) -> AppData:
         """
-        The app_data function is a property that returns the AppData object.
+        The app_data method is a property that returns the cached AppData
+        object
 
         :return: The data from the app_data
         :rtype: AppData
         """
         return self._app_data
 
     def clear(self):
         """
-        The clear function is used to clear the status, logs, backup and data
+        The clear method is used to clear the status, logs, backup and data
         variables.
 
         :param self: Refer to the class instance
         :return: None
-        :rtype: None
         """
         self._status = None
         self._logs = None
         self._backup = None
         self._app_data = None
 
     def update(self, *args):
         """
-        The update function is used to update the data of a given instance.
+        The update method is used to update the data of a given instance.
         It takes in an arbitrary number of arguments, and updates the
         corresponding data if it is one of the following types:
         StatusData, LogsData, BackupData or AppData.
         If any other type is provided as an argument to this function,
         a SquareException will be raised.
 
-        :param self: Refer to the class instance
         :param args: Pass a variable number of arguments to a function
         :return: None
-        :rtype: None
         """
         for arg in args:
             if isinstance(arg, StatusData):
                 self._status = arg
             elif isinstance(arg, LogsData):
                 self._logs = arg
             elif isinstance(arg, BackupData):
@@ -131,24 +133,20 @@
                     for i in [
                         StatusData,
                         LogsData,
                         BackupData,
                         AppData,
                     ]
                 ]
-                raise SquareException(
+                raise errors.SquareException(
                     f'you must provide stats of the following types:\n{types}'
                 )
 
 
-class AbstractApplication(ABC):
-    """Abstract application class"""
-
-
-class Application:
+class Application(CaptureListenerManager):
     """Represents an application"""
 
     __slots__ = [
         '_client',
         '_http',
         '_listener',
         '_data',
@@ -172,78 +170,76 @@
         ram: PositiveInt,
         lang: str,
         cluster: str,
         isWebsite: bool,
         desc: str | None = None,
     ) -> None:
         """
-        The `__init__` function is called when the class is instantiated.
+        The `__init__` method is called when the class is instantiated.
         It sets up all the attributes that are passed in as arguments,
         and does any other initialization your class needs before It's ready
         for use.
 
 
-        :param self: Refer to the class instance.
-        :param client: 'Client': Store a reference to the client that created
+        :param client: Store a reference to the client that created
         this app.
-        :param http: HTTPClient: Make http requests to the api.
-        :param id: str: The id of the app.
-        :param tag: str: The tag of the app.
-        :param ram: PositiveInt: The amount of ram that is allocated.
-        :param lang: str: The programming language of the app.
-        :param cluster: str: The cluster that the app is hosted on
-        :param isWebsite: bool: Whether if the app is a website
-        :param desc: str | None: Define the description of the app
+        :param http: Store a reference to the HTTPClient
+        :param id: The application id
+        :param tag: The tag of the app
+        :param ram: The amount of ram that is allocated
+        :param lang: The programming language of the app
+        :param cluster: The cluster that the app is hosted on
+        :param isWebsite: Whether if the app is a website
+        :param desc: Define the description of the app
 
         :return: None
-        :rtype: None
         """
         self._id: str = id
         self._tag: str = tag
         self._desc: str | None = desc
         self._ram: PositiveInt = ram
         self._lang: str = lang
         self._cluster: str = cluster
         self._isWebsite: bool = isWebsite
         self._client: 'Client' = client
         self._http: HTTPClient = http
         self._listener: CaptureListenerManager = CaptureListenerManager()
         self.cache: AppCache = AppCache()
         self.always_avoid_listeners: bool = False
+        super().__init__()
 
     def __repr__(self) -> str:
         """
-        The __repr__ function is used to create a string representation of an
+        The `__repr__` method is used to create a string representation of an
         object.
         This is useful for debugging, logging and other instances where you
         would want a string representation of the object.
         The __repr__ function should return a string that would make sense to
         someone looking at the results in the interactive interpreter.
 
-
-        :param self: Refer to the class instance
         :return: The class name, tag and id of the element
+        :rtype: str
         """
         return f'<{self.__class__.__name__} tag={self.tag} id={self.id}>'
 
     @property
     def client(self) -> 'Client':
         """
-        The client function is a property that returns the client object.
+        The client method is a property that returns the client object.
 
         :return: The client instance
         :rtype: Client
         """
         return self._client
 
     @property
     def id(self) -> str:
         """
         The id function is a property that returns
-         the id of the application.
+        the id of the application.
 
         :return: The id of the application
         :rtype: str
         """
         return self._id
 
     @property
@@ -313,152 +309,160 @@
         indicating whether th application is a website.
 
         :return: A boolean value, true or false
         :rtype: bool
         """
         return self._isWebsite
 
-    def capture(self, endpoint: Endpoint) -> Callable:
+    @staticmethod
+    def _notify_listener(endpoint: Endpoint):
         """
-        The capture function is a decorator that can be used to add a function
+        The _notify_listener function is a decorator that call a listener after
+        the decorated coroutine is called
+
+        :param endpoint: the endpoint for witch the listener will fetch
+        :return: a callable
+        """
+
+        def wrapper(func: Callable):
+            @wraps(func)
+            async def decorator(self: Application, *args, **kwargs) -> Any:
+                result = await func(self, *args, **kwargs)
+                avoid_listener = kwargs.pop('avoid_listener', False)
+                if not (avoid_listener or self.always_avoid_listeners):
+                    await self.notify(
+                        endpoint=endpoint,
+                        before=self.cache.app_data,
+                        after=result,
+                        extra=kwargs.get('extra'),
+                    )
+                return result
+
+            return decorator
+
+        return wrapper
+
+    @staticmethod
+    def _update_cache(func: Callable):
+        """
+        This is a decorator checks whether the kwargs `update_cache` in the
+        decorated coroutine is not False, and updates the application cache
+
+        :param func:
+        :return: a callable
+        """
+
+        @wraps(func)
+        async def wrapper(self, *args, **kwargs):
+            update_cache = kwargs.pop('update_cache', True)
+            result = await func(self, *args, **kwargs)
+            if update_cache:
+                self.cache.update(result)
+            return result
+
+        return wrapper
+
+    def capture(self, endpoint: Endpoint, **kwargs) -> Callable:
+        """
+        The capture function is a decorator that can be used to add a callable
         to be called when a request is made to the specified endpoint.
 
         :param self: Refer to the class instance.
         :param endpoint: Endpoint: Specify which endpoint the function will be
         called on
         :return: A decorator
         :rtype: Callable
         """
-        allowed_endpoints: tuple[Endpoint, Endpoint, Endpoint, Endpoint] = (
-            Endpoint.logs(),
-            Endpoint.app_status(),
-            Endpoint.backup(),
-            Endpoint.app_data(),
-        )
 
-        def wrapper(func) -> None:
+        def wrapper(
+            call: Callable[[Endpoint, Endpoint], Any]
+        ) -> Callable[[Endpoint, Endpoint], Any]:
             """
             The wrapper function is a decorator that takes in the endpoint as
             an argument.
             It then checks if the endpoint is allowed, and if it isn't, raises
             a SquareException.
             If there's no capture_listener for that endpoint yet, it adds one
             with the function passed to wrapper().
             Otherwise, it raises another SquareException.
 
-            :param func: Pass the function to be wrapped
+            :param call: Pass the function to be wrapped
             :return: The wrapper function itself
             :rtype: None
+            :raises InvalidListener: Raised if the endpoint is already
+            registered
             """
-            if endpoint not in allowed_endpoints:
-                raise SquareException(
-                    f'the endpoint to capture must be {allowed_endpoints}'
-                )
-
-            if self._listener.get_capture_listener(endpoint) is None:
-                return self._listener.add_capture_listener(endpoint, func)
-            raise SquareException(
-                f'Already exists an capture_listener for {endpoint}'
-                f'{self._listener.get_capture_listener(endpoint)}'
+            for key, value in kwargs.items():
+                if key not in ListenerConfig.__annotations__:
+                    raise ValueError(
+                        f'Invalid listener configuration: "{key}={value}"'
+                    )
+            config = ListenerConfig(**kwargs)
+            listener = Listener(
+                app=self,
+                client=self.client,
+                endpoint=endpoint,
+                callback=call,
+                config=config,
             )
+            self.include_listener(listener)
+            return call
 
         return wrapper
 
-    async def data(
-        self, avoid_listener: bool = None, update_cache: bool = True
-    ) -> AppData:
+    @_update_cache
+    @_notify_listener(Endpoint.app_data())
+    async def data(self, *_args, **__kwargs) -> AppData:
         """
-        The data function is used to retrieve the data of an app.
+        The data method is used to retrieve the data of this app.
 
-        :param update_cache: if True, update the application cache
-        :param avoid_listener: whether the capture listener will be called
         :param self: Refer to the class instance
         :return: A AppData object
         :rtype: AppData
         """
         app_data: AppData = await self.client.app_data(self.id)
-        avoid_listener = avoid_listener or self.always_avoid_listeners
-        if not avoid_listener:
-            endpoint: Endpoint = Endpoint.app_data()
-            await self._listener.on_capture(
-                endpoint=endpoint,
-                before=self.cache.app_data,
-                after=app_data,
-            )
-        if update_cache:
-            self.cache.update(app_data)
         return app_data
 
-    async def logs(
-        self, avoid_listener: bool = None, update_cache: bool = True
-    ) -> LogsData:
+    @_update_cache
+    @_notify_listener(Endpoint.logs())
+    async def logs(self, *_args, **__kwargs) -> LogsData:
         """
-        The logs function is used to get the application's logs.
+        The logs method is used to get the application's logs.
 
         :param self: Refer to the class instance
-        :param update_cache: if True, update the application cache
-        :param avoid_listener: whether the capture listener will be called
         :return: A LogsData object
         :rtype: LogsData
         """
         logs: LogsData = await self.client.get_logs(self.id)
-        avoid_listener = avoid_listener or self.always_avoid_listeners
-        if not avoid_listener:
-            endpoint: Endpoint = Endpoint.logs()
-            await self._listener.on_capture(
-                endpoint=endpoint, before=self.cache.logs, after=logs
-            )
-        if update_cache:
-            self.cache.update(logs)
         return logs
 
-    async def status(
-        self, avoid_listener: bool = None, update_cache: bool = True
-    ) -> StatusData:
+    @_update_cache
+    @_notify_listener(Endpoint.app_status())
+    async def status(self, *_args, **__kwargs) -> StatusData:
         """
         The status function returns the status of an application.
 
         :param self: Refer to the class instance
-        :param update_cache: if True, update the application cache
-        :param avoid_listener: whether the capture listener will be called
         :return: A StatusData object
         :rtype: StatusData
         """
         status: StatusData = await self.client.app_status(self.id)
-        avoid_listener = avoid_listener or self.always_avoid_listeners
-        if not avoid_listener:
-            endpoint: Endpoint = Endpoint.app_status()
-            await self._listener.on_capture(
-                endpoint=endpoint, before=self.cache.status, after=status
-            )
-        if update_cache:
-            self.cache.update(status)
         return status
 
-    async def backup(
-        self, avoid_listener: bool = None, update_cache: bool = True
-    ) -> BackupData:
+    @_update_cache
+    @_notify_listener(Endpoint.backup())
+    async def backup(self, *_args, **__kwargs) -> BackupData:
         """
         The backup function is used to create a backup of the application.
 
         :param self: Refer to the class instance
-        :param update_cache: if True, update the application cache
-        :param avoid_listener: whether the capture listener will be called
         :return: A BackupData object
         :rtype: BackupData
         """
         backup: BackupData = await self.client.backup(self.id)
-        avoid_listener = avoid_listener or self.always_avoid_listeners
-        if not avoid_listener:
-            endpoint: Endpoint = Endpoint.backup()
-            await self._listener.on_capture(
-                endpoint=endpoint, before=self.cache.backup, after=backup
-            )
-        if update_cache:
-            self.cache.update(backup)
         return backup
 
     async def start(self) -> Response:
         """
         The start function starts the application.
 
         :param self: Refer to the class instance
```

### Comparing `squarecloud_api-3.3.2/squarecloud/cli/app.py` & `squarecloud_api-3.4.0/squarecloud/cli/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 )
 @click.pass_context
 @run_async
 async def app_group(ctx: Context, app_id: str, token: str):
     if not app_id:
         click.echo(ctx.get_help())
         return
-    client = Client(token, debug=False)
+    client = Client(token, log_level='CRITICAL')
     if not ctx.invoked_subcommand:
         with Console().status('loading'):
             app = await client.app(app_id)
             table = Table(title=app.tag, header_style='purple')
             table.add_column('Tag', justify='center')
             table.add_column('ID', justify='center')
             table.add_column('RAM', justify='center')
@@ -110,15 +110,15 @@
     type=click.STRING,
     prompt='API KEY',
     hide_input=True,
 )
 @click.pass_context
 @run_async
 async def app_list(ctx: Context, token: str):
-    client = Client(token, debug=False)
+    client = Client(token, log_level='CRITICAL')
     with Console().status('loading'):
         apps: list[Application] = await client.all_apps()
     if not apps:
         print(
             Panel(
                 'You do not have any application',
                 title_align='left',
@@ -295,16 +295,16 @@
     required=True,
     type=click.STRING,
     prompt='API KEY',
     hide_input=True,
 )
 @run_async
 async def upload_app(token: str, file: BufferedReader):
-    client = Client(token, debug=False)
-    with Console().status('loading'):
+    client = Client(token, log_level='CRITICAL')
+    with Console().status('uploading'):
         upload_data: UploadData = await client.upload_app(
             file=squarecloud.File(file)
         )
         panel = Panel(
             f'Application with id {upload_data.id} has been uploaded',
             title='App uploaded',
             title_align='left',
```

### Comparing `squarecloud_api-3.3.2/squarecloud/cli/files.py` & `squarecloud_api-3.4.0/squarecloud/cli/files.py`

 * *Files identical despite different names*

### Comparing `squarecloud_api-3.3.2/squarecloud/cli/main.py` & `squarecloud_api-3.4.0/squarecloud/cli/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,25 @@
+from pathlib import Path
 from typing import Literal
 
 import click
 from click import prompt
 from dotenv import load_dotenv
 from rich import print
-from rich.console import Console
 from rich.panel import Panel
-from rich.table import Table
-
-from squarecloud.client import Client, create_config_file
-from squarecloud.data import StatisticsData
 
 from ..errors import RequestError, SquareException
-from . import cli, run_async
+from ..utils import ConfigFile
+from . import cli
 from .app import app_list, upload_app
 from .files import app_group
 
 load_dotenv()
 
 
-@cli.command(
-    name='statistics', help='Get statistics information about the host'
-)
-@click.option(
-    '--token',
-    '-t',
-    help='your api token',
-    envvar='SQUARECLOUD_KEY',
-    required=True,
-    type=click.STRING,
-    prompt='API KEY',
-    hide_input=True,
-)
-@run_async
-async def get_squarecloud_statistics(token: str):
-    client = Client(api_key=token, debug=False)
-
-    with Console().status('loading'):
-        statistics_data: StatisticsData = await client.statistics()
-    table = Table(title='Statistics', header_style='purple')
-
-    table.add_column('Apps', justify='center')
-    table.add_column('Websites', justify='center')
-    table.add_column('Time', justify='center')
-    table.add_column('Ping', justify='center')
-    table.add_column('Users', justify='center')
-
-    table.add_row(
-        str(statistics_data.apps),
-        str(statistics_data.websites),
-        str(statistics_data.ping),
-        str(statistics_data.users),
-        style='green',
-    )
-    print(table)
-
-
 @click.command(
     name='create-config-file',
     help='Create a config file to upload an application',
 )
 @click.argument(
     'output_file',
     type=click.Path(),
@@ -127,57 +87,54 @@
     version: Literal['recommended', 'latest'] = 'recommended',
     description: str | None = None,
     subdomain: str | None = None,
     start: str | None = None,
     auto_restart: bool | None = None,
 ):
 
-    content = create_config_file(
-        path='/',
+    config_file = ConfigFile(
         display_name=display_name,
         main=main,
         memory=memory,
         version=version,
         description=description,
         subdomain=subdomain,
         start=start,
         auto_restart=auto_restart,
-        save=False,
     )
     if output_file:
-        with open(output_file, 'w') as f:
-            f.write(content)
+        if not Path(output_file).exists():
+            raise Exception(f'File or directory {output_file} not exists')
         print(
             Panel(
                 f'\u2728  file saved successfully at {output_file}',
                 border_style='green',
                 style='green',
             )
         )
         return
     else:
         print(
             Panel(
-                content,
+                config_file.content(),
                 title='squarecloud.app',
                 border_style='purple',
                 style='green',
             )
         )
         r = prompt(
             'would you like to save the file? [y/N]',
             type=click.BOOL,
             default='Y',
         )
     if r:
         path = prompt(
             'where do you want to save the file', default='squarecloud.app'
         )
-        with open(path, 'w') as f:
-            f.write(content)
+        config_file.save(path)
         print(
             Panel(
                 f'\u2728  file saved successfully at {path}',
                 border_style='green',
                 style='green',
             )
         )
@@ -207,7 +164,11 @@
         print(
             Panel(
                 str(e),
                 title_align='left',
                 style='red',
             ),
         )
+
+
+if __name__ == '__main__':
+    safe_entry_point()
```

### Comparing `squarecloud_api-3.3.2/squarecloud/data.py` & `squarecloud_api-3.4.0/squarecloud/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, Dict, Literal
 
-from pydantic import conint
+from pydantic import confloat, conint
 from pydantic.dataclasses import dataclass
-from typing_extensions import TypedDict
 
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=invalid-name
 
 
 @dataclass(frozen=True)
 class PlanData:
@@ -29,16 +28,16 @@
     memory: Dict[str, Any]
     duration: Dict[str, Any] | None
 
     def to_dict(self):
         return self.__dict__.copy()
 
 
-# @dataclass(frozen=True)
-class Language(TypedDict):
+@dataclass(frozen=True)
+class Language:
     name: str
     version: str
 
 
 @dataclass(frozen=True)
 class StatusData:
     """
@@ -82,37 +81,35 @@
 @dataclass(frozen=True)
 class AppData:
     """
     Application data class
 
     :ivar id: The application ID
     :ivar name: The application name
-    :ivar owner: The application owner ID
     :ivar cluster: The cluster that the app is hosted on
     :ivar ram: The amount of RAM that application is using
     :ivar language The programming language of the app.:
     :ivar isWebsite: Whether if the app is a website
 
     :type id: str
     :type name: str
-    :type owner: str
     :type cluster: str
-    :type ram: conint(ge=0);
+    :type ram: confloat(ge=0);
     :type language: Language
     :type isWebsite: bool
     :type gitIntegration: bool
     :type domain: str | None = None
     :type custom: str | None = None
     :type desc: str | None = None
     """
 
     id: str
     name: str
     cluster: str
-    ram: conint(ge=0)
+    ram: confloat(ge=0)
     language: str
     cluster: str
     isWebsite: bool
     gitIntegration: bool
     domain: str | None = None
     custom: str | None = None
     desc: str | None = None
@@ -232,25 +229,25 @@
     :ivar cpu: Cpu of the uploaded application
     :ivar description: Description of the uploaded application
     :ivar subdomain: Subdomain of the uploaded application (only in websites)
 
     :type id: str
     :type tag: str
     :type language: Language
-    :type ram: conint(ge=0)
-    :type cpu: conint(ge=0)
+    :type ram: confloat(ge=0)
+    :type cpu: confloat(ge=0)
     :type subdomain: str | None = None
     :type description: str | None = None
     """
 
     id: str
     tag: str
     language: Language
-    ram: conint(ge=0)
-    cpu: conint(ge=0)
+    ram: confloat(ge=0)
+    cpu: confloat(ge=0)
     subdomain: str | None = None
     description: str | None = None
 
     def to_dict(self):
         return self.__dict__.copy()
 
 
@@ -263,55 +260,31 @@
     :ivar name: File/Directory name
     :ivar size: File size
     :ivar lastModified: Last modification time
     :ivar path: File/Directory path
 
     :type type: Literal['file', 'directory']
     :type name: str
-    :type size: conint(ge=0)
+    :type size: confloat(ge=0)
     :type lastModified: conint(ge=0) | float
     :type path: str
     """
 
+    app_id: str
     type: Literal['file', 'directory']
     name: str
-    size: conint(ge=0)
+    size: confloat(ge=0)
     lastModified: conint(ge=0) | float
     path: str
 
     def to_dict(self):
         return self.__dict__.copy()
 
 
 @dataclass(frozen=True)
-class StatisticsData:
-    """
-    Host statistics
-
-    :ivar users: Amount of users that uses the host
-    :ivar apps: Amount of apps hosted
-    :ivar websites: Amount of websites hosted
-    :ivar ping: Service ping
-
-    :type users: conint(ge=0)
-    :type apps: conint(ge=0)
-    :type websites: conint(ge=0)
-    :type ping: conint(ge=0)
-    """
-
-    users: conint(ge=0)
-    apps: conint(ge=0)
-    websites: conint(ge=0)
-    ping: conint(ge=0)
-
-    def to_dict(self):
-        return self.__dict__.copy()
-
-
-@dataclass(frozen=True)
 class DeployData:
     id: str
     state: str
     date: datetime
 
     def to_dict(self):
         return self.__dict__.copy()
```

### Comparing `squarecloud_api-3.3.2/squarecloud/errors.py` & `squarecloud_api-3.4.0/squarecloud/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .file import File
+from typing import Callable
 
 
 class SquareException(Exception):
     """abstract class SquareException"""
 
     def __init__(self, message: str = 'An unexpected error occurred'):
         self.message = message
@@ -111,26 +111,26 @@
 
 
 class InvalidConfig(RequestError):
     """
     raised when the config file is corrupt or invalid.
     """
 
-    def __init__(self, file: File, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.message = f'{file.filename} have a invalid config file'
+        self.message = 'invalid config file'
 
 
 class InvalidDisplayName(InvalidConfig):
     """
     raised when the display name in the config file is invalid.
     """
 
-    def __init__(self, file: File, *args, **kwargs):
-        super().__init__(file=file, *args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.message = 'Invalid display name in config file'
 
 
 class MissingDisplayName(InvalidConfig):
     """
     raised when the display name in the config file is missing.
     """
@@ -141,16 +141,16 @@
 
 
 class InvalidMain(InvalidConfig):
     """
     raised when the main file in the config file is invalid.
     """
 
-    def __init__(self, file: File, *args, **kwargs):
-        super().__init__(file=file, *args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.message = 'Invalid main file in config file'
 
 
 class MissingMainFile(InvalidConfig):
     """
     raised when the main file in the config file is missing.
     """
@@ -161,16 +161,16 @@
 
 
 class InvalidMemory(InvalidConfig):
     """
     raised when the memory value in the config file is invalid.
     """
 
-    def __init__(self, file: File, *args, **kwargs):
-        super().__init__(file=file, *args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.message = 'Invalid memory value in config file'
 
 
 class MissingMemory(InvalidConfig):
     """
     raised when the memory value in the config file is missing.
     """
@@ -181,16 +181,16 @@
 
 
 class InvalidVersion(InvalidConfig):
     """
     raised when the version value in the config file is invalid.
     """
 
-    def __init__(self, file: File, *args, **kwargs):
-        super().__init__(file=file, *args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.message = 'Invalid version value in config file'
 
 
 class MissingVersion(InvalidConfig):
     """
     raised when the version value in the config file is missing.
     """
@@ -201,20 +201,31 @@
 
 
 class InvalidAccessToken(RequestError):
     """
     raised when the GitHub access token provided by the user is invalid.
     """
 
-
-def __init__(self, *args, **kwargs):
-    super().__init__(*args, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
 
 class InvalidDomain(RequestError):
     """
     raised when an invalid domain is provided
     """
 
     def __init__(self, domain: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.message = f'{domain} is a invalid custom domain'
+        self.message = f'"{domain}" is a invalid custom domain'
+
+
+class InvalidStart(InvalidConfig):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.message = 'Invalid start value in configuration file'
+
+
+class InvalidListener(SquareException):
+    def __init__(self, listener: Callable, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.listener = listener
```

### Comparing `squarecloud_api-3.3.2/squarecloud/file.py` & `squarecloud_api-3.4.0/squarecloud/file.py`

 * *Files identical despite different names*

### Comparing `squarecloud_api-3.3.2/squarecloud/http/endpoints.py` & `squarecloud_api-3.4.0/squarecloud/http/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,322 +1,298 @@
-# pylint: disable=missing-module-docstring
-
-from __future__ import annotations
-
-from typing import Any, Dict
-
-# pylint: disable=missing-function-docstring
-
-
-class Endpoint:
-    """Endpoint"""
-
-    # ENDPOINTS_V1 = {
-    #     'USER_ME': {'METHOD': 'GET', 'PATH': '/user'},
-    #     'USER_INFO': {'METHOD': 'GET', 'PATH': '/user/{user_id}'},
-    #     'APP_STATUS': {'METHOD': 'GET', 'PATH': '/status/{app_id}'},
-    #     'LOGS': {'METHOD': 'GET', 'PATH': '/logs/{app_id}'},
-    #     'FULL_LOGS': {'METHOD': 'GET', 'PATH': '/full-logs/{app_id}'},
-    #     'START': {'METHOD': 'POST', 'PATH': '/start/{app_id}'},
-    #     'STOP': {'METHOD': 'POST', 'PATH': '/stop/{app_id}'},
-    #     'RESTART': {'METHOD': 'POST', 'PATH': '/restart/{app_id}'},
-    #     'BACKUP': {'METHOD': 'GET', 'PATH': '/backup/{app_id}'},
-    #     'COMMIT': {'METHOD': 'POST', 'PATH': '/commit/{app_id}'},
-    #     'DELETE': {'METHOD': 'POST', 'PATH': '/delete/{app_id}'},
-    #     'UPLOAD': {'METHOD': 'POST', 'PATH': '/upload'},
-    # }
-
-    ENDPOINTS_V2 = {
-        'USER_ME': {'METHOD': 'GET', 'PATH': '/user'},
-        'APP_DATA': {'METHOD': 'GET', 'PATH': '/apps/{app_id}'},
-        'USER_INFO': {'METHOD': 'GET', 'PATH': '/user/{user_id}'},
-        'APP_STATUS': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/status'},
-        'LOGS': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/logs'},
-        'START': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/start'},
-        'STOP': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/stop'},
-        'RESTART': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/restart'},
-        'BACKUP': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/backup'},
-        'COMMIT': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/commit'},
-        'DELETE_APP': {'METHOD': 'DELETE', 'PATH': '/apps/{app_id}/delete'},
-        'UPLOAD_APP': {'METHOD': 'POST', 'PATH': '/apps/upload'},
-        'STATISTICS': {'METHOD': 'GET', 'PATH': '/service/statistics'},
-        'FILES_LIST': {
-            'METHOD': 'GET',
-            'PATH': '/apps/{app_id}/files/list?path={path}',
-        },
-        'FILES_READ': {
-            'METHOD': 'GET',
-            'PATH': '/apps/{app_id}/files/read?path={path}',
-        },
-        'FILES_CREATE': {
-            'METHOD': 'POST',
-            'PATH': '/apps/{app_id}/files/create',
-        },
-        'FILES_DELETE': {
-            'METHOD': 'DELETE',
-            'PATH': '/apps/{app_id}/files/delete?path={path}',
-        },
-        'LAST_DEPLOYS': {
-            'METHOD': 'GET',
-            'PATH': '/apps/{app_id}/deploy/list',
-        },
-        'GITHUB_INTEGRATION': {
-            'METHOD': 'POST',
-            'PATH': '/apps/{app_id}/deploy/git-webhook',
-        },
-        'CUSTOM_DOMAIN': {
-            'METHOD': 'POST',
-            'PATH': '/apps/{app_id}/network/custom/{custom_domain}',
-        },
-        'DOMAIN_ANALYTICS': {
-            'METHOD': 'GET',
-            'PATH': '/apps/{app_id}/network/analytics',
-        },
-    }
-
-    def __init__(self, name: str) -> None:
-        """
-        The __init__ function is called when the class is instantiated.
-        It sets up the instance of the class, and defines its attributes.
-        The __init__ function takes in a name parameter, which it uses to look
-        up an endpoint from ENDPOINTS_V2.
-        ENDPOINTS_V2 is a dictionary that contains all of our endpoints for
-        version 2 of our API.
-
-        :param self: Represent the instance of the class
-        :param name: str: Set the name of the endpoint
-        :return: None
-        """
-
-        endpoint: Dict[str, Any] = self.ENDPOINTS_V2[name]
-        self.name: str = name
-        self.method: str = endpoint['METHOD']
-        self.path: str = endpoint['PATH']
-
-    def __eq__(self, other: Endpoint):
-        """
-        The __eq__ function is used to compare two objects of the same class.
-        It returns True if they are equal, and False otherwise.
-
-        :param self: Refer to the current instance of the class
-        :param other: Endpoint: Check if the other object is an instance of
-        endpoint
-        :return: A boolean value
-        """
-        return isinstance(other, Endpoint) and self.name == other.name
-
-    def __repr__(self):
-        """
-        The __repr__ function is used to compute the &quot;official&quot;
-        string representation of an object.
-        This is how you would make an object of the class. The goal of
-
-        :param self: Represent the instance of the class
-        :return: A string that is the representation of an object
-        """
-        return f"{Endpoint.__name__}('{self.name}')"
-
-    @classmethod
-    def user_me(cls) -> Endpoint:
-        """Returns an Endpoint object that represents the /user/me endpoint."""
-        return cls('USER_ME')
-
-    @classmethod
-    def app_data(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the /apps/{app_id} endpoint.
-        """
-        return cls('APP_DATA')
-
-    @classmethod
-    def user_info(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the /user/{user_id}
-        endpoint.
-        """
-        return cls('USER_INFO')
-
-    @classmethod
-    def app_status(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/status endpoint.
-        """
-        return cls('APP_STATUS')
-
-    @classmethod
-    def logs(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/logs endpoint.
-        """
-        return cls('LOGS')
-
-    @classmethod
-    def start(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/start endpoint.
-        """
-        return cls('START')
-
-    @classmethod
-    def stop(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/stop endpoint.
-        """
-        return cls('STOP')
-
-    @classmethod
-    def restart(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/restart endpoint.
-        """
-        return cls('RESTART')
-
-    @classmethod
-    def backup(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/backup endpoint.
-        """
-        return cls('BACKUP')
-
-    @classmethod
-    def commit(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/commit endpoint.
-        """
-        return cls('COMMIT')
-
-    @classmethod
-    def delete_app(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/delete endpoint.
-        """
-        return cls('DELETE_APP')
-
-    @classmethod
-    def upload(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/upload endpoint.
-        """
-        return cls('UPLOAD_APP')
-
-    @classmethod
-    def files_list(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/files/list endpoint.
-        """
-        return cls('FILES_LIST')
-
-    @classmethod
-    def files_read(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/files/read endpoint.
-        """
-        return cls('FILES_READ')
-
-    @classmethod
-    def files_create(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/files/create endpoint.
-        """
-        return cls('FILES_CREATE')
-
-    @classmethod
-    def files_delete(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/files/delete endpoint.
-        """
-        return cls('FILES_DELETE')
-
-    @classmethod
-    def statistics(cls) -> Endpoint:
-        """
-        Returns an Endpoint object that represents the
-        /service/statistics endpoint.
-        """
-        return cls('STATISTICS')
-
-    @classmethod
-    def last_deploys(cls):
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/deploy/list endpoint.
-        """
-
-        return cls('LAST_DEPLOYS')
-
-    @classmethod
-    def github_integration(cls):
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/deploy/git-webhook endpoint.
-        """
-        return cls('GITHUB_INTEGRATION')
-
-    @classmethod
-    def domain_analytics(cls):
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/network/analytics endpoint.
-        """
-        return cls('DOMAIN_ANALYTICS')
-
-    @classmethod
-    def custom_domain(cls):
-        """
-        Returns an Endpoint object that represents the
-        /apps/{app_id}/network/custom/{custom_domain} endpoint.
-        """
-        return cls('CUSTOM_DOMAIN')
-
-
-# pylint: disable=too-few-public-methods
-class Router:
-    """Represents a route"""
-
-    # BASE_V1: str = 'https://api.squarecloud.app/v1/public'
-    BASE_V2: str = 'https://api.squarecloud.app/v2'
-
-    # noinspection StrFormat
-    def __init__(self, endpoint: Endpoint, **params) -> None:
-        """
-        The __init__ function is called when the class is instantiated.
-        It sets up the instance of the class, and it's where you define your
-        attributes.
-
-
-        :param self: Represent the instance of the class
-        :param endpoint: Endpoint: Define the endpoint
-        :param **params: Pass in the parameters for the url
-        :return: None
-        """
-        self.endpoint: Endpoint = endpoint
-        self.method: str = endpoint.method
-        self.path: str = endpoint.path
-        url: str = self.BASE_V2 + self.path.format(**params)
-        if params:
-            url.format(params)
-        self.url = url
-
-    def __repr__(self):
-        """
-        The __repr__ function is used to generate a string representation of
-        an object.
-        This function should return a printable representation of the object,
-        and it will be used whenever you call str() on that object.
-
-        :param self: Represent the instance of the class
-        :return: A string that is a valid python expression
-        """
-        return f"{Router.__name__}(path='{self.path}', method='{self.method}')"
+from __future__ import annotations
+
+
+class Endpoint:
+    """Endpoint"""
+
+    # ENDPOINTS_V1 = {
+    #     'USER_ME': {'METHOD': 'GET', 'PATH': '/user'},
+    #     'USER_INFO': {'METHOD': 'GET', 'PATH': '/user/{user_id}'},
+    #     'APP_STATUS': {'METHOD': 'GET', 'PATH': '/status/{app_id}'},
+    #     'LOGS': {'METHOD': 'GET', 'PATH': '/logs/{app_id}'},
+    #     'FULL_LOGS': {'METHOD': 'GET', 'PATH': '/full-logs/{app_id}'},
+    #     'START': {'METHOD': 'POST', 'PATH': '/start/{app_id}'},
+    #     'STOP': {'METHOD': 'POST', 'PATH': '/stop/{app_id}'},
+    #     'RESTART': {'METHOD': 'POST', 'PATH': '/restart/{app_id}'},
+    #     'BACKUP': {'METHOD': 'GET', 'PATH': '/backup/{app_id}'},
+    #     'COMMIT': {'METHOD': 'POST', 'PATH': '/commit/{app_id}'},
+    #     'DELETE': {'METHOD': 'POST', 'PATH': '/delete/{app_id}'},
+    #     'UPLOAD': {'METHOD': 'POST', 'PATH': '/upload'},
+    # }
+
+    ENDPOINTS_V2 = {
+        'USER': {'METHOD': 'GET', 'PATH': '/user'},
+        'APP_DATA': {'METHOD': 'GET', 'PATH': '/apps/{app_id}'},
+        'APP_STATUS': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/status'},
+        'LOGS': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/logs'},
+        'START': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/start'},
+        'STOP': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/stop'},
+        'RESTART': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/restart'},
+        'BACKUP': {'METHOD': 'GET', 'PATH': '/apps/{app_id}/backup'},
+        'COMMIT': {'METHOD': 'POST', 'PATH': '/apps/{app_id}/commit'},
+        'DELETE_APP': {'METHOD': 'DELETE', 'PATH': '/apps/{app_id}/delete'},
+        'UPLOAD_APP': {'METHOD': 'POST', 'PATH': '/apps/upload'},
+        'FILES_LIST': {
+            'METHOD': 'GET',
+            'PATH': '/apps/{app_id}/files/list?path={path}',
+        },
+        'FILES_READ': {
+            'METHOD': 'GET',
+            'PATH': '/apps/{app_id}/files/read?path={path}',
+        },
+        'FILES_CREATE': {
+            'METHOD': 'POST',
+            'PATH': '/apps/{app_id}/files/create',
+        },
+        'FILES_DELETE': {
+            'METHOD': 'DELETE',
+            'PATH': '/apps/{app_id}/files/delete?path={path}',
+        },
+        'LAST_DEPLOYS': {
+            'METHOD': 'GET',
+            'PATH': '/apps/{app_id}/deploy/list',
+        },
+        'GITHUB_INTEGRATION': {
+            'METHOD': 'POST',
+            'PATH': '/apps/{app_id}/deploy/git-webhook',
+        },
+        'CUSTOM_DOMAIN': {
+            'METHOD': 'POST',
+            'PATH': '/apps/{app_id}/network/custom/{custom_domain}',
+        },
+        'DOMAIN_ANALYTICS': {
+            'METHOD': 'GET',
+            'PATH': '/apps/{app_id}/network/analytics',
+        },
+    }
+
+    def __init__(self, name: str) -> None:
+        """
+        The __init__ function is called when the class is instantiated.
+        It sets up the instance of the class, and defines its attributes.
+        The __init__ function takes in a name parameter, which it uses to look
+        up an endpoint from ENDPOINTS_V2.
+        ENDPOINTS_V2 is a dictionary that contains all of our endpoints for
+        version 2 of our API.
+
+        :param self: Represent the instance of the class
+        :param name: str: Set the name of the endpoint
+        :return: None
+        """
+        if not (endpoint := self.ENDPOINTS_V2.get(name)):
+            raise ValueError(f"Invalid endpoint: '{name}'")
+        self.name: str = name
+        self.method: str = endpoint['METHOD']
+        self.path: str = endpoint['PATH']
+
+    def __eq__(self, other: Endpoint):
+        """
+        The __eq__ function is used to compare two objects of the same class.
+        It returns True if they are equal, and False otherwise.
+
+        :param self: Refer to the current instance of the class
+        :param other: Endpoint: Check if the other object is an instance of
+        endpoint
+        :return: A boolean value
+        """
+        return isinstance(other, Endpoint) and self.name == other.name
+
+    def __repr__(self):
+        """
+        The __repr__ function is used to compute the &quot;official&quot;
+        string representation of an object.
+        This is how you would make an object of the class. The goal of
+
+        :param self: Represent the instance of the class
+        :return: A string that is the representation of an object
+        """
+        return f"{Endpoint.__name__}('{self.name}')"
+
+    @classmethod
+    def user(cls) -> Endpoint:
+        """Returns an Endpoint object that represents the /user endpoint."""
+        return cls('USER')
+
+    @classmethod
+    def app_data(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the /apps/{app_id} endpoint.
+        """
+        return cls('APP_DATA')
+
+    @classmethod
+    def app_status(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/status endpoint.
+        """
+        return cls('APP_STATUS')
+
+    @classmethod
+    def logs(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/logs endpoint.
+        """
+        return cls('LOGS')
+
+    @classmethod
+    def start(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/start endpoint.
+        """
+        return cls('START')
+
+    @classmethod
+    def stop(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/stop endpoint.
+        """
+        return cls('STOP')
+
+    @classmethod
+    def restart(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/restart endpoint.
+        """
+        return cls('RESTART')
+
+    @classmethod
+    def backup(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/backup endpoint.
+        """
+        return cls('BACKUP')
+
+    @classmethod
+    def commit(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/commit endpoint.
+        """
+        return cls('COMMIT')
+
+    @classmethod
+    def delete_app(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/delete endpoint.
+        """
+        return cls('DELETE_APP')
+
+    @classmethod
+    def upload(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/upload endpoint.
+        """
+        return cls('UPLOAD_APP')
+
+    @classmethod
+    def files_list(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/files/list endpoint.
+        """
+        return cls('FILES_LIST')
+
+    @classmethod
+    def files_read(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/files/read endpoint.
+        """
+        return cls('FILES_READ')
+
+    @classmethod
+    def files_create(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/files/create endpoint.
+        """
+        return cls('FILES_CREATE')
+
+    @classmethod
+    def files_delete(cls) -> Endpoint:
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/files/delete endpoint.
+        """
+        return cls('FILES_DELETE')
+
+    @classmethod
+    def last_deploys(cls):
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/deploy/list endpoint.
+        """
+
+        return cls('LAST_DEPLOYS')
+
+    @classmethod
+    def github_integration(cls):
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/deploy/git-webhook endpoint.
+        """
+        return cls('GITHUB_INTEGRATION')
+
+    @classmethod
+    def domain_analytics(cls):
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/network/analytics endpoint.
+        """
+        return cls('DOMAIN_ANALYTICS')
+
+    @classmethod
+    def custom_domain(cls):
+        """
+        Returns an Endpoint object that represents the
+        /apps/{app_id}/network/custom/{custom_domain} endpoint.
+        """
+        return cls('CUSTOM_DOMAIN')
+
+
+# pylint: disable=too-few-public-methods
+class Router:
+    """Represents a route"""
+
+    # BASE_V1: str = 'https://api.squarecloud.app/v1/public'
+    BASE_V2: str = 'https://api.squarecloud.app/v2'
+
+    # noinspection StrFormat
+    def __init__(self, endpoint: Endpoint, **params) -> None:
+        """
+        The __init__ function is called when the class is instantiated.
+        It sets up the instance of the class, and it's where you define your
+        attributes.
+
+
+        :param self: Represent the instance of the class
+        :param endpoint: Endpoint: Define the endpoint
+        :param **params: Pass in the parameters for the url
+        :return: None
+        """
+        self.endpoint: Endpoint = endpoint
+        self.method: str = endpoint.method
+        self.path: str = endpoint.path
+        url: str = self.BASE_V2 + self.path.format(**params)
+        if params:
+            url.format(params)
+        self.url = url
+
+    def __repr__(self):
+        """
+        The __repr__ function is used to generate a string representation of
+        an object.
+        This function should return a printable representation of the object,
+        and it will be used whenever you call str() on that object.
+
+        :param self: Represent the instance of the class
+        :return: A string that is a valid python expression
+        """
+        return f"{Router.__name__}(path='{self.path}', method='{self.method}')"
```

### Comparing `squarecloud_api-3.3.2/PKG-INFO` & `squarecloud_api-3.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7371 7561  : 2.1.Name: squa
 00000020: 7265 636c 6f75 642d 6170 690a 5665 7273  recloud-api.Vers
-00000030: 696f 6e3a 2033 2e33 2e32 0a53 756d 6d61  ion: 3.3.2.Summa
+00000030: 696f 6e3a 2033 2e34 2e30 0a53 756d 6d61  ion: 3.4.0.Summa
 00000040: 7279 3a20 5371 7561 7265 436c 6f75 6420  ry: SquareCloud 
 00000050: 4150 4920 7772 6170 7065 720a 486f 6d65  API wrapper.Home
 00000060: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 00000070: 6974 6875 622e 636f 6d2f 7371 7561 7265  ithub.com/square
 00000080: 636c 6f75 646f 6663 2f77 7261 7070 6572  cloudofc/wrapper
 00000090: 2d61 7069 2d70 790a 4c69 6365 6e73 653a  -api-py.License:
 000000a0: 204d 4954 0a41 7574 686f 723a 2052 6f62   MIT.Author: Rob
@@ -37,83 +37,116 @@
 00000240: 3a20 6169 6f68 7474 7020 283d 3d33 2e39  : aiohttp (==3.9
 00000250: 2e33 290a 5265 7175 6972 6573 2d44 6973  .3).Requires-Dis
 00000260: 743a 2063 6c69 636b 2028 3e3d 382e 312e  t: click (>=8.1.
 00000270: 362c 3c39 2e30 2e30 290a 5265 7175 6972  6,<9.0.0).Requir
 00000280: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
 00000290: 6320 283e 3d32 2e35 2e32 2c3c 332e 302e  c (>=2.5.2,<3.0.
 000002a0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000002b0: 3a20 7079 7468 6f6e 2d64 6f74 656e 7620  : python-dotenv 
-000002c0: 283e 3d31 2e30 2e30 2c3c 322e 302e 3029  (>=1.0.0,<2.0.0)
-000002d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000002e0: 7269 6368 2028 3e3d 3133 2e35 2e32 2c3c  rich (>=13.5.2,<
-000002f0: 3134 2e30 2e30 290a 5072 6f6a 6563 742d  14.0.0).Project-
-00000300: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
-00000310: 6f6e 2c20 6874 7470 733a 2f2f 646f 6373  on, https://docs
-00000320: 2e73 7175 6172 6563 6c6f 7564 2e61 7070  .squarecloud.app
-00000330: 2f73 646b 732f 7079 0a50 726f 6a65 6374  /sdks/py.Project
-00000340: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
-00000350: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000360: 2e63 6f6d 2f73 7175 6172 6563 6c6f 7564  .com/squarecloud
-00000370: 6f66 632f 7772 6170 7065 722d 6170 692d  ofc/wrapper-api-
-00000380: 7079 0a44 6573 6372 6970 7469 6f6e 2d43  py.Description-C
-00000390: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000003a0: 742f 6d61 726b 646f 776e 0a0a 5b53 7175  t/markdown..[Squ
-000003b0: 6172 6520 436c 6f75 645d 3a20 6874 7470  are Cloud]: http
-000003c0: 733a 2f2f 7371 7561 7265 636c 6f75 642e  s://squarecloud.
-000003d0: 6170 700a 0a5b 5371 7561 7265 2043 6c6f  app..[Square Clo
-000003e0: 7564 2041 5049 5d3a 2068 7474 7073 3a2f  ud API]: https:/
-000003f0: 2f64 6f63 732e 7371 7561 7265 636c 6f75  /docs.squareclou
-00000400: 642e 6170 702f 6170 692d 7265 6665 7265  d.app/api-refere
-00000410: 6e63 652f 0a0a 5b40 616c 6d61 5d3a 2068  nce/..[@alma]: h
-00000420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000430: 6d2f 526f 6265 7274 2d4e 6f67 7565 6972  m/Robert-Nogueir
-00000440: 610a 0a23 2073 7175 6172 6563 6c6f 7564  a..# squarecloud
-00000450: 2d61 7069 0a0a 7371 7561 7265 636c 6f75  -api..squareclou
-00000460: 642d 6170 6920 6973 2061 2077 7261 7070  d-api is a wrapp
-00000470: 6572 2066 6f72 2074 6865 205b 5371 7561  er for the [Squa
-00000480: 7265 2043 6c6f 7564 2041 5049 5d20 6d61  re Cloud API] ma
-00000490: 696e 7465 6420 6279 205b 4061 6c6d 615d  inted by [@alma]
-000004a0: 0a0a 0a23 2320 496e 7374 616c 6c69 6e67  ...## Installing
-000004b0: 0a0a 6060 6060 0a70 6970 2069 6e73 7461  ..````.pip insta
-000004c0: 6c6c 2073 7175 6172 6563 6c6f 7564 2d61  ll squarecloud-a
-000004d0: 7069 0a60 6060 600a 0a0a 2323 2047 6574  pi.````...## Get
-000004e0: 7469 6e67 2061 7069 206b 6579 0a0a 746f  ting api key..to
-000004f0: 2067 6574 2079 6f75 7220 6170 6920 6b65   get your api ke
-00000500: 792f 746f 6b65 6e20 6a75 7374 2067 6f20  y/token just go 
-00000510: 746f 2074 6865 205b 5371 7561 7265 2043  to the [Square C
-00000520: 6c6f 7564 5d20 7765 6273 6974 6520 616e  loud] website an
-00000530: 640a 7265 6769 7374 6572 2f6c 6f67 696e  d.register/login
-00000540: 2c20 6166 7465 7220 7468 6174 2067 6f0a  , after that go.
-00000550: 746f 2060 6461 7368 626f 6172 6460 203e  to `dashboard` >
-00000560: 2060 6d79 2061 6363 6f75 6e74 6020 3e20   `my account` > 
-00000570: 6052 6567 656e 6572 6174 6520 4150 492f  `Regenerate API/
-00000580: 434c 4920 4b45 5960 2061 6e64 2063 6f70  CLI KEY` and cop
-00000590: 7920 7468 6520 6b65 792e 0a0a 3e20 2323  y the key...> ##
-000005a0: 205b 446f 6375 6d65 6e74 6174 696f 6e5d   [Documentation]
-000005b0: 2868 7474 7073 3a2f 2f64 6f63 732e 7371  (https://docs.sq
-000005c0: 7561 7265 636c 6f75 642e 6170 702f 7364  uarecloud.app/sd
-000005d0: 6b73 2f70 7929 0a3e 2079 6f75 2063 616e  ks/py).> you can
-000005e0: 2072 6561 6420 7468 6520 646f 6375 6d65   read the docume
-000005f0: 6e74 6174 696f 6e20 5b2a 2a68 6572 652a  ntation [**here*
-00000600: 2a5d 2868 7474 7073 3a2f 2f64 6f63 732e  *](https://docs.
-00000610: 7371 7561 7265 636c 6f75 642e 6170 702f  squarecloud.app/
-00000620: 7364 6b73 2f70 7929 2e0a 0a23 2320 4261  sdks/py)...## Ba
-00000630: 7369 6320 7573 6167 650a 6060 6070 7974  sic usage.```pyt
-00000640: 686f 6e0a 696d 706f 7274 2061 7379 6e63  hon.import async
-00000650: 696f 0a0a 696d 706f 7274 2073 7175 6172  io..import squar
-00000660: 6563 6c6f 7564 2061 7320 7371 7561 7265  ecloud as square
-00000670: 0a0a 636c 6965 6e74 203d 2073 7175 6172  ..client = squar
-00000680: 652e 436c 6965 6e74 2827 4150 495f 4b45  e.Client('API_KE
-00000690: 5927 2c20 6465 6275 673d 5472 7565 290a  Y', debug=True).
-000006a0: 0a61 7379 6e63 2064 6566 206d 6169 6e28  .async def main(
-000006b0: 293a 0a20 2020 2073 7461 7475 7320 3d20  ):.    status = 
-000006c0: 6177 6169 7420 636c 6965 6e74 2e61 7070  await client.app
-000006d0: 5f73 7461 7475 7328 6170 705f 6964 3d27  _status(app_id='
-000006e0: 6170 706c 6963 6174 696f 6e5f 6964 2729  application_id')
-000006f0: 0a20 2020 2070 7269 6e74 2873 7461 7475  .    print(statu
-00000700: 7329 0a20 2020 2070 7269 6e74 2873 7461  s).    print(sta
-00000710: 7475 732e 7261 6d29 0a20 2020 2070 7269  tus.ram).    pri
-00000720: 6e74 2873 7461 7475 732e 6370 7529 0a0a  nt(status.cpu)..
-00000730: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
-00000740: 2829 290a 6060 600a 0a23 2320 4c69 6365  ()).```..## Lice
-00000750: 6e73 650a 0a4d 4954 204c 6963 656e 7365  nse..MIT License
-00000760: 0a0a                                     ..
+000002b0: 3a20 7079 7069 2028 3e3d 322e 312c 3c33  : pypi (>=2.1,<3
+000002c0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+000002d0: 743a 2070 7974 686f 6e2d 646f 7465 6e76  t: python-dotenv
+000002e0: 2028 3e3d 312e 302e 302c 3c32 2e30 2e30   (>=1.0.0,<2.0.0
+000002f0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000300: 2072 6963 6820 283e 3d31 332e 352e 322c   rich (>=13.5.2,
+00000310: 3c31 342e 302e 3029 0a50 726f 6a65 6374  <14.0.0).Project
+00000320: 2d55 524c 3a20 446f 6375 6d65 6e74 6174  -URL: Documentat
+00000330: 696f 6e2c 2068 7474 7073 3a2f 2f64 6f63  ion, https://doc
+00000340: 732e 7371 7561 7265 636c 6f75 642e 6170  s.squarecloud.ap
+00000350: 702f 7364 6b73 2f70 790a 5072 6f6a 6563  p/sdks/py.Projec
+00000360: 742d 5552 4c3a 2052 6570 6f73 6974 6f72  t-URL: Repositor
+00000370: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+00000380: 622e 636f 6d2f 7371 7561 7265 636c 6f75  b.com/squareclou
+00000390: 646f 6663 2f77 7261 7070 6572 2d61 7069  dofc/wrapper-api
+000003a0: 2d70 790a 4465 7363 7269 7074 696f 6e2d  -py.Description-
+000003b0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+000003c0: 7874 2f6d 6172 6b64 6f77 6e0a 0a5b 5371  xt/markdown..[Sq
+000003d0: 7561 7265 2043 6c6f 7564 5d3a 2068 7474  uare Cloud]: htt
+000003e0: 7073 3a2f 2f73 7175 6172 6563 6c6f 7564  ps://squarecloud
+000003f0: 2e61 7070 0a0a 5b53 7175 6172 6520 436c  .app..[Square Cl
+00000400: 6f75 6420 4150 495d 3a20 6874 7470 733a  oud API]: https:
+00000410: 2f2f 646f 6373 2e73 7175 6172 6563 6c6f  //docs.squareclo
+00000420: 7564 2e61 7070 2f61 7069 2d72 6566 6572  ud.app/api-refer
+00000430: 656e 6365 2f0a 0a5b 4061 6c6c 6d61 5d3a  ence/..[@allma]:
+00000440: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000450: 636f 6d2f 526f 6265 7274 2d4e 6f67 7565  com/Robert-Nogue
+00000460: 6972 610a 0a0a 3c64 6976 2061 6c69 676e  ira...<div align
+00000470: 3d22 6365 6e74 6572 223e 0a20 203c 696d  ="center">.  <im
+00000480: 6720 616c 743d 2253 7175 6172 6520 436c  g alt="Square Cl
+00000490: 6f75 6420 4261 6e6e 6572 2220 7372 633d  oud Banner" src=
+000004a0: 2268 7474 7073 3a2f 2f63 646e 2e73 7175  "https://cdn.squ
+000004b0: 6172 6563 6c6f 7564 2e61 7070 2f70 6e67  arecloud.app/png
+000004c0: 2f67 6974 6875 622d 7265 6164 6d65 2e70  /github-readme.p
+000004d0: 6e67 223e 0a3c 2f64 6976 3e0a 0a3c 6831  ng">.</div>..<h1
+000004e0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000004f0: 7371 7561 7265 636c 6f75 642d 6170 693c  squarecloud-api<
+00000500: 2f68 313e 0a0a 3c70 2061 6c69 676e 3d22  /h1>..<p align="
+00000510: 6365 6e74 6572 223e 4120 5079 7468 6f6e  center">A Python
+00000520: 2053 444b 2066 6f72 2063 6f6e 7375 6d69   SDK for consumi
+00000530: 6e67 2074 6865 203c 6120 6872 6566 3d22  ng the <a href="
+00000540: 6874 7470 733a 2f2f 7371 7561 7265 636c  https://squarecl
+00000550: 6f75 642e 6170 7022 2074 6172 6765 743d  oud.app" target=
+00000560: 225f 626c 616e 6b22 3e53 7175 6172 6520  "_blank">Square 
+00000570: 436c 6f75 643c 2f61 3e20 4150 492e 3c2f  Cloud</a> API.</
+00000580: 703e 0a0a 2323 2049 6e73 7461 6c6c 6174  p>..## Installat
+00000590: 696f 6e0a 0a60 6060 6073 6865 6c6c 0a70  ion..````shell.p
+000005a0: 6970 2069 6e73 7461 6c6c 2073 7175 6172  ip install squar
+000005b0: 6563 6c6f 7564 2d61 7069 0a60 6060 600a  ecloud-api.````.
+000005c0: 0a49 6620 796f 7520 696e 7465 6e64 2074  .If you intend t
+000005d0: 6f20 7573 6520 7468 6973 2053 444b 2066  o use this SDK f
+000005e0: 6f72 2063 6f6d 6d61 6e64 2d6c 696e 6520  or command-line 
+000005f0: 696e 7465 7266 6163 6520 2843 4c49 2920  interface (CLI) 
+00000600: 6f70 6572 6174 696f 6e73 2c20 636f 6e73  operations, cons
+00000610: 6964 6572 0a69 6e73 7461 6c6c 696e 6720  ider.installing 
+00000620: 6974 2077 6974 6820 7069 7078 3a0a 6060  it with pipx:.``
+00000630: 6060 7368 656c 6c0a 7069 7078 2069 6e73  ``shell.pipx ins
+00000640: 7461 6c6c 2073 7175 6172 6563 6c6f 7564  tall squarecloud
+00000650: 2d61 7069 0a60 6060 600a 0a23 2320 4765  -api.````..## Ge
+00000660: 7474 696e 6720 6170 6920 6b65 790a 0a74  tting api key..t
+00000670: 6f20 6765 7420 796f 7572 2061 7069 206b  o get your api k
+00000680: 6579 2f74 6f6b 656e 206a 7573 7420 676f  ey/token just go
+00000690: 2074 6f20 7468 6520 5b53 7175 6172 6520   to the [Square 
+000006a0: 436c 6f75 645d 2077 6562 7369 7465 2061  Cloud] website a
+000006b0: 6e64 0a72 6567 6973 7465 722f 6c6f 6769  nd.register/logi
+000006c0: 6e2c 2061 6674 6572 2074 6861 7420 676f  n, after that go
+000006d0: 0a74 6f20 6064 6173 6862 6f61 7264 6020  .to `dashboard` 
+000006e0: 3e20 606d 7920 6163 636f 756e 7460 203e  > `my account` >
+000006f0: 2060 5265 6765 6e65 7261 7465 2041 5049   `Regenerate API
+00000700: 2f43 4c49 204b 4559 6020 616e 6420 636f  /CLI KEY` and co
+00000710: 7079 2074 6865 206b 6579 2e0a 0a23 2320  py the key...## 
+00000720: 446f 6375 6d65 6e74 6174 696f 6e0a 5669  Documentation.Vi
+00000730: 7369 7420 6f75 7220 5b6f 6666 6963 6961  sit our [officia
+00000740: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00000750: 2868 7474 7073 3a2f 2f64 6f63 732e 7371  (https://docs.sq
+00000760: 7561 7265 636c 6f75 642e 6170 702f 7364  uarecloud.app/sd
+00000770: 6b73 2f70 7929 2066 6f72 206d 6f72 6520  ks/py) for more 
+00000780: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00000790: 7420 686f 7720 746f 2075 7365 2074 6869  t how to use thi
+000007a0: 7320 6c69 6272 6172 792e 0a0a 2323 2047  s library...## G
+000007b0: 6574 7469 6e67 2073 7461 7274 6564 0a0a  etting started..
+000007c0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+000007d0: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
+000007e0: 7371 7561 7265 636c 6f75 6420 6173 2073  squarecloud as s
+000007f0: 7175 6172 650a 0a63 6c69 656e 7420 3d20  quare..client = 
+00000800: 7371 7561 7265 2e43 6c69 656e 7428 2741  square.Client('A
+00000810: 5049 5f4b 4559 2729 0a0a 6173 796e 6320  PI_KEY')..async 
+00000820: 6465 6620 6d61 696e 2829 3a0a 2020 2020  def main():.    
+00000830: 7374 6174 7573 203d 2061 7761 6974 2063  status = await c
+00000840: 6c69 656e 742e 6170 705f 7374 6174 7573  lient.app_status
+00000850: 2861 7070 5f69 643d 2761 7070 6c69 6361  (app_id='applica
+00000860: 7469 6f6e 5f69 6427 290a 2020 2020 7072  tion_id').    pr
+00000870: 696e 7428 7374 6174 7573 290a 2020 2020  int(status).    
+00000880: 7072 696e 7428 7374 6174 7573 2e72 616d  print(status.ram
+00000890: 290a 2020 2020 7072 696e 7428 7374 6174  ).    print(stat
+000008a0: 7573 2e63 7075 290a 0a61 7379 6e63 696f  us.cpu)..asyncio
+000008b0: 2e72 756e 286d 6169 6e28 2929 0a60 6060  .run(main()).```
+000008c0: 0a0a 2323 2043 6f6e 7472 6962 7574 696e  ..## Contributin
+000008d0: 670a 0a46 6565 6c20 6672 6565 2074 6f20  g..Feel free to 
+000008e0: 636f 6e74 7269 6275 7465 2077 6974 6820  contribute with 
+000008f0: 7375 6767 6573 7469 6f6e 7320 6f72 2062  suggestions or b
+00000900: 7567 2072 6570 6f72 7473 2061 7420 6f75  ug reports at ou
+00000910: 7220 5b47 6974 4875 6220 7265 706f 7369  r [GitHub reposi
+00000920: 746f 7279 5d28 6874 7470 733a 2f2f 6769  tory](https://gi
+00000930: 7468 7562 2e63 6f6d 2f73 7175 6172 6563  thub.com/squarec
+00000940: 6c6f 7564 6f66 632f 7772 6170 7065 722d  loudofc/wrapper-
+00000950: 6170 692d 7079 292e 0a0a 2323 2041 7574  api-py)...## Aut
+00000960: 686f 7273 0a0a 2d20 5b40 616c 6c6d 615d  hors..- [@allma]
+00000970: 0a0a                                     ..
```

