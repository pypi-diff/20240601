# Comparing `tmp/pydolarvenezuela-1.6.1.tar.gz` & `tmp/pydolarvenezuela-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.6.1.tar", last modified: Thu May 30 07:43:31 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.6.2.tar", last modified: Sat Jun  1 18:32:06 2024, max compression
```

## Comparing `pydolarvenezuela-1.6.1.tar` & `pydolarvenezuela-1.6.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:31.051182 pydolarvenezuela-1.6.1/
--rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.6.1/LICENSE
--rw-rw-rw-   0        0        0    19253 2024-05-30 07:43:31.046187 pydolarvenezuela-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2024-05-30 04:08:53.000000 pydolarvenezuela-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:30.896197 pydolarvenezuela-1.6.1/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2794 2024-05-30 07:42:54.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:30.935191 pydolarvenezuela-1.6.1/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:30.965189 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/images.py
--rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/monitor.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      605 2024-05-30 03:42:26.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:31.011205 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5893 2024-05-30 07:42:25.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/alcambio.py
--rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:31.035187 pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/calculator.py
--rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/extras.py
--rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/time.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:43:31.039188 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0    19253 2024-05-30 07:43:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      933 2024-05-30 07:43:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:43:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-30 07:43:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-30 07:43:30.000000 pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-30 07:43:01.000000 pydolarvenezuela-1.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 07:43:31.051182 pydolarvenezuela-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-30 07:43:05.000000 pydolarvenezuela-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:06.102986 pydolarvenezuela-1.6.2/
+-rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0    19254 2024-06-01 18:32:06.097984 pydolarvenezuela-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4970 2024-06-01 18:11:34.000000 pydolarvenezuela-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:05.836986 pydolarvenezuela-1.6.2/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2285 2024-06-01 18:18:48.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:05.904986 pydolarvenezuela-1.6.2/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:05.963993 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/monitor.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0     1708 2024-06-01 18:19:28.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:06.022986 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     6818 2024-06-01 04:32:39.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/alcambio.py
+-rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:06.081987 pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/calculator.py
+-rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/extras.py
+-rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/time.py
+-rw-rw-rw-   0        0        0      824 2024-06-01 18:10:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela/version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:32:06.088984 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0    19254 2024-06-01 18:32:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2024-06-01 18:32:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 18:32:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-06-01 18:32:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 18:32:05.000000 pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-06-01 18:09:42.000000 pydolarvenezuela-1.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 18:32:06.104984 pydolarvenezuela-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-06-01 18:09:47.000000 pydolarvenezuela-1.6.2/setup.py
```

### Comparing `pydolarvenezuela-1.6.1/LICENSE` & `pydolarvenezuela-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/PKG-INFO` & `pydolarvenezuela-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.6.1
+Version: 1.6.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -230,15 +230,15 @@
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| AlCambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
+| Al Cambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
```

### Comparing `pydolarvenezuela-1.6.1/README.md` & `pydolarvenezuela-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| AlCambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
+| Al Cambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
```

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/models/monitor.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/models/monitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,25 +51,56 @@
                 if property not in ('banks', 'last_update'):
                     try:
                         self._update_item(old_data, values, property)
                     except KeyError:
                         pass
                 elif property == 'banks': # Comparación de propiedades de los datos BCV
                     banks = values[property]
-                    for i, bank in enumerate(old_data[property]):
-                        if i < len(banks) and bank['title'] == banks[i]['title']:
-                            self._update_item(old_data[property], banks, i)
+                    for i, _ in enumerate(banks):
+                        self._update_item(old_data[property], banks, i)
                 elif property == 'last_update':
                     old_data[property] = values[property]
 
             self._redis.set_data(key, json.dumps(old_data), self.db.ttl)
             values = json.loads(self._redis.get_data(key))
             
         return values 
     
+    def _update_price(self, old_data: dict, new_data: dict, i: Any):
+        old_price = old_data[i]['price']
+        new_price = new_data[i]['price']
+        price_old = new_data[i].get('price_old', None) # Valor preciso
+        change    = round(float(new_price - old_price), 2)
+        percent   = float(f'{round(float((change / new_price) * 100 if old_price != 0 else 0), 2)}'.replace('-', ' '))
+        symbol    = "" if change == 0 else "▲" if change >= 0 else "▼"
+        color     = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
+        last_update = new_data[i].get('last_update', None)
+
+        change = float(str(change).replace('-', ' '))
+
+        old_data[i].update({
+            'price': new_price,
+            'change': change,
+            'percent': percent,
+            'color': color,
+            'symbol': symbol,
+        })
+        
+        # Comprueba si los atributos tienen valor. se agregan y/o actualizan
+        if last_update and price_old:
+            old_data[i].update({
+                'price_old': price_old,
+                'last_update': last_update
+            })
+            
+        elif last_update: 
+            old_data[i].update({
+                'last_update': last_update
+            })
+
     def _update_item(self, old_data: dict, new_data: dict, i: Any):
         """
         Evalúa la estructura de cada monitor en `old_data`. Elimina los atributos que sean `None` (Cada estructura es diferente según el proveedor) y realiza los cálculos necesarios.
 
         Estructura inicial (para la primera vez):
         ```python
         class Monitor:
@@ -80,51 +111,38 @@
             image: Optional[str] = None  
             percent: Optional[float] = 0.0
             change: Optional[float] = 0.0  
             color: Optional[str] = "neutral" 
             symbol: Optional[str] = "" 
         ```
         """
-        structure_monitor = asdict(Monitor(**old_data[i]))
-        for key in list(structure_monitor.keys()):
-            if structure_monitor[key] is None:
-                del structure_monitor[key]
-        old_data[i] = structure_monitor
         
-        if old_data[i]['price'] != new_data[i]['price']:
-            old_price = old_data[i]['price']
-            new_price = new_data[i]['price']
-            price_old = new_data[i].get('price_old', None) # Valor preciso
-            change    = round(float(new_price - old_price), 2)
-            percent   = float(f'{round(float((change / new_price) * 100 if old_price != 0 else 0), 2)}'.replace('-', ' '))
-            symbol    = "" if change == 0 else "▲" if change >= 0 else "▼"
-            color     = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
-            last_update = new_data[i].get('last_update', None)
-
-            change = float(str(change).replace('-', ' '))
+        if isinstance(i, str) or isinstance(i, int) and i < len(old_data):
+            structure_monitor = asdict(Monitor(**old_data[i]))
+            for key in list(structure_monitor.keys()):
+                if structure_monitor[key] is None:
+                    del structure_monitor[key]
+            old_data[i] = structure_monitor
 
-            old_data[i].update({
-                'price': new_price,
-                'change': change,
-                'percent': percent,
-                'color': color,
-                'symbol': symbol,
-            })
-            
-            # Comprueba si los atributos tienen valor. se agregan y/o actualizan
-            if last_update and price_old:
-                old_data[i].update({
-                    'price_old': price_old,
-                    'last_update': last_update
-                })
-                
-            elif last_update: 
-                old_data[i].update({
-                    'last_update': last_update
-                })
+        # Ambos consultan si el precio es diferente para realizar cambios.
+        # Hay diferentes datos que se distribuyeron como list, {str: dict}.
+        if isinstance(i, int): # Actualiza los datos de 'old_data' con los datos de 'new_data' basándose en el título del item.
+            title_items = [item['title'] for item in old_data]
+            if new_data[i]['title'] in title_items:
+                index_old_data = title_items.index(new_data[i]['title'])
+                if old_data[index_old_data]['price'] != new_data[i]['price']:
+                    self._update_price(old_data, new_data, index_old_data)
+            else:
+                old_data.append(new_data[i])
+        else: # Actualiza los datos de 'old_data' con los datos de 'new_data' basándose en el key del item.
+            if i in old_data: 
+                if old_data[i]['price'] != new_data[i]['price']:
+                    self._update_price(old_data, new_data, i)
+            else:
+                old_data[i] = new_data[i]
 
     def _get_values_specifics(self, type_monitor: str = None, property: str = None, prettify: bool = False):
         data = self._load_data()
         if not type_monitor:
             return data
         
         try:
```

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/alcambio.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/alcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/calculator.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/extras.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/extras.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela/utils/time.py` & `pydolarvenezuela-1.6.2/pyDolarVenezuela/utils/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.6.1
+Version: 1.6.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -230,15 +230,15 @@
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
 | Exchange Monitor | https://exchangemonitor.net/dolar-venezuela | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | CriptoDolar | https://criptodolar.net/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | BCV (Banco Central de Venezuela) | http://www.bcv.org.ve/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 | Italcambio | https://www.italcambio.com/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
-| AlCambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
+| Al Cambio | https://alcambio.app/ | ![Active](https://img.shields.io/badge/Activo-brightgreen) |
 
 pyDolarVenezuela tiene como objetivo principal brindar una solución eficiente y confiable para acceder a información relevante sobre el valor del dólar en Venezuela, ofreciendo así una herramienta valiosa para desarrolladores interesados en trabajar en este ámbito.
 
 ## Instalación
 ``` sh
 pip install pyDolarVenezuela
 ```
```

### Comparing `pydolarvenezuela-1.6.1/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.6.2/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pyDolarVenezuela/__init__.py
 pyDolarVenezuela/network.py
 pyDolarVenezuela/pages.py
+pyDolarVenezuela/version.py
 pyDolarVenezuela.egg-info/PKG-INFO
 pyDolarVenezuela.egg-info/SOURCES.txt
 pyDolarVenezuela.egg-info/dependency_links.txt
 pyDolarVenezuela.egg-info/requires.txt
 pyDolarVenezuela.egg-info/top_level.txt
 pyDolarVenezuela/data/__init__.py
 pyDolarVenezuela/data/redis.py
```

### Comparing `pydolarvenezuela-1.6.1/pyproject.toml` & `pydolarvenezuela-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.6.1"
+version = "1.6.2"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.6.1/setup.py` & `pydolarvenezuela-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.6.1'
+VERSION = '1.6.2'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

