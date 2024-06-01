# Comparing `tmp/ws_sync-0.6.3.tar.gz` & `tmp/ws_sync-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_sync-0.6.3.tar", max compression
+gzip compressed data, was "ws_sync-0.6.4.tar", max compression
```

## Comparing `ws_sync-0.6.3.tar` & `ws_sync-0.6.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4912 2024-02-20 18:33:05.515422 ws_sync-0.6.3/README.md
--rw-r--r--   0        0        0      374 2024-04-24 16:12:00.282742 ws_sync-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      429 2024-04-03 03:54:28.931620 ws_sync-0.6.3/ws_sync/__init__.py
--rw-r--r--   0        0        0     3484 2024-04-03 03:52:59.911008 ws_sync-0.6.3/ws_sync/decorators.py
--rw-r--r--   0        0        0      842 2024-01-31 22:47:04.922252 ws_sync-0.6.3/ws_sync/id.py
--rw-r--r--   0        0        0     5071 2024-04-24 15:50:52.693591 ws_sync-0.6.3/ws_sync/session.py
--rw-r--r--   0        0        0    16692 2024-04-19 10:31:36.837688 ws_sync-0.6.3/ws_sync/sync.py
--rw-r--r--   0        0        0      705 2024-04-03 03:01:49.284779 ws_sync-0.6.3/ws_sync/utils.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ws_sync-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     5106 2024-04-26 03:06:07.270012 ws_sync-0.6.4/README.md
+-rw-r--r--   0        0        0      375 2024-06-01 20:48:31.927358 ws_sync-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      559 2024-04-26 02:52:33.014497 ws_sync-0.6.4/ws_sync/__init__.py
+-rw-r--r--   0        0        0     9235 2024-04-26 03:04:38.100685 ws_sync-0.6.4/ws_sync/decorators.py
+-rw-r--r--   0        0        0      945 2024-04-25 19:10:36.721604 ws_sync-0.6.4/ws_sync/id.py
+-rw-r--r--   0        0        0     5206 2024-04-25 18:45:54.416955 ws_sync-0.6.4/ws_sync/session.py
+-rw-r--r--   0        0        0    16699 2024-04-25 22:52:32.821755 ws_sync-0.6.4/ws_sync/sync.py
+-rw-r--r--   0        0        0      705 2024-04-03 03:01:49.284779 ws_sync-0.6.4/ws_sync/utils.py
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 ws_sync-0.6.4/PKG-INFO
```

### Comparing `ws_sync-0.6.3/README.md` & `ws_sync-0.6.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,89 +24,91 @@
     def add(self, note):
         self.notes.append(note)
 ```
 
 To sync it to the frontend, it is as simple as:
 
 ```diff
-+from ws_sync import Sync
++from ws_sync import sync_all
 
 class Notes:
++   @sync_all("NOTES")  # create the sync object and define the key
     def __init__(self):
         # my attributes, as usual
         self.title = "My Notes"
         self.notes = []
 
-+       # create the sync object and define the key of the object
-+       self.sync = Sync("NOTES", self)
-    
     @property
     def total_length(self):
         return sum(len(note) for note in self.notes)
     
 +   async def rename(self, new_title):
         self.title = new_title
-+       await self.sync() # make sure the frontend knows about the change
++       await self.sync()  # make sure the frontend knows about the change
     
 +   async def add(self, note):
         self.notes.append(note)
-+       await self.sync() # make sure the frontend knows about the change
++       await self.sync()  # make sure the frontend knows about the change
 ```
 
 The `Sync("Notes", self)` call automatically detects the attributes to sync in `self`, which are all attributes or `@properties` that do not start with an underscore. You can also specify the attributes to sync manually:
 
 ```python
-self.sync = Sync("NOTES", self,
+@sync_only("NOTES",
     title = ...,
     notes = ...,
-    total_length = "totalLength",
+    total_length = "size",
 )
 ```
 
 The keyword argument is the local name of the attribute, the value is the name of the attribute in the frontend. If the value is `...`, the local and frontend name are the same. This is useful if you want to rename an attribute in the frontend without changing the name in the backend (e.g. snake_case to camelCase).
 
+For more info on the options and examples, see [ws_sync.decorators docs](https://joongwonseo.github.io/ws-sync/ws_sync/decorators.html).
+
 #### Frontend
-On the frontend, you can use the `useSync` hook to sync the state to the backend:
+On the frontend, you can use the `useSynced` hook to sync the state to the backend:
 
 ```jsx
 const Notes = () => {
-    const notes = useSync("NOTES", {
+    const notes = useSynced("NOTES", {
         title: "",
         notes: [],
     })
 
     return (
         <div>
             <h1>{notes.title}</h1>
             <ul>{notes.notes.map(note => <li>{note}</li>)}</ul>
         </div>
     )
 }
 ```
 
-The second parameter of `useSync` is the initial state.
+The second parameter of `useSynced` is the initial state.
 
 The returned `notes` object not only contains the state, but also the setters and syncers:
 
 ```jsx
 const Notes = () => {
-    const notes = useSync("NOTES", {
+    const notes = useSynced("NOTES", {
         title: "",
         notes: [],
     })
 
     return (
         <div>
             <input value={notes.title} onChange={e => notes.syncTitle(e.target.value)} />
             <ul>{notes.notes.map(note => <li>{note}</li>)}</ul>
         </div>
     )
 }
 ```
 
+For more info on the react library, see [ws-sync-react](https://github.com/JoongWonSeo/ws-sync-react).
+
 ### Actions
 Actions are a way to call methods on the remote (action handlers), usually frontend -> backend.
 
 `TODO`
 
 ### Tasks
 Tasks are like actions, but for long-running operations and can be cancelled.
```

### Comparing `ws_sync-0.6.3/ws_sync/session.py` & `ws_sync-0.6.4/ws_sync/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from starlette.websockets import WebSocket, WebSocketDisconnect
 
 from .utils import nonblock_call
 
 # session context
 session_context: ContextVar[Session] = ContextVar("session_context")
+"""Per-task session context. Within concurrent async tasks, this context variable can be used to access the current Session object."""
 
 
 class Session:
     """
     This is a counter-part to the SessionManager in the frontend.
     There should be one instance of this class per user session, even across reconnects of the websocket. This means the states that belong to the user session should be subscribed to the events of this class.
     It defines a simple state-syncing protocol between the frontend and the backend, every event being of type {type: str, data: any}.
```

### Comparing `ws_sync-0.6.3/ws_sync/sync.py` & `ws_sync-0.6.4/ws_sync/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
     async def __call__(
         self,
         if_since_last: float | None = None,
         toast: str = None,
         type: ToastType = "default",
     ):
-        """
+        """@public
         Sync all registered attributes.
 
         Args:
             if_since_last: only sync if the last sync was before this many seconds
             toast: toast message to send after syncing
             type: toast type
         """
```

### Comparing `ws_sync-0.6.3/ws_sync/utils.py` & `ws_sync-0.6.4/ws_sync/utils.py`

 * *Files identical despite different names*

### Comparing `ws_sync-0.6.3/PKG-INFO` & `ws_sync-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ws-sync
-Version: 0.6.3
+Version: 0.6.4
 Summary: Keep objects synchronized over a persistent WebSocket session
 Author: Joong-Won Seo
 Author-email: joong.won.seo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jsonpatch (>=1.33,<2.0)
-Requires-Dist: starlette (>=0.35.1,<0.36.0)
+Requires-Dist: starlette (>=0.37.2)
 Description-Content-Type: text/markdown
 
 # `ws-sync`: WebSocket Sync
 
 This library defines a very simple WebSocket and JSON & JSON Patch based protocol for keeping the python backend and the browser frontend in sync. There's a [corresponding react library](https://github.com/JoongWonSeo/ws-sync-react) that implements the frontend side of the protocol.
 
 ## Quickstart
@@ -41,89 +41,91 @@
     def add(self, note):
         self.notes.append(note)
 ```
 
 To sync it to the frontend, it is as simple as:
 
 ```diff
-+from ws_sync import Sync
++from ws_sync import sync_all
 
 class Notes:
++   @sync_all("NOTES")  # create the sync object and define the key
     def __init__(self):
         # my attributes, as usual
         self.title = "My Notes"
         self.notes = []
 
-+       # create the sync object and define the key of the object
-+       self.sync = Sync("NOTES", self)
-    
     @property
     def total_length(self):
         return sum(len(note) for note in self.notes)
     
 +   async def rename(self, new_title):
         self.title = new_title
-+       await self.sync() # make sure the frontend knows about the change
++       await self.sync()  # make sure the frontend knows about the change
     
 +   async def add(self, note):
         self.notes.append(note)
-+       await self.sync() # make sure the frontend knows about the change
++       await self.sync()  # make sure the frontend knows about the change
 ```
 
 The `Sync("Notes", self)` call automatically detects the attributes to sync in `self`, which are all attributes or `@properties` that do not start with an underscore. You can also specify the attributes to sync manually:
 
 ```python
-self.sync = Sync("NOTES", self,
+@sync_only("NOTES",
     title = ...,
     notes = ...,
-    total_length = "totalLength",
+    total_length = "size",
 )
 ```
 
 The keyword argument is the local name of the attribute, the value is the name of the attribute in the frontend. If the value is `...`, the local and frontend name are the same. This is useful if you want to rename an attribute in the frontend without changing the name in the backend (e.g. snake_case to camelCase).
 
+For more info on the options and examples, see [ws_sync.decorators docs](https://joongwonseo.github.io/ws-sync/ws_sync/decorators.html).
+
 #### Frontend
-On the frontend, you can use the `useSync` hook to sync the state to the backend:
+On the frontend, you can use the `useSynced` hook to sync the state to the backend:
 
 ```jsx
 const Notes = () => {
-    const notes = useSync("NOTES", {
+    const notes = useSynced("NOTES", {
         title: "",
         notes: [],
     })
 
     return (
         <div>
             <h1>{notes.title}</h1>
             <ul>{notes.notes.map(note => <li>{note}</li>)}</ul>
         </div>
     )
 }
 ```
 
-The second parameter of `useSync` is the initial state.
+The second parameter of `useSynced` is the initial state.
 
 The returned `notes` object not only contains the state, but also the setters and syncers:
 
 ```jsx
 const Notes = () => {
-    const notes = useSync("NOTES", {
+    const notes = useSynced("NOTES", {
         title: "",
         notes: [],
     })
 
     return (
         <div>
             <input value={notes.title} onChange={e => notes.syncTitle(e.target.value)} />
             <ul>{notes.notes.map(note => <li>{note}</li>)}</ul>
         </div>
     )
 }
 ```
 
+For more info on the react library, see [ws-sync-react](https://github.com/JoongWonSeo/ws-sync-react).
+
 ### Actions
 Actions are a way to call methods on the remote (action handlers), usually frontend -> backend.
 
 `TODO`
 
 ### Tasks
 Tasks are like actions, but for long-running operations and can be cancelled.
```

