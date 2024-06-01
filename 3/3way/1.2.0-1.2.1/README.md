# Comparing `tmp/3way-1.2.0.tar.gz` & `tmp/3way-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3way-1.2.0.tar", last modified: Mon May 27 11:40:05 2024, max compression
+gzip compressed data, was "3way-1.2.1.tar", last modified: Mon May 27 12:05:37 2024, max compression
```

## Comparing `3way-1.2.0.tar` & `3way-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.118833 3way-1.2.0/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.010834 3way-1.2.0/.github/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.034834 3way-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 kali      (1000) kali      (1000)      368 2024-05-27 00:00:00.000000 3way-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 kali      (1000) kali      (1000)      324 2024-05-27 00:00:00.000000 3way-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.046834 3way-1.2.0/3way.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     7073 2024-05-27 11:40:03.000000 3way-1.2.0/3way.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      836 2024-05-27 11:40:04.000000 3way-1.2.0/3way.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-27 11:40:03.000000 3way-1.2.0/3way.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-27 11:40:03.000000 3way-1.2.0/3way.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-27 11:40:03.000000 3way-1.2.0/3way.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    21165 2024-05-27 10:57:51.000000 3way-1.2.0/Freeway
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.078834 3way-1.2.0/FreewayTools/
--rw-r--r--   0 kali      (1000) kali      (1000)      570 2024-05-27 10:34:51.000000 3way-1.2.0/FreewayTools/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    20007 2024-05-27 11:00:13.000000 3way-1.2.0/FreewayTools/audit.py
--rw-r--r--   0 kali      (1000) kali      (1000)    13348 2024-05-27 10:59:24.000000 3way-1.2.0/FreewayTools/beacon_spam.py
--rw-r--r--   0 kali      (1000) kali      (1000)      739 2024-05-20 13:21:18.000000 3way-1.2.0/FreewayTools/checkmac.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1634 2024-05-24 20:28:12.000000 3way-1.2.0/FreewayTools/colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19102 2024-05-20 13:21:18.000000 3way-1.2.0/FreewayTools/deauth.py
--rw-r--r--   0 kali      (1000) kali      (1000)    20583 2024-05-27 11:12:12.000000 3way-1.2.0/FreewayTools/evil_twin.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11726 2024-05-20 16:16:19.000000 3way-1.2.0/FreewayTools/fuzzer.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2056 2024-05-20 13:21:18.000000 3way-1.2.0/FreewayTools/hopper.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.082834 3way-1.2.0/FreewayTools/lists/
--rw-r--r--   0 kali      (1000) kali      (1000)    10865 2024-05-20 13:21:18.000000 3way-1.2.0/FreewayTools/lists/ssid_list.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    27655 2024-05-20 13:21:18.000000 3way-1.2.0/FreewayTools/monitor.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1384 2024-05-27 11:02:28.000000 3way-1.2.0/FreewayTools/updater.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1063 2024-05-27 11:22:15.000000 3way-1.2.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     7073 2024-05-27 11:40:05.114833 3way-1.2.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     6847 2024-05-27 11:21:42.000000 3way-1.2.0/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-05-20 13:21:18.000000 3way-1.2.0/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-27 11:40:05.118833 3way-1.2.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1779 2024-05-27 11:39:14.000000 3way-1.2.0/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.018834 3way-1.2.0/templates/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.090834 3way-1.2.0/templates/Valentines/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 21:25:53.000000 3way-1.2.0/templates/Valentines/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3585 2024-05-24 21:26:16.000000 3way-1.2.0/templates/Valentines/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.094833 3way-1.2.0/templates/google/
--rw-r--r--   0 kali      (1000) kali      (1000)       68 2024-05-23 21:57:13.000000 3way-1.2.0/templates/google/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)    13219 2024-05-25 14:16:01.000000 3way-1.2.0/templates/google/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.102833 3way-1.2.0/templates/mcd/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 16:00:34.000000 3way-1.2.0/templates/mcd/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3813 2024-05-25 14:16:01.000000 3way-1.2.0/templates/mcd/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.106833 3way-1.2.0/templates/mrhacker/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 20:43:05.000000 3way-1.2.0/templates/mrhacker/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     6536 2024-05-25 14:16:01.000000 3way-1.2.0/templates/mrhacker/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 11:40:05.110833 3way-1.2.0/templates/mrhacker/static/
--rw-r--r--   0 kali      (1000) kali      (1000)    31471 2024-05-24 21:06:33.000000 3way-1.2.0/templates/mrhacker/static/mrhacker.png
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.737558 3way-1.2.1/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.581558 3way-1.2.1/.github/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.637558 3way-1.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 kali      (1000) kali      (1000)      368 2024-05-27 00:00:00.000000 3way-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      324 2024-05-27 00:00:00.000000 3way-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.653558 3way-1.2.1/3way.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7618 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      836 2024-05-27 12:05:37.000000 3way-1.2.1/3way.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    21165 2024-05-27 10:57:51.000000 3way-1.2.1/Freeway
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.693558 3way-1.2.1/FreewayTools/
+-rw-r--r--   0 kali      (1000) kali      (1000)      570 2024-05-27 10:34:51.000000 3way-1.2.1/FreewayTools/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    20007 2024-05-27 11:00:13.000000 3way-1.2.1/FreewayTools/audit.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    13348 2024-05-27 10:59:24.000000 3way-1.2.1/FreewayTools/beacon_spam.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      739 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/checkmac.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1634 2024-05-24 20:28:12.000000 3way-1.2.1/FreewayTools/colors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19102 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/deauth.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    20583 2024-05-27 11:12:12.000000 3way-1.2.1/FreewayTools/evil_twin.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11726 2024-05-20 16:16:19.000000 3way-1.2.1/FreewayTools/fuzzer.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2056 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/hopper.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.697558 3way-1.2.1/FreewayTools/lists/
+-rw-r--r--   0 kali      (1000) kali      (1000)    10865 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/lists/ssid_list.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    27655 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/monitor.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1384 2024-05-27 12:04:49.000000 3way-1.2.1/FreewayTools/updater.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1063 2024-05-27 11:22:15.000000 3way-1.2.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     7618 2024-05-27 12:05:37.737558 3way-1.2.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     7392 2024-05-27 12:02:23.000000 3way-1.2.1/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-05-20 13:21:18.000000 3way-1.2.1/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-27 12:05:37.737558 3way-1.2.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1779 2024-05-27 12:04:41.000000 3way-1.2.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.613558 3way-1.2.1/templates/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.705558 3way-1.2.1/templates/Valentines/
+-rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 21:25:53.000000 3way-1.2.1/templates/Valentines/action.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     3585 2024-05-24 21:26:16.000000 3way-1.2.1/templates/Valentines/index.html
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.713558 3way-1.2.1/templates/google/
+-rw-r--r--   0 kali      (1000) kali      (1000)       68 2024-05-23 21:57:13.000000 3way-1.2.1/templates/google/action.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    13219 2024-05-25 14:16:01.000000 3way-1.2.1/templates/google/index.html
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.717558 3way-1.2.1/templates/mcd/
+-rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 16:00:34.000000 3way-1.2.1/templates/mcd/action.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     3813 2024-05-25 14:16:01.000000 3way-1.2.1/templates/mcd/index.html
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.725558 3way-1.2.1/templates/mrhacker/
+-rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 20:43:05.000000 3way-1.2.1/templates/mrhacker/action.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     6536 2024-05-25 14:16:01.000000 3way-1.2.1/templates/mrhacker/index.html
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.729558 3way-1.2.1/templates/mrhacker/static/
+-rw-r--r--   0 kali      (1000) kali      (1000)    31471 2024-05-24 21:06:33.000000 3way-1.2.1/templates/mrhacker/static/mrhacker.png
```

### Comparing `3way-1.2.0/3way.egg-info/PKG-INFO` & `3way-1.2.1/3way.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3way
-Version: 1.2.0
+Version: 1.2.1
 Summary: Freeway for network pentesting
 Home-page: https://github.com/FLOCK4H/Freeway
 Author: FLOCK4H
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -33,43 +33,52 @@
 
 - IEEE 802.11 Packet Monitoring
 - Deauthentication Attack
 - Beacon Flood
 - Packet Fuzzer
 - Network Audit
 - Channel Hopper
+- Evil Twin
 
 <sub>Description of the features can be found in Section 6</sub>
 
 <h2><strong>3. Preparation</strong></h2>
 
 It is **necessary** to have:
 - A network adapter supporting monitor mode and frame injection.
 - An operating system running a Linux distribution.
 - Python 3+ installed.
 
 <sub>Optionally, install Scapy and Rich packages for Python if not installing via pip (see Section 4)</sub>
 
 <h2><strong>4. Setup</strong></h2>
 
+A: Install via PyPi (pip)
+
+```
+  $ sudo pip install 3way
+```
+
+B: Install or run manually
+
 First, clone the repository:
 
     git clone https://github.com/FLOCK4H/Freeway
 
 Navigate to the cloned repository:
 
     cd Freeway
 
-<strong>A:</strong> Install dependencies and Freeway.
+<strong>Option 1:</strong> Install dependencies and Freeway.
 
 <sub>This will allow to launch the tool from anywhere</sub>
 
     sudo pip install .
 
-<strong>B:</strong> Run without installation using Python.
+<strong>Option 2:</strong> Run without installation using Python.
 
 <sub>Must be called from the /Freeway directory</sub>
 
     sudo pip install scapy rich
     sudo python Freeway
 
 <h2><strong>5. Usage</strong></h2>
@@ -118,15 +127,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for every action.
   To list all parameters for a given action, just provide -a argument without -p.
 </pre>
 </div>
 </details>
 
@@ -134,14 +144,15 @@
 
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and return the result onto the python's curses display. Catches SSIDs, MACs, Clients, Uptime, Channel, Signal (dBm), Encryption and resolves manufacturer. Catches PMKIDs in hashcat crackable format, and 4-way Handshakes, as well as other EAPOL packets. Logs the captured session to the **/caps** folder or every captured packet if _Save output_ was selected.
 - **Deauthentication Attack (Deauthing)** - Disconnects a device from the network by sending a packet containing AP<sup>1</sup> address, device address (or broadcast for _Mass Deauthing_) and the deauthentication frame with a reason of kicking the client(s). In case where a device address is a broadcast address, the AP will in most cases disconnect all clients at once. Freeway creates separate thread for every AP or client found in order to make deauthing maximally efficient.
 - **Beacon Flood Attack** - Floods the nearby WiFi scanners with fake or malformed APs. It can cause the devices looking for WiFi to behave abnormally (e.g. crash, freeze, drain the battery or run slower) and disrupt the nearby network traffic. User is able to specify his own ssid list, use the default one and generate correct (but random) or malformed beacon packets.
 - **Packet Fuzzer** - Fuzzing is a technique of network vulnerability assesment by sending a wide array of malformed or semi-random data to network interfaces and observing the responses. Freeway covers: **Replay captured packets (RX&TX<sup>2</sup>)**, **Spam CTS/RTS or Probe requests** and **Flood an AP with Authentication or Association Frames**. Devices that will capture fuzzed packets will behave differently depending on vulnerability level of receiver (!USE WITH CAUTION!).
 - **Network Audit** - Gathers all possible information about specific network and returns them onto the curses view. Tracks all clients signal and last activity, as well as resolve the manufacturer.
 - **Channel Hopper** - Changes the current channel of the network adapter. Helpful in making specific attacks more successful.
+- **Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this 'legitimate' AP asks user for login/ bank credentials, or to download malware. First, there's a normal AP created, most times with an ESSID and MAC of existing network. Then, we host our captive portal (e.g., login website), so a normal web server, that reroutes users to our `index.html` trying to associate with the network we spoof.
 
 <sup>1<sup>**Access Points**</sup></sup>
 
 <sup>2<sup>**Transceive and receive at the same time**</sup></sup>
 
 <h2><strong>8. Uninstall</strong></h2>
 
@@ -153,15 +164,15 @@
 
 <h2>TODO</h2>
 
 ✅ Evil Twin attack
 
 ✅ Version & update checker
 
-★ PyPi Release
+✅ PyPi Release
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: 3way Version: 1.2.0 Summary: Freeway for network
+Metadata-Version: 2.1 Name: 3way Version: 1.2.1 Summary: Freeway for network
 pentesting Home-page: https://github.com/FLOCK4H/Freeway Author: FLOCK4H
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE
        [Freeway logo]$${\color{red}Freeway\ for\ Network\ Pentesting}$$
                  RReeaadd tthhee aarrttiiccllee aabboouutt FFrreeeewwaayy,, nnooww oonn _M_e_d_i_u_m
 
 > [!NOTE] > Before using the software, the user must agree to the EULA when
 prompted
 ********** 11.. OOvveerrvviieeww **********
 **Freeway** is a Python scapy-based tool for WiFi penetration that aim to help
 ethical hackers and pentesters develop their skills and knowledge in auditing
 and securing home or enterprise networks.
 ********** 22.. FFeeaattuurreess **********
 - IEEE 802.11 Packet Monitoring - Deauthentication Attack - Beacon Flood -
-Packet Fuzzer - Network Audit - Channel Hopper Description of the features can
-be found in Section 6
+Packet Fuzzer - Network Audit - Channel Hopper - Evil Twin Description of the
+features can be found in Section 6
 ********** 33.. PPrreeppaarraattiioonn **********
 It is **necessary** to have: - A network adapter supporting monitor mode and
 frame injection. - An operating system running a Linux distribution. - Python
 3+ installed. Optionally, install Scapy and Rich packages for Python if not
 installing via pip (see Section 4)
 ********** 44.. SSeettuupp **********
-First, clone the repository: git clone https://github.com/FLOCK4H/Freeway
-Navigate to the cloned repository: cd Freeway AA:: Install dependencies and
-Freeway. This will allow to launch the tool from anywhere sudo pip install . BB::
-Run without installation using Python. Must be called from the /Freeway
-directory sudo pip install scapy rich sudo python Freeway
+A: Install via PyPi (pip) ``` $ sudo pip install 3way ``` B: Install or run
+manually First, clone the repository: git clone https://github.com/FLOCK4H/
+Freeway Navigate to the cloned repository: cd Freeway OOppttiioonn 11:: Install
+dependencies and Freeway. This will allow to launch the tool from anywhere sudo
+pip install . OOppttiioonn 22:: Run without installation using Python. Must be called
+from the /Freeway directory sudo pip install scapy rich sudo python Freeway
 ********** 55.. UUssaaggee **********
 This tool comes with its own **command line interface (CLI)** and can be run
 without specifying any additional arguments. CClliicckk ttoo eexxppaanndd tthhee CCLLII uussaaggee
 sudo Freeway Follow the prompt to select the network adapter (see Section 3): !
 [image](https://github.com/FLOCK4H/Freeway/assets/161654571/653c9304-3256-4444-
 8f3f-0677134c8af8) Select the feature and parameter(s): ![image](https://
 github.com/FLOCK4H/Freeway/assets/161654571/2444922e-6f1b-4958-99ea-
@@ -52,15 +53,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for
 every action.
   To list all parameters for a given action, just provide -a argument without -
 p.
 ********** 66.. DDeettaaiillss **********
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and
@@ -85,23 +87,29 @@
 responses. Freeway covers: **Replay captured packets (RX&TX2)**, **Spam CTS/RTS
 or Probe requests** and **Flood an AP with Authentication or Association
 Frames**. Devices that will capture fuzzed packets will behave differently
 depending on vulnerability level of receiver (!USE WITH CAUTION!). - **Network
 Audit** - Gathers all possible information about specific network and returns
 them onto the curses view. Tracks all clients signal and last activity, as well
 as resolve the manufacturer. - **Channel Hopper** - Changes the current channel
-of the network adapter. Helpful in making specific attacks more successful.
-1**Access Points** 2**Transceive and receive at the same time**
+of the network adapter. Helpful in making specific attacks more successful. -
+**Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this
+'legitimate' AP asks user for login/ bank credentials, or to download malware.
+First, there's a normal AP created, most times with an ESSID and MAC of
+existing network. Then, we host our captive portal (e.g., login website), so a
+normal web server, that reroutes users to our `index.html` trying to associate
+with the network we spoof. 1**Access Points** 2**Transceive and receive at the
+same time**
 ********** 88.. UUnniinnssttaallll **********
 In case where Freeway doesn't meet the expectations and was installed via pip,
 the removal process is as easy: sudo pip uninstall 3way The rename to 3way is
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
-â Evil Twin attack â Version & update checker â PyPi Release
+â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
 formatting in beacon_spam.py
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
 Android 11+, versions below Android 11 and above Android 5 were not tested.)
```

### Comparing `3way-1.2.0/3way.egg-info/SOURCES.txt` & `3way-1.2.1/3way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/Freeway` & `3way-1.2.1/Freeway`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/__init__.py` & `3way-1.2.1/FreewayTools/__init__.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/audit.py` & `3way-1.2.1/FreewayTools/audit.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/beacon_spam.py` & `3way-1.2.1/FreewayTools/beacon_spam.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/checkmac.py` & `3way-1.2.1/FreewayTools/checkmac.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/colors.py` & `3way-1.2.1/FreewayTools/colors.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/deauth.py` & `3way-1.2.1/FreewayTools/deauth.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/evil_twin.py` & `3way-1.2.1/FreewayTools/evil_twin.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/fuzzer.py` & `3way-1.2.1/FreewayTools/fuzzer.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/hopper.py` & `3way-1.2.1/FreewayTools/hopper.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/lists/ssid_list.txt` & `3way-1.2.1/FreewayTools/lists/ssid_list.txt`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/monitor.py` & `3way-1.2.1/FreewayTools/monitor.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/FreewayTools/updater.py` & `3way-1.2.1/FreewayTools/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return latest_release["tag_name"]
     except ConnectionError:
         pass
     except Exception as e:
         wprint(str(e))
 
 def get_current_version():
-    return "1.2.0"
+    return "1.2.1"
 
 def update():
     cprint("Checking for updates..")
     
     current_version = get_current_version()
     latest_version = get_latest_version()
     if latest_version is None:
```

### Comparing `3way-1.2.0/LICENSE` & `3way-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/PKG-INFO` & `3way-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3way
-Version: 1.2.0
+Version: 1.2.1
 Summary: Freeway for network pentesting
 Home-page: https://github.com/FLOCK4H/Freeway
 Author: FLOCK4H
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -33,43 +33,52 @@
 
 - IEEE 802.11 Packet Monitoring
 - Deauthentication Attack
 - Beacon Flood
 - Packet Fuzzer
 - Network Audit
 - Channel Hopper
+- Evil Twin
 
 <sub>Description of the features can be found in Section 6</sub>
 
 <h2><strong>3. Preparation</strong></h2>
 
 It is **necessary** to have:
 - A network adapter supporting monitor mode and frame injection.
 - An operating system running a Linux distribution.
 - Python 3+ installed.
 
 <sub>Optionally, install Scapy and Rich packages for Python if not installing via pip (see Section 4)</sub>
 
 <h2><strong>4. Setup</strong></h2>
 
+A: Install via PyPi (pip)
+
+```
+  $ sudo pip install 3way
+```
+
+B: Install or run manually
+
 First, clone the repository:
 
     git clone https://github.com/FLOCK4H/Freeway
 
 Navigate to the cloned repository:
 
     cd Freeway
 
-<strong>A:</strong> Install dependencies and Freeway.
+<strong>Option 1:</strong> Install dependencies and Freeway.
 
 <sub>This will allow to launch the tool from anywhere</sub>
 
     sudo pip install .
 
-<strong>B:</strong> Run without installation using Python.
+<strong>Option 2:</strong> Run without installation using Python.
 
 <sub>Must be called from the /Freeway directory</sub>
 
     sudo pip install scapy rich
     sudo python Freeway
 
 <h2><strong>5. Usage</strong></h2>
@@ -118,15 +127,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for every action.
   To list all parameters for a given action, just provide -a argument without -p.
 </pre>
 </div>
 </details>
 
@@ -134,14 +144,15 @@
 
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and return the result onto the python's curses display. Catches SSIDs, MACs, Clients, Uptime, Channel, Signal (dBm), Encryption and resolves manufacturer. Catches PMKIDs in hashcat crackable format, and 4-way Handshakes, as well as other EAPOL packets. Logs the captured session to the **/caps** folder or every captured packet if _Save output_ was selected.
 - **Deauthentication Attack (Deauthing)** - Disconnects a device from the network by sending a packet containing AP<sup>1</sup> address, device address (or broadcast for _Mass Deauthing_) and the deauthentication frame with a reason of kicking the client(s). In case where a device address is a broadcast address, the AP will in most cases disconnect all clients at once. Freeway creates separate thread for every AP or client found in order to make deauthing maximally efficient.
 - **Beacon Flood Attack** - Floods the nearby WiFi scanners with fake or malformed APs. It can cause the devices looking for WiFi to behave abnormally (e.g. crash, freeze, drain the battery or run slower) and disrupt the nearby network traffic. User is able to specify his own ssid list, use the default one and generate correct (but random) or malformed beacon packets.
 - **Packet Fuzzer** - Fuzzing is a technique of network vulnerability assesment by sending a wide array of malformed or semi-random data to network interfaces and observing the responses. Freeway covers: **Replay captured packets (RX&TX<sup>2</sup>)**, **Spam CTS/RTS or Probe requests** and **Flood an AP with Authentication or Association Frames**. Devices that will capture fuzzed packets will behave differently depending on vulnerability level of receiver (!USE WITH CAUTION!).
 - **Network Audit** - Gathers all possible information about specific network and returns them onto the curses view. Tracks all clients signal and last activity, as well as resolve the manufacturer.
 - **Channel Hopper** - Changes the current channel of the network adapter. Helpful in making specific attacks more successful.
+- **Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this 'legitimate' AP asks user for login/ bank credentials, or to download malware. First, there's a normal AP created, most times with an ESSID and MAC of existing network. Then, we host our captive portal (e.g., login website), so a normal web server, that reroutes users to our `index.html` trying to associate with the network we spoof.
 
 <sup>1<sup>**Access Points**</sup></sup>
 
 <sup>2<sup>**Transceive and receive at the same time**</sup></sup>
 
 <h2><strong>8. Uninstall</strong></h2>
 
@@ -153,15 +164,15 @@
 
 <h2>TODO</h2>
 
 ✅ Evil Twin attack
 
 ✅ Version & update checker
 
-★ PyPi Release
+✅ PyPi Release
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: 3way Version: 1.2.0 Summary: Freeway for network
+Metadata-Version: 2.1 Name: 3way Version: 1.2.1 Summary: Freeway for network
 pentesting Home-page: https://github.com/FLOCK4H/Freeway Author: FLOCK4H
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE
        [Freeway logo]$${\color{red}Freeway\ for\ Network\ Pentesting}$$
                  RReeaadd tthhee aarrttiiccllee aabboouutt FFrreeeewwaayy,, nnooww oonn _M_e_d_i_u_m
 
 > [!NOTE] > Before using the software, the user must agree to the EULA when
 prompted
 ********** 11.. OOvveerrvviieeww **********
 **Freeway** is a Python scapy-based tool for WiFi penetration that aim to help
 ethical hackers and pentesters develop their skills and knowledge in auditing
 and securing home or enterprise networks.
 ********** 22.. FFeeaattuurreess **********
 - IEEE 802.11 Packet Monitoring - Deauthentication Attack - Beacon Flood -
-Packet Fuzzer - Network Audit - Channel Hopper Description of the features can
-be found in Section 6
+Packet Fuzzer - Network Audit - Channel Hopper - Evil Twin Description of the
+features can be found in Section 6
 ********** 33.. PPrreeppaarraattiioonn **********
 It is **necessary** to have: - A network adapter supporting monitor mode and
 frame injection. - An operating system running a Linux distribution. - Python
 3+ installed. Optionally, install Scapy and Rich packages for Python if not
 installing via pip (see Section 4)
 ********** 44.. SSeettuupp **********
-First, clone the repository: git clone https://github.com/FLOCK4H/Freeway
-Navigate to the cloned repository: cd Freeway AA:: Install dependencies and
-Freeway. This will allow to launch the tool from anywhere sudo pip install . BB::
-Run without installation using Python. Must be called from the /Freeway
-directory sudo pip install scapy rich sudo python Freeway
+A: Install via PyPi (pip) ``` $ sudo pip install 3way ``` B: Install or run
+manually First, clone the repository: git clone https://github.com/FLOCK4H/
+Freeway Navigate to the cloned repository: cd Freeway OOppttiioonn 11:: Install
+dependencies and Freeway. This will allow to launch the tool from anywhere sudo
+pip install . OOppttiioonn 22:: Run without installation using Python. Must be called
+from the /Freeway directory sudo pip install scapy rich sudo python Freeway
 ********** 55.. UUssaaggee **********
 This tool comes with its own **command line interface (CLI)** and can be run
 without specifying any additional arguments. CClliicckk ttoo eexxppaanndd tthhee CCLLII uussaaggee
 sudo Freeway Follow the prompt to select the network adapter (see Section 3): !
 [image](https://github.com/FLOCK4H/Freeway/assets/161654571/653c9304-3256-4444-
 8f3f-0677134c8af8) Select the feature and parameter(s): ![image](https://
 github.com/FLOCK4H/Freeway/assets/161654571/2444922e-6f1b-4958-99ea-
@@ -52,15 +53,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for
 every action.
   To list all parameters for a given action, just provide -a argument without -
 p.
 ********** 66.. DDeettaaiillss **********
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and
@@ -85,23 +87,29 @@
 responses. Freeway covers: **Replay captured packets (RX&TX2)**, **Spam CTS/RTS
 or Probe requests** and **Flood an AP with Authentication or Association
 Frames**. Devices that will capture fuzzed packets will behave differently
 depending on vulnerability level of receiver (!USE WITH CAUTION!). - **Network
 Audit** - Gathers all possible information about specific network and returns
 them onto the curses view. Tracks all clients signal and last activity, as well
 as resolve the manufacturer. - **Channel Hopper** - Changes the current channel
-of the network adapter. Helpful in making specific attacks more successful.
-1**Access Points** 2**Transceive and receive at the same time**
+of the network adapter. Helpful in making specific attacks more successful. -
+**Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this
+'legitimate' AP asks user for login/ bank credentials, or to download malware.
+First, there's a normal AP created, most times with an ESSID and MAC of
+existing network. Then, we host our captive portal (e.g., login website), so a
+normal web server, that reroutes users to our `index.html` trying to associate
+with the network we spoof. 1**Access Points** 2**Transceive and receive at the
+same time**
 ********** 88.. UUnniinnssttaallll **********
 In case where Freeway doesn't meet the expectations and was installed via pip,
 the removal process is as easy: sudo pip uninstall 3way The rename to 3way is
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
-â Evil Twin attack â Version & update checker â PyPi Release
+â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
 formatting in beacon_spam.py
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
 Android 11+, versions below Android 11 and above Android 5 were not tested.)
```

### Comparing `3way-1.2.0/README.md` & `3way-1.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,43 +23,52 @@
 
 - IEEE 802.11 Packet Monitoring
 - Deauthentication Attack
 - Beacon Flood
 - Packet Fuzzer
 - Network Audit
 - Channel Hopper
+- Evil Twin
 
 <sub>Description of the features can be found in Section 6</sub>
 
 <h2><strong>3. Preparation</strong></h2>
 
 It is **necessary** to have:
 - A network adapter supporting monitor mode and frame injection.
 - An operating system running a Linux distribution.
 - Python 3+ installed.
 
 <sub>Optionally, install Scapy and Rich packages for Python if not installing via pip (see Section 4)</sub>
 
 <h2><strong>4. Setup</strong></h2>
 
+A: Install via PyPi (pip)
+
+```
+  $ sudo pip install 3way
+```
+
+B: Install or run manually
+
 First, clone the repository:
 
     git clone https://github.com/FLOCK4H/Freeway
 
 Navigate to the cloned repository:
 
     cd Freeway
 
-<strong>A:</strong> Install dependencies and Freeway.
+<strong>Option 1:</strong> Install dependencies and Freeway.
 
 <sub>This will allow to launch the tool from anywhere</sub>
 
     sudo pip install .
 
-<strong>B:</strong> Run without installation using Python.
+<strong>Option 2:</strong> Run without installation using Python.
 
 <sub>Must be called from the /Freeway directory</sub>
 
     sudo pip install scapy rich
     sudo python Freeway
 
 <h2><strong>5. Usage</strong></h2>
@@ -108,15 +117,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for every action.
   To list all parameters for a given action, just provide -a argument without -p.
 </pre>
 </div>
 </details>
 
@@ -124,14 +134,15 @@
 
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and return the result onto the python's curses display. Catches SSIDs, MACs, Clients, Uptime, Channel, Signal (dBm), Encryption and resolves manufacturer. Catches PMKIDs in hashcat crackable format, and 4-way Handshakes, as well as other EAPOL packets. Logs the captured session to the **/caps** folder or every captured packet if _Save output_ was selected.
 - **Deauthentication Attack (Deauthing)** - Disconnects a device from the network by sending a packet containing AP<sup>1</sup> address, device address (or broadcast for _Mass Deauthing_) and the deauthentication frame with a reason of kicking the client(s). In case where a device address is a broadcast address, the AP will in most cases disconnect all clients at once. Freeway creates separate thread for every AP or client found in order to make deauthing maximally efficient.
 - **Beacon Flood Attack** - Floods the nearby WiFi scanners with fake or malformed APs. It can cause the devices looking for WiFi to behave abnormally (e.g. crash, freeze, drain the battery or run slower) and disrupt the nearby network traffic. User is able to specify his own ssid list, use the default one and generate correct (but random) or malformed beacon packets.
 - **Packet Fuzzer** - Fuzzing is a technique of network vulnerability assesment by sending a wide array of malformed or semi-random data to network interfaces and observing the responses. Freeway covers: **Replay captured packets (RX&TX<sup>2</sup>)**, **Spam CTS/RTS or Probe requests** and **Flood an AP with Authentication or Association Frames**. Devices that will capture fuzzed packets will behave differently depending on vulnerability level of receiver (!USE WITH CAUTION!).
 - **Network Audit** - Gathers all possible information about specific network and returns them onto the curses view. Tracks all clients signal and last activity, as well as resolve the manufacturer.
 - **Channel Hopper** - Changes the current channel of the network adapter. Helpful in making specific attacks more successful.
+- **Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this 'legitimate' AP asks user for login/ bank credentials, or to download malware. First, there's a normal AP created, most times with an ESSID and MAC of existing network. Then, we host our captive portal (e.g., login website), so a normal web server, that reroutes users to our `index.html` trying to associate with the network we spoof.
 
 <sup>1<sup>**Access Points**</sup></sup>
 
 <sup>2<sup>**Transceive and receive at the same time**</sup></sup>
 
 <h2><strong>8. Uninstall</strong></h2>
 
@@ -143,15 +154,15 @@
 
 <h2>TODO</h2>
 
 ✅ Evil Twin attack
 
 ✅ Version & update checker
 
-★ PyPi Release
+✅ PyPi Release
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
```

#### html2text {}

```diff
@@ -5,27 +5,28 @@
 prompted
 ********** 11.. OOvveerrvviieeww **********
 **Freeway** is a Python scapy-based tool for WiFi penetration that aim to help
 ethical hackers and pentesters develop their skills and knowledge in auditing
 and securing home or enterprise networks.
 ********** 22.. FFeeaattuurreess **********
 - IEEE 802.11 Packet Monitoring - Deauthentication Attack - Beacon Flood -
-Packet Fuzzer - Network Audit - Channel Hopper Description of the features can
-be found in Section 6
+Packet Fuzzer - Network Audit - Channel Hopper - Evil Twin Description of the
+features can be found in Section 6
 ********** 33.. PPrreeppaarraattiioonn **********
 It is **necessary** to have: - A network adapter supporting monitor mode and
 frame injection. - An operating system running a Linux distribution. - Python
 3+ installed. Optionally, install Scapy and Rich packages for Python if not
 installing via pip (see Section 4)
 ********** 44.. SSeettuupp **********
-First, clone the repository: git clone https://github.com/FLOCK4H/Freeway
-Navigate to the cloned repository: cd Freeway AA:: Install dependencies and
-Freeway. This will allow to launch the tool from anywhere sudo pip install . BB::
-Run without installation using Python. Must be called from the /Freeway
-directory sudo pip install scapy rich sudo python Freeway
+A: Install via PyPi (pip) ``` $ sudo pip install 3way ``` B: Install or run
+manually First, clone the repository: git clone https://github.com/FLOCK4H/
+Freeway Navigate to the cloned repository: cd Freeway OOppttiioonn 11:: Install
+dependencies and Freeway. This will allow to launch the tool from anywhere sudo
+pip install . OOppttiioonn 22:: Run without installation using Python. Must be called
+from the /Freeway directory sudo pip install scapy rich sudo python Freeway
 ********** 55.. UUssaaggee **********
 This tool comes with its own **command line interface (CLI)** and can be run
 without specifying any additional arguments. CClliicckk ttoo eexxppaanndd tthhee CCLLII uussaaggee
 sudo Freeway Follow the prompt to select the network adapter (see Section 3): !
 [image](https://github.com/FLOCK4H/Freeway/assets/161654571/653c9304-3256-4444-
 8f3f-0677134c8af8) Select the feature and parameter(s): ![image](https://
 github.com/FLOCK4H/Freeway/assets/161654571/2444922e-6f1b-4958-99ea-
@@ -49,15 +50,16 @@
 
   Actions:
   1 or monitor,
   2 or deauth,
   3 or beacon_spam,
   4 or fuzzer,
   5 or audit,
-  6 or hopper
+  6 or hopper,
+  7 or eviltwin
 
   Parameters must be provided in the same format as in the CLI, specific for
 every action.
   To list all parameters for a given action, just provide -a argument without -
 p.
 ********** 66.. DDeettaaiillss **********
 - **Packet Monitor** - Sniffs the WiFi packets in the air, analyze them and
@@ -82,23 +84,29 @@
 responses. Freeway covers: **Replay captured packets (RX&TX2)**, **Spam CTS/RTS
 or Probe requests** and **Flood an AP with Authentication or Association
 Frames**. Devices that will capture fuzzed packets will behave differently
 depending on vulnerability level of receiver (!USE WITH CAUTION!). - **Network
 Audit** - Gathers all possible information about specific network and returns
 them onto the curses view. Tracks all clients signal and last activity, as well
 as resolve the manufacturer. - **Channel Hopper** - Changes the current channel
-of the network adapter. Helpful in making specific attacks more successful.
-1**Access Points** 2**Transceive and receive at the same time**
+of the network adapter. Helpful in making specific attacks more successful. -
+**Evil Twin** - Hosts a legitimate Access Point with Captive Portal, this
+'legitimate' AP asks user for login/ bank credentials, or to download malware.
+First, there's a normal AP created, most times with an ESSID and MAC of
+existing network. Then, we host our captive portal (e.g., login website), so a
+normal web server, that reroutes users to our `index.html` trying to associate
+with the network we spoof. 1**Access Points** 2**Transceive and receive at the
+same time**
 ********** 88.. UUnniinnssttaallll **********
 In case where Freeway doesn't meet the expectations and was installed via pip,
 the removal process is as easy: sudo pip uninstall 3way The rename to 3way is
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
-â Evil Twin attack â Version & update checker â PyPi Release
+â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
 formatting in beacon_spam.py
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
 Android 11+, versions below Android 11 and above Android 5 were not tested.)
```

### Comparing `3way-1.2.0/setup.py` & `3way-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 shutil.copytree(f"{source}/{template}", f"{destination}/{template}")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='3way',
-    version='1.2.0',
+    version='1.2.1',
     author='FLOCK4H',
     url='https://github.com/FLOCK4H/Freeway',
     description='Freeway for network pentesting',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `3way-1.2.0/templates/Valentines/index.html` & `3way-1.2.1/templates/Valentines/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/templates/google/index.html` & `3way-1.2.1/templates/google/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/templates/mcd/index.html` & `3way-1.2.1/templates/mcd/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/templates/mrhacker/index.html` & `3way-1.2.1/templates/mrhacker/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.0/templates/mrhacker/static/mrhacker.png` & `3way-1.2.1/templates/mrhacker/static/mrhacker.png`

 * *Files identical despite different names*

