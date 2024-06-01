# Comparing `tmp/HakObserverpy-0.6.4.tar.gz` & `tmp/HakObserverpy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HakObserverpy-0.6.4.tar", last modified: Tue May 14 07:29:43 2024, max compression
+gzip compressed data, was "HakObserverpy-0.6.5.tar", last modified: Sat Jun  1 09:58:45 2024, max compression
```

## Comparing `HakObserverpy-0.6.4.tar` & `HakObserverpy-0.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 07:29:43.536583 HakObserverpy-0.6.4/
-drwxrwxrwx   0        0        0        0 2024-05-14 07:29:43.514582 HakObserverpy-0.6.4/HakObserverpy/
--rw-rw-rw-   0        0        0     9618 2024-05-14 07:29:29.000000 HakObserverpy-0.6.4/HakObserverpy/HakObserverpy.py
--rw-rw-rw-   0        0        0      332 2024-05-14 07:29:33.000000 HakObserverpy-0.6.4/HakObserverpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 07:29:43.534581 HakObserverpy-0.6.4/HakObserverpy.egg-info/
--rw-rw-rw-   0        0        0      705 2024-05-14 07:29:43.000000 HakObserverpy-0.6.4/HakObserverpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-14 07:29:43.000000 HakObserverpy-0.6.4/HakObserverpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:29:43.000000 HakObserverpy-0.6.4/HakObserverpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-14 07:29:43.000000 HakObserverpy-0.6.4/HakObserverpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 07:29:43.000000 HakObserverpy-0.6.4/HakObserverpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      705 2024-05-14 07:29:43.535582 HakObserverpy-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 HakObserverpy-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 07:29:43.536583 HakObserverpy-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-05-14 07:29:10.000000 HakObserverpy-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 09:58:45.679000 HakObserverpy-0.6.5/
+drwxrwxrwx   0        0        0        0 2024-06-01 09:58:45.612000 HakObserverpy-0.6.5/HakObserverpy/
+-rw-rw-rw-   0        0        0     6190 2024-06-01 09:58:25.000000 HakObserverpy-0.6.5/HakObserverpy/HakObserverpy.py
+-rw-rw-rw-   0        0        0      281 2024-06-01 09:57:43.000000 HakObserverpy-0.6.5/HakObserverpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 09:58:45.667000 HakObserverpy-0.6.5/HakObserverpy.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-06-01 09:58:45.000000 HakObserverpy-0.6.5/HakObserverpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-06-01 09:58:45.000000 HakObserverpy-0.6.5/HakObserverpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 09:58:45.000000 HakObserverpy-0.6.5/HakObserverpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-01 09:58:45.000000 HakObserverpy-0.6.5/HakObserverpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-01 09:58:45.000000 HakObserverpy-0.6.5/HakObserverpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-06-01 09:58:45.674000 HakObserverpy-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 HakObserverpy-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 09:58:45.678000 HakObserverpy-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-06-01 09:57:39.000000 HakObserverpy-0.6.5/setup.py
```

### Comparing `HakObserverpy-0.6.4/HakObserverpy/HakObserverpy.py` & `HakObserverpy-0.6.5/HakObserverpy/HakObserverpy.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     log_entry = {
         "time": error_time,
         "type": Type,
         "details": Message
     }
     
-    # Create or append to log.json
+    #Create or append to log.json
     with open("log.json", "a+") as log_file:
         log_file.seek(0)
         if log_file.read(1):
             log_file.write(",\n")
         else:
             log_file.write("[\n")
         json.dump(log_entry, log_file, indent=4)
@@ -36,45 +36,41 @@
     log("get_installed_applications", "Starting")
     get_installed_applications(HWDeviceID)
     log("get_installed_applications", "Completed")
 
     collect_firewall_logs()
 
 def collect_firewall_logs():
-    # Use PowerShell to collect firewall logs
+    #Use PowerShell to collect firewall logs
     powershell_command = """
     $events = Get-WinEvent -LogName 'Security' -MaxEvents 100
     $logs = $events | ForEach-Object { $_.Message }
     $logs
     """
     logs = subprocess.check_output(["powershell", "-Command", powershell_command], shell=True)
     return logs.decode('utf-8')
     
 def get_installed_applications(HWDeviceID):
-
-    
-
-
-    # Example: Retrieve installed applications and their version numbers from the Windows Registry
+    #Example: Retrieve installed applications and their version numbers from the Windows Registry
     key = r"SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall"
     installed_apps = []
     with winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, key) as reg_key:
         for i in range(winreg.QueryInfoKey(reg_key)[0]):
             try:
                 app_key = winreg.EnumKey(reg_key, i)
                 with winreg.OpenKey(reg_key, app_key) as app_reg_key:
                     app_name = winreg.QueryValueEx(app_reg_key, "DisplayName")[0]
                     app_version = winreg.QueryValueEx(app_reg_key, "DisplayVersion")[0]
                     app_name = str(app_name).replace("-","").replace("/","").replace("(","").replace(")","")
 
-                    # Replace special characters in app_name
+                    #Replace special characters in app_name
                     
                     url = f"https://api.hakware.com/HakObserver/DeviceApps/{HWDeviceID}/{app_name}/{app_version}"
 
-                    # Make a GET request to the URL
+                    #Make a GET request to the URL
                     session = HTMLSession()
                 
                     response = session.get(url, verify=False)
 
                     if response.status_code == 200:
                         print("Device Data inserted successfully via API.")
                     else:
@@ -85,34 +81,34 @@
                     installed_apps.append({"name": app_name, "version": app_version})
             except FileNotFoundError:
                 pass
     return installed_apps
 
 def get_system_usage(HWDeviceID,ObserverVersion):
 
-    # Example: Retrieve OS version using system-specific commands
+    #Example: Retrieve OS version using system-specific commands
     os_version = str(subprocess.check_output("ver", shell=True)).replace('(', '').replace(')', '')
 
-    # Retrieve CPU, RAM, and disk usage
+    # CPU, RAM, and disk usage
     cpu_usage = psutil.cpu_percent()
     ram_usage = psutil.virtual_memory().percent
-    #disk_usage = psutil.disk_usage('C:').percent  # Replace 'C:' with appropriate drive letter
+    #disk_usage = psutil.disk_usage('C:').percent  Replace 'C:' with appropriate drive letter
 
-    # Retrieve total memory
+    #Retrieve total memory
     total_memory = psutil.virtual_memory().total
     total_memory_gb = total_memory / (1024**3)
-    # Retrieve total number of CPUs and cores
-    total_cpus = psutil.cpu_count(logical=False)  # Physical CPUs
-    total_cores = psutil.cpu_count(logical=True)  # Logical CPUs (cores)
+    #Retrieve total number of CPUs and cores
+    total_cpus = psutil.cpu_count(logical=False)  #Physical CPUs
+    total_cores = psutil.cpu_count(logical=True)  #Logical CPUs (cores)
 
   
 
     device_name = str(platform.node()).replace('(', '').replace(')', ''),
     processor = str(platform.processor()).replace('(', '').replace(')', ''),
-    device_id = str(platform.node()).replace('(', '').replace(')', ''),  # You may replace this with an appropriate identifier for your system
+    device_id = str(platform.node()).replace('(', '').replace(')', ''),  #You may replace this with an appropriate identifier for your system
     system_type = str(platform.system()).replace('(', '').replace(')', '')
 
 
     
     ObserverVersion = str(ObserverVersion).replace("(","").replace(")","").replace(",","").replace("\\r\\n","").replace("'","")
     device_id =str(device_id).replace("(","").replace(")","").replace(",","").replace("\\r\\n","").replace("'","")
     device_name = str(device_name).replace("(","").replace(")","").replace(",","").replace("\\r\\n","").replace("'","")
@@ -129,15 +125,15 @@
 
     from requests_html import HTMLSession
 
     url = f"https://api.hakware.com/HakObserver/Device/{HWDeviceID}/{ObserverVersion}/{device_name}/{processor}/{device_id}/{system_type}/{os_version}/{total_memory_gb}/{total_cpus}/{total_cores}"
     
   
 
-    # Make a GET request to the URL
+    #Make a GET request to the URL
     session = HTMLSession()
    
     response = session.get(url, verify=False, timeout=10)
 
     print(response)
 
     if response.status_code == 200:
@@ -148,98 +144,8 @@
         "cpu_usage_percent": cpu_usage,
         "ram_usage_percent": ram_usage,
         #"disk_usage_percent": disk_usage,
         "total_memory": total_memory_gb,
         "total_cpus": total_cpus,
         "total_cores": total_cores
     }
-
-
 ###############################################################################################################################################################################
-
-def LinInitiateCollecection(HWDeviceID, ObserverVersion):  
-   
-
-    Linget_system_usage(HWDeviceID,ObserverVersion)
-
-
-    Linget_installed_applications(HWDeviceID)
-
-
-    Lincollect_firewall_logs()
-
-def Lincollect_firewall_logs():
-    # Placeholder function for firewall log collection on Linux
-    pass
-    
-def Linget_installed_applications(HWDeviceID):
-    installed_apps = []
-
-    # Use dpkg-query to list installed packages
-    try:
-        dpkg_output = subprocess.check_output(["dpkg-query", "-l"], universal_newlines=True)
-        lines = dpkg_output.strip().split('\n')[5:]  # Skip first 5 lines which are headers
-        for line in lines:
-            columns = line.split()
-            if len(columns) >= 2:
-                app_name = columns[1]
-                app_version = columns[2]
-                installed_apps.append({"name": app_name, "version": app_version})
-    except subprocess.CalledProcessError as e:
-        print("Error:", e)
-
-    # Now you can process installed_apps list as needed
-    for app in installed_apps:
-        # Replace special characters in app_name
-        app_name = app['name'].replace("-", "").replace("/", "").replace("(", "").replace(")", "")
-        app_version = app['version'].replace("-", "").replace("/", "").replace("(", "").replace(")", "").replace("'","").replace("+"," ")
-        # Hakware API URL for inserting installed applications
-        url = f"https://api.hakware.com/HakObserver/DeviceApps/{HWDeviceID}/{app_name}/{app_version}"
-
-        # Make a GET request to the URL
-        session = HTMLSession()
-        response = session.get(url, verify=False)
-
-        if response.status_code == 200:
-            print(f"Installed application '{app_name}' version '{app['version']}' data inserted successfully via API.")
-        else:
-            print(url)
-            print(f"Failed to insert installed application '{app_name}' version '{app_version}' data via API. Status code: {response.status_code}")
-
-    return installed_apps
-
-def Linget_system_usage(HWDeviceID, ObserverVersion):
-    # Retrieve system information
-    os_version = platform.platform()
-    cpu_usage = psutil.cpu_percent()
-    ram_usage = psutil.virtual_memory().percent
-    total_memory = psutil.virtual_memory().total / (1024**3)
-    total_cpus = psutil.cpu_count(logical=False)
-    total_cores = psutil.cpu_count(logical=True)
-    device_name = platform.node()
-    processor = platform.processor()
-    device_id = platform.node()
-    system_type = platform.system()
-
-    if processor == '':
-        processor = 'unknown' 
-
-    # API URL
-    url = f"https://api.hakware.com/HakObserver/Device/{HWDeviceID}/{ObserverVersion}/{device_name}/{processor}/{device_id}/{system_type}/{os_version}/{total_memory}/{total_cpus}/{total_cores}"
-
-    print(url)
-    # Make a GET request to the URL
-    session = HTMLSession()
-    response = session.get(url, verify=False, timeout=10)
-
-    if response.status_code == 200:
-        print("Device Data inserted successfully via API.")
-    else:
-        print(f"Failed to insert data via API. Status code: {response.status_code}")
-
-    return {
-        "cpu_usage_percent": cpu_usage,
-        "ram_usage_percent": ram_usage,
-        "total_memory": total_memory,
-        "total_cpus": total_cpus,
-        "total_cores": total_cores
-    }
```

### Comparing `HakObserverpy-0.6.4/HakObserverpy.egg-info/PKG-INFO` & `HakObserverpy-0.6.5/HakObserverpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.4/PKG-INFO` & `HakObserverpy-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverpy-0.6.4/setup.py` & `HakObserverpy-0.6.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from setuptools import setup, find_packages
 
 setup(
     name='HakObserverpy',  # Your package name
-    version='0.6.4',  # Start with a version number
+    version='0.6.5',  # Start with a version number
     description='A package connect endpoints to the Hakware Application',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
```

