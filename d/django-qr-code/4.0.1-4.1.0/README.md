# Comparing `tmp/django-qr-code-4.0.1.tar.gz` & `tmp/django_qr_code-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-qr-code-4.0.1.tar", last modified: Sun Jan  7 12:45:33 2024, max compression
+gzip compressed data, was "django_qr_code-4.1.0.tar", last modified: Sat Jun  1 13:11:05 2024, max compression
```

## Comparing `django-qr-code-4.0.1.tar` & `django_qr_code-4.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     9278 2024-01-07 12:45:05.000000 django-qr-code-4.0.1/CHANGELOG.md
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     1529 2021-11-16 21:38:16.000000 django-qr-code-4.0.1/LICENSE
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       55 2021-01-23 20:27:44.000000 django-qr-code-4.0.1/MANIFEST.in
--rw-r--r--   0 philippe  (1000) philippe  (1000)    30217 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/PKG-INFO
--rw-rw-r--   0 philippe  (1000) philippe  (1000)    29259 2024-01-03 23:20:15.000000 django-qr-code-4.0.1/README.md
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/django_qr_code.egg-info/
--rw-r--r--   0 philippe  (1000) philippe  (1000)    30217 2024-01-07 12:45:33.000000 django-qr-code-4.0.1/django_qr_code.egg-info/PKG-INFO
--rw-rw-r--   0 philippe  (1000) philippe  (1000)      501 2024-01-07 12:45:33.000000 django-qr-code-4.0.1/django_qr_code.egg-info/SOURCES.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2024-01-07 12:45:33.000000 django-qr-code-4.0.1/django_qr_code.egg-info/dependency_links.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       37 2024-01-07 12:45:33.000000 django-qr-code-4.0.1/django_qr_code.egg-info/requires.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)        8 2024-01-07 12:45:33.000000 django-qr-code-4.0.1/django_qr_code.egg-info/top_level.txt
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/qr_code/
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       22 2024-01-03 23:39:07.000000 django-qr-code-4.0.1/qr_code/__init__.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)      124 2022-02-20 23:50:56.000000 django-qr-code-4.0.1/qr_code/apps.py
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/qr_code/qrcode/
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       92 2024-01-03 22:02:59.000000 django-qr-code-4.0.1/qr_code/qrcode/__init__.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)      841 2022-02-20 23:50:56.000000 django-qr-code-4.0.1/qr_code/qrcode/constants.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     5444 2024-01-03 22:02:59.000000 django-qr-code-4.0.1/qr_code/qrcode/maker.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     7559 2024-01-03 22:02:59.000000 django-qr-code-4.0.1/qr_code/qrcode/serve.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)    38004 2024-01-03 23:38:12.000000 django-qr-code-4.0.1/qr_code/qrcode/utils.py
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/qr_code/templatetags/
--rw-r--r--   0 philippe  (1000) philippe  (1000)        0 2018-03-08 16:56:52.000000 django-qr-code-4.0.1/qr_code/templatetags/__init__.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     8309 2024-01-03 22:02:59.000000 django-qr-code-4.0.1/qr_code/templatetags/qr_code.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)      286 2022-02-20 23:50:56.000000 django-qr-code-4.0.1/qr_code/urls.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     6135 2022-07-28 16:40:40.000000 django-qr-code-4.0.1/qr_code/views.py
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2024-01-07 12:45:33.266524 django-qr-code-4.0.1/setup.cfg
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     1473 2024-01-03 23:38:12.000000 django-qr-code-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:05.307239 django_qr_code-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-06-01 13:11:05.303239 django_qr_code-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:05.303239 django_qr_code-4.1.0/django_qr_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-06-01 13:11:05.000000 django_qr_code-4.1.0/django_qr_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-01 13:11:05.000000 django_qr_code-4.1.0/django_qr_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:11:05.000000 django_qr_code-4.1.0/django_qr_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-01 13:11:05.000000 django_qr_code-4.1.0/django_qr_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 13:11:05.000000 django_qr_code-4.1.0/django_qr_code.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:05.303239 django_qr_code-4.1.0/qr_code/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:05.303239 django_qr_code-4.1.0/qr_code/qrcode/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/qrcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/qrcode/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/qrcode/maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/qrcode/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37810 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/qrcode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:05.303239 django_qr_code-4.1.0/qr_code/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/templatetags/qr_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/qr_code/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:11:05.307239 django_qr_code-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-06-01 13:11:01.000000 django_qr_code-4.1.0/setup.py
```

### Comparing `django-qr-code-4.0.1/CHANGELOG.md` & `django_qr_code-4.1.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # Change Log
 
-# 4.0.1 (2024-01-04)
+## 4.1.0 (2024-06-01)
+* Upgrade dependencies and drop support for Python < 3.10 and Pydantic <2.7.
+* Add the capability to generate embedded Base64 SVG images as data URIs through template tags (in addition to the API capability introduced in version 4.0.1).
+* Add support for alternative text customization (both template tags and API).
+* Add support for CSS classes injection (both template tags and API).
+* Reorganize and improve documentation.
+
+## 4.0.1 (2024-01-04)
 * Upgrade dependencies, and drop support for Pydantic <2.5, Django<4.2, Python 3.8
 * Remove dependency to pytz.
 * Add support for Python 3.12.
 * Add support for Django 5.0.
 * Introduce support for floating point size QR code modules.
 * Introduce embedded Base64 SVG image as data URI.
 * Behavior change: white background is no longer interpreted as transparent for SVG output (#41). If you want to avoid path fill of SVG to reduce the size of the SVG image, you have to explicitly set `light_color` to `None` in `QRCodeOptions`.
 
 ## 3.1.2 (2023-04-10)
 * Fix bug in `WifiConfig` data class (#43).
 * Fix typo in documentation (#45)
 * Add support for Django 4.1 and Django 4.2.
 * Add support for Python 3.11.
+* Improved documentation.
 
 ## 3.1.1 (2022-07-28)
 * Fix regression in demo site due to improper runtime type validation on `QRCodeOptions`.
 * Minor improvements to documentation.
 * Modernize code syntax for Python >= 3.7.
 
 ## 3.1.0 (2022-06-26)
```

### Comparing `django-qr-code-4.0.1/LICENSE` & `django_qr_code-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-qr-code-4.0.1/qr_code/qrcode/constants.py` & `django_qr_code-4.1.0/qr_code/qrcode/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
-from typing import Optional, Union
+from typing import Optional
 
 QR_CODE_GENERATION_VERSION_DATE: datetime = datetime(year=2020, month=9, day=8, hour=12)
 SIZE_DICT: dict = {"t": 6, "s": 12, "m": 18, "l": 30, "h": 48}
 ERROR_CORRECTION_DICT: dict = {"L": "l", "M": "m", "Q": "q", "H": "h"}
-DEFAULT_MODULE_SIZE: Union[str, int] = "m"
+DEFAULT_MODULE_SIZE: str | int = "m"
 DEFAULT_BORDER_SIZE: int = 4
 DEFAULT_VERSION: Optional[int] = None
 DEFAULT_IMAGE_FORMAT: str = "svg"
 DEFAULT_ERROR_CORRECTION: str = "m"
 DEFAULT_ECI: bool = False
 DEFAULT_BOOST_ERROR: bool = True
 DEFAULT_ENCODING: str = "utf-8"
```

### Comparing `django-qr-code-4.0.1/qr_code/qrcode/serve.py` & `django_qr_code-4.1.0/qr_code/qrcode/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import urllib.parse
 from collections.abc import Mapping
 from datetime import datetime
-from typing import Optional, Union, Any
+from typing import Optional, Any
 
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser, User
 from django.core.signing import Signer
 from django.urls import reverse
 from django.utils.crypto import get_random_string
 from django.utils.encoding import force_str
@@ -28,30 +28,30 @@
 
 def _get_url_protection_settings() -> Optional[Mapping]:
     if hasattr(settings, "QR_CODE_URL_PROTECTION") and isinstance(settings.QR_CODE_URL_PROTECTION, Mapping):
         return settings.QR_CODE_URL_PROTECTION
     return None
 
 
-def _options_allow_external_request(url_protection_options: Mapping, user: Union[User, AnonymousUser, None]) -> bool:
+def _options_allow_external_request(url_protection_options: Mapping, user: User | AnonymousUser | None) -> bool:
     # Evaluate the callable if required.
     if callable(url_protection_options[constants.ALLOWS_EXTERNAL_REQUESTS_FOR_REGISTERED_USER]):
         allows_external_request = url_protection_options[constants.ALLOWS_EXTERNAL_REQUESTS_FOR_REGISTERED_USER](user or AnonymousUser())
     elif url_protection_options[constants.ALLOWS_EXTERNAL_REQUESTS_FOR_REGISTERED_USER] is True:
         allows_external_request = user and user.pk and user.is_authenticated
     else:
         allows_external_request = False
     return allows_external_request
 
 
-def requires_url_protection_token(user: Union[User, AnonymousUser, None] = None) -> bool:
+def requires_url_protection_token(user: User | AnonymousUser | None = None) -> bool:
     return not _options_allow_external_request(get_url_protection_options(), user)
 
 
-def allows_external_request_from_user(user: Union[User, AnonymousUser, None] = None) -> bool:
+def allows_external_request_from_user(user: User | AnonymousUser | None = None) -> bool:
     return _options_allow_external_request(get_url_protection_options(), user)
 
 
 def get_url_protection_options() -> dict:
     options = _get_default_url_protection_options()
     settings_options = _get_url_protection_settings()
     if settings_options is not None:
```

### Comparing `django-qr-code-4.0.1/qr_code/qrcode/utils.py` & `django_qr_code-4.1.0/qr_code/qrcode/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,53 +52,50 @@
         dark_module_color: Union[tuple, str, bool, None] = False,
         quiet_zone_color: Union[tuple, str, bool, None] = False,
     ) -> None:
         """
         :param size: The size of the QR code as an integer, float, Decimal or a string. Default is *'m'*.
         :type: str, int, float or Decimal
         :param int border: The size of the border (blank space around the code).
-        :param version: The version of the QR code gives the size of the matrix.
-            Default is *None* which mean automatic in order to avoid data overflow.
-        :param version: QR Code version. If the value is ``None`` (default), the
-            minimal version which fits for the input data will be used.
-            Valid values: "M1", "M2", "M3", "M4" (for Micro QR codes) or an
-            integer between 1 and 40 (for QR codes).
-            The `version` parameter is case insensitive.
+        :param version: The version of the QR code gives the size of the matrix. Default is *None* which mean automatic
+            in order to avoid data overflow.
+
+        :param version: QR Code version. If the value is ``None`` (default), the minimal version which fits for the
+            input data will be used. Valid values: "M1", "M2", "M3", "M4" (for Micro QR codes) or an integer between
+            1 and 40 (for QR codes). The `version` parameter is case insensitive.
+
         :type version: int, str or None
-        :param str image_format: The graphics format used to render the QR code.
-            It can be either *'svg'* or *'png'*. Default is *'svg'*.
-        :param str error_correction: How much error correction that might be required
-            to read the code. It can be either *'L'*, *'M'*, *'Q'*, or *'H'*. Default is *'M'*.
+        :param str image_format: The graphics format used to render the QR code. It can be either *'svg'* or *'png'*. Default is *'svg'*.
+        :param str error_correction: How much error correction that might be required to read the code. It can be
+            either *'L'*, *'M'*, *'Q'*, or *'H'*. Default is *'M'*.
+
         :param bool boost_error: Tells whether the QR code encoding engine tries to increase the error correction level
-            if it does not affect the version. Error correction level is not increased when it impacts the version of
-            the code.
+            if it does not affect the version. Error correction level is not increased when it impacts the version of the code.
+
         :param bool micro: Indicates if a Micro QR Code should be created. Default: False
-        :param encoding: Indicates the encoding in mode "byte". By default
-            `encoding` is ``UTF-8``. When set to ``None``, the implementation tries to use the standard conform
-            ISO/IEC 8859-1 encoding and if it does not fit, it will use UTF-8. Note that no ECI mode indicator is
-            inserted by default (see :paramref:`eci`).
-            The `encoding` parameter is case-insensitive.
+        :param encoding: Indicates the encoding in mode "byte". By default `encoding` is ``UTF-8``. When set to
+            ``None``, the implementation tries to use the standard conform ISO/IEC 8859-1 encoding and if it does not
+            fit, it will use UTF-8. Note that no ECI mode indicator is inserted by default (see ``eci``). The `encoding`
+            parameter is case-insensitive.
+
         :type encoding: str or None
-        :param bool eci: Indicates if binary data which does not use the default
-            encoding (ISO/IEC 8859-1) should enforce the ECI mode. Since a lot
-            of QR code readers do not support the ECI mode, this feature is
-            disabled by default and the data is encoded in the provided
-            `encoding` using the usual "byte" mode. Set `eci` to ``True`` if
-            an ECI header should be inserted into the QR Code. Note that
-            the implementation may not know the ECI designator for the provided
-            `encoding` and may raise an exception if the ECI designator cannot
-            be found.
-            The ECI mode is not supported by Micro QR Codes.
-        :param dark_color: Color of the dark modules (default: black). The
-            color can be provided as ``(R, G, B)`` tuple, as hexadecimal
-            format (``#RGB``, ``#RRGGBB`` ``RRGGBBAA``), or web color
-            name (i.e. ``red``). If alpha transparency is supported (i.e. PNG and SVG), hexadecimal values like #RRGGBBAA are accepted.
-        :param light_color: Color of the light modules (default: transparent).
-            See `color` for valid values. If light is set to ``None`` the
-            light modules will be transparent.
+        :param bool eci: Indicates if binary data which does not use the default encoding (ISO/IEC 8859-1) should
+            enforce the ECI mode. Since a lot of QR code readers do not support the ECI mode, this feature is disabled
+            by default and the data is encoded in the provided `encoding` using the usual "byte" mode. Set ``eci`` to
+            ``True`` if an ECI header should be inserted into the QR Code. Note that the implementation may not know
+            the ECI designator for the provided `encoding` and may raise an exception if the ECI designator cannot be
+            found. The ECI mode is not supported by Micro QR Codes.
+
+        :param dark_color: Color of the dark modules (default: black). The color can be provided as ``(R, G, B)`` tuple,
+            as hexadecimal format (``#RGB``, ``#RRGGBB`` ``RRGGBBAA``), or web color name (i.e. ``red``). If alpha
+            transparency is supported (i.e. PNG and SVG), hexadecimal values like #RRGGBBAA are accepted.
+
+        :param light_color: Color of the light modules (default: transparent). See `color` for valid values. If light
+            is set to ``None`` the light modules will be transparent.
+
         :param finder_dark_color: Color of the dark finder modules (default: same as ``dark_color``)
         :param finder_light_color: Color of the light finder modules (default: same as ``light_color``)
         :param data_dark_color: Color of the dark data modules (default: same as ``dark_color``)
         :param data_light_color: Color of the light data modules (default: same as ``light_color``)
         :param version_dark_color: Color of the dark version modules (default: same as ``dark_color``)
         :param version_light_color: Color of the light version modules (default: same as ``light_color``)
         :param format_dark_color: Color of the dark format modules (default: same as ``dark_color``)
@@ -107,20 +104,21 @@
         :param alignment_light_color: Color of the light alignment modules (default: same as ``light_color``)
         :param timing_dark_color: Color of the dark timing pattern modules (default: same as ``dark_color``)
         :param timing_light_color: Color of the light timing pattern modules (default: same as ``light_color``)
         :param separator_color: Color of the separator (default: same as ``light_color``)
         :param dark_module_color: Color of the dark module (default: same as ``dark_color``)
         :param quiet_zone_color: Color of the quiet zone modules (default: same as ``light_color``)
 
-        The *size* parameter gives the size of each module of the QR code matrix. It can be either a positive integer or one of the following letters:
-            * t or T: tiny (value: 6)
-            * s or S: small (value: 12)
-            * m or M: medium (value: 18)
-            * l or L: large (value: 30)
-            * h or H: huge (value: 48)
+        The *size* parameter gives the size of each module of the QR code matrix. It can be either a positive integer
+        or one of the following letters:
+        * t or T: tiny (value: 6)
+        * s or S: small (value: 12)
+        * m or M: medium (value: 18)
+        * l or L: large (value: 30)
+        * h or H: huge (value: 48)
 
         For PNG image format the size unit is in pixels, while the unit is 0.1 mm for SVG format.
 
         The *border* parameter controls how many modules thick the border should be (blank space around the code).
         The default is 4, which is the minimum according to the specs.
 
         The *version* parameter is an integer from 1 to 40 that controls the size of the QR code matrix. Set to None to
@@ -128,18 +126,18 @@
         177 x 177 matrix.
         The size grows by 4 modules/side.
         For Micro QR codes, valid values are "M1", "M2", "M3", "M4".
 
         There are 4 error correction levels used for QR codes, with each one adding different amounts of "backup" data
         depending on how much damage the QR code is expected to suffer in its intended environment, and hence how much
         error correction may be required. The correction level can be configured with the *error_correction* parameter as follow:
-            * l or L: error correction level L – up to 7% damage
-            * m or M: error correction level M – up to 15% damage
-            * q or Q: error correction level Q – up to 25% damage
-            * h or H: error correction level H – up to 30% damage
+        * l or L: error correction level L – up to 7% damage
+        * m or M: error correction level M – up to 15% damage
+        * q or Q: error correction level Q – up to 25% damage
+        * h or H: error correction level H – up to 30% damage
 
         You may enforce the creation of a Micro QR Code with `micro=True`. The `micro` option defaults to `False`.
 
         The `encoding` option controls the text encoding used in mode "byte" (used for any general text content). By default `encoding` is ``UTF-8``. When set to ``None``, the implementation (based on Segno) tries to use the standard conform ISO/IEC 8859-1 encoding and if it does not fit, it will use UTF-8. Note that no ECI mode indicator is inserted by default (see `eci` option). The `encoding` parameter is case-insensitive.
 
         The `boost_error` indicates whether the QR code encoding engine (Segno) tries to increase the error correction level if it does not affect the version. Error correction level is not increased when it impacts the version of the code.
 
@@ -243,15 +241,15 @@
     def _size_as_number(self) -> Union[int, float, str, Decimal]:
         """Returns the size as integer value.
 
         :rtype: int or float
         """
         size = self._size
         if _can_be_cast_to_int(size):
-            actual_size = int(size)     # type: ignore
+            actual_size = int(size)  # type: ignore
             if actual_size < 1:
                 actual_size = SIZE_DICT[DEFAULT_MODULE_SIZE]
         elif isinstance(size, (float, Decimal)):
             actual_size = size  # type: ignore
             if actual_size < Decimal("0.01"):
                 actual_size = SIZE_DICT[DEFAULT_MODULE_SIZE]
         elif isinstance(size, str):
@@ -410,15 +408,15 @@
         def is_naive_datetime(t) -> bool:
             return t.tzinfo is None or t.tzinfo.utcoffset(t) is None
 
         def get_datetime_str(t) -> str:
             if is_naive_datetime(t):
                 return t.strftime("%Y%m%dT%H%M%S")
             else:
-                t_utc = t.astimezone(zoneinfo.ZoneInfo('UTC'))
+                t_utc = t.astimezone(zoneinfo.ZoneInfo("UTC"))
                 return t_utc.strftime("%Y%m%dT%H%M%SZ")
 
         event_str = f"""BEGIN:VCALENDAR
 PRODID:Django QR Code
 VERSION:2.0
 BEGIN:VEVENT
 DTSTAMP:{(self.dtstamp or datetime.datetime.utcnow()).astimezone(zoneinfo.ZoneInfo('UTC')).strftime("%Y%m%dT%H%M%SZ")}
@@ -666,25 +664,23 @@
     Creates a QR code which encodes a `vCard <https://en.wikipedia.org/wiki/VCard>`_
     version 3.0.
 
     Only a subset of available `vCard 3.0 properties <https://tools.ietf.org/html/rfc2426>`
     is supported.
 
     Fields meaning:
-    name: The name. If it contains a semicolon, the first part
-            is treated as lastname and the second part is treated as forename.
+    name: The name. If it contains a semicolon, the first part is treated as lastname and the second part is treated as forename.
     displayname: Common name.
     email: E-mail address. Multiple values are allowed.
     phone: Phone number. Multiple values are allowed.
     fax: Fax number. Multiple values are allowed.
     videophone: Phone number for video calls. Multiple values are allowed.
     memo: A notice for the contact.
     nickname: Nickname.
-    birthday: Birthday. If a string is provided, it should encode the
-                     date as ``YYYY-MM-DD`` value.
+    birthday: Birthday. If a string is provided, it should encode the date as ``YYYY-MM-DD`` value.
     url: Homepage. Multiple values are allowed.
     pobox: P.O. box (address information).
     street: Street address.
     city: City (address information).
     region: Region (address information).
     zipcode: Zip code (address information).
     country: Country (address information).
```

### Comparing `django-qr-code-4.0.1/qr_code/views.py` & `django_qr_code-4.1.0/qr_code/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,25 @@
 
 
 @condition(etag_func=qr_code_etag, last_modified_func=qr_code_last_modified)
 @cache_qr_code()
 def serve_qr_code_image(request) -> HttpResponse:
     """Serve an image that represents the requested QR code.
 
-    IMPORTANT NOTE: Each boolean option mentioned below (value True/False) must be passed as `<option name>=1` for `True`, respectively `<option name>=0` for `False`.
+    IMPORTANT NOTE: Each boolean option mentioned below (value True/False) must be passed as `<option name>=1` for
+    `True`, respectively `<option name>=0` for `False`.
 
-    You may pass any argument available for :py:func:`qr_code.qrcode.utils.QRCodeOptions.__init__` to adjust the appearance of the returned QR code. The arguments must be passed as query
+    You may pass any argument available for :py:func:`qr_code.qrcode.utils.QRCodeOptions.__init__` to adjust the
+    appearance of the returned QR code. The arguments must be passed as query
     string arguments in the URL. Additionally, the following arguments are available:
-        * cache_enabled: boolean – Tells the generator to work around the caching mechanism if it is empty (default: True/undefined).
-        * token: str – By default, the application only serves QR code images for authenticated URLs (requests generated from your application and addressed to your application).
-            The authentication uses a HMAC to sign the request query arguments. The authentication code is passed as a query argument named `token` which is automatically generated
-            by `qr_url_from_text` or `qr_url_from_data`.
+    * cache_enabled: boolean – Tells the generator to work around the caching mechanism if it is empty (default: True/undefined).
+    * token: str – By default, the application only serves QR code images for authenticated URLs (requests generated
+    from your application and addressed to your application). The authentication uses a HMAC to sign the request query
+    arguments. The authentication code is passed as a query argument named `token` which is automatically generated
+    by `qr_url_from_text` or `qr_url_from_data`.
     """
     qr_code_options = get_qr_code_option_from_request(request)
     # Handle image access protection (we do not allow external requests for anyone).
     check_image_access_permission(request, qr_code_options)
     force_text = False
     if "bytes" in request.GET:
         try:
```

### Comparing `django-qr-code-4.0.1/setup.py` & `django_qr_code-4.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     license="BSD 3-clause",
     author="Philippe Docourt",
     author_email="philippe@docourt.ch",
     maintainer="Philippe Docourt",
     description="An application that provides tools for displaying QR codes on your Django site.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["segno>=1.6", "django>=4.2", "pydantic>=2.5"],
-    python_requires=">=3.8",
+    install_requires=["segno>=1.6", "django>=4.2", "pydantic>=2.7"],
+    python_requires=">=3.10",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3 :: Only",
```

