# Comparing `tmp/monstr_terminal-0.1.1.tar.gz` & `tmp/monstr_terminal-0.1.2.tar.gz`

## Comparing `monstr_terminal-0.1.1.tar` & `monstr_terminal-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/.gitmodules
--rw-r--r--   0        0        0   125183 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/event_view.png
--rw-r--r--   0        0        0    59976 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/poster.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/__init__.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/alias.py
--rw-r--r--   0        0        0    42601 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/event_view.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/event_view_consumer.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/mirror.py
--rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/poster.py
--rw-r--r--   0        0        0    16199 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/profile_search.py
--rw-r--r--   0        0        0    19945 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/run_relay.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/signer.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/app/__init__.py
--rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/app/post.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/__init__.py
--rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/message_app.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/post_loop_app.py
--rw-r--r--   0        0        0    20615 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/LICENSE
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    15762 2020-02-02 00:00:00.000000 monstr_terminal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   125183 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/event_view.png
+-rw-r--r--   0        0        0    59976 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/poster.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/__init__.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/alias.py
+-rw-r--r--   0        0        0    42624 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/event_view.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/event_view_consumer.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/mirror.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/poster.py
+-rw-r--r--   0        0        0    16199 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/profile_search.py
+-rw-r--r--   0        0        0    16329 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/run_relay.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/signer.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/app/__init__.py
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/app/post.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/__init__.py
+-rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/message_app.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/post_loop_app.py
+-rw-r--r--   0        0        0    20623 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/LICENSE
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15762 2020-02-02 00:00:00.000000 monstr_terminal-0.1.2/PKG-INFO
```

### Comparing `monstr_terminal-0.1.1/event_view.png` & `monstr_terminal-0.1.2/event_view.png`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/poster.png` & `monstr_terminal-0.1.2/poster.png`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/alias.py` & `monstr_terminal-0.1.2/src/monstr_terminal/alias.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/event_view.py` & `monstr_terminal-0.1.2/src/monstr_terminal/event_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from monstr.ident.profile import ContactList
 from monstr.client.client import ClientPool, Client
 from monstr.client.event_handlers import DeduplicateAcceptor, LengthAcceptor, \
     NotOnlyNumbersAcceptor, EventHandler, LastEventHandler, FilterAcceptor
 from monstr.util import util_funcs, ConfigError
 from monstr.inbox import Inbox
 from monstr.encrypt import Keys
-from monstr.signing import SignerInterface, BasicKeySigner
+from monstr.signing.signing import SignerInterface, BasicKeySigner
 from monstr.event.event import Event
 from monstr_terminal.cmd_line.util import FormattedEventPrinter, JSONPrinter, ContentPrinter
 from monstr_terminal.util import load_toml, get_keys_from_str
 
 # defaults if not otherwise given
 # working directory it'll be created it it doesn't exist
 WORK_DIR = f'{Path.home()}/.nostrpy/'
@@ -1016,15 +1016,15 @@
             asyncio.create_task(print_handler.ado_event(
                 the_client=None,
                 sub_id=None,
                 evt=events))
             last_event_track.do_event(the_client, sub_id, events)
 
         # called at query completetion - which might not be until timeout if we have bad relays
-        def first_pull_complete():
+        def first_pull_complete(events: [Event]):
             nonlocal keep_running
             keep_running = exit == 'never'
             if keep_running:
                 asyncio.create_task(my_printer.astatus('*** listening for more events ***'))
 
         # TODO: fix client so that do event can be [handlers] and we wouldnt need adhoc_do_event
         await my_client.query(filters=boot_e_filter,
```

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/event_view_consumer.py` & `monstr_terminal-0.1.2/src/monstr_terminal/event_view_consumer.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/mirror.py` & `monstr_terminal-0.1.2/src/monstr_terminal/mirror.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/poster.py` & `monstr_terminal-0.1.2/src/monstr_terminal/poster.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from monstr.ident.alias import ProfileFileAlias
 from monstr.client.client import ClientPool, Client
 from monstr.event.event import Event
 from monstr_terminal.app.post import PostApp
 from monstr.inbox import Inbox
 from monstr_terminal.cmd_line.post_loop_app import PostAppGui
 from monstr.encrypt import Keys
-from monstr.signing import BasicKeySigner, SignerInterface
+from monstr.signing.signing import BasicKeySigner, SignerInterface
 from monstr.util import util_funcs, ConfigError
 from monstr_terminal.util import load_toml
 
 # defaults if not otherwise given
 # working directory it'll be created it it doesn't exist
 WORK_DIR = f'{Path.home()}/.nostrpy/'
 # relay/s to attach to
```

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/profile_search.py` & `monstr_terminal-0.1.2/src/monstr_terminal/profile_search.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/run_relay.py` & `monstr_terminal-0.1.2/src/monstr_terminal/run_relay.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import shutil
 try:
     from stem.control import Controller
 except Exception as e:
     pass
 from monstr.relay.relay import Relay
 from monstr.relay.accept_handlers import LengthAcceptReqHandler, CreateAtAcceptor, AuthenticatedAcceptor
+from monstr.relay.tor import TORService
 from monstr.event.persist_postgres import RelayPostgresEventStore
 from monstr.event.persist_sqlite import ARelaySQLiteEventStore
 from monstr.event.persist_memory import RelayMemoryEventStore
 from monstr.event.expire import ASQLiteNIP40Expirer, MemoryNIP40Expirer
 from monstr.util import ConfigError
 from monstr_terminal.util import load_toml
 import ssl
@@ -398,122 +399,29 @@
 
 
     # access via tor?
     if enable_tor:
         with TORService(relay_port=port,
                         service_dir=tor_dir,
                         password=tor_password,
-                        isSSL=protocol=='wss',
+                        is_ssl=protocol=='wss',
                         empheral=tor_empheral) as my_tor:
             print_run_info()
             await my_relay.start(host=host,
                                  port=port,
                                  end_point=end_point,
                                  ssl_context=ssl_context)
     else:
         print_run_info()
         await my_relay.start(host=host,
                              port=port,
                              end_point=end_point,
                              ssl_context=ssl_context)
 
 
-class TORService:
-
-    def __init__(self, relay_port, service_dir=None, password=None, isSSL = False, empheral=True):
-        try:
-            if Controller:
-                pass
-        except NameError as ne:
-            raise ConfigError(f'No Controller class - try pip install stem')
-
-        # the relays actual port if we were to it normally
-        self._relay_port = relay_port
-
-
-
-        # password used to auth with controller
-        # best to supply - but without and if tor_browser is running we still might be ok
-        # (don't quite understand the exact way this is working)
-        self._password = password
-
-        # the tor service will either be on port 80 http or 443 https
-        self._service_port = 80
-        if isSSL:
-            self._service_port = 443
-
-        # create the tor service as empheral
-        self._empheral = empheral
-
-        # if not empheral then this is the directory where the hidden service will be created
-        # just give the actual dir, the full path is worked out using the controller class
-        # for example something like/home/monty/tor-browser/Browser/TorBrowser/Data/[service_dir]
-        self._hidden_service_dir = service_dir
-        if self._hidden_service_dir is None:
-            self._hidden_service_dir = 'monstr_relay'
-
-
-
-    def __enter__(self):
-        # this will be default port probably 9051
-        self._controller = Controller.from_port()
-        if self._password is None:
-            self._controller.authenticate()
-        else:
-            self._controller.authenticate(password=self._password)
-
-
-        # address of service when we have it
-        onion_addr = None
-
-        # we'll get a new onion address each time
-        if self._empheral:
-            print(self._service_port)
-            result = self._controller.create_ephemeral_hidden_service({self._service_port: self._relay_port},
-                                                                      await_publication=True)
-
-            onion_addr = result.service_id + '.onion'
-
-        # after first create the onion address will be the same
-        else:
-            base_dir = self._controller.get_conf('DataDirectory', '/tmp')
-            actual_dir = os.path.join(base_dir, self._hidden_service_dir)
-
-            print(f' * Creating our hidden service {self._hidden_service_dir} in {base_dir}')
-            result = self._controller.create_hidden_service(actual_dir,
-                                                            self._service_port,
-                                                            target_port=self._relay_port)
-
-            onion_addr = None
-            if result:
-                onion_addr = result.hostname
-            else:
-                # probably the service already exists, try open the service_dir/hostname file
-                # not sure why create_hidden_services doesn't just return that for us anyway?
-                try:
-                    f = open(os.path.join(actual_dir, 'hostname'), "r")
-                    lines = f.readlines()
-                    onion_addr = lines[0]
-                except Exception as e:
-                    pass
-
-        if onion_addr:
-            print(f" hidden service is available at {onion_addr}")
-        else:
-            print(
-                f" Unable to determine our service's hostname, probably due to being unable to read the hidden service directory")
-
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        print(" * Shutting down our hidden service")
-        self._controller.close()
-        self._controller.remove_hidden_service(self._hidden_service_dir)
-        shutil.rmtree(self._hidden_service_dir)
-
-
 if __name__ == "__main__":
     logging.getLogger().setLevel(logging.ERROR)
 
     def sigint_handler(signal, frame):
         sys.exit(0)
 
     signal.signal(signal.SIGINT, sigint_handler)
```

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/util.py` & `monstr_terminal-0.1.2/src/monstr_terminal/util.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/app/post.py` & `monstr_terminal-0.1.2/src/monstr_terminal/app/post.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/message_app.py` & `monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/message_app.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/post_loop_app.py` & `monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/post_loop_app.py`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/src/monstr_terminal/cmd_line/util.py` & `monstr_terminal-0.1.2/src/monstr_terminal/cmd_line/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from prompt_toolkit.formatted_text import FormattedText
 from monstr.event.event import Event
 from monstr.encrypt import Keys
 from monstr.inbox import Inbox
 from monstr.client.client import Client
 from monstr.ident.profile import Profile, NIP5Helper, NIP5Error
 from monstr.ident.event_handlers import ProfileEventHandler
-from monstr.signing import SignerInterface
+from monstr.signing.signing import SignerInterface
 from monstr.entities import Entities
 from monstr.util import util_funcs
 
 
 class EventPrinter:
 
     # print the event
```

### Comparing `monstr_terminal-0.1.1/LICENSE` & `monstr_terminal-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/README.md` & `monstr_terminal-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `monstr_terminal-0.1.1/pyproject.toml` & `monstr_terminal-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "monstr>=0.1.2",
+    "monstr>=0.1.6",
     "prompt_toolkit>=3.0.38",
     "toml>=0.10.2",
 ]
 
 [project.urls]
 Documentation = "https://github.com/monty888/monstr_terminal#readme"
 Issues = "https://github.com/monty888/monstr_terminal/issues"
```

### Comparing `monstr_terminal-0.1.1/PKG-INFO` & `monstr_terminal-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: monstr-terminal
-Version: 0.1.1
+Version: 0.1.2
 Summary: Monstr Terminal: command line tools for nostr
 Project-URL: Documentation, https://github.com/monty888/monstr_terminal#readme
 Project-URL: Issues, https://github.com/monty888/monstr_terminal/issues
 Project-URL: Source, https://github.com/monty888/monstr_terminal
 Author-email: monty <monty@monty888.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: monstr>=0.1.2
+Requires-Dist: monstr>=0.1.6
 Requires-Dist: prompt-toolkit>=3.0.38
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
 # install
 
 ```sh
```

