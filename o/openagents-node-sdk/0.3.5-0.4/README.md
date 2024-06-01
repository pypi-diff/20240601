# Comparing `tmp/openagents_node_sdk-0.3.5.tar.gz` & `tmp/openagents_node_sdk-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.3.5.tar", last modified: Sat May 18 08:29:13 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.4.tar", last modified: Sat Jun  1 12:37:06 2024, max compression
```

## Comparing `openagents_node_sdk-0.3.5.tar` & `openagents_node_sdk-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/JobContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:37:06.757305 openagents_node_sdk-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-01 12:37:06.757305 openagents_node_sdk-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:37:06.757305 openagents_node_sdk-0.4/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/JobContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:37:06.757305 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-01 12:37:06.000000 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 12:37:06.000000 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 12:37:06.000000 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 12:37:06.000000 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 12:37:06.000000 openagents_node_sdk-0.4/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 12:37:06.757305 openagents_node_sdk-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 12:37:04.000000 openagents_node_sdk-0.4/setup.py
```

### Comparing `openagents_node_sdk-0.3.5/LICENSE` & `openagents_node_sdk-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/README.md` & `openagents_node_sdk-0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # OpenAgents Node - Python SDK
 
 
 A Python SDK for developing OpenAgents nodes.
 
+## Requirements
+- Python 3.11 or higher
+
 ## Installation
 
 ```bash
 pip install openagents-node-sdk
 ```
 
 ## Usage Example
@@ -14,70 +17,78 @@
 ```python
 from openagents import JobRunner,OpenAgentsNode,NodeConfig,RunnerConfig
 
 # Define a runner
 class MyRunner (JobRunner):
     def __init__(self):
         # Set the runner metadata, template and filter
-        super().__init__(\
+        super().__init__(
             RunnerConfig(
                 meta={
                     "kind":5003,
                     "name":"My Action",
                     "description":"This is a new action",
                     "tos": "https://example.com/tos",
                     "privacy": "https://example.com/privacy",
                     "picture": "https://example.com/icon.png",
                     "tags": ["tag1","tag2"],
                     "website": "https://example.com",
                     "author": "John Doe"
                 },
+                # Filters are regular expressions that are used to define which jobs this runner can run
                 filter={
-                    "filterByKind":5003,
+                    "filterByKind": "5003",
                     #AND
                     "filterByRunOn": "my-new-action"
                 },
-                template="""
+                # Mustache template (https://mustache.github.io/)
+                template=""" 
                 {
                     "kind": {{meta.kind}},
                     "created_at": {{sys.timestamp_seconds}},
                     "tags": [
                         ["param","run-on", "my-new-action" ],                             
                         ["param", "k", "{{in.k}}"],
-                        ["output" , "{{out.content}}"]
+                        ["output" , "{{in.outputType}}"],
                         {{#in.queries}}
                         ["i", "{{value}}", "{{type}}", "",  "query"],
                         {{/in.queries}}                       
                         ["expiration", "{{sys.expiration_timestamp_seconds}}"],
                     ],
                     "content":""
                 }""",
+                 # In JSON Schema format (https://json-schema.org/)
                 sockets={
                     "in": {
                         "k": {
-                            "title": "K",
-                            "description":"This is a number"
+                            "title": "MyNumber",
+                            "description":"This is a number",
                             "type":"integer",
                             "default": 0,
                         },
                         "queries": {
-                            "title": "Queries",
+                            "title": "MyArray",
                             "type":"array",
-                            "description":"This is an array of queries",
+                            "description":"This is an array of strings",
                             "items": {
                                 "type":"string"
                             }
+                        },
+                        "outputType": {
+                            "title": "Output Type",
+                            "type": "string",
+                            "description": "The output type of the event",
+                            "default": "application/json"
                         }
                     },
                     "out": {
-                        "contentType": {
-                            "title": "Content Type",
+                        "output": {
+                            "title": "Output",
                             "type": "string",
-                            "description": "The content of the event",
-                            "default": "application/json"
+                            "description": "The output content"
                         }
                     }
                 }
             )
         )
 
     async def init(self, node):
@@ -109,17 +120,30 @@
 
 
 
 # Initialize the node
 myNode = OpenAgentsNode(NodeConfig(
     meta={
         "name":"My Node",
-        "description":"This is a new node"
+        "description":"This is a new node",
         "version": "1.0"
     }
 ))
+
 # Register the runner (you can register multiple runners)
 myNode.registerRunner(MyRunner())
 # Start the node
 myNode.start()
+```
+For more information check the [OpenAgents Python SDK Documentation](https://docs.openagents.com/python-sdk)
+
+----
+*Note: By default the node will connect to OpenAgents open pool *(playground.openagents.com 6021 ssl)*, this can be changed by setting the following environment variables:*
 
+```bash
+POOL_ADDRESS="playground.openagents.com" # custom pool address
+POOL_PORT="6021" #  custom pool port
+POOL_SSL="true" # or "false"
 ```
+*To learn how to host your own pool check the [Running a Pool](https://docs.openagents.com/running-a-pool) documentation.*
+
+
```

### Comparing `openagents_node_sdk-0.3.5/openagents/Disk.py` & `openagents_node_sdk-0.4/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/DiskReader.py` & `openagents_node_sdk-0.4/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/DiskWriter.py` & `openagents_node_sdk-0.4/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/JobContext.py` & `openagents_node_sdk-0.4/openagents/JobContext.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/JobRunner.py` & `openagents_node_sdk-0.4/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/Logger.py` & `openagents_node_sdk-0.4/openagents/Logger.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/NodeConfig.py` & `openagents_node_sdk-0.4/openagents/NodeConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.4/openagents/OpenAgentsNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     - NODE_VERSION: The version of the node. Defaults to "0.0.1".
     - NODE_DESCRIPTION: The description of the node. Defaults to "".
     - POOL_ADDRESS: The address of the pool. Defaults to "
     - POOL_PORT: The port of the pool. Defaults to 5000.
     - POOL_SSL: Whether to use SSL for the pool. Defaults to False.
     - NODE_TPS: The ticks per second of the node main loop. Defaults to 10.
     - NODE_TOKEN: The token of the node. Defaults to None.
+    - NWC: Nostr wallet connect URL
     """
   
     def __init__(self, config: NodeConfig):
         self.meta = config.getMeta()
             
         self.nextNodeAnnounce = 0        
         self.channel = None
@@ -126,25 +127,32 @@
                 # 20 MB
                 ('grpc.max_send_message_length', 1024*1024*20),
                 ('grpc.max_receive_message_length', 1024*1024*20)
             ]
 
             interceptors=None
             nodeToken = os.getenv('NODE_TOKEN', None)
-            if nodeToken:
-                metadata=[
-                    ("authorization", str(nodeToken))
-                ]
+            nwc = os.getenv('NWC', None)
+            if nodeToken or nwc:
+                metadata=[]
+                if nwc:
+                    metadata.append(("nwc", str(nwc)))                
+                if nodeToken:
+                    metadata.append(("authorization", str(nodeToken)))                    
                 if interceptors is None: interceptors=[]
                 interceptors.append(HeaderAdderInterceptor0(metadata))
                 interceptors.append(HeaderAdderInterceptor1(metadata))
                 interceptors.append(HeaderAdderInterceptor2(metadata))
                 interceptors.append(HeaderAdderInterceptor3(metadata))
                 
-
+            if nwc:
+                self.getLogger().info("This node can receive payments")
+            else: 
+                self.getLogger().warn("This node is not enabled to receive payments. Please provide a NWC URL")
+                
             if self.poolSsl:
                 self.channel = grpc.aio.secure_channel(self.poolAddress+":"+str(self.poolPort), grpc.ssl_channel_credentials(),options,interceptors=interceptors)
             else:
                 self.channel = grpc.aio.insecure_channel(self.poolAddress+":"+str(self.poolPort),options,interceptors=interceptors)
             
             self.rpcClient = rpc_pb2_grpc.PoolConnectorStub(self.channel)
             
@@ -194,21 +202,25 @@
         try:
             if not runner.initialized:
                 runner.initialized=True
                 await runner.init(self)
             client = self._getClient()
             jobs=[]
             filter = runner.getFilter()
+            meta = runner.getMeta()
+            prices = "prices" in meta and meta["prices"] or None
+
             self.lockedJobs = [x for x in self.lockedJobs if time.time()-x[1] < 60]
             jobs.extend((await client.getPendingJobs(rpc_pb2.RpcGetPendingJobs(
                 filterByRunOn =  filter["filterByRunOn"] if "filterByRunOn" in filter else None,
                 filterByCustomer = filter["filterByCustomer"] if "filterByCustomer" in filter else None,
                 filterByDescription = filter["filterByDescription"] if "filterByDescription" in filter else None,
                 filterById = filter["filterById"] if "filterById" in filter else None,
                 filterByKind  = filter["filterByKind"] if "filterByKind" in filter else None,
+                filterByBids = prices,
                 wait=60000,
                 # exclude failed jobs
                 excludeId = [x[0] for x in self.lockedJobs]
             ))).jobs)    
 
             if len(jobs)>0 : self.getLogger().log(str(len(jobs))+" pending jobs for "+runner.__class__.__name__)
             else : self.getLogger().finer("No pending jobs for "+runner.__class__.__name__)
@@ -308,15 +320,15 @@
                         reg["nextAnnouncementTimestamp"] = int(time.time()*1000) + res.refreshInterval
                         self.getLogger().log("Template announced, next announcement in "+str(res.refreshInterval)+" ms")
                 except Exception as e:
                     self.getLogger().error("Error announcing template "+ str(e), None)
                     reg["nextAnnouncementTimestamp"] = int(time.time()*1000) + 5000
         except Exception as e:
             self.getLogger().error("Error reannouncing "+str(e), None)
-        await asyncio.sleep(5000.0/1000.0)
+        await asyncio.sleep(5)
         asyncio.create_task(self.reannounce())
   
     async def _loop(self):
         """
         The main loop of the node.
         """
         promises = [reg["runner"].loop(self) for reg in self.registeredRunners]
```

### Comparing `openagents_node_sdk-0.3.5/openagents/RunnerConfig.py` & `openagents_node_sdk-0.4/openagents/RunnerConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.5/setup.py` & `openagents_node_sdk-0.4/setup.py`

 * *Files identical despite different names*

