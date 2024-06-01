# Comparing `tmp/drf_cookie_jwtauth-0.0.1.tar.gz` & `tmp/drf_cookie_jwtauth-0.0.2.tar.gz`

## Comparing `drf_cookie_jwtauth-0.0.1.tar` & `drf_cookie_jwtauth-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/.gitattributes
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/pytest.ini
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/admin.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/manager.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/middleware.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/models.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/settings.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/tokens.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/utils.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/src/jwtauth/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/test_auth.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/test_tokens.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/test_views/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/test_views/urls.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/tests/test_views/views.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/LICENSE
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/.gitattributes
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/pytest.ini
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/admin.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/manager.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/middleware.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/models.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/settings.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/tokens.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/utils.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/src/jwtauth/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/test_auth.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/test_tokens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/test_views/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/test_views/urls.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/tests/test_views/views.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.2/PKG-INFO
```

### Comparing `drf_cookie_jwtauth-0.0.1/.github/workflows/python-package.yml` & `drf_cookie_jwtauth-0.0.2/.github/workflows/python-test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Python package
+name: Python Test
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
   build:
+    name: Test 🧪
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
@@ -26,16 +27,18 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
     - name: Test with pytest
       run: |
         pytest
-    - name: Install Hatch
-      run: pip install hatch
-    - name: Build dist
-      run: hatch build
-    - name: Upload package artifact
-      uses: actions/upload-artifact@v3
-      with:
-        name: jwtauth-${{ matrix.python-version }}
-        path: dist/jwtauth-0.0.1.tar.gz
+  lint:
+    name: Lint 🧹
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: psf/black@stable
+      - name: Run flake8 ❄
+        uses: py-actions/flake8@v2
+        with:
+          max-line-length: "100"
+          plugins: "flake8-bugbear==22.1.11 flake8-black"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drf_cookie_jwtauth-0.0.1/src/jwtauth/manager.py` & `drf_cookie_jwtauth-0.0.2/src/jwtauth/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,20 @@
             # authentication token (even if expired) and a valid refresh token
             return
 
         if not self.access_token.valid() or not self.refresh_token.valid():
             # we end up here if:
             # - one of the tokens was forged by a malicious user
             # - the refresh token was blacklisted
-            raise exceptions.AuthenticationFailed('Invalid tokens')
+            raise exceptions.AuthenticationFailed("Invalid tokens")
 
         if self.access_token.expired():
             if self.refresh_token.expired():
                 # both tokens are expired, the user has to log in again
-                raise exceptions.AuthenticationFailed('Expired tokens')
+                raise exceptions.AuthenticationFailed("Expired tokens")
 
             # we silently refresh the authentication token and let the user in
             self.silent_refresh = True
             self.access_token = self.refresh_token.gen_access_token()
 
         # the authentication token is valid and not expired
         self.user = self.access_token.user
@@ -69,15 +69,19 @@
             set_access_token(response, self.refresh_token.gen_access_token())
 
         if self.logging_in:
             set_access_token(response, self.access_token)
             set_refresh_token(response, self.refresh_token)
 
         if self.logging_out:
-            if self.refresh_token and self.refresh_token.valid() and not self.refresh_token.expired():
+            if (
+                self.refresh_token
+                and self.refresh_token.valid()
+                and not self.refresh_token.expired()
+            ):
                 # blacklist the token if valid and still alive
                 self.refresh_token.blacklist()
 
             delete_access_token(response)
             delete_refresh_token(response)
 
 
@@ -87,18 +91,18 @@
 
     return token_class(from_encoding=request.COOKIES[key])
 
 
 def set_token(response, key, token):
     if settings.DEBUG:
         # locally, we allow non-secure cookies
-        response.set_cookie(key, token.encoding, httponly=True, samesite='Strict', secure=False)
+        response.set_cookie(key, token.encoding, httponly=True, samesite="Strict", secure=False)
         return
 
-    response.set_cookie(key, token.encoding, httponly=True, samesite='Strict', secure=True)
+    response.set_cookie(key, token.encoding, httponly=True, samesite="Strict", secure=True)
 
 
 def get_access_token(request):
     return get_token(request, ACCESS_TOKEN_KEY, AccessToken)
 
 
 def get_refresh_token(request):
```

### Comparing `drf_cookie_jwtauth-0.0.1/src/jwtauth/middleware.py` & `drf_cookie_jwtauth-0.0.2/src/jwtauth/middleware.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.1/src/jwtauth/settings.py` & `drf_cookie_jwtauth-0.0.2/src/jwtauth/settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 
     setting, value = kwargs["setting"], kwargs["value"]
 
     if setting == "JWTAUTH":
         api_settings = APISettings(value, DEFAULTS, ())
 
 
-setting_changed.connect(reload_api_settings)
+setting_changed.connect(reload_api_settings)
```

### Comparing `drf_cookie_jwtauth-0.0.1/src/jwtauth/tokens.py` & `drf_cookie_jwtauth-0.0.2/src/jwtauth/tokens.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,44 @@
 
 from jwtauth.utils import generate_unique_token
 from jwtauth.settings import api_settings
 from jwtauth.models import BlacklistedToken, ActiveToken
 
 import jwt
 
-IAT = 'iat'
-EXP = 'exp'
+IAT = "iat"
+EXP = "exp"
 
 UserModel = get_user_model()
 
 
 class Token:
     registered_claims = [IAT, EXP]
 
-    def __init__(self, from_encoding: str = None, from_data: dict = None, duration: timedelta = None):
+    def __init__(
+        self, from_encoding: str = None, from_data: dict = None, duration: timedelta = None
+    ):
         """
         Initialize a JWT token, either decoding it from a string or encoding it from data.
 
-        :param from_encoding: The encoded token string. If this is provided, the token will be decoded.
-        :param from_data: The data to encode into this token. If this is provided, the token will be encoded.
-        :param duration: The duration for which the token is valid. Converted into integer seconds and used to
-            set the expiration field of the JWT.
+        :param from_encoding: The encoded token string. If this is provided,
+            the token will be decoded.
+        :param from_data: The data to encode into this token. If this is provided,
+            the token will be encoded.
+        :param duration: The duration for which the token is valid. Converted into integer
+            seconds and used to set the expiration field of the JWT.
         """
         if not from_encoding and not from_data:
             raise Exception("Please specify either the data or the encoding to create the token.")
 
         if from_encoding and from_data:
             raise Exception(
                 "Please specify either the data to encode the token or the "
-                "encoding from which to derive the data, not both.")
+                "encoding from which to derive the data, not both."
+            )
 
         if from_data and not timedelta:
             raise Exception("Please specify a duration for the token.")
 
         self.data = None
         self.encoding = None
 
@@ -68,34 +73,32 @@
         self.jwt_data = {
             **self.data,
             IAT: self.iat,
             EXP: self.exp,
         }
 
         self.encoding = jwt.encode(
-            self.jwt_data,
-            api_settings.SIGNING_KEY,
-            algorithm=api_settings.ALGORITHM
+            self.jwt_data, api_settings.SIGNING_KEY, algorithm=api_settings.ALGORITHM
         )
 
     def decode(self, data) -> bool:
 
         self.encoding = data
 
         try:
             self.jwt_data = jwt.decode(
                 self.encoding,
                 api_settings.SIGNING_KEY,
                 algorithms=[api_settings.ALGORITHM],
                 options={
                     # if the token is expired we still want to have an instance with expired=True,
                     # thus we verify exp ourselves rather than having jwt throw an exception
-                    'verify_exp': False,
-                    'require': self.registered_claims
-                }
+                    "verify_exp": False,
+                    "require": self.registered_claims,
+                },
             )
 
             self.data = self.jwt_data.copy()
 
             # remove jwt registered claims from user data
             for k in Token.registered_claims:
                 self.data.pop(k)
@@ -123,27 +126,25 @@
 
 
 class UserToken(Token):
     """A token that is associated with a user.
 
     This token is used by both access and refresh tokens.
     """
-    USER_ID_KEY = 'user_id'
+
+    USER_ID_KEY = "user_id"
 
     def __init__(self, *args, **kwargs):
         self.user = None
         super().__init__(*args, **kwargs)
 
     def encode(self, user, data=None) -> None:
         self.user = user
 
-        super().encode({
-            **(data or {}),
-            self.USER_ID_KEY: user.id
-        })
+        super().encode({**(data or {}), self.USER_ID_KEY: user.id})
 
     def decode(self, data) -> bool:
         if not super().decode(data):
             return False
 
         if self.USER_ID_KEY not in self.jwt_data:
             return False
@@ -164,34 +165,32 @@
 
 class AccessToken(UserToken):
 
     def __init__(self, from_encoding=None, from_user=None):
         super().__init__(
             from_encoding=from_encoding,
             from_data=from_user,
-            duration=api_settings.ACCESS_TOKEN_LIFETIME
+            duration=api_settings.ACCESS_TOKEN_LIFETIME,
         )
 
 
 class RefreshToken(UserToken):
-    TOKEN_STRING_KEY = 'token_string'
+    TOKEN_STRING_KEY = "token_string"
 
     def __init__(self, from_encoding=None, from_user=None):
         self.token_string = None
         super().__init__(
             from_encoding=from_encoding,
             from_data=from_user,
-            duration=api_settings.REFRESH_TOKEN_LIFETIME
+            duration=api_settings.REFRESH_TOKEN_LIFETIME,
         )
 
     def encode(self, user, data=None) -> None:
         self.token_string = generate_unique_token()
-        super().encode(user, {
-            self.TOKEN_STRING_KEY: self.token_string
-        })
+        super().encode(user, {self.TOKEN_STRING_KEY: self.token_string})
 
     def decode(self, data) -> bool:
         if not super().decode(data):
             return False
 
         if self.TOKEN_STRING_KEY not in self.data:
             return False
@@ -199,33 +198,26 @@
         self.token_string = self.data[self.TOKEN_STRING_KEY]
         return True
 
     def save(self) -> ActiveToken:
         if not self.valid():
             raise Exception("Invalid token cannot be saved!")
 
-        mod = ActiveToken(
-            token_string=self.token_string,
-            owner=self.user,
-            exp=self.exp
-        )
+        mod = ActiveToken(token_string=self.token_string, owner=self.user, exp=self.exp)
 
         mod.save()
         return mod
 
     def blacklist(self) -> None:
         if not self.valid():
             raise Exception("Invalid token cannot be blacklisted!")
 
         ActiveToken.objects.filter(token_string=self.token_string).delete()
 
-        mod = BlacklistedToken(
-            token_string=self.token_string,
-            exp=self.exp
-        )
+        mod = BlacklistedToken(token_string=self.token_string, exp=self.exp)
 
         mod.save()
 
     def blacklisted(self) -> bool:
         if not self.is_valid:
             raise Exception("Invalid token cannot be evaluated against the blacklist!")
```

### Comparing `drf_cookie_jwtauth-0.0.1/src/jwtauth/utils.py` & `drf_cookie_jwtauth-0.0.2/src/jwtauth/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from random import SystemRandom
 
 from jwtauth.models import ActiveToken
 
-UNICODE_ASCII_CHARACTER_SET = ('abcdefghijklmnopqrstuvwxyz'
-                               'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-                               '0123456789')
+UNICODE_ASCII_CHARACTER_SET = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
 
 
 def generate_token(length=30, chars=UNICODE_ASCII_CHARACTER_SET):
-    """From OAuthLib: https://github.com/oauthlib/oauthlib/tree/d4b6699f8ccb608152b764919e0bd3d38a7b171f
+    """
+    From OAuthLib:
+    https://github.com/oauthlib/oauthlib/tree/d4b6699f8ccb608152b764919e0bd3d38a7b171f
 
     Generates a non-guessable OAuth token
 
     OAuth (1 and 2) does not specify the format of tokens except that they
     should be strings of random characters. Tokens should not be guessable
     and entropy when generating the random characters is important. Which is
     why SystemRandom is used instead of the default random.choice method.
     """
 
     rand = SystemRandom()
-    return ''.join(rand.choice(chars) for x in range(length))
+    return "".join(rand.choice(chars) for x in range(length))
 
 
 def generate_unique_token():
     while True:
         token = generate_token()
 
         # loop until the token does not match an existing one;
```

### Comparing `drf_cookie_jwtauth-0.0.1/tests/conftest.py` & `drf_cookie_jwtauth-0.0.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,49 @@
 from django.conf import settings
 
 
 def pytest_configure():
 
     settings.configure(
         DATABASES={
-            'default': {'ENGINE': 'django.db.backends.sqlite3', 'NAME': ':memory:'},
-            'other': {'ENGINE': 'django.db.backends.sqlite3', 'NAME': 'other'},
+            "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"},
+            "other": {"ENGINE": "django.db.backends.sqlite3", "NAME": "other"},
         },
         SECRET_KEY="abcd1234",
         MIDDLEWARE=(
-            'jwtauth.middleware.AuthenticationMiddleware',
-            'django.contrib.sessions.middleware.SessionMiddleware',
-            'django.middleware.common.CommonMiddleware',
-            'django.contrib.auth.middleware.AuthenticationMiddleware',
-            'django.contrib.messages.middleware.MessageMiddleware',
+            "jwtauth.middleware.AuthenticationMiddleware",
+            "django.contrib.sessions.middleware.SessionMiddleware",
+            "django.middleware.common.CommonMiddleware",
+            "django.contrib.auth.middleware.AuthenticationMiddleware",
+            "django.contrib.messages.middleware.MessageMiddleware",
         ),
         INSTALLED_APPS=(
-            'django.contrib.admin',
-            'django.contrib.auth',
-            'django.contrib.contenttypes',
-            'django.contrib.messages',
+            "django.contrib.admin",
+            "django.contrib.auth",
+            "django.contrib.contenttypes",
+            "django.contrib.messages",
             "rest_framework",
             "jwtauth",
             "tests.test_views",
         ),
         ROOT_URLCONF="tests.test_views.urls",
         REST_FRAMEWORK={
-            'DEFAULT_AUTHENTICATION_CLASSES': [
-                'jwtauth.JwtAuthentication',
+            "DEFAULT_AUTHENTICATION_CLASSES": [
+                "jwtauth.JwtAuthentication",
             ],
-        }
+        },
     )
 
     django.setup()
 
 
 @pytest.fixture
 def user_a_password():
     return "abc12345#"
 
 
 @pytest.fixture
 def user_a(user_a_password):
     from django.contrib.auth.models import User
+
     user = User.objects.create_user("john", "lennon@thebeatles.com", user_a_password)
     return user
```

### Comparing `drf_cookie_jwtauth-0.0.1/tests/test_auth.py` & `drf_cookie_jwtauth-0.0.2/tests/test_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from django.urls import reverse
 from django.test import Client
 from jwtauth.models import ActiveToken, BlacklistedToken
 
 
 def login(username, password):
     client = Client()
-    response = client.post(reverse("login"), {
-        "username": username,
-        "password": password
-    }, content_type="application/json")
+    response = client.post(
+        reverse("login"),
+        {"username": username, "password": password},
+        content_type="application/json",
+    )
 
     assert response.status_code == 204
     assert len(response.cookies) == 2
 
     client.cookies = response.cookies
     return client, response
 
@@ -62,14 +63,14 @@
 @pytest.mark.django_db
 def test_logout(logged_client):
     response = logged_client.delete(reverse("logout"))
     assert response.status_code == 204
 
     for cookie in response.cookies.values():
         # verify the cookie has been deleted
-        assert cookie['max-age'] == 0
+        assert cookie["max-age"] == 0
 
     # verify the active token has been removed
     assert ActiveToken.objects.count() == 0
 
     # verify the refresh token has been blacklisted
     assert BlacklistedToken.objects.count() == 1
```

### Comparing `drf_cookie_jwtauth-0.0.1/tests/test_tokens.py` & `drf_cookie_jwtauth-0.0.2/tests/test_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,43 @@
     assert token.expired()
 
 
 def test_token_no_exp():
     # try decoding a token without an 'exp' claim and verify it is marked as invalid
     encoding = jwt.encode(
         {"data": 42, "iat": datetime.now(tz=timezone.utc)},
-        api_settings.SIGNING_KEY, algorithm=api_settings.ALGORITHM)
+        api_settings.SIGNING_KEY,
+        algorithm=api_settings.ALGORITHM,
+    )
     token = Token(from_encoding=encoding)
     assert not token.valid()
 
 
 def test_token_no_iat():
     # try decoding a token without a 'iat' claim and verify it is marked as invalid
     encoding = jwt.encode(
         {"data": 42, "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5)},
-        api_settings.SIGNING_KEY, algorithm=api_settings.ALGORITHM)
+        api_settings.SIGNING_KEY,
+        algorithm=api_settings.ALGORITHM,
+    )
     token = Token(from_encoding=encoding)
     assert not token.valid()
 
 
 def test_token_decode_expired():
     # create a token with a duration of 0 seconds, encode it, decode it
     # and verify it is marked as expired
     encoded = Token(from_data={"data": 42}, duration=timedelta())
     decoded = Token(from_encoding=encoded.encoding)
     assert decoded.expired()
 
 
 def test_bad_token():
     # try to decode random data and verify the token is marked as invalid
-    decoded = Token(from_encoding='12345')
+    decoded = Token(from_encoding="12345")
     assert not decoded.valid()
 
 
 def test_invalid_signature():
     # try to decode a token with an invalid signature and verify it is marked as invalid
     original = Token(from_data={"data": 42}, duration=timedelta(minutes=5))
     encoding = jwt.encode(original.jwt_data, "new_key", algorithm="HS256")
@@ -104,40 +108,44 @@
     decoded = AccessToken(from_encoding=encoding)
     assert not decoded.valid()
 
 
 def test_user_token_missing_user_id():
     # create a valid token but with missing user id and
     # check that it is marked as invalid
-    token = AccessToken(from_encoding=jwt.encode(
-        {
-            "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
-            "iat": datetime.now(tz=timezone.utc),
-            # missing user ID
-        },
-        api_settings.SIGNING_KEY,
-        algorithm=api_settings.ALGORITHM
-    ))
+    token = AccessToken(
+        from_encoding=jwt.encode(
+            {
+                "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
+                "iat": datetime.now(tz=timezone.utc),
+                # missing user ID
+            },
+            api_settings.SIGNING_KEY,
+            algorithm=api_settings.ALGORITHM,
+        )
+    )
 
     assert not token.valid()
 
 
 @pytest.mark.django_db
 def test_user_token_wrong_user_id():
     # create a valid token but with a non-existing user id and
     # check that it is marked as invalid
-    token = UserToken(from_encoding=jwt.encode(
-        {
-            "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
-            "iat": datetime.now(tz=timezone.utc),
-            AccessToken.USER_ID_KEY: 1234  # non-existing user
-        },
-        api_settings.SIGNING_KEY,
-        algorithm=api_settings.ALGORITHM
-    ))
+    token = UserToken(
+        from_encoding=jwt.encode(
+            {
+                "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
+                "iat": datetime.now(tz=timezone.utc),
+                AccessToken.USER_ID_KEY: 1234,  # non-existing user
+            },
+            api_settings.SIGNING_KEY,
+            algorithm=api_settings.ALGORITHM,
+        )
+    )
 
     assert not token.valid()
 
 
 @pytest.mark.django_db
 def test_refresh_token(user_a):
     # create a refresh token and verify it is marked as valid and not expired
@@ -192,23 +200,25 @@
     assert not decoded.valid()
 
 
 @pytest.mark.django_db
 def test_refresh_token_missing_token_string(user_a):
     # create a valid token but with a non-existing user id and
     # check that it is marked as invalid
-    token = RefreshToken(from_encoding=jwt.encode(
-        {
-            "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
-            "iat": datetime.now(tz=timezone.utc),
-            AccessToken.USER_ID_KEY: user_a.id,
-        },
-        api_settings.SIGNING_KEY,
-        algorithm=api_settings.ALGORITHM
-    ))
+    token = RefreshToken(
+        from_encoding=jwt.encode(
+            {
+                "exp": datetime.now(tz=timezone.utc) + timedelta(minutes=5),
+                "iat": datetime.now(tz=timezone.utc),
+                AccessToken.USER_ID_KEY: user_a.id,
+            },
+            api_settings.SIGNING_KEY,
+            algorithm=api_settings.ALGORITHM,
+        )
+    )
 
     assert not token.valid()
 
 
 @pytest.mark.django_db
 def test_gen_access_token(user_a):
     ref_token = RefreshToken(from_user=user_a)
```

### Comparing `drf_cookie_jwtauth-0.0.1/tests/test_views/views.py` & `drf_cookie_jwtauth-0.0.2/tests/test_views/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,55 +6,50 @@
 from rest_framework.exceptions import AuthenticationFailed
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 
 from jwtauth import login, logout
 
 
-@api_view(['POST'])
+@api_view(["POST"])
 def login_view(request):
     body = JSONParser().parse(request)
 
-    user = authenticate(
-        username=body['username'],
-        password=body['password']
-    )
+    user = authenticate(username=body["username"], password=body["password"])
 
     if user is None:
         # credentials are not valid
-        raise AuthenticationFailed('Invalid username or password.', 403)
+        raise AuthenticationFailed("Invalid username or password.", 403)
 
     login(request, user)
     return Response(status=204)
 
 
-@api_view(['GET'])
+@api_view(["GET"])
 @permission_classes([IsAuthenticated])
 def logged_view(request):
     return Response(status=204)
 
 
 class LoggedView(APIView):
     permission_classes = [IsAuthenticated]
 
     def get(self, request):
         return Response(status=204)
 
 
-@api_view(['GET'])
+@api_view(["GET"])
 def username_view(request):
 
     username = ""
 
     if request.user.is_authenticated:
         username = request.user.username
 
-    return Response({
-        "username": username
-    })
+    return Response({"username": username})
 
 
-@api_view(['DELETE'])
+@api_view(["DELETE"])
 @permission_classes([IsAuthenticated])
 def logout_view(request):
     logout(request)
     return Response(status=204)
```

### Comparing `drf_cookie_jwtauth-0.0.1/LICENSE` & `drf_cookie_jwtauth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.1/README.md` & `drf_cookie_jwtauth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.1/pyproject.toml` & `drf_cookie_jwtauth-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/jwtauth"]
 
 [project]
 name = "drf-cookie-jwtauth"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lorenzo Celli", email="lorenzo.celli00@gmail.com" },
 ]
 description = "JWT-based authentication for Django REST Framework"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,8 +19,11 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "Django~=5.0.2",
   "PyJWT~=2.8.0",
   "djangorestframework~=3.14.0",
-]
+]
+
+[tool.black]
+line-length = 100
```

### Comparing `drf_cookie_jwtauth-0.0.1/PKG-INFO` & `drf_cookie_jwtauth-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: drf-cookie-jwtauth
-Version: 0.0.1
+Version: 0.0.2
 Summary: JWT-based authentication for Django REST Framework
 Author-email: Lorenzo Celli <lorenzo.celli00@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

