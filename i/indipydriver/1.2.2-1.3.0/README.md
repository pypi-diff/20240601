# Comparing `tmp/indipydriver-1.2.2.tar.gz` & `tmp/indipydriver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.2.2.tar` & `indipydriver-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.2/LICENSE
--rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.2/README.md
--rw-r--r--   0        0        0      658 2024-05-20 09:54:27.000000 indipydriver-1.2.2/indipydriver/__init__.py
--rw-r--r--   0        0        0    18853 2024-05-19 21:11:41.000000 indipydriver-1.2.2/indipydriver/comms.py
--rw-r--r--   0        0        0    24981 2024-05-16 20:54:58.000000 indipydriver-1.2.2/indipydriver/events.py
--rw-r--r--   0        0        0    22537 2024-05-19 21:52:18.000000 indipydriver-1.2.2/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    11485 2024-05-19 21:17:11.000000 indipydriver-1.2.2/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12256 2024-05-16 20:34:45.000000 indipydriver-1.2.2/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43660 2024-05-19 21:32:10.000000 indipydriver-1.2.2/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-05-20 09:54:15.000000 indipydriver-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2542 2024-06-01 10:45:39.000000 indipydriver-1.3.0/README.md
+-rw-r--r--   0        0        0      573 2024-05-31 21:04:28.000000 indipydriver-1.3.0/indipydriver/__init__.py
+-rw-r--r--   0        0        0    21467 2024-05-30 12:50:41.000000 indipydriver-1.3.0/indipydriver/comms.py
+-rw-r--r--   0        0        0    24981 2024-05-16 20:54:58.000000 indipydriver-1.3.0/indipydriver/events.py
+-rw-r--r--   0        0        0    22591 2024-05-31 21:07:24.000000 indipydriver-1.3.0/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    20110 2024-05-30 16:24:26.000000 indipydriver-1.3.0/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12256 2024-05-16 20:34:45.000000 indipydriver-1.3.0/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43620 2024-05-31 21:15:51.000000 indipydriver-1.3.0/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0     5007 2024-05-31 21:01:28.000000 indipydriver-1.3.0/indipydriver/remote.py
+-rw-r--r--   0        0        0      853 2024-06-01 09:52:07.000000 indipydriver-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 indipydriver-1.3.0/PKG-INFO
```

### Comparing `indipydriver-1.2.2/LICENSE` & `indipydriver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.2/README.md` & `indipydriver-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # indipydriver
 
-This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
+This is a pure python package, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
+
+It has one dependency, indipyclient, which itself is pure python and has no further dependencies.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
 Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
@@ -18,15 +20,15 @@
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
 
 The driver has methods which should be overwritten.
 
-async def clientevent(self, event)
+async def rxevent(self, event)
 
 This is called whenever data is received from the client, typically to set an instrument parameter. The event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
```

### Comparing `indipydriver-1.2.2/indipydriver/__init__.py` & `indipydriver-1.3.0/indipydriver/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 
 
-
-import logging
-logging.getLogger('indipydriver').addHandler(logging.NullHandler())
-
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.2.2"
+version = "1.3.0"
```

### Comparing `indipydriver-1.2.2/indipydriver/comms.py` & `indipydriver-1.3.0/indipydriver/comms.py`

 * *Files 11% similar despite different names*

```diff
@@ -213,31 +213,29 @@
         await asyncio.gather(rx.run_rx(readerque),
                              tx.run_tx(writerque)
                              )
 
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
-    def __init__(self, blobstatus, writer, timer):
-        self.blobstatus = blobstatus
+    def __init__(self, sendchecker, writer, timer):
+        self.sendchecker = sendchecker
         self.writer = writer
         self.timer = timer
 
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on the port writer"""
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit
             txdata = await writerque.get()
             writerque.task_done()
-            if len(txdata) and not self.blobstatus.allowed(txdata):
+            if not self.sendchecker.allowed(txdata):
                 # this data should not be transmitted, discard it
-                # however if the vector has no content, but perhaps just message and state
-                # still allow it
                 continue
             # this data can be transmitted
             if txdata.tag == "setBLOBVector" and len(txdata):
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # Send to the port
@@ -254,30 +252,35 @@
 
 
 class Port_RX(STDIN_RX):
     """Produces xml.etree.ElementTree data from data received on the port,
        this is used by Portcomms as one half of the communications path.
        This overwrites methods of the STDIN_RX parent class."""
 
-    def __init__(self, blobstatus, reader):
-        self.blobstatus = blobstatus
+    def __init__(self, sendchecker, reader, timer):
+        self.sendchecker = sendchecker
         self.reader = reader
+        # update timer every time something received
+        # in the last 15 seconds
+        # this can be read to see if it has elapsed
+        self.timer = timer
 
 
     async def run_rx(self, readerque):
         "pass data to readerque"
         source = self.datasource()
         async for rxdata in source:
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
             if rxdata.tag == "enableBLOB":
-                # set permission flags in the blobstatus object
-                self.blobstatus.setpermissions(rxdata)
+                # set permission flags in the sendchecker object
+                self.sendchecker.setpermissions(rxdata)
             # and place rxdata into readerque
             await readerque.put(rxdata)
+            self.timer.update()
 
 
 
     async def datainput(self):
         "Generator producing binary string of data from the port"
         binarydata = b""
         while True:
@@ -323,23 +326,24 @@
 class Portcomms():
     """If indipydriver.comms is set to an instance of this class it is
        used to implement communications via a port"""
 
     def __init__(self, devices, host="localhost", port=7624):
         # devices is a dictionary of device name to device this driver owns
         self.devices = devices
-        self.blobstatus = BLOBSstatus(devices)
+        self.sendchecker = SendChecker(devices)
         self.host = host
         self.port = port
         self.connected = False
 
         # timer used to force a data transmission after timeout seconds
         # this will cause an exception if the connection is broken and will shut down
         # the connection
-        self.timer = TXTimer(timeout = 15)
+        self.txtimer = TXTimer()
+        self.rxtimer = TXTimer()
 
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         self.readerque = readerque
         self.writerque = writerque
         logger.info(f"Listening on {self.host} : {self.port}")
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
@@ -349,36 +353,36 @@
     async def _monitor_connection(self):
         """If connected and not transmitting, send def vectors every self.timeout seconds
            This ensures that if the connection has failed, due to the client disconnecting, the write
            to the port operation will cause a failure exception which will close the connection"""
         while True:
             await asyncio.sleep(5)
             # this is tested every five seconds
-            if self.connected and self.writerque.empty() and self.readerque.empty():
-                # only need to test if the queue are empty
-                if self.timer.elapsed():
-                    # no transmission in timeout seconds so send defVectors
-                    for device in self.devices.values():
-                        if not device.enable:
+            if self.connected and self.txtimer.elapsed() and self.rxtimer.elapsed():
+                # Nothing recently transmitted or received so send defVectors
+                for device in self.devices.values():
+                    if not device.enable:
+                        continue
+                    for vector in device.values():
+                        if not vector.enable:
                             continue
-                        for vector in device.values():
-                            await vector.send_defVector()
+                        await vector.send_defVector()
 
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         if self.connected:
             # already connected, can only handle one connection
             writer.close()
             await writer.wait_closed()
             return
         self.connected = True
         addr = writer.get_extra_info('peername')
-        rx = Port_RX(self.blobstatus, reader)
-        tx = Port_TX(self.blobstatus, writer, self.timer)
+        rx = Port_RX(self.sendchecker, reader, self.rxtimer)
+        tx = Port_TX(self.sendchecker, writer, self.txtimer)
         logger.info(f"Connection received from {addr}")
         try:
             txtask = asyncio.create_task(tx.run_tx(self.writerque))
             rxtask = asyncio.create_task(rx.run_rx(self.readerque))
             montask = asyncio.create_task(self._monitor_connection())
             await asyncio.gather(txtask, rxtask, montask)
         except Exception as e:
@@ -397,43 +401,73 @@
             xmldata = que.get_nowait()
             que.task_done()
     except asyncio.QueueEmpty:
         # que is now empty, nothing further to do
         pass
 
 
-class BLOBSstatus:
-    "Carries the enableBLOB status on a device or property"
+class SendChecker:
+    """Carries the enableBLOB status on a device or property, and does checks
+       to ensure valid data is being transmitted"""
 
-    def __init__(self, devices):
+    def __init__(self, devices, remotes=None):
         "For every device, propertyvector create a status list of (Other allowed, BLOB allowed)"
+        self.remotes = remotes
+        self.devices = devices
         self.devicestatus = {}
         # create a dictionary of devicenames : list of propertynames for that device
         self.deviceproperties = {}
         for devicename, device in devices.items():
             self.deviceproperties[devicename] = []
             for propertyvector in device.values():
                 # Initially set with BLOBs not allowed
                 self.devicestatus[(devicename, propertyvector.name)] = (True, False)
                 self.deviceproperties[devicename].append(propertyvector.name)
 
 
     def allowed(self, xmldata):
         "Return True if this xmldata can be transmitted, False otherwise"
+        if xmldata.tag.startswith("new"):
+            # new tags are sent from client to server, not from server back to client
+            return False
+        # allow anything with zero contents, such as getProperties
+        if not len(xmldata):
+            return True
         devicename = xmldata.get("device")
         if devicename is None:
-            # either a getproperties or message, only deny it if ALL Other allowed are False
+            # deny it if ALL Other allowed are False
             # so this connection is dedictated to BLOBs only
             for status in self.devicestatus.values():
                 if status[0]:
                     return True
             return False
         if not (devicename in self.deviceproperties):
+            # devicename not recognised, check if it is in remotes
+            if not self.remotes:
+                return False
+            for remcon in self.remotes:
+                for devicename, device in remcon.items():
+                    if devicename in self.devices:
+                        # A duplicate address, this should never occur
+                        logger.error(f"Duplicate device name {devicename}")
+                        return False
+                    if devicename in self.deviceproperties:
+                        continue
+                    # so this devicename not recorded, add it
+                    self.deviceproperties[devicename] = []
+                    for propertyvector in device.values():
+                        # Initially set with BLOBs not allowed
+                        self.devicestatus[(devicename, propertyvector.name)] = (True, False)
+                        self.deviceproperties[devicename].append(propertyvector.name)
+
+        # self.deviceproperties should now include all known device names
+        if not (devicename in self.deviceproperties):
             # devicename not recognised
             return False
+
         # so we have a devicename, get propertyname
         name = xmldata.get("name")
         # if name missing, could be a message, cannot be a setBLOBVector
         if name is None:
             # only deny it if ALL other allowed are False for this device
             properties = self.deviceproperties[devicename]
             for name in properties:
@@ -460,15 +494,34 @@
         # commands by setting Also or made the only command by setting Only.
 
         devicename = rxdata.get("device")
         if devicename is None:
             # invalid
             return
         if not (devicename in self.deviceproperties):
-            # devicename not recognised
+            # devicename not recognised, check if it is in remotes
+            if not self.remotes:
+                return
+            for remcon in self.remotes:
+                for devicename, device in remcon.items():
+                    if devicename in self.devices:
+                        # A duplicate address, this should never occur
+                        logger.error(f"Duplicate device name {devicename}")
+                        return
+                    if devicename in self.deviceproperties:
+                        continue
+                    # so this devicename not recorded, add it
+                    self.deviceproperties[devicename] = []
+                    for propertyvector in device.values():
+                        # Initially set with BLOBs not allowed
+                        self.devicestatus[(devicename, propertyvector.name)] = (True, False)
+                        self.deviceproperties[devicename].append(propertyvector.name)
+
+        if not (devicename in self.deviceproperties):
+            # devicename not recognised, cannot set any permissions
             return
         value = rxdata.text.strip()
         if value == "Never":
             perm = (True, False)    # (Other allowed, BLOB not allowed)
         elif value == "Also":
             perm = (True, True)     # (Other allowed, BLOB allowed)
         elif value == "Only":
```

### Comparing `indipydriver-1.2.2/indipydriver/events.py` & `indipydriver-1.3.0/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.2/indipydriver/ipydriver.py` & `indipydriver-1.3.0/indipydriver/ipydriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
        tasks is a list of co-routines that you may have created to
        operate your instruments, the co-routines set in this list
        will all be started when the driver is run.
        The tasks argument was introduced in version 1.1.0.
 
        driverdata will be an attribute dictionary of any hardware
        data that may be usefull.
+
+       This object is also a mapping, of devicename:deviceobject
        """
 
     @staticmethod
     def indi_number_to_float(value):
         """The INDI spec allows a number of different number formats, given any number string, this returns a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
         try:
@@ -314,15 +316,15 @@
         For example: call your own code to operate hardware
         then update the appropriate vectors, and send updated
         values to the client using
         await vector.send_setVector()"""
         pass
 
 
-    async def clientevent(self, event):
+    async def rxevent(self, event):
         """Override this. On receiving data, this is called, and should
            handle any necessary actions.
            event is an object describing the event, with attributes
            devicename, vectorname, vector, root
            where vector is the properties vector the event refers to, and
            root is an xml.etree.ElementTree object of the received xml"""
         match event:
@@ -447,19 +449,19 @@
         """As default, does nothing and is not called.
 
            If required, override this to handle any necessary device actions.
            This should be called from the driver 'hardware' method if it is used."""
         pass
 
 
-    async def devclientevent(self, event, *args, **kwargs):
+    async def devrxevent(self, event, *args, **kwargs):
         """As default, does nothing and is not called.
 
            If required, override this to handle any necessary device actions.
-           This should be called from the driver 'clientevent' method if it is used."""
+           This should be called from the driver 'rxevent' method if it is used."""
         pass
 
 
     async def devsnoopevent(self, event, *args, **kwargs):
         """As default, does nothing and is not called.
 
            If required, override this to handle any necessary device actions.
```

### Comparing `indipydriver-1.2.2/indipydriver/propertymembers.py` & `indipydriver-1.3.0/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.2/indipydriver/propertyvectors.py` & `indipydriver-1.3.0/indipydriver/propertyvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,19 +197,19 @@
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
                 elif root.tag == "newSwitchVector":
                     # create event
                     event = newSwitchVector(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
                 logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
 
     def _make_defVector(self, message='', timestamp=None):
@@ -389,15 +389,15 @@
             await asyncio.sleep(0)
             # test if any xml data has been received
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
                 logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     @property
     def perm(self):
@@ -550,19 +550,19 @@
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
                 elif root.tag == "newTextVector":
                     # create event
                     event = newTextVector(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
                 logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
@@ -728,19 +728,19 @@
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
                 elif root.tag == "newNumberVector":
                     # create event
                     event = newNumberVector(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
                 logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
@@ -921,23 +921,23 @@
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
                 elif root.tag == "enableBLOB":
                     # create event
                     event = enableBLOB(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
                 elif root.tag == "newBLOBVector":
                     # create event
                     event = newBLOBVector(self.devicename, self.name, self, root)
-                    await self.driver.clientevent(event)
+                    await self.driver.rxevent(event)
             except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
                 logger.exception("Unable to create event from received data")
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
```

### Comparing `indipydriver-1.2.2/pyproject.toml` & `indipydriver-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.2.2"
+version = "1.3.0"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
+dependencies = ["indipyclient>=0.2.0"]
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
 Source = "https://github.com/bernie-skipole/indipydriver"
```

### Comparing `indipydriver-1.2.2/PKG-INFO` & `indipydriver-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.2.2
+Version: 1.3.0
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
+Requires-Dist: indipyclient>=0.2.0
 Project-URL: Documentation, https://indipydriver.readthedocs.io
 Project-URL: Source, https://github.com/bernie-skipole/indipydriver
 
 # indipydriver
 
-This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
+This is a pure python package, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
+
+It has one dependency, indipyclient, which itself is pure python and has no further dependencies.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
 Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
@@ -33,15 +36,15 @@
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
 
 The driver has methods which should be overwritten.
 
-async def clientevent(self, event)
+async def rxevent(self, event)
 
 This is called whenever data is received from the client, typically to set an instrument parameter. The event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
```

