# Comparing `tmp/dj_shop_cart-7.0.3.tar.gz` & `tmp/dj_shop_cart-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_shop_cart-7.0.3.tar", max compression
+gzip compressed data, was "dj_shop_cart-7.1.0.tar", max compression
```

## Comparing `dj_shop_cart-7.0.3.tar` & `dj_shop_cart-7.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1086 2022-03-12 08:29:42.000000 dj_shop_cart-7.0.3/LICENSE
--rw-r--r--   0        0        0     3947 2023-03-28 08:19:35.296580 dj_shop_cart-7.0.3/README.md
--rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-7.0.3/dj_shop_cart/__init__.py
--rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-7.0.3/dj_shop_cart/apps.py
--rw-r--r--   0        0        0    10400 2023-06-06 14:36:13.645013 dj_shop_cart-7.0.3/dj_shop_cart/cart.py
--rw-r--r--   0        0        0     1236 2022-06-23 07:20:53.000000 dj_shop_cart-7.0.3/dj_shop_cart/conf.py
--rw-r--r--   0        0        0      212 2022-03-19 11:48:30.000000 dj_shop_cart-7.0.3/dj_shop_cart/context_processors.py
--rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-7.0.3/dj_shop_cart/migrations/0001_initial.py
--rw-r--r--   0        0        0      351 2023-02-27 16:50:20.854935 dj_shop_cart-7.0.3/dj_shop_cart/migrations/0002_rename_items_cart_data.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.3/dj_shop_cart/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-7.0.3/dj_shop_cart/models.py
--rw-r--r--   0        0        0     1205 2023-06-06 14:40:10.145584 dj_shop_cart-7.0.3/dj_shop_cart/protocols.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.0.3/dj_shop_cart/py.typed
--rw-r--r--   0        0        0     2419 2023-02-27 17:39:56.532528 dj_shop_cart-7.0.3/dj_shop_cart/storages.py
--rw-r--r--   0        0        0      202 2022-03-19 18:55:22.000000 dj_shop_cart-7.0.3/dj_shop_cart/utils.py
--rw-r--r--   0        0        0     1727 2023-06-06 14:40:23.676504 dj_shop_cart-7.0.3/pyproject.toml
--rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 dj_shop_cart-7.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-06-01 09:50:11.672798 dj_shop_cart-7.1.0/LICENSE
+-rw-r--r--   0        0        0     3728 2024-06-01 09:50:11.673798 dj_shop_cart-7.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-7.1.0/dj_shop_cart/__init__.py
+-rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-7.1.0/dj_shop_cart/apps.py
+-rw-r--r--   0        0        0    10358 2024-06-01 10:40:32.489171 dj_shop_cart-7.1.0/dj_shop_cart/cart.py
+-rw-r--r--   0        0        0     1236 2022-06-23 07:20:53.000000 dj_shop_cart-7.1.0/dj_shop_cart/conf.py
+-rw-r--r--   0        0        0      212 2022-03-19 11:48:30.000000 dj_shop_cart-7.1.0/dj_shop_cart/context_processors.py
+-rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/migrations/0001_initial.py
+-rw-r--r--   0        0        0      351 2023-02-27 16:50:20.854935 dj_shop_cart-7.1.0/dj_shop_cart/migrations/0002_rename_items_cart_data.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-7.1.0/dj_shop_cart/models.py
+-rw-r--r--   0        0        0      435 2023-08-08 08:20:31.233795 dj_shop_cart-7.1.0/dj_shop_cart/protocols.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/py.typed
+-rw-r--r--   0        0        0     2419 2023-02-27 17:39:56.532528 dj_shop_cart-7.1.0/dj_shop_cart/storages.py
+-rw-r--r--   0        0        0      202 2022-03-19 18:55:22.000000 dj_shop_cart-7.1.0/dj_shop_cart/utils.py
+-rw-r--r--   0        0        0     1720 2024-06-01 10:41:26.954157 dj_shop_cart-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 dj_shop_cart-7.1.0/PKG-INFO
```

### Comparing `dj_shop_cart-7.0.3/LICENSE` & `dj_shop_cart-7.1.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020, 2021 Samuel Colvin
+Copyright (c) 2022, DEGNON Tobi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dj_shop_cart-7.0.3/README.md` & `dj_shop_cart-7.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 ```
 
 ## Used By
 
 This project is used by the following companies:
 
 - [Fêmy bien être](https://www.femybienetre.com/)
+- [Bjørn Art](https://bjornart.dk/)
 
 ## Development
 
 Poetry is required (not really, you can set up the environment however you want and install the requirements
 manually) to set up a virtualenv, install it then run the following:
 
 ```sh
@@ -124,12 +125,7 @@
 pytest
 ```
 
 ## Feedback
 
 If you have any feedback, please reach out to me at tobidegnon@proton.me.
 
-## Credits
-
-Thanks to [Jetbrains](https://jb.gg/OpenSource) for providing an Open Source license for this project.
-
-<img height="200" src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo (Main) logo.">
```

### Comparing `dj_shop_cart-7.0.3/dj_shop_cart/cart.py` & `dj_shop_cart-7.1.0/dj_shop_cart/cart.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             product_model_path=f"{product.__class__.__module__}.{product.__class__.__name__}",
             metadata=metadata,
         )
 
 
 @define(kw_only=True)
 class Cart:
-    request: HttpRequest
     storage: Storage
     prefix: str = field(default=DEFAULT_CART_PREFIX)
     _metadata: dict = field(factory=dict)
     _items: list[CartItem] = Factory(list)
 
     def __len__(self) -> int:
         return self.unique_count
@@ -275,15 +274,15 @@
             self._metadata = {}
         self.save()
 
     @classmethod
     def new(cls, request: HttpRequest, prefix: str = DEFAULT_CART_PREFIX) -> Cart:
         """Appropriately create a new cart instance. This builder load existing cart if needed."""
         storage = get_module(conf.CART_STORAGE_BACKEND)(request)
-        instance = cls(request=request, storage=storage, prefix=prefix)
+        instance = cls(storage=storage, prefix=prefix)
         try:
             data = storage.load().get(prefix, {})
         except AttributeError:
             data = {}
 
         metadata = data.get("metadata", {})
         items = data.get("items", [])
```

### Comparing `dj_shop_cart-7.0.3/dj_shop_cart/conf.py` & `dj_shop_cart-7.1.0/dj_shop_cart/conf.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.3/dj_shop_cart/migrations/0001_initial.py` & `dj_shop_cart-7.1.0/dj_shop_cart/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.3/dj_shop_cart/storages.py` & `dj_shop_cart-7.1.0/dj_shop_cart/storages.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.0.3/pyproject.toml` & `dj_shop_cart-7.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-shop-cart"
-version = "7.0.3"
+version = "7.1.0"
 description = "Simple django cart manager for your django projects."
 authors = ["Tobi DEGNON <tobidegnon@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tobi-De/dj-shop-cart"
 homepage = "https://tobi-de.github.io/dj-shop-cart/"
 keywords = ["django", "python", "cart", "shop", "ecommerce"]
@@ -21,31 +21,31 @@
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-Django = ">=3.0"
-attrs = "^22.2.0"
+python = "^3.10"
+Django = "^4.0"
+attrs = "^23.2.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
-pytest-django = "^4.5.2"
-mypy = "^1.1.1"
-pre-commit = "^3.2.1"
-black = "^23.1.0"
-isort = "^5.12.0"
-django-stubs = "^1.16.0"
-factory-boy = "^3.2.1"
-ipython = "^8.11.0"
-redis = "^4.5.3"
-hiredis = "^2.2.2"
-pytest-pretty = "^1.1.1"
+pytest = "^8.2.1"
+pytest-django = "^4.8.0"
+mypy = "^1.10.0"
+pre-commit = "^3.7.1"
+black = "^24.4.2"
+isort = "^5.13.2"
+django-stubs = "^5.0.2"
+factory-boy = "^3.3.0"
+ipython = "^8.25.0"
+redis = "^5.0.4"
+hiredis = "^2.3.2"
+pytest-pretty = "^1.2.0"
 
 [tool.black]
 target-version = ['py37']
 
 [tool.isort]
 profile = "black"
 add_imports = "from __future__ import annotations"
@@ -62,9 +62,9 @@
 allow_untyped_defs = true
 
 [tool.pytest.ini_options]
 addopts = "--ds=tests.settings --reuse-db"
 python_files = ["tests.py", "test_*.py"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dj_shop_cart-7.0.3/PKG-INFO` & `dj_shop_cart-7.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: dj-shop-cart
-Version: 7.0.3
+Version: 7.1.0
 Summary: Simple django cart manager for your django projects.
 Home-page: https://tobi-de.github.io/dj-shop-cart/
 License: MIT
 Keywords: django,python,cart,shop,ecommerce
 Author: Tobi DEGNON
 Author-email: tobidegnon@protonmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=3.0)
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Django (>=4.0,<5.0)
+Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Project-URL: Repository, https://github.com/Tobi-De/dj-shop-cart
 Description-Content-Type: text/markdown
 
 # dj-shop-cart
 
 A simple and flexible cart manager for your django projects.
 
@@ -134,14 +132,15 @@
 ```
 
 ## Used By
 
 This project is used by the following companies:
 
 - [Fêmy bien être](https://www.femybienetre.com/)
+- [Bjørn Art](https://bjornart.dk/)
 
 ## Development
 
 Poetry is required (not really, you can set up the environment however you want and install the requirements
 manually) to set up a virtualenv, install it then run the following:
 
 ```sh
@@ -155,13 +154,8 @@
 pytest
 ```
 
 ## Feedback
 
 If you have any feedback, please reach out to me at tobidegnon@proton.me.
 
-## Credits
-
-Thanks to [Jetbrains](https://jb.gg/OpenSource) for providing an Open Source license for this project.
-
-<img height="200" src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" alt="JetBrains Logo (Main) logo.">
```

