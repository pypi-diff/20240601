# Comparing `tmp/zabbix_cachet-2.1.1.tar.gz` & `tmp/zabbix_cachet-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zabbix_cachet-2.1.1.tar", max compression
+gzip compressed data, was "zabbix_cachet-2.1.2.tar", max compression
```

## Comparing `zabbix_cachet-2.1.1.tar` & `zabbix_cachet-2.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1083 2017-01-30 15:57:26.000000 zabbix_cachet-2.1.1/LICENSE
--rw-r--r--   0        0        0     3045 2024-05-26 20:39:13.438929 zabbix_cachet-2.1.1/README.md
--rw-r--r--   0        0        0      646 2024-05-26 20:42:28.720469 zabbix_cachet-2.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.1/src/zabbix_cachet/__init__.py
--rw-r--r--   0        0        0    12408 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.1/src/zabbix_cachet/cachet.py
--rw-r--r--   0        0        0      524 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.1/src/zabbix_cachet/excepltions.py
--rwxr-xr-x   0        0        0    18036 2024-05-26 20:42:28.732469 zabbix_cachet-2.1.1/src/zabbix_cachet/main.py
--rw-r--r--   0        0        0     9575 2024-05-19 17:17:19.654178 zabbix_cachet-2.1.1/src/zabbix_cachet/zabbix.py
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 zabbix_cachet-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-01-30 15:57:26.000000 zabbix_cachet-2.1.2/LICENSE
+-rw-r--r--   0        0        0     3064 2024-05-26 20:58:53.828499 zabbix_cachet-2.1.2/README.md
+-rw-r--r--   0        0        0      646 2024-06-01 13:08:13.715304 zabbix_cachet-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.2/src/zabbix_cachet/__init__.py
+-rw-r--r--   0        0        0    12408 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.2/src/zabbix_cachet/cachet.py
+-rw-r--r--   0        0        0      524 2024-05-05 00:47:43.490949 zabbix_cachet-2.1.2/src/zabbix_cachet/excepltions.py
+-rwxr-xr-x   0        0        0    17824 2024-06-01 13:05:44.898231 zabbix_cachet-2.1.2/src/zabbix_cachet/main.py
+-rw-r--r--   0        0        0     9704 2024-06-01 11:33:06.247076 zabbix_cachet-2.1.2/src/zabbix_cachet/zabbix.py
+-rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 zabbix_cachet-2.1.2/PKG-INFO
```

### Comparing `zabbix_cachet-2.1.1/LICENSE` & `zabbix_cachet-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zabbix_cachet-2.1.1/README.md` & `zabbix_cachet-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
    ```bash
    pip install zabbix-cachet
    ```
 2. Rename `config-example.yml` to `config.yml` and fill a file with your settings.
 3. Define `CONFIG_FILE` environment variable which point to your `config.yml` or change current work directory to folder with config 
 4. Launch `zabbix-cachet`
 
-## Apt
+## Apt (outdated release)
 1. Add official Zabbix-Cachet [PPA](https://launchpad.net/~reg-tem4uk/+archive/ubuntu/zabbix-cachet):
     ```bash
     add-apt-repository ppa:reg-tem4uk/zabbix-cachet
     apt-get update
     ```
 2. Install the package: `apt-get install zabbix-cachet`
 3. Configure it: `nano /etc/zabbix-cachet.yml`
```

### Comparing `zabbix_cachet-2.1.1/pyproject.toml` & `zabbix_cachet-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zabbix-cachet"
-version = "2.1.1"
+version = "2.1.2"
 description = "Python daemon which provides synchronisation between Zabbix IT Services and Cachet"
 authors = ["Artem Alexandrov <qk4l@tem4uk.ru>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.8,<4.0"
```

### Comparing `zabbix_cachet-2.1.1/src/zabbix_cachet/cachet.py` & `zabbix_cachet-2.1.2/src/zabbix_cachet/cachet.py`

 * *Files identical despite different names*

### Comparing `zabbix_cachet-2.1.1/src/zabbix_cachet/excepltions.py` & `zabbix_cachet-2.1.2/src/zabbix_cachet/excepltions.py`

 * *Files identical despite different names*

### Comparing `zabbix_cachet-2.1.1/src/zabbix_cachet/main.py` & `zabbix_cachet-2.1.2/src/zabbix_cachet/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,23 @@
 
 from zabbix_cachet.cachet import Cachet
 from zabbix_cachet.excepltions import ZabbixNotAvailable, ZabbixCachetException
 from zabbix_cachet.zabbix import Zabbix, ZabbixService
 
 __author__ = 'Artem Aleksandrov <qk4l()tem4uk.ru>'
 __license__ = """The MIT License (MIT)"""
-__version__ = '2.1.1'
+__version__ = '2.1.2'
+
+
+@dataclass
+class ConfigTemplates:
+    acknowledgement: str = "{message}\n\n###### {ack_time} by {author}\n\n______\n"
+    acknowledgement_time_strftime: str = '%b %d, %H:%M %z'
+    investigating: str = ''
+    resolving: str = ''
 
 
 class Config:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
@@ -52,25 +60,15 @@
             self.app_settings = config['settings']
 
             if self.app_settings.get('time_zone'):
                 self.tz = pytz.timezone(self.app_settings['time_zone'])
             else:
                 self.tz = None
 
-            incident_templates_defaults = {
-                'acknowledgement': "{message}\n\n###### {ack_time} by {author}\n\n______\n",
-                'investigation': '',
-                'resolving': '',
-            }
-
-            self.templates = config.get('templates')
-            for template_name, default_value in incident_templates_defaults.items():
-                if self.templates.get(template_name, None) is None:
-                    self.templates[template_name] = default_value
-
+            self.templates = ConfigTemplates(**config.get('templates'))
             self.initialized = True
 
 
 @dataclass
 class ZabbixCachetMap:
     cachet_component_id: int
     cachet_component_name: str
@@ -98,14 +96,19 @@
         5 - disaster.
     Cachet Incident Statuses:
         0 - Scheduled - This status is used for a scheduled status.
         1 - Investigating - You have reports of a problem, and you're currently looking into them.
         2 - Identified - You've found the issue, and you're working on a fix.
         3 - Watching - You've since deployed a fix, and you're currently watching the situation. # Does not use for now
         4 - Fixed
+
+    Zabbix Trigger <> Cachet Incident mapping
+        New - Investigating
+        Acknowledged - Identified
+        Resolved - Fixed
     @return: boolean
     """
     config = Config()
     for i in service_map:  # type: ZabbixCachetMap
         # inc_status = 1
         # comp_status = 1
         # inc_name = ''
@@ -123,20 +126,17 @@
             # component in operational mode
             if str(component_status) == '1':
                 continue
             else:
                 # component not operational mode. Resolve it.
                 last_inc = cachet.get_incident(i.cachet_component_id)
                 if str(last_inc['id']) != '0':
-                    if config.templates['resolving']:
-                        inc_msg = config.templates['resolving'].format(
-                            time=datetime.datetime.now(tz=config.tz).strftime('%b %d, %H:%M'),
-                        ) + cachet.get_incident(i.cachet_component_id)['message']
-                    else:
-                        inc_msg = cachet.get_incident(i.cachet_component_id)['message']
+                    inc_msg = config.templates.resolving.format(
+                        time=datetime.datetime.now(tz=config.tz).strftime('%b %d, %H:%M'),
+                    ) + cachet.get_incident(i.cachet_component_id)['message']
                     cachet.upd_incident(last_inc['id'],
                                         status=4,
                                         component_id=i.cachet_component_id,
                                         component_status=1,
                                         message=inc_msg)
                 # Incident does not exist. Just change component status
                 else:
@@ -167,20 +167,18 @@
             if not zbx_event:
                 logging.warning(f'Failed to get zabbix event for trigger {trigger_id}')
                 # Mock zbx_event for further usage
                 zbx_event = {'acknowledged': '0'}
             if zbx_event.get('acknowledged', '0') == '1':
                 inc_status = 2
                 for msg in zbx_event['acknowledges']:  # type: dict
-                    # TODO: Add timezone?
-                    #       Move format to config file
                     author = msg.get('name', '') + ' ' + msg.get('surname', '')
-                    ack_time = datetime.datetime.fromtimestamp(int(msg['clock']), tz=config.tz).strftime(
-                        '%b %d, %H:%M')
-                    ack_msg = config.templates['acknowledgement'].format(
+                    ack_time = (datetime.datetime.fromtimestamp(int(msg['clock']), tz=config.tz).
+                                strftime(config.templates.acknowledgement_time_strftime))
+                    ack_msg = config.templates.acknowledgement.format(
                         message=msg['message'],
                         ack_time=ack_time,
                         author=author
                     )
                     if ack_msg not in inc_msg:
                         inc_msg = ack_msg + inc_msg
             else:
@@ -190,29 +188,30 @@
             if int(trigger['priority']) >= 4:
                 comp_status = 4
             elif int(trigger['priority']) == 3:
                 comp_status = 3
             else:
                 comp_status = 2
 
-            if not inc_msg and config.templates['']:
+            if not inc_msg and config.templates.investigating:
                 if zbx_event:
                     zbx_event_clock = int(zbx_event.get('clock'))
                     zbx_event_time = datetime.datetime.fromtimestamp(zbx_event_clock, tz=config.tz).strftime(
                         '%b %d, %H:%M')
                 else:
                     zbx_event_time = ''
-                inc_msg = config.templates['investigation'].format(
+                inc_msg = config.templates.investigating.format(
                     group=i.cachet_group_name,
                     component=i.cachet_component_name,
                     time=zbx_event_time,
                     trigger_description=trigger.get('comments', ''),
                     trigger_name=trigger.get('description', ''),
                 )
 
+            # Just in case when user set investigating template to empty string
             if not inc_msg and trigger.get('comments'):
                 inc_msg = trigger.get('comments')
             elif not inc_msg:
                 inc_msg = trigger.get('description')
 
             if i.cachet_group_name:
                 inc_name = i.cachet_group_name + ' | ' + inc_name
```

### Comparing `zabbix_cachet-2.1.1/src/zabbix_cachet/zabbix.py` & `zabbix_cachet-2.1.2/src/zabbix_cachet/zabbix.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,24 +115,27 @@
                 tags=tags,
                 only_true=True)
         return trigger
 
     @pyzabbix_safe({})
     def get_event(self, triggerid):
         """
+        https://www.zabbix.com/documentation/current/en/manual/api/reference/event/get
         Get event information based on triggerid
         @param triggerid: string
         @return: dict of data
         """
         zbx_event = self.zapi.event.get(
             select_acknowledges='extend',
             expandDescription='true',
             object=0,
             value=1,
-            objectids=triggerid)
+            objectids=triggerid,
+            sortfield=['clock']
+        )
         if len(zbx_event) >= 1:
             return zbx_event[-1]
         return zbx_event
 
     @pyzabbix_safe([])
     def get_service(self, name: str = '', serviceid: Union[List, str] = None,
                     parentids: str = '') -> List[Dict]:
```

### Comparing `zabbix_cachet-2.1.1/PKG-INFO` & `zabbix_cachet-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zabbix-cachet
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python daemon which provides synchronisation between Zabbix IT Services and Cachet
 License: MIT
 Author: Artem Alexandrov
 Author-email: qk4l@tem4uk.ru
 Requires-Python: >3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
    ```bash
    pip install zabbix-cachet
    ```
 2. Rename `config-example.yml` to `config.yml` and fill a file with your settings.
 3. Define `CONFIG_FILE` environment variable which point to your `config.yml` or change current work directory to folder with config 
 4. Launch `zabbix-cachet`
 
-## Apt
+## Apt (outdated release)
 1. Add official Zabbix-Cachet [PPA](https://launchpad.net/~reg-tem4uk/+archive/ubuntu/zabbix-cachet):
     ```bash
     add-apt-repository ppa:reg-tem4uk/zabbix-cachet
     apt-get update
     ```
 2. Install the package: `apt-get install zabbix-cachet`
 3. Configure it: `nano /etc/zabbix-cachet.yml`
```

