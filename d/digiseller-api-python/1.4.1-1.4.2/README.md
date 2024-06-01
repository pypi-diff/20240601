# Comparing `tmp/digiseller_api_python-1.4.1.tar.gz` & `tmp/digiseller_api_python-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiseller_api_python-1.4.1.tar", last modified: Tue Feb 20 22:02:36 2024, max compression
+gzip compressed data, was "digiseller_api_python-1.4.2.tar", last modified: Sat Jun  1 03:09:49 2024, max compression
```

## Comparing `digiseller_api_python-1.4.1.tar` & `digiseller_api_python-1.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:02:36.167568 digiseller_api_python-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-20 22:02:27.000000 digiseller_api_python-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    32039 2024-02-20 22:02:36.167568 digiseller_api_python-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31469 2024-02-20 22:02:27.000000 digiseller_api_python-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:02:36.167568 digiseller_api_python-1.4.1/digiseller_api_python/
--rw-r--r--   0 runner    (1001) docker     (127)   110419 2024-02-20 22:02:27.000000 digiseller_api_python-1.4.1/digiseller_api_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 22:02:36.167568 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32039 2024-02-20 22:02:36.000000 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-20 22:02:36.000000 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 22:02:36.000000 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-20 22:02:36.000000 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-20 22:02:36.000000 digiseller_api_python-1.4.1/digiseller_api_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 22:02:36.171568 digiseller_api_python-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-20 22:02:27.000000 digiseller_api_python-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:09:49.924225 digiseller_api_python-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-01 03:09:45.000000 digiseller_api_python-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34294 2024-06-01 03:09:49.920225 digiseller_api_python-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33586 2024-06-01 03:09:45.000000 digiseller_api_python-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:09:49.920225 digiseller_api_python-1.4.2/digiseller_api_python/
+-rw-r--r--   0 runner    (1001) docker     (127)   109843 2024-06-01 03:09:45.000000 digiseller_api_python-1.4.2/digiseller_api_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:09:49.920225 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34294 2024-06-01 03:09:49.000000 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-06-01 03:09:49.000000 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:09:49.000000 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 03:09:49.000000 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 03:09:49.000000 digiseller_api_python-1.4.2/digiseller_api_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:09:49.924225 digiseller_api_python-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-01 03:09:45.000000 digiseller_api_python-1.4.2/setup.py
```

### Comparing `digiseller_api_python-1.4.1/LICENSE` & `digiseller_api_python-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `digiseller_api_python-1.4.1/PKG-INFO` & `digiseller_api_python-1.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,93 @@
 Metadata-Version: 2.1
 Name: digiseller_api_python
-Version: 1.4.1
-Summary: Interaction with Digiseller API
+Version: 1.4.2
+Summary: Interaction with Digiseller API via Python
 Home-page: https://github.com/Ernieleo/Digiseller-API-Python
 Author: Ernieleo
 Author-email: ernieleo@vk.com
 Project-URL: Documentation, https://my.digiseller.com/inside/api.asp
-Keywords: api client
-Classifier: Programming Language :: Python :: 3.7
+Project-URL: Download, https://pypi.org/project/digiseller-api-python/
+Project-URL: Write me, https://t.me/ernieleo
+Keywords: digiseller api python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Digiseller API python
-Код предоставляется как есть, любые предложения по улучшению - исправлению приветствуются.  
-Функционал основан на информации с сайта Digiseller.  
-
-Данный проект не является официальным, мы не имеем никакого отношения к команде разработчиков сервиса Digiseller.
-Возможны ошибки в работе некоторых методов, комплексного тестирования не проводилось.  
-Не каждый запрос API и его описание в документации на сайте Digiseller соответствует действительности.
+# Digiseller API Python
+
+[![PyPI version](https://img.shields.io/pypi/v/digiseller-api-python.svg)](https://pypi.org/project/digiseller-api-python)
+[![Downloads](https://img.shields.io/pypi/dm/digiseller-api-python)](https://pypistats.org/packages/digiseller-api-python)
+[![License](https://img.shields.io/github/license/Ernieleo/digiseller-api-python)](https://github.com/Ernieleo/digiseller-api-python/blob/main/LICENSE)
+
+Digiseller API Python — это библиотека Python для доступа к API Digiseller. 
+
+Добавлено 70 методов из числа представленных в документации.
+
+**Важное примечание**: Данный проект не является официальным.  
+Я не имею никакого отношения к команде разработчиков сервиса Digiseller.  
+
+Возможны ошибки в некоторых запросах, так как комплексное тестирование не проводилось.  
+Часть запросов из документации на сайте Digiseller не соответствуют действительности.  
+
+Ознакомиться с документацией API вы можете на [сайте Digiseller](https://my.digiseller.com/inside/api.asp)
+
 ## Установка
 
-Установить с [pypi.org](https://pypi.org/project/digiseller-api-python/)
+Вы можете установить с сервиса [PyPI](https://pypi.org/project/digiseller-api-python/)
+
 ```sh
-pip3 install digiseller-api-python
+pip install digiseller-api-python
 ```
 
-Для ручной установки: [ernieleo/digiseller-api-python](https://github.com/Ernieleo/digiseller-api-python) с репозитория.
+Для ручной установки с репозитория
 ```sh
 pip3 install git+https://github.com/Ernieleo/digiseller-api-python.git
-```
+````
 
-## Подключение
-Получить API Ключ [👉тут👈](https://my.digiseller.com/inside/api_keys.asp)  
-Получить ID Продавца [👉тут👈](https://my.digiseller.com/)
+## Простая демонстрация
 
-Инициализировать класс модуля с передачей ID продавца и API Ключа
+Получить API Ключ 👉[тут](https://my.digiseller.com/inside/api_keys.asp)👈  
+Получить ID Продавца 👉[тут](https://my.digiseller.com/)👈
 
-```py
+```python
 from digiseller_api_python import Api
 
-api = Api(seller_id="ВашSellerID", api_key="API-KEY")
-print(api.chat_list(...))
+Digiseller_Api = Api(seller_id="11155533", api_key="CA1SF69A000A46D00039F01Z11017V39")
+
+# Получение данных пользователя указанных при заказе по уникальному коду
+def get_account_info_from_digiseller(unique_code):
+    data = Digiseller_Api.unique_code(unique_code)
+    email = None
+    password = None
+
+    for option in data["options"]:
+        if option["name"] in ["Почта аккаунта ChatGPT", "ChatGPT account email"]:
+            email = option["value"]
+        elif option["name"] in ["Пароль аккаунта ChatGPT", "ChatGPT account password"]:
+            password = option["value"]
+
+    return email, password
 ```
 
-## Доступные вызовы API
-Сгенерирован список с помощью ChatGPT, возможны опечатки.
+Используется для получения логина и пароля указанных покупателем при оформлении заказа в полях ввода (Параметры) текстовых данных. Поиск требуемого поля осуществляется по названию, указывается названия поля на двух языках, название поля параметра полученного в сведениях о заказе по уникальному коду, зависит от языка браузера пользователя.
+
+## Разработка
+Любой вклад в проект приветствуется.  
+Если вы хотите помочь в разработке, следуйте правилам API сервиса Digiseller и придерживайтесь общего стиля кода. Создайте запрос на cлияние и я его рассмотрю!
+
+## Доступные методы API
+Cписок был сгенерирован при помощи ChatGPT, возможны неточности.  
+Каждая функция вызова описана в самом коде, смотрите информацию в IDE. 
 
-Параметры взяты с официальной документации, значения соответствуют.
+Параметры запросов с документации API, значения соответствуют.
 1. Название: `Поиск и проверка платежа по уникальному коду`
     - Функция: `unique_code`
     - Параметры: `unique_code: str`
     - Ответ: `Ответ от сервера в формате JSON`
     - [Ссылка на API](https://my.digiseller.com/inside/api_general.asp#searchuniquecode)
 
 2. Название: `Информация о продаже по номеру заказа`
```

### Comparing `digiseller_api_python-1.4.1/README.md` & `digiseller_api_python-1.4.2/digiseller_api_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,93 @@
-# Digiseller API python
-Код предоставляется как есть, любые предложения по улучшению - исправлению приветствуются.  
-Функционал основан на информации с сайта Digiseller.  
-
-Данный проект не является официальным, мы не имеем никакого отношения к команде разработчиков сервиса Digiseller.
-Возможны ошибки в работе некоторых методов, комплексного тестирования не проводилось.  
-Не каждый запрос API и его описание в документации на сайте Digiseller соответствует действительности.
+Metadata-Version: 2.1
+Name: digiseller_api_python
+Version: 1.4.2
+Summary: Interaction with Digiseller API via Python
+Home-page: https://github.com/Ernieleo/Digiseller-API-Python
+Author: Ernieleo
+Author-email: ernieleo@vk.com
+Project-URL: Documentation, https://my.digiseller.com/inside/api.asp
+Project-URL: Download, https://pypi.org/project/digiseller-api-python/
+Project-URL: Write me, https://t.me/ernieleo
+Keywords: digiseller api python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Digiseller API Python
+
+[![PyPI version](https://img.shields.io/pypi/v/digiseller-api-python.svg)](https://pypi.org/project/digiseller-api-python)
+[![Downloads](https://img.shields.io/pypi/dm/digiseller-api-python)](https://pypistats.org/packages/digiseller-api-python)
+[![License](https://img.shields.io/github/license/Ernieleo/digiseller-api-python)](https://github.com/Ernieleo/digiseller-api-python/blob/main/LICENSE)
+
+Digiseller API Python — это библиотека Python для доступа к API Digiseller. 
+
+Добавлено 70 методов из числа представленных в документации.
+
+**Важное примечание**: Данный проект не является официальным.  
+Я не имею никакого отношения к команде разработчиков сервиса Digiseller.  
+
+Возможны ошибки в некоторых запросах, так как комплексное тестирование не проводилось.  
+Часть запросов из документации на сайте Digiseller не соответствуют действительности.  
+
+Ознакомиться с документацией API вы можете на [сайте Digiseller](https://my.digiseller.com/inside/api.asp)
+
 ## Установка
 
-Установить с [pypi.org](https://pypi.org/project/digiseller-api-python/)
+Вы можете установить с сервиса [PyPI](https://pypi.org/project/digiseller-api-python/)
+
 ```sh
-pip3 install digiseller-api-python
+pip install digiseller-api-python
 ```
 
-Для ручной установки: [ernieleo/digiseller-api-python](https://github.com/Ernieleo/digiseller-api-python) с репозитория.
+Для ручной установки с репозитория
 ```sh
 pip3 install git+https://github.com/Ernieleo/digiseller-api-python.git
-```
+````
 
-## Подключение
-Получить API Ключ [👉тут👈](https://my.digiseller.com/inside/api_keys.asp)  
-Получить ID Продавца [👉тут👈](https://my.digiseller.com/)
+## Простая демонстрация
 
-Инициализировать класс модуля с передачей ID продавца и API Ключа
+Получить API Ключ 👉[тут](https://my.digiseller.com/inside/api_keys.asp)👈  
+Получить ID Продавца 👉[тут](https://my.digiseller.com/)👈
 
-```py
+```python
 from digiseller_api_python import Api
 
-api = Api(seller_id="ВашSellerID", api_key="API-KEY")
-print(api.chat_list(...))
+Digiseller_Api = Api(seller_id="11155533", api_key="CA1SF69A000A46D00039F01Z11017V39")
+
+# Получение данных пользователя указанных при заказе по уникальному коду
+def get_account_info_from_digiseller(unique_code):
+    data = Digiseller_Api.unique_code(unique_code)
+    email = None
+    password = None
+
+    for option in data["options"]:
+        if option["name"] in ["Почта аккаунта ChatGPT", "ChatGPT account email"]:
+            email = option["value"]
+        elif option["name"] in ["Пароль аккаунта ChatGPT", "ChatGPT account password"]:
+            password = option["value"]
+
+    return email, password
 ```
 
-## Доступные вызовы API
-Сгенерирован список с помощью ChatGPT, возможны опечатки.
+Используется для получения логина и пароля указанных покупателем при оформлении заказа в полях ввода (Параметры) текстовых данных. Поиск требуемого поля осуществляется по названию, указывается названия поля на двух языках, название поля параметра полученного в сведениях о заказе по уникальному коду, зависит от языка браузера пользователя.
+
+## Разработка
+Любой вклад в проект приветствуется.  
+Если вы хотите помочь в разработке, следуйте правилам API сервиса Digiseller и придерживайтесь общего стиля кода. Создайте запрос на cлияние и я его рассмотрю!
+
+## Доступные методы API
+Cписок был сгенерирован при помощи ChatGPT, возможны неточности.  
+Каждая функция вызова описана в самом коде, смотрите информацию в IDE. 
 
-Параметры взяты с официальной документации, значения соответствуют.
+Параметры запросов с документации API, значения соответствуют.
 1. Название: `Поиск и проверка платежа по уникальному коду`
     - Функция: `unique_code`
     - Параметры: `unique_code: str`
     - Ответ: `Ответ от сервера в формате JSON`
     - [Ссылка на API](https://my.digiseller.com/inside/api_general.asp#searchuniquecode)
 
 2. Название: `Информация о продаже по номеру заказа`
```

### Comparing `digiseller_api_python-1.4.1/digiseller_api_python/__init__.py` & `digiseller_api_python-1.4.2/digiseller_api_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 "timestamp": current_time,
                 "sign": sign
             }
             response = self.session.post(self.URL + 'apilogin', json=data)
             if response.status_code == 200:
                 response_data = response.json()
                 self.token = response_data.get('token')
-                self.token_expiration = current_time + 5400  # Жизнь токена - 1.5 часа [По докам 2, но на всякий]
+                self.token_expiration = current_time + 5400  # Жизнь токена - 1.5 часа [По докам 2, но на всякий меньше]
             else:
                 raise ValueError("Не удалось получить токен.")
         return self.token
 
     """ Общие методы """
 
     def __request(self, method, uri_path, **options):
@@ -83,34 +83,31 @@
 
         headers = {'Accept': 'application/json; charset=UTF-8'}
         if 'files' not in options:
             headers['Content-Type'] = 'application/json'
         if 'headers' in options:
             headers.update(options.pop('headers'))
         options['headers'] = headers
-
-        response = self.session.request(method, self.URL + uri_path, **options)
         try:
-            if response.status_code == 200 and response.text:
-                data = response.json()
-                if 'retval' in data and data['retval'] != 0:
-                    error_message = f"Ошибка в API: '{data.get('retdesc', 'Неизвестная ошибка Digiseller API')}'"
-                    if 'errors' in data:
-                        for error in data['errors']:
-                            message = next((msg['value'] for msg in error['message'] if msg['locale'] == 'ru-RU'),
-                                           next((msg['value'] for msg in error['message'] if msg['locale'] == 'en-US'), "Неизвестная ошибка"))
-                            error_message += f". Код ошибки: '{error['code']}'. Причина ошибки: '{message}'."
-                    raise ValueError(error_message)
-                return data
-            elif response.status_code == 200 and not response.text:
-                return {"message": "Запрос выполнен успешно"}
-            else:
-                raise Exception(f'Ошибка при обработке ответа! HTTP Код состояния: {response.status_code}, содержимое: {response.text}')
-        except json.decoder.JSONDecodeError:
-            raise ValueError(f"Ошибка декодирования JSON: Код HTTP '{response.status_code}'\nТело ответа: '{response.text}'")
+            response = self.session.request(method, self.URL + uri_path, **options)
+            try:
+                if response.status_code == 200:
+                    if response.text:
+                        return response.json()
+                    elif not response.text:
+                        return {"message": "Запрос выполнен успешно"}
+                elif response.status_code == 400:
+                    return response.json()
+                else:
+                    raise ValueError(f'Ошибка при обработке ответа! HTTP Код состояния: {response.status_code}, содержимое: {response.text}')
+            except json.decoder.JSONDecodeError:
+                raise ValueError(f"Ошибка декодирования JSON: Код HTTP '{response.status_code}'\nТело ответа: '{response.text}'")
+
+        except Exception:
+            raise
 
     def unique_code(self, unique_code: str):
         """
         Поиск и проверка платежа по уникальному коду.
 
         Args:
             unique_code (int): 	уникальный 16-ти значный код, который покупатель получает после оплаты.
```

### Comparing `digiseller_api_python-1.4.1/digiseller_api_python.egg-info/PKG-INFO` & `digiseller_api_python-1.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,74 @@
-Metadata-Version: 2.1
-Name: digiseller_api_python
-Version: 1.4.1
-Summary: Interaction with Digiseller API
-Home-page: https://github.com/Ernieleo/Digiseller-API-Python
-Author: Ernieleo
-Author-email: ernieleo@vk.com
-Project-URL: Documentation, https://my.digiseller.com/inside/api.asp
-Keywords: api client
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Digiseller API python
-Код предоставляется как есть, любые предложения по улучшению - исправлению приветствуются.  
-Функционал основан на информации с сайта Digiseller.  
-
-Данный проект не является официальным, мы не имеем никакого отношения к команде разработчиков сервиса Digiseller.
-Возможны ошибки в работе некоторых методов, комплексного тестирования не проводилось.  
-Не каждый запрос API и его описание в документации на сайте Digiseller соответствует действительности.
+# Digiseller API Python
+
+[![PyPI version](https://img.shields.io/pypi/v/digiseller-api-python.svg)](https://pypi.org/project/digiseller-api-python)
+[![Downloads](https://img.shields.io/pypi/dm/digiseller-api-python)](https://pypistats.org/packages/digiseller-api-python)
+[![License](https://img.shields.io/github/license/Ernieleo/digiseller-api-python)](https://github.com/Ernieleo/digiseller-api-python/blob/main/LICENSE)
+
+Digiseller API Python — это библиотека Python для доступа к API Digiseller. 
+
+Добавлено 70 методов из числа представленных в документации.
+
+**Важное примечание**: Данный проект не является официальным.  
+Я не имею никакого отношения к команде разработчиков сервиса Digiseller.  
+
+Возможны ошибки в некоторых запросах, так как комплексное тестирование не проводилось.  
+Часть запросов из документации на сайте Digiseller не соответствуют действительности.  
+
+Ознакомиться с документацией API вы можете на [сайте Digiseller](https://my.digiseller.com/inside/api.asp)
+
 ## Установка
 
-Установить с [pypi.org](https://pypi.org/project/digiseller-api-python/)
+Вы можете установить с сервиса [PyPI](https://pypi.org/project/digiseller-api-python/)
+
 ```sh
-pip3 install digiseller-api-python
+pip install digiseller-api-python
 ```
 
-Для ручной установки: [ernieleo/digiseller-api-python](https://github.com/Ernieleo/digiseller-api-python) с репозитория.
+Для ручной установки с репозитория
 ```sh
 pip3 install git+https://github.com/Ernieleo/digiseller-api-python.git
-```
+````
 
-## Подключение
-Получить API Ключ [👉тут👈](https://my.digiseller.com/inside/api_keys.asp)  
-Получить ID Продавца [👉тут👈](https://my.digiseller.com/)
+## Простая демонстрация
 
-Инициализировать класс модуля с передачей ID продавца и API Ключа
+Получить API Ключ 👉[тут](https://my.digiseller.com/inside/api_keys.asp)👈  
+Получить ID Продавца 👉[тут](https://my.digiseller.com/)👈
 
-```py
+```python
 from digiseller_api_python import Api
 
-api = Api(seller_id="ВашSellerID", api_key="API-KEY")
-print(api.chat_list(...))
+Digiseller_Api = Api(seller_id="11155533", api_key="CA1SF69A000A46D00039F01Z11017V39")
+
+# Получение данных пользователя указанных при заказе по уникальному коду
+def get_account_info_from_digiseller(unique_code):
+    data = Digiseller_Api.unique_code(unique_code)
+    email = None
+    password = None
+
+    for option in data["options"]:
+        if option["name"] in ["Почта аккаунта ChatGPT", "ChatGPT account email"]:
+            email = option["value"]
+        elif option["name"] in ["Пароль аккаунта ChatGPT", "ChatGPT account password"]:
+            password = option["value"]
+
+    return email, password
 ```
 
-## Доступные вызовы API
-Сгенерирован список с помощью ChatGPT, возможны опечатки.
+Используется для получения логина и пароля указанных покупателем при оформлении заказа в полях ввода (Параметры) текстовых данных. Поиск требуемого поля осуществляется по названию, указывается названия поля на двух языках, название поля параметра полученного в сведениях о заказе по уникальному коду, зависит от языка браузера пользователя.
+
+## Разработка
+Любой вклад в проект приветствуется.  
+Если вы хотите помочь в разработке, следуйте правилам API сервиса Digiseller и придерживайтесь общего стиля кода. Создайте запрос на cлияние и я его рассмотрю!
+
+## Доступные методы API
+Cписок был сгенерирован при помощи ChatGPT, возможны неточности.  
+Каждая функция вызова описана в самом коде, смотрите информацию в IDE. 
 
-Параметры взяты с официальной документации, значения соответствуют.
+Параметры запросов с документации API, значения соответствуют.
 1. Название: `Поиск и проверка платежа по уникальному коду`
     - Функция: `unique_code`
     - Параметры: `unique_code: str`
     - Ответ: `Ответ от сервера в формате JSON`
     - [Ссылка на API](https://my.digiseller.com/inside/api_general.asp#searchuniquecode)
 
 2. Название: `Информация о продаже по номеру заказа`
```

### Comparing `digiseller_api_python-1.4.1/setup.py` & `digiseller_api_python-1.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='digiseller_api_python',
-    version='1.4.1',
+    version='1.4.2',
     author='Ernieleo',
     author_email='ernieleo@vk.com',
-    description='Interaction with Digiseller API',
+    description='Interaction with Digiseller API via Python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Ernieleo/Digiseller-API-Python',
     packages=find_packages(),
     install_requires=['requests>=2.31.0'],
     classifiers=[
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
-    keywords='api client',
+    keywords='digiseller api python',
     project_urls={
-        'Documentation': 'https://my.digiseller.com/inside/api.asp'
+        'Documentation': 'https://my.digiseller.com/inside/api.asp',
+        'Download': 'https://pypi.org/project/digiseller-api-python/',
+        'Write me': 'https://t.me/ernieleo'
     },
-    python_requires='>=3.7'
+    python_requires='>=3.8'
 )
```

