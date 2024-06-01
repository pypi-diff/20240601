# Comparing `tmp/ltasg-0.0.6.tar.gz` & `tmp/ltasg-0.0.6.post1.tar.gz`

## Comparing `ltasg-0.0.6.tar` & `ltasg-0.0.6.post1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ltasg-0.0.6/main.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.6/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/__init__.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/api.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/constants.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/traffic.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/helpers/helpers.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/transport/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/transport/bus.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/transport/taxi.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/transport/train.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.6/src/ltasg/transport/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.6/test/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.6/test/test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.6/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.6/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.6/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/main.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/requirements.txt
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/api.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/constants.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/traffic.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/helpers/helpers.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/transport/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/transport/bus.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/transport/taxi.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/transport/train.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/src/ltasg/transport/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/test/__init__.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/test/test.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/pyproject.toml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ltasg-0.0.6.post1/PKG-INFO
```

### Comparing `ltasg-0.0.6/src/ltasg/transport/bus.py` & `ltasg-0.0.6.post1/src/ltasg/transport/bus.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from ..transport.transport import Transport
-from ..constants import TransportType
-from ..helpers.helpers import transform_data
-
-
-class Bus(Transport):
-    def __init__(self, base_url, api_key) -> None:
-        super().__init__(base_url=base_url,api_key= api_key)
-        self.bus_services = self.transport_services[TransportType.BUS]
-    
-    async def arrival(self, bus_stop_code: int, bus_no: int):
-        data = await self.lta_api.fetch(self.bus_services['ARRIVAL'], query_params={
-            "BusStopCode": bus_stop_code,
-            "ServiceNo": bus_no
-        })
-        return data["Services"]
-    
-    async def services(self):
-        data = await self.lta_api.fetch(self.bus_services['SERVICES'])
-        return transform_data(data)
-    async def stop_services(self, bus_stop_code):
-        data = transform_data(await self.lta_api.fetch(self.bus_services['ROUTES']))
-        services = [ service["ServiceNo"] for service in data if service['BusStopCode'] == str(bus_stop_code)]
-        return services
-    async def routes(self):
-        data = await self.lta_api.fetch(self.bus_services['ROUTES'])
-        return transform_data(data)
-
-    async def stops(self):
-        data = await self.lta_api.fetch(self.bus_services['STOPS'])
-        return transform_data(data)
+from ..transport.transport import Transport
+from ..constants import TransportType
+from ..helpers.helpers import transform_data
+
+
+class Bus(Transport):
+    def __init__(self, base_url, api_key) -> None:
+        super().__init__(base_url=base_url,api_key= api_key)
+        self.bus_services = self.transport_services[TransportType.BUS]
+    
+    async def arrival(self, bus_stop_code: int, bus_no: int):
+        data = await self.lta_api.fetch(self.bus_services['ARRIVAL'], query_params={
+            "BusStopCode": bus_stop_code,
+            "ServiceNo": bus_no
+        })
+        return data["Services"]
+    
+    async def services(self):
+        data = await self.lta_api.fetch(self.bus_services['SERVICES'])
+        return transform_data(data)
+    async def stop_services(self, bus_stop_code):
+        data = transform_data(await self.lta_api.fetch(self.bus_services['ROUTES']))
+        services = [ service["ServiceNo"] for service in data if service['BusStopCode'] == str(bus_stop_code)]
+        return services
+    async def routes(self):
+        data = await self.lta_api.fetch(self.bus_services['ROUTES'])
+        return transform_data(data)
+
+    async def stops(self):
+        data = await self.lta_api.fetch(self.bus_services['STOPS'])
+        return transform_data(data)
```

### Comparing `ltasg-0.0.6/src/ltasg/transport/taxi.py` & `ltasg-0.0.6.post1/src/ltasg/transport/taxi.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from ..transport.transport import Transport
-from ..constants import TransportType
-from ..helpers.helpers import transform_data
-
-class Taxi(Transport):
-    def __init__(self, base_url, api_key) -> None:
-        super().__init__(base_url=base_url,api_key= api_key)
-        self.taxi_services = self.transport_services[TransportType.TAXI]
-
-    async def availability(self):
-        data = await self.lta_api.fetch(self.taxi_services["AVAILABILITY"])
-        return transform_data(data)
-    
-    async def stands(self):
-        data = await self.lta_api.fetch(self.taxi_services["STANDS"])
+from ..transport.transport import Transport
+from ..constants import TransportType
+from ..helpers.helpers import transform_data
+
+class Taxi(Transport):
+    def __init__(self, base_url, api_key) -> None:
+        super().__init__(base_url=base_url,api_key= api_key)
+        self.taxi_services = self.transport_services[TransportType.TAXI]
+
+    async def availability(self):
+        data = await self.lta_api.fetch(self.taxi_services["AVAILABILITY"])
+        return transform_data(data)
+    
+    async def stands(self):
+        data = await self.lta_api.fetch(self.taxi_services["STANDS"])
         return transform_data(data)
```

### Comparing `ltasg-0.0.6/.gitignore` & `ltasg-0.0.6.post1/.gitignore`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-# Vscode settings
-.vscode
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# Vscode settings
+.vscode
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
```

### Comparing `ltasg-0.0.6/PKG-INFO` & `ltasg-0.0.6.post1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ltasg
-Version: 0.0.6
+Version: 0.0.6.post1
 Summary: A LTA Datamall API Wrapper Library for Python
 Project-URL: Homepage, https://github.com/ashe/ltasg
 Project-URL: Issues, https://github.com/ashe/ltasg/issues
 Author-email: Aw Sheng Xiang <awshengxiang@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

