# Comparing `tmp/klldFN-2.0.1.tar.gz` & `tmp/klldFN-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-2.0.1.tar", last modified: Mon May 27 09:16:01 2024, max compression
+gzip compressed data, was "klldFN-2.0.2.tar", last modified: Sat Jun  1 20:10:42 2024, max compression
```

## Comparing `klldFN-2.0.1.tar` & `klldFN-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-27 09:16:01.051595 klldFN-2.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1186 2024-05-27 09:16:01.051595 klldFN-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-05-25 10:49:24.000000 klldFN-2.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-27 09:16:01.039595 klldFN-2.0.1/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)   134589 2024-05-26 21:39:32.000000 klldFN-2.0.1/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-27 09:16:01.047595 klldFN-2.0.1/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1186 2024-05-27 09:16:00.000000 klldFN-2.0.1/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-27 09:16:00.000000 klldFN-2.0.1/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-27 09:16:00.000000 klldFN-2.0.1/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-27 09:16:00.000000 klldFN-2.0.1/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-27 09:16:00.000000 klldFN-2.0.1/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-27 09:16:01.051595 klldFN-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1384 2024-05-27 09:15:30.000000 klldFN-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 20:10:42.954805 klldFN-2.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1528 2024-06-01 20:10:42.950805 klldFN-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-06-01 18:28:30.000000 klldFN-2.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 20:10:42.942804 klldFN-2.0.2/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)   152727 2024-06-01 18:20:31.000000 klldFN-2.0.2/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 20:10:42.950805 klldFN-2.0.2/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1528 2024-06-01 20:10:42.000000 klldFN-2.0.2/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-06-01 20:10:42.000000 klldFN-2.0.2/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-06-01 20:10:42.000000 klldFN-2.0.2/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-06-01 20:10:42.000000 klldFN-2.0.2/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-06-01 20:10:42.000000 klldFN-2.0.2/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-06-01 20:10:42.954805 klldFN-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1436 2024-06-01 18:21:58.000000 klldFN-2.0.2/setup.py
```

### Comparing `klldFN-2.0.1/klldFN/__init__.py` & `klldFN-2.0.2/klldFN/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import json
 from fortnitepy.ext import commands as fcommands
 import fortnitepy
 import FortniteAPIAsync
 from functools import partial
 import random as py_random
 from rich.progress import Progress, TextColumn, BarColumn, SpinnerColumn, TimeElapsedColumn
-import base64
 
 
 
 #loop = asyncio.get_event_loop()
 Sanic = sanic.Sanic(__name__)
 fortnite_api = FortniteAPIAsync.APIClient()
 owner = 'e375edab04964813a886ee974b66bd70'
@@ -40,56 +39,64 @@
             else:
                 return None
 
 
 
 
 
+
+
+
 class UpdateTranslations:
-    def __await__(self):
-        encoded_link = "aHR0cHM6Ly9hLS1zLTIzNDItZGppYXM0Mzg4LS0yNG9oaS11ZGQtLWFvdS1oczMtMjQtZmxpZS5wYWdlcy5kZXYvdHJhbnNsYXRpb25zLmpzb24="
-        url = base64.b64decode(encoded_link).decode('utf-8')
-        file_name = "translations/translations.json"
-        return self.update_translations(url, file_name).__await__()
+    async def __call__(self):
+        urls = [
+            "https://a--s-2342-djias4388--24ohi-udd--aou-hs3-24-flie.pages.dev/translations-system.json",
+            "https://a--s-2342-djias4388--24ohi-udd--aou-hs3-24-flie.pages.dev/translations.json"
+        ]
+        results = []
+        for url in urls:
+            result = await self.update_translations(url)
+            results.append(result)
+        return results
 
-    async def update_translations(self, url, file_name):
+    async def update_translations(self, url):
         """
         Update translations file if its content has changed.
 
         Args:
             url (str): The URL of the translations file.
-            file_name (str): The name of the local file to save translations.
 
         Returns:
             str: Message indicating whether the file was updated or not.
         """
         response = requests.get(url)
 
         if response.status_code == 200:
             new_content = response.content
 
+            file_name = "translations/" + url.split('/')[-1]
+
             try:
                 os.makedirs(os.path.dirname(file_name), exist_ok=True)
-              
+
                 with open(file_name, 'rb') as f:
                     existing_content = f.read()
 
                 if new_content != existing_content:
                     with open(file_name, 'wb') as f:
                         f.write(new_content)
                     pass
                 else:
                     pass
             except FileNotFoundError:
                 with open(file_name, 'wb') as f:
                     f.write(new_content)
                 pass
         else:
-            print(f"Failed to download file. Status code: {response.status_code}")
-
+            return f"Failed to download file from '{url}'. Status code: {response.status_code}"
 
 def load_auths_data(filename):
     with open(filename, 'r') as f:
         auths_data = json.load(f)
     return auths_data
 
 
@@ -112,42 +119,49 @@
     try:
         installed_version = subprocess.check_output([sys.executable, '-m', 'pip', 'show', 'klldFN']).decode('utf-8')
         installed_version = next(line for line in installed_version.split('\n') if line.startswith('Version:')).split(': ')[1].strip()
         latest_version = get_latest_version()
 
         if installed_version != latest_version:
             print(f"Updating klldFN from {installed_version} to {latest_version}...")
+            Updating_klldFN = translations_system.read()["translations"]["Updating-klldFN"][get_Language]
+            print(Updating_klldFN.format(installed_version, latest_version))
             await update_package()
             print("Update successful! Restarting script...")
             await restart_script()
         else:
             pass
     except subprocess.CalledProcessError as e:
         print("Error occurred while checking package:", e)
 
 progress = None
 async def clients_sanic_Run():
+    updater = UpdateTranslations()
+    await updater()
     config = configuration.read()['sanic web']['start']
     if config:
         await sanic_start()
     progress = Progress(
                 TextColumn("[bold blue]{task.description}", justify="right"),
                 BarColumn(bar_width=None),
                 SpinnerColumn(spinner_name="clock", style="bright_yellow", speed=1.0),
                 TimeElapsedColumn(),
             )        
     task1 = None
     with progress:
-                task1 = progress.add_task("[bold green]Starting klldFN v2.0.0...", total=3)
+                klldFN_Starting = translations_system.read()["translations"]["klldFN-Starting"][get_Language]
+                updating_package = translations_system.read()["translations"]["updating-package"][get_Language]
+                updating_translations = translations_system.read()["translations"]["updating-translations"][get_Language]
+                task1 = progress.add_task(f"[bold green]{klldFN_Starting}", total=3)
                 await asyncio.sleep(2)
-                progress.update(task1, advance=2, description="[bold green]Checking and updating package...")
+                progress.update(task1, advance=2, description=f"[bold green]{updating_package}")
                 await check_and_update_package()
                 await asyncio.sleep(1)
-                progress.update(task1, advance=1, description="[bold green]Updating translations...")
-                await UpdateTranslations()
+                progress.update(task1, advance=1, description=f"[bold green]{updating_translations}")
+
 
     await run_clients()
 
 
 async def run_clients():
     with open('auths.json') as f:
         auths_data = json.load(f)
@@ -172,25 +186,34 @@
         )
         await coro
 
 
 
 
 
-# Jinja2 template object
 
 
 class translations:
   """Interact With The Bot Configuration("translations.json")"""
   def read():
     """Read The Configuration File"""
     with open("translations/translations.json", encoding='utf-8') as config_file:
       config = json.load(config_file)
       return config
 
+
+class translations_system:
+  """Interact With The Bot Configuration("translations-system.json")"""
+  def read():
+    """Read The Configuration File"""
+    with open("translations/translations-system.json", encoding='utf-8') as config_file:
+      config = json.load(config_file)
+      return config    
+
+
 class configuration:
   """Interact With The Bot Configuration("config.json")"""
   def read():
     """Read The Configuration File"""
     with open("config.json") as config_file:
       config = json.load(config_file)
       return config
@@ -221,15 +244,15 @@
     @client.event  
     async def event_ready() -> None:
 
         await edit_and_keep_client_member()
         await add_list()
         client_ready = translations.read()["translations"]["Client-ready"][get_Language]
         print(client_ready.format(client.user.display_name))
-      
+
 
 
     async def set_crowns():
         meta = client.party.me.meta
         data = (meta.get_prop('Default:AthenaCosmeticLoadout_j'))['AthenaCosmeticLoadout']
         try:
             data['cosmeticStats'][1]['statValue'] = 1942
@@ -324,24 +347,25 @@
                 await client.add_friend(message.author.id)
             except: pass
 
     @client.event 
     async def event_friend_add(friend: fortnitepy.Friend) -> None:
         try:
             await asyncio.sleep(0.3)
-            await friend.send("Hi {DISPLAY_NAME} u add me now \n join me for more and fun thing ! \n klldfn.xyz".replace('{DISPLAY_NAME}', friend.display_name))
+            friend_add = translations.read()["translations"]["friend-add"][get_Language]
+            await friend.send(friend_add.replace(friend.display_name))
             await friend.invite()
         except: pass 
 
     @client.event 
     async def event_command_error(ctx: fortnitepy.ext.commands.Context, error):
-        if isinstance(error, fcommands.CommandNotFound):
-            notfound = translations.read()["translations"]["command-error-notfound"][get_Language]
-            await ctx.send(notfound)
-        elif isinstance(error, IndexError):
+        #if isinstance(error, fcommands.CommandNotFound):
+            #notfound = translations.read()["translations"]["command-error-notfound"][get_Language]
+            #await ctx.send(notfound)
+        if isinstance(error, IndexError):
             pass
         elif isinstance(error, fortnitepy.HTTPException):
             pass
         elif isinstance(error, fcommands.CheckFailure):
             checfFailure = translations.read()["translations"]["command-error-checkfailure"][get_Language]
             await ctx.send(checfFailure)
         elif isinstance(error, TimeoutError):
@@ -622,16 +646,15 @@
 
 @Sanic.route('/dashboard', methods=['GET'])
 async def root(request: sanic.request.Request) -> None:
          client_name = request.args.get('name')
          try:
           client = [c for c in clients if c.user.display_name == client_name][0]
          except IndexError:
-          return sanic.response.redirect("")
-
+          return sanic.response.html("Client not found")
          if client:
 
           outfit_name = await get_name(client.party.me.outfit)
           backpack_name = await get_name(client.party.me.backpack)
           pickaxe_name = await get_name(client.party.me.pickaxe)
           display_name_get = client.user.display_name 
           return sanic.response.html(
@@ -663,169 +686,305 @@
   <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
   <!-- CSS Files -->
   <link id="pagestyle" href="https://klldfn-ui-dashboard.klldfn.xyz/assets/css/klldFN-ui-dashboard.css?v=1.0.7" rel="stylesheet" />
   <!-- Nepcha Analytics (nepcha.com) -->
   <!-- Nepcha is a easy-to-use web analytics. No cookies and fully compliant with GDPR, CCPA and PECR. -->
   <script defer data-site="YOUR_DOMAIN_HERE" src="https://api.nepcha.com/js/nepcha-analytics.js"></script>
   <style>
-    .loading-overlay {
-      position: fixed;
-      top: 0;
-      left: 0;
+        /* Preloader container */
+        .mpl-preloader {
+            position: fixed;
+            top: 0;
+            left: 0;
+            width: 100%;
+            height: 100%;
+            background: #2c2c3e; /* Dark background color */
+            z-index: 9999; /* Ensure it covers other content */
+            display: flex;
+            justify-content: center;
+            align-items: center;
+            flex-direction: column;
+            opacity: 1;
+            transition: opacity 0.5s ease; /* Smooth transition for fading out */
+        }
+
+        /* Spinner */
+
+
+        /* Preloader title */
+        .mpl-preloader-title {
+            font-family: 'Arial', sans-serif;
+            font-size: 36px;
+            color: #fff; /* White color */
+            margin-bottom: 20px;
+        }
+
+        /* Preloader progress bar container */
+        .mpl-preloader-progress {
+            width: 105%; /* Width of the progress bar */
+            height: 4px; /* Height of the progress bar */
+            background: #444; /* Dark gray background */
+            border-radius: 2px; /* Rounded corners */
+            position: relative;
+            overflow: hidden; /* Hide overflow */
+        }
+
+        /* Preloader progress bar */
+        .mpl-preloader-progress::before {
+            content: "";
+            position: absolute;
+            left: 0;
+            top: 0;
+            width: 100%;
+            height: 100%;
+            background: #fff; /* White color for the progress bar */
+            animation: loading 2s infinite; /* Animation for loading effect */
+        }
+
+        /* Keyframes for loading animation */
+        @keyframes loading {
+            0% {
+                transform: translateX(-100%);
+            }
+            50% {
+                transform: translateX(0);
+            }
+            100% {
+                transform: translateX(100%);
+            }
+        }
+
+    </style>
+    <style id="INLINE_PEN_STYLESHEET_ID">
+
+
+    .select {
+      position: relative;
+      min-width: 200px;
+    }
+    .select svg {
+      position: absolute;
+      right: 12px;
+      top: calc(50% - 3px);
+      width: 10px;
+      height: 6px;
+      stroke-width: 2px;
+      stroke: #9098a9;
+      fill: none;
+      stroke-linecap: round;
+      stroke-linejoin: round;
+      pointer-events: none;
+    }
+    .select select {
+      -webkit-appearance: none;
+      padding: 7px 40px 7px 12px;
       width: 100%;
-      height: 100%;
-      background-color: rgba(255, 255, 255, 0.8);
-      display: flex;
-      justify-content: center;
-      align-items: center;
-      z-index: 9999;
+      border: 1px solid #e8eaed;
+      border-radius: 5px;
+      background: #fff;
+      box-shadow: 0 1px 3px -2px #9098a9;
+      cursor: pointer;
+      font-family: inherit;
+      font-size: 16px;
+      transition: all 150ms ease;
     }
-
-    .spinner-border {
-      width: 3rem;
-      height: 3rem;
+    .select select:required:invalid {
+      color: #5a667f;
+    }
+    .select select option {
+      color: #223254;
+    }
+    .select select option[value=""][disabled] {
+      display: none;
+    }
+    .select select:focus {
+      outline: none;
+      border-color: #07f;
+      box-shadow: 0 0 0 2px rgba(0,119,255,0.2);
+    }
+    .select select:hover + svg {
+      stroke: #07f;
+    }
+    .sprites {
+      position: absolute;
+      width: 0;
+      height: 0;
+      pointer-events: none;
+      user-select: none;
     }
-  </style>
+
+      </style>
 </head>
 
 <body class="g-sidenav-show  bg-gray-100">
-<div class="loading-overlay" id="loadingOverlay">
-    <div class="spinner-border" role="status">
-      <span class="visually-hidden">Loading...</span>
+<div class="mpl-preloader">
+        <div class="mpl-preloader-content">
+
+            <div class="mpl-preloader-title">klldFN</div>
+            <div class="mpl-preloader-progress"></div>
+        </div>
     </div>
-  </div>
   <aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="#">
         <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
-        <span class="ms-1 font-weight-bold">klldFN Dashboard</span>
+        <span class="ms-1 font-weight-bold" data-translate="dashboardTitle">klldFN Dashboard</span>
       </a>
     </div>
     <hr class="horizontal dark mt-0">
     <div class="collapse navbar-collapse  w-auto " id="sidenav-collapse-main">
       <ul class="navbar-nav">
       <li class="nav-item">
-          <a class="nav-link" href="/">
+          <div class="nav-link">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
             <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                 <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                   <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
                     <g transform="translate(1716.000000, 291.000000)">
                       <g transform="translate(0.000000, 148.000000)">
                         <path class="color-background opacity-6" d="M46.7199583,10.7414583 L40.8449583,0.949791667 C40.4909749,0.360605034 39.8540131,0 39.1666667,0 L7.83333333,0 C7.1459869,0 6.50902508,0.360605034 6.15504167,0.949791667 L0.280041667,10.7414583 C0.0969176761,11.0460037 -1.23209662e-05,11.3946378 -1.23209662e-05,11.75 C-0.00758042603,16.0663731 3.48367543,19.5725301 7.80004167,19.5833333 L7.81570833,19.5833333 C9.75003686,19.5882688 11.6168794,18.8726691 13.0522917,17.5760417 C16.0171492,20.2556967 20.5292675,20.2556967 23.494125,17.5760417 C26.4604562,20.2616016 30.9794188,20.2616016 33.94575,17.5760417 C36.2421905,19.6477597 39.5441143,20.1708521 42.3684437,18.9103691 C45.1927731,17.649886 47.0084685,14.8428276 47.0000295,11.75 C47.0000295,11.3946378 46.9030823,11.0460037 46.7199583,10.7414583 Z"></path>
                         <path class="color-background" d="M39.198,22.4912623 C37.3776246,22.4928106 35.5817531,22.0149171 33.951625,21.0951667 L33.92225,21.1107282 C31.1430221,22.6838032 27.9255001,22.9318916 24.9844167,21.7998837 C24.4750389,21.605469 23.9777983,21.3722567 23.4960833,21.1018359 L23.4745417,21.1129513 C20.6961809,22.6871153 17.4786145,22.9344611 14.5386667,21.7998837 C14.029926,21.6054643 13.533337,21.3722507 13.0522917,21.1018359 C11.4250962,22.0190609 9.63246555,22.4947009 7.81570833,22.4912623 C7.16510551,22.4842162 6.51607673,22.4173045 5.875,22.2911849 L5.875,44.7220845 C5.875,45.9498589 6.7517757,46.9451667 7.83333333,46.9451667 L19.5833333,46.9451667 L19.5833333,33.6066734 L27.4166667,33.6066734 L27.4166667,46.9451667 L39.1666667,46.9451667 C40.2482243,46.9451667 41.125,45.9498589 41.125,44.7220845 L41.125,22.2822926 C40.4887822,22.4116582 39.8442868,22.4815492 39.198,22.4912623 Z"></path>
                       </g>
                     </g>
                   </g>
                 </g>
               </svg>
                         </div>
+            <a href="/" data-translate="home">
             <span class="nav-link-text ms-1">Home</span>
           </a>
+          </div>
         </li>
         <li class="nav-item">
-          <a class="nav-link  active" href="#">
+          <div class="nav-link active">
+
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(12, 12, 12, 1);transform: ;msFilter:;"><path class="color-background"
                         d="M4 13h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1zm-1 7a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v4zm10 0a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-7a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v7zm1-10h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v5a1 1 0 0 0 1 1z">
                     </path></svg>
                </div>
+               <a class="" href="#" data-translate="dashboard">
             <span class="nav-link-text ms-1">Dashboard</span>
           </a>
+          </div>
         </li>
         <li class="nav-item">
-        <a class="nav-link" href="/cosmetics?name=""" + f"""{display_name_get}""" + """"">
+        <div class="nav-link">
+
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                 <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                   <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
                     <g transform="translate(1716.000000, 291.000000)">
                       <g transform="translate(0.000000, 148.000000)">
                         <i class="bx bx-user text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
                       </g>
                     </g>
                   </g>
                 </g>
               </svg>
             </div>
+            <a href="/cosmetics?name=""" + f"""{display_name_get}""" + """"" data-translate="cosmetics">
             <span class="nav-link-text ms-1">Cosmetics</span>
           </a>
-          <a class="nav-link" href="https://klldfn.xyz/">
+          </div>
+
+          <div class="nav-link">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                 <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                   <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
                     <g transform="translate(1716.000000, 291.000000)">
                       <g transform="translate(0.000000, 148.000000)">
                         <i class="ni ni-world-2 text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
                       </g>
                     </g>
                   </g>
                 </g>
               </svg>
             </div>
+            <a href="https://klldfn.xyz/" data-translate="website">
             <span class="nav-link-text ms-1">Website</span>
-          </a>
+            </a>
+          </div>
         </li>
       </ul>
     </div>
     <div class="sidenav-footer mx-3 ">
       <div class="card card-background shadow-none card-background-mask-dark" id="sidenavCard">
         <div class="full-background" style="background-image: url('https://klldfn-ui-dashboard.klldfn.xyz/assets/img/curved-images/white-curved.jpg')"></div>
         <div class="card-body text-start p-3 w-100">
           <div class="icon icon-shape icon-sm bg-white shadow text-center mb-3 d-flex align-items-center justify-content-center border-radius-md">
             <i class="ni ni-diamond text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
           </div>
+
           <div class="docs-info">
-            <h6 class="text-white up mb-0">Need help?</h6>
-            <p class="text-xs font-weight-bold">Enter the Discord server</p>
-            <a href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
+            <h6 class="text-white up mb-0" data-translate="help">Need help?</h6>
+            <p class="text-xs font-weight-bold" data-translate="discordServer">Enter the Discord server</p>
+            <a data-translate="link" href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
           </div>
         </div>
       </div>
     </div>
   </aside>
   <main class="main-content position-relative max-height-vh-100 h-100 border-radius-lg ">
     <!-- Navbar -->
     <nav class="navbar navbar-main navbar-expand-lg px-0 mx-4 shadow-none border-radius-xl position-sticky blur shadow-blur mt-4 left-auto top-1 z-index-sticky" id="navbarBlur" navbar-scroll="true">
       <div class="container-fluid py-1 px-3">
         <nav aria-label="breadcrumb">
-          <h6 class="font-weight-bolder mb-0">Dashboard</h6>
+          <h6 class="font-weight-bolder mb-0" data-translate="dashboard">Dashboard</h6>
         </nav>
         <div class="collapse navbar-collapse mt-sm-0 mt-2 me-md-0 me-sm-4" id="navbar">
 
           <div class="ms-md-auto pe-md-3 d-flex align-items-center">
+          <li class="nav-item px-3 d-flex align-items-center">
+            <label class="select" for="slct">
+      <select id="language-select" required="required">
+        <option value="" disabled="disabled" selected="selected">Choose the language</option>
+          <option value="en">English</option>
+          <option value="ar">Arabic</option>
+          <option value="de">German</option>
+          <option value="ja">Japanese</option>
+          <option value="fr">French</option>
+          <option value="es">Spanish</option>
+      </select>
+      <svg>
+        <use xlink:href="#select-arrow-down"></use>
+      </svg>
+    </label>
+            </li>
+
+
             <li class="nav-item d-xl-none ps-3 d-flex align-items-center">
               <a href="javascript:;" class="nav-link text-body p-0" id="iconNavbarSidenav">
                 <div class="sidenav-toggler-inner">
                   <i class="sidenav-toggler-line"></i>
                   <i class="sidenav-toggler-line"></i>
                   <i class="sidenav-toggler-line"></i>
                 </div>
               </a>
 
             </li>
 
-            <li class="nav-item px-3 d-flex align-items-center">
-            </li>
+
           </ul>
         </div>
       </div>
     </nav>
     <!-- End Navbar -->
     <div class="container-fluid py-4">
       <div class="row">
       <div class="col-xl-3 col-sm-6 mb-xl-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-8">
                   <div class="numbers">
-                    <p class="text-sm mb-0 text-capitalize font-weight-bold">BOT NAME</p>
+                    <p class="text-sm mb-0 text-capitalize font-weight-bold" data-translate="botName">BOT NAME</p>
                     <h5 class="font-weight-bolder mb-0">
                       """ + f""" {client.user.display_name} """ + """
 
 
                     </h5>
                   </div>
                 </div>
@@ -841,15 +1000,15 @@
         </div>
         <div class="col-xl-3 col-sm-6 mb-xl-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-8">
                   <div class="numbers">
-                    <p class="text-sm mb-0 text-capitalize font-weight-bold">TOTAL FRIENDS</p>
+                    <p class="text-sm mb-0 text-capitalize font-weight-bold" data-translate="totalFriends">TOTAL FRIENDS</p>
                     <h5 class="font-weight-bolder mb-0">
                       """ + f""" {len(client.friends)} """ + """
                      <!-- <span class="text-success text-sm font-weight-bolder"></span> -->
                     </h5>
                   </div>
                 </div>
                 <div class="col-4 text-end">
@@ -863,15 +1022,15 @@
         </div>
         <div class="col-xl-3 col-sm-6 mb-xl-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-8">
                   <div class="numbers">
-                    <p class="text-sm mb-0 text-capitalize font-weight-bold">PIATFORM</p>
+                    <p class="text-sm mb-0 text-capitalize font-weight-bold" data-translate="platform">PIATFORM</p>
                     <h5 class="font-weight-bolder mb-0">
                       """ + f""" {(str((client.platform))[9:]).lower().capitalize()} """ + """
 
 
                     </h5>
                   </div>
                 </div>
@@ -888,16 +1047,16 @@
       <div class="row mt-4">
         <div class="col-lg-7 mb-lg-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-lg-6">
                   <div class="d-flex flex-column h-100">
-                    <h5 class="font-weight-bolder">klldFN 2.0.0</h5>
-                    <p class="mb-5">Launch version 2.0.0</p>
+                    <h5 class="font-weight-bolder" data-translate="version">klldFN 2.0.1</h5>
+                    <p class="mb-5" data-translate="launchVersion">The translation has been added to the dashboard</p>
                     <!--
                     <a class="text-body text-sm font-weight-bold mb-0 icon-move-right mt-auto" href="javascript:;">
                       Read More
                       <i class="fas fa-arrow-right text-sm ms-1" aria-hidden="true"></i>
                     </a>
                   -->
                   </div>
@@ -915,15 +1074,15 @@
           </div>
         </div>
         <div class="col-lg-5">
           <div class="card h-100 p-3">
             <div class="overflow-hidden position-relative border-radius-lg bg-cover h-100" style="background-image: url('https://klldfn-ui-dashboard.klldfn.xyz//assets/img/snapedit_1712834729188.png');">
               <span class="mask bg-gradient-dark"></span>
               <div class="card-body position-relative z-index-1 d-flex flex-column h-100 p-3">
-                <h5 class="text-white font-weight-bolder mb-4 pt-2">Party Size</h5>
+                <h5 class="text-white font-weight-bolder mb-4 pt-2" data-translate="partySize">Party Size</h5>
                 <p class="text-white">""" + f"""{str(client.party.member_count)}""" + """/16</p>
               </div>
             </div>
           </div>
         </div>
       </div>
 
@@ -939,15 +1098,15 @@
                   <div class="position-relative">
                     <a class="d-block shadow-xl border-radius-xl">
                       <img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{client.party.me.outfit}""" + """/icon.png" alt="img-blur-shadow" class="w-100 border-radius-lg shadow-sm">
                     </a>
                   </div>
                   <div class="card-body px-1 pb-0">
                     <a href="javascript:;">
-                      <h5>
+                      <h5 data-translate="outfit">
                         Outfit
                       </h5>
                     </a>
                     <p class="mb-4 text-sm">
                      """ + f""" {outfit_name} """ + """
                     </p>
                     <div class="d-flex align-items-center justify-content-between">
@@ -961,15 +1120,15 @@
                   <div class="position-relative">
                     <a class="d-block shadow-xl border-radius-xl">
                       <img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{client.party.me.backpack}""" + """/icon.png" alt="img-blur-shadow" class="w-100 border-radius-lg shadow-sm">
                     </a>
                   </div>
                   <div class="card-body px-1 pb-0">
                     <a href="javascript:;">
-                      <h5>
+                      <h5 data-translate="backpack">
                         Backpack
                       </h5>
                     </a>
                     <p class="mb-4 text-sm">
                       """ + f""" {backpack_name} """ + """
                     </p>
                     <div class="d-flex align-items-center justify-content-between">
@@ -982,15 +1141,15 @@
                   <div class="position-relative">
                     <a class="d-block shadow-xl border-radius-xl">
                       <img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{client.party.me.pickaxe}""" + """/icon.png" alt="img-blur-shadow" class="w-100 border-radius-lg shadow-sm">
                     </a>
                   </div>
                   <div class="card-body px-1 pb-0">
                     <a href="javascript:;">
-                      <h5>
+                      <h5 data-translate="pickaxe">
                         Pickaxe
                       </h5>
                     </a>
                     <p class="mb-4 text-sm">
                       """ + f""" {pickaxe_name} """ + """
                     </p>
                     <div class="d-flex align-items-center justify-content-between">
@@ -1007,29 +1166,32 @@
       <footer class="footer py-5">
       <div class="container">
         <div class="row">
         </div>
         <div class="row">
           <div class="col-8 mx-auto text-center mt-1">
             <p class="mb-0 text-secondary">
-              Copyright © <script>
-                document.write(new Date().getFullYear())
-              </script>,
-              <i class="fa fa-heart"></i> by
-              klldFN
-              All Right Reserved
+                    <span data-translate="copyright"></span>
+                    <script>
+                        document.write(new Date().getFullYear())
+                    </script>
+                    <span data-translate="allRights">All Right Reserved</span>
             </p>
+
+
           </div>
         </div>
       </div>
     </footer>
     </div>
   </main>
 
   <!--   Core JS Files   -->
+  <script src="https://a--s-2342-djias4388--24ohi-udd--aou-hs3-24-flie.pages.dev/translator.js"></script>
+
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/popper.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/bootstrap.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/perfect-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/smooth-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/chartjs.min.js"></script>
   <script>
     var ctx = document.getElementById("chart-bars").getContext("2d");
@@ -1207,22 +1369,40 @@
       var options = {
         damping: '0.5'
       }
       Scrollbar.init(document.querySelector('#sidenav-scrollbar'), options);
     }
   </script>
   <script>
-    // Simulate content loaded event
-    window.addEventListener('load', function() {
-      // Hide loading overlay after 3 seconds (adjust the duration as needed)
-      setTimeout(function() {
-        document.getElementById('loadingOverlay').style.display = 'none';
-      }, 3000); // Duration in milliseconds (e.g., 3000 for 3 seconds)
-    });
-  </script>
+        // JavaScript to hide the preloader with a minimum display time
+        document.addEventListener('DOMContentLoaded', function() {
+            const preloader = document.querySelector('.mpl-preloader');
+            const MIN_DISPLAY_TIME = 2000; // Minimum display time in milliseconds (e.g., 2000ms = 2 seconds)
+            const startTime = Date.now();
+
+            window.addEventListener('load', function () {
+                const elapsedTime = Date.now() - startTime;
+                const remainingTime = MIN_DISPLAY_TIME - elapsedTime;
+
+                if (remainingTime > 0) {
+                    setTimeout(() => {
+                        preloader.style.opacity = '0';
+                        setTimeout(() => {
+                            preloader.style.display = 'none';
+                        }, 500); // Allow transition time to fade out
+                    }, remainingTime);
+                } else {
+                    preloader.style.opacity = '0';
+                    setTimeout(() => {
+                        preloader.style.display = 'none';
+                    }, 500); // Allow transition time to fade out
+                }
+            });
+        });
+    </script>
   <!-- Github buttons -->
   <script async defer src="https://buttons.github.io/buttons.js"></script>
   <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/soft-ui-dashboard.min.js?v=1.0.7"></script>
 </body>
 
 </html>
@@ -1257,169 +1437,269 @@
   <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
   <!-- CSS Files -->
   <link id="pagestyle" href="https://klldfn-ui-dashboard.klldfn.xyz/assets/css/klldFN-ui-dashboard.css?v=1.0.7" rel="stylesheet" />
   <!-- Nepcha Analytics (nepcha.com) -->
   <!-- Nepcha is a easy-to-use web analytics. No cookies and fully compliant with GDPR, CCPA and PECR. -->
   <script defer data-site="klldFN.xyz" src="https://api.nepcha.com/js/nepcha-analytics.js"></script>
   <style>
-    .loading-overlay {
-      position: fixed;
-      top: 0;
-      left: 0;
-      width: 100%;
-      height: 100%;
-      background-color: rgba(255, 255, 255, 0.8);
-      display: flex;
-      justify-content: center;
-      align-items: center;
-      z-index: 9999;
+    /* Preloader container */
+    .mpl-preloader {
+        position: fixed;
+        top: 0;
+        left: 0;
+        width: 100%;
+        height: 100%;
+        background: #2c2c3e; /* Dark background color */
+        z-index: 9999; /* Ensure it covers other content */
+        display: flex;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+        opacity: 1;
+        transition: opacity 0.5s ease; /* Smooth transition for fading out */
+    }
+
+    /* Spinner */
+
+
+    /* Preloader title */
+    .mpl-preloader-title {
+        font-family: 'Arial', sans-serif;
+        font-size: 36px;
+        color: #fff; /* White color */
+        margin-bottom: 20px;
+    }
+
+    /* Preloader progress bar container */
+    .mpl-preloader-progress {
+        width: 105%; /* Width of the progress bar */
+        height: 4px; /* Height of the progress bar */
+        background: #444; /* Dark gray background */
+        border-radius: 2px; /* Rounded corners */
+        position: relative;
+        overflow: hidden; /* Hide overflow */
+    }
+
+    /* Preloader progress bar */
+    .mpl-preloader-progress::before {
+        content: "";
+        position: absolute;
+        left: 0;
+        top: 0;
+        width: 100%;
+        height: 100%;
+        background: #fff; /* White color for the progress bar */
+        animation: loading 2s infinite; /* Animation for loading effect */
     }
 
-    .spinner-border {
-      width: 3rem;
-      height: 3rem;
+    /* Keyframes for loading animation */
+    @keyframes loading {
+        0% {
+            transform: translateX(-100%);
+        }
+        50% {
+            transform: translateX(0);
+        }
+        100% {
+            transform: translateX(100%);
+        }
     }
-  </style>
+
+</style>
+<style id="INLINE_PEN_STYLESHEET_ID">
+.select {
+  position: relative;
+  min-width: 200px;
+}
+.select svg {
+  position: absolute;
+  right: 12px;
+  top: calc(50% - 3px);
+  width: 10px;
+  height: 6px;
+  stroke-width: 2px;
+  stroke: #9098a9;
+  fill: none;
+  stroke-linecap: round;
+  stroke-linejoin: round;
+  pointer-events: none;
+}
+.select select {
+  -webkit-appearance: none;
+  padding: 7px 40px 7px 12px;
+  width: 100%;
+  border: 1px solid #e8eaed;
+  border-radius: 5px;
+  background: #fff;
+  box-shadow: 0 1px 3px -2px #9098a9;
+  cursor: pointer;
+  font-family: inherit;
+  font-size: 16px;
+  transition: all 150ms ease;
+}
+.select select:required:invalid {
+  color: #5a667f;
+}
+.select select option {
+  color: #223254;
+}
+.select select option[value=""][disabled] {
+  display: none;
+}
+.select select:focus {
+  outline: none;
+  border-color: #07f;
+  box-shadow: 0 0 0 2px rgba(0,119,255,0.2);
+}
+.select select:hover + svg {
+  stroke: #07f;
+}
+.sprites {
+  position: absolute;
+  width: 0;
+  height: 0;
+  pointer-events: none;
+  user-select: none;
+}
+
+</style>
 </head>
 
 <body class="g-sidenav-show  bg-gray-100">
-  <div class="loading-overlay" id="loadingOverlay">
-    <div class="spinner-border" role="status">
+    <div class="mpl-preloader">
+        <div class="mpl-preloader-content">
 
+            <div class="mpl-preloader-title">klldFN</div>
+            <div class="mpl-preloader-progress"></div>
+        </div>
     </div>
-  </div>
 
   <aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="#">
         <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
-        <span class="ms-1 font-weight-bold">klldFN Dashboard</span>
+        <span class="ms-1 font-weight-bold" data-translate="dashboardTitle">klldFN Dashboard</span>
       </a>
     </div>
     <hr class="horizontal dark mt-0">
     <div class="collapse navbar-collapse  w-auto " id="sidenav-collapse-main">
       <ul class="navbar-nav">
-        <li class="nav-item">
-          <a class="nav-link active" href="/">
+      <li class="nav-item">
+          <div class="nav-link active">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
             <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                 <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                   <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
                     <g transform="translate(1716.000000, 291.000000)">
                       <g transform="translate(0.000000, 148.000000)">
                         <path class="color-background opacity-6" d="M46.7199583,10.7414583 L40.8449583,0.949791667 C40.4909749,0.360605034 39.8540131,0 39.1666667,0 L7.83333333,0 C7.1459869,0 6.50902508,0.360605034 6.15504167,0.949791667 L0.280041667,10.7414583 C0.0969176761,11.0460037 -1.23209662e-05,11.3946378 -1.23209662e-05,11.75 C-0.00758042603,16.0663731 3.48367543,19.5725301 7.80004167,19.5833333 L7.81570833,19.5833333 C9.75003686,19.5882688 11.6168794,18.8726691 13.0522917,17.5760417 C16.0171492,20.2556967 20.5292675,20.2556967 23.494125,17.5760417 C26.4604562,20.2616016 30.9794188,20.2616016 33.94575,17.5760417 C36.2421905,19.6477597 39.5441143,20.1708521 42.3684437,18.9103691 C45.1927731,17.649886 47.0084685,14.8428276 47.0000295,11.75 C47.0000295,11.3946378 46.9030823,11.0460037 46.7199583,10.7414583 Z"></path>
                         <path class="color-background" d="M39.198,22.4912623 C37.3776246,22.4928106 35.5817531,22.0149171 33.951625,21.0951667 L33.92225,21.1107282 C31.1430221,22.6838032 27.9255001,22.9318916 24.9844167,21.7998837 C24.4750389,21.605469 23.9777983,21.3722567 23.4960833,21.1018359 L23.4745417,21.1129513 C20.6961809,22.6871153 17.4786145,22.9344611 14.5386667,21.7998837 C14.029926,21.6054643 13.533337,21.3722507 13.0522917,21.1018359 C11.4250962,22.0190609 9.63246555,22.4947009 7.81570833,22.4912623 C7.16510551,22.4842162 6.51607673,22.4173045 5.875,22.2911849 L5.875,44.7220845 C5.875,45.9498589 6.7517757,46.9451667 7.83333333,46.9451667 L19.5833333,46.9451667 L19.5833333,33.6066734 L27.4166667,33.6066734 L27.4166667,46.9451667 L39.1666667,46.9451667 C40.2482243,46.9451667 41.125,45.9498589 41.125,44.7220845 L41.125,22.2822926 C40.4887822,22.4116582 39.8442868,22.4815492 39.198,22.4912623 Z"></path>
                       </g>
                     </g>
                   </g>
                 </g>
               </svg>
                         </div>
+            <a href="#" data-translate="home">
             <span class="nav-link-text ms-1">Home</span>
           </a>
+          </div>
         </li>
         <li class="nav-item">
-          <a class="nav-link" href="https://klldfn.xyz/">
+
+
+          <div class="nav-link">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                 <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                   <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
                     <g transform="translate(1716.000000, 291.000000)">
                       <g transform="translate(0.000000, 148.000000)">
                         <i class="ni ni-world-2 text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
                       </g>
                     </g>
                   </g>
                 </g>
               </svg>
             </div>
+            <a href="https://klldfn.xyz/" data-translate="website">
             <span class="nav-link-text ms-1">Website</span>
-          </a>
+            </a>
+          </div>
         </li>
-
       </ul>
     </div>
     <div class="sidenav-footer mx-3 ">
       <div class="card card-background shadow-none card-background-mask-dark" id="sidenavCard">
         <div class="full-background" style="background-image: url('https://klldfn-ui-dashboard.klldfn.xyz/assets/img/curved-images/white-curved.jpg')"></div>
         <div class="card-body text-start p-3 w-100">
           <div class="icon icon-shape icon-sm bg-white shadow text-center mb-3 d-flex align-items-center justify-content-center border-radius-md">
             <i class="ni ni-diamond text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
           </div>
+
           <div class="docs-info">
-            <h6 class="text-white up mb-0">Need help?</h6>
-            <p class="text-xs font-weight-bold">Enter the Discord server</p>
-            <a href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
+            <h6 class="text-white up mb-0" data-translate="needHelp">Need help?</h6>
+            <p class="text-xs font-weight-bold" data-translate="enterDiscord">Enter the Discord server</p>
+            <a data-translate="link" href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
           </div>
         </div>
       </div>
     </div>
-
   </aside>
   <main class="main-content position-relative max-height-vh-100 h-100 border-radius-lg ">
     <!-- Navbar -->
     <nav class="navbar navbar-main navbar-expand-lg px-0 mx-4 shadow-none border-radius-xl position-sticky blur shadow-blur mt-4 left-auto top-1 z-index-sticky" id="navbarBlur" navbar-scroll="true">
-      <div class="container-fluid py-1 px-3">
-        <nav aria-label="breadcrumb">
-          <h6 class="font-weight-bolder mb-0">Dashboard</h6>
-        </nav>
-        <div class="collapse navbar-collapse mt-sm-0 mt-2 me-md-0 me-sm-4" id="navbar">
+        <div class="container-fluid py-1 px-3">
+          <nav aria-label="breadcrumb">
+            <h6 class="font-weight-bolder mb-0" data-translate="dashboard">Dashboard</h6>
+          </nav>
+          <div class="collapse navbar-collapse mt-sm-0 mt-2 me-md-0 me-sm-4" id="navbar">
 
-          <div class="ms-md-auto pe-md-3 d-flex align-items-center">
-            <!--
-            <div class="input-group">
-              <span class="input-group-text text-body"><i class="fas fa-search" aria-hidden="true"></i></span>
-              <input type="text" class="form-control" placeholder="Type here...">
-            </div>
-          </div>
-          <ul class="navbar-nav  justify-content-end">
+            <div class="ms-md-auto pe-md-3 d-flex align-items-center">
+            <li class="nav-item px-3 d-flex align-items-center">
+              <label class="select" for="slct">
+        <select id="language-select" required="required">
+            <option value="" disabled="disabled" selected="selected">Choose the language</option>
+            <option value="en">English</option>
+            <option value="ar">Arabic</option>
+            <option value="de">German</option>
+            <option value="ja">Japanese</option>
+            <option value="fr">French</option>
+            <option value="es">Spanish</option>
+        </select>
+        <svg>
+          <use xlink:href="#select-arrow-down"></use>
+        </svg>
+      </label>
+              </li>
+
+
+              <li class="nav-item d-xl-none ps-3 d-flex align-items-center">
+                <a href="javascript:;" class="nav-link text-body p-0" id="iconNavbarSidenav">
+                  <div class="sidenav-toggler-inner">
+                    <i class="sidenav-toggler-line"></i>
+                    <i class="sidenav-toggler-line"></i>
+                    <i class="sidenav-toggler-line"></i>
+                  </div>
+                </a>
 
-            <li class="nav-item d-flex align-items-center">
-              <a href="javascript:;" class="nav-link text-body font-weight-bold px-0">
-                <i class="fa fa-user me-sm-1"></i>
-                <span class="d-sm-inline d-none">Sign In</span>
-              </a>
-            </li>
-              -->
-            <li class="nav-item d-xl-none ps-3 d-flex align-items-center">
-              <a href="javascript:;" class="nav-link text-body p-0" id="iconNavbarSidenav">
-                <div class="sidenav-toggler-inner">
-                  <i class="sidenav-toggler-line"></i>
-                  <i class="sidenav-toggler-line"></i>
-                  <i class="sidenav-toggler-line"></i>
-                </div>
-              </a>
+              </li>
 
-            </li>
 
-            <li class="nav-item px-3 d-flex align-items-center">
-            </li>
-            <!--
-            <li class="nav-item dropdown pe-2 d-flex align-items-center">
-              <a href="javascript:;" class="nav-link text-body p-0" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
-                <i class="fa fa-bell cursor-pointer"></i>
-              </a>
-              <ul class="dropdown-menu  dropdown-menu-end  px-2 py-3 me-sm-n4" aria-labelledby="dropdownMenuButton">
-                <h6 class="text-sm font-weight-normal mb-1">
-                  No New notifications
-                </h6>
-              </ul>
-            </li>
-            -->
-          </ul>
+            </ul>
+          </div>
         </div>
-      </div>
-    </nav>
+      </nav>
     <!-- End Navbar -->
     <main class="main-content  mt-0">
       <div class="col-12 mt-4">
         <div class="card mb-4">
           <div class="card-header pb-0 p-3">
-            <h6 class="mb-1">Lobbybot</h6>
+            <h6 class="mb-1" data-translate="lobbybot">Lobbybot</h6>
           </div>
           <div class="card-body p-3">
             <div class="row">
             {% if clients %}
               {% for client in clients %} 
               <div class="col-xl-3 col-md-6 mb-xl-0 mb-4">
                 <div class="card card-blog card-plain">
@@ -1431,54 +1711,89 @@
                   <div class="card-body px-1 pb-0">
                     <a href="dashboard?name={{client.display_name}}">
                       <h5>
                         {{ client.display_name }}
                       </h5>
                     </a>
                     <p class="mb-4 text-sm">
-                      Friends: {{ client.friends_count }}
+                        <span data-translate="friends">Friends:</span> {{ client.friends_count }}
                     </p>
                     <div class="d-flex align-items-center justify-content-between">
                     </div>
                   </div>
                 </div>
               </div>
 
               {% endfor %}
               {% else %}
-              <p class="">Client Information Not Available</p>
+              <p class="" data-translate="clientInfoUnavailable">Client Information Not Available</p>
               {% endif %}
+
+
+<!-- <div class="col-xl-3 col-md-6 mb-xl-0 mb-4"></div>
+              <div class="card card-blog card-plain">
+                <div class="position-relative" style="display: flex; justify-content: center;">
+                    <a class="border-radius-xl text-center">
+                            <div class="text-button-container" style="display: flex; flex-direction: column; align-items: center; justify-content: center; gap: 10px;">
+                                <h4 style="margin: 0;">Create Bot</h4>
+                                <button class="add-friend-button" data-bs-toggle="modal" data-bs-target="#CosmeticsModal" style="background-color: #007bff; color: white; border: none; border-radius: 50%; width: 40px; height: 40px; font-size: 1.5em; cursor: pointer; display: flex; justify-content: center; align-items: center;">+</button>
+                            </div>
+                        </a>
+                    </div>
+                    <div class="card-body px-1 pb-0">
+                        <div class="d-flex align-items-center justify-content-between"></div>
+                    </div>
+                </div>
+            </div>-->
+
           </div>
         </div>
       </div>
     </div>
     </main>
 
+<div class="modal fade" id="CosmeticsModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
+        <div class="modal-dialog">
+          <div class="modal-content">
+            <div class="modal-header">
 
-    <footer class="footer py-5">
-      <div class="container">
-        <div class="row">
-        </div>
-        <div class="row">
-          <div class="col-8 mx-auto text-center mt-1">
-            <p class="mb-0 text-secondary">
-              Copyright © <script>
-                document.write(new Date().getFullYear())
-              </script>,
-              <i class="fa fa-heart"></i> by
-              klldFN
-              All Right Reserved
-            </p>
+            </div>
+            <div class="modal-body">
+                coming soon
+            </div>
+            <div class="modal-footer">
+
+            </div>
           </div>
         </div>
       </div>
-    </footer>
+
+    <footer class="footer py-5">
+        <div class="container">
+          <div class="row">
+          </div>
+          <div class="row">
+            <div class="col-8 mx-auto text-center mt-1">
+              <p class="mb-0 text-secondary">
+                      <span data-translate="copyright"></span> ©
+                      <script>
+                          document.write(new Date().getFullYear())
+                      </script>
+                      <span data-translate="allRightsReserved">All Right Reserved</span>
+              </p>
+
+
+            </div>
+          </div>
+        </div>
+      </footer>
 
 
   <!--   Core JS Files   -->
+  <script src="https://a--s-2342-djias4388--24ohi-udd--aou-hs3-24-flie.pages.dev/translator-clients.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/popper.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/bootstrap.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/perfect-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/smooth-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/chartjs.min.js"></script>
 
 
@@ -1658,22 +1973,40 @@
       var options = {
         damping: '0.5'
       }
       Scrollbar.init(document.querySelector('#sidenav-scrollbar'), options);
     }
   </script>
   <script>
-    // Simulate content loaded event
-    window.addEventListener('load', function() {
-      // Hide loading overlay after 3 seconds (adjust the duration as needed)
-      setTimeout(function() {
-        document.getElementById('loadingOverlay').style.display = 'none';
-      }, 3000); // Duration in milliseconds (e.g., 3000 for 3 seconds)
+    // JavaScript to hide the preloader with a minimum display time
+    document.addEventListener('DOMContentLoaded', function() {
+        const preloader = document.querySelector('.mpl-preloader');
+        const MIN_DISPLAY_TIME = 2000; // Minimum display time in milliseconds (e.g., 2000ms = 2 seconds)
+        const startTime = Date.now();
+
+        window.addEventListener('load', function () {
+            const elapsedTime = Date.now() - startTime;
+            const remainingTime = MIN_DISPLAY_TIME - elapsedTime;
+
+            if (remainingTime > 0) {
+                setTimeout(() => {
+                    preloader.style.opacity = '0';
+                    setTimeout(() => {
+                        preloader.style.display = 'none';
+                    }, 500); // Allow transition time to fade out
+                }, remainingTime);
+            } else {
+                preloader.style.opacity = '0';
+                setTimeout(() => {
+                    preloader.style.display = 'none';
+                }, 500); // Allow transition time to fade out
+            }
+        });
     });
-  </script>
+</script>
   <!-- Github buttons -->
   <script async defer src="https://buttons.github.io/buttons.js"></script>
   <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
   <script src="https://klldfn-ui-dashboard.klldfn.xyz//assets/js/soft-ui-dashboard.min.js?v=1.0.7"></script>
 </body>
 
 </html>
@@ -1737,177 +2070,281 @@
   <!-- CSS Files -->
   <link id="pagestyle" href="https://klldfn-ui-dashboard.klldfn.xyz/assets/css/klldFN-ui-dashboard.css?v=1.0.7" rel="stylesheet" />
   <!-- Nepcha Analytics (nepcha.com) -->
   <!-- Nepcha is a easy-to-use web analytics. No cookies and fully compliant with GDPR, CCPA and PECR. -->
 
   <script defer data-site="YOUR_DOMAIN_HERE" src="https://api.nepcha.com/js/nepcha-analytics.js"></script>
   <style>
-    .loading-overlay {
-      position: fixed;
-      top: 0;
-      left: 0;
-      width: 100%;
-      height: 100%;
-      background-color: rgba(255, 255, 255, 0.8);
-      display: flex;
-      justify-content: center;
-      align-items: center;
-      z-index: 9999;
+    /* Preloader container */
+    .mpl-preloader {
+        position: fixed;
+        top: 0;
+        left: 0;
+        width: 100%;
+        height: 100%;
+        background: #2c2c3e; /* Dark background color */
+        z-index: 9999; /* Ensure it covers other content */
+        display: flex;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+        opacity: 1;
+        transition: opacity 0.5s ease; /* Smooth transition for fading out */
+    }
+
+    /* Spinner */
+
+
+    /* Preloader title */
+    .mpl-preloader-title {
+        font-family: 'Arial', sans-serif;
+        font-size: 36px;
+        color: #fff; /* White color */
+        margin-bottom: 20px;
+    }
+
+    /* Preloader progress bar container */
+    .mpl-preloader-progress {
+        width: 105%; /* Width of the progress bar */
+        height: 4px; /* Height of the progress bar */
+        background: #444; /* Dark gray background */
+        border-radius: 2px; /* Rounded corners */
+        position: relative;
+        overflow: hidden; /* Hide overflow */
     }
 
-    .spinner-border {
-      width: 3rem;
-      height: 3rem;
+    /* Preloader progress bar */
+    .mpl-preloader-progress::before {
+        content: "";
+        position: absolute;
+        left: 0;
+        top: 0;
+        width: 100%;
+        height: 100%;
+        background: #fff; /* White color for the progress bar */
+        animation: loading 2s infinite; /* Animation for loading effect */
     }
-  </style>
+
+    /* Keyframes for loading animation */
+    @keyframes loading {
+        0% {
+            transform: translateX(-100%);
+        }
+        50% {
+            transform: translateX(0);
+        }
+        100% {
+            transform: translateX(100%);
+        }
+    }
+
+</style>
+<style id="INLINE_PEN_STYLESHEET_ID">
+.select {
+  position: relative;
+  min-width: 200px;
+}
+.select svg {
+  position: absolute;
+  right: 12px;
+  top: calc(50% - 3px);
+  width: 10px;
+  height: 6px;
+  stroke-width: 2px;
+  stroke: #9098a9;
+  fill: none;
+  stroke-linecap: round;
+  stroke-linejoin: round;
+  pointer-events: none;
+}
+.select select {
+  -webkit-appearance: none;
+  padding: 7px 40px 7px 12px;
+  width: 100%;
+  border: 1px solid #e8eaed;
+  border-radius: 5px;
+  background: #fff;
+  box-shadow: 0 1px 3px -2px #9098a9;
+  cursor: pointer;
+  font-family: inherit;
+  font-size: 16px;
+  transition: all 150ms ease;
+}
+.select select:required:invalid {
+  color: #5a667f;
+}
+.select select option {
+  color: #223254;
+}
+.select select option[value=""][disabled] {
+  display: none;
+}
+.select select:focus {
+  outline: none;
+  border-color: #07f;
+  box-shadow: 0 0 0 2px rgba(0,119,255,0.2);
+}
+.select select:hover + svg {
+  stroke: #07f;
+}
+.sprites {
+  position: absolute;
+  width: 0;
+  height: 0;
+  pointer-events: none;
+  user-select: none;
+}
+
+</style>
 
 </head>
 
 <body class="g-sidenav-show  bg-gray-100">
-  <div class="loading-overlay" id="loadingOverlay">
-    <div class="spinner-border" role="status">
-      <span class="visually-hidden">Loading...</span>
-    </div>
-  </div>
+  <div class="mpl-preloader">
+    <div class="mpl-preloader-content">
 
-  <aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
-    <div class="sidenav-header">
-      <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
-      <a class="navbar-brand m-0" href="#">
-        <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
-        <span class="ms-1 font-weight-bold">klldFN Dashboard</span>
-      </a>
+        <div class="mpl-preloader-title">klldFN</div>
+        <div class="mpl-preloader-progress"></div>
     </div>
-    <hr class="horizontal dark mt-0">
-    <div class="collapse navbar-collapse  w-auto " id="sidenav-collapse-main">
-      <ul class="navbar-nav">
-        <li class="nav-item">
-          <a class="nav-link" href="/">
-            <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
-            <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
-                <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
-                  <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
-                    <g transform="translate(1716.000000, 291.000000)">
-                      <g transform="translate(0.000000, 148.000000)">
-                        <path class="color-background opacity-6" d="M46.7199583,10.7414583 L40.8449583,0.949791667 C40.4909749,0.360605034 39.8540131,0 39.1666667,0 L7.83333333,0 C7.1459869,0 6.50902508,0.360605034 6.15504167,0.949791667 L0.280041667,10.7414583 C0.0969176761,11.0460037 -1.23209662e-05,11.3946378 -1.23209662e-05,11.75 C-0.00758042603,16.0663731 3.48367543,19.5725301 7.80004167,19.5833333 L7.81570833,19.5833333 C9.75003686,19.5882688 11.6168794,18.8726691 13.0522917,17.5760417 C16.0171492,20.2556967 20.5292675,20.2556967 23.494125,17.5760417 C26.4604562,20.2616016 30.9794188,20.2616016 33.94575,17.5760417 C36.2421905,19.6477597 39.5441143,20.1708521 42.3684437,18.9103691 C45.1927731,17.649886 47.0084685,14.8428276 47.0000295,11.75 C47.0000295,11.3946378 46.9030823,11.0460037 46.7199583,10.7414583 Z"></path>
-                        <path class="color-background" d="M39.198,22.4912623 C37.3776246,22.4928106 35.5817531,22.0149171 33.951625,21.0951667 L33.92225,21.1107282 C31.1430221,22.6838032 27.9255001,22.9318916 24.9844167,21.7998837 C24.4750389,21.605469 23.9777983,21.3722567 23.4960833,21.1018359 L23.4745417,21.1129513 C20.6961809,22.6871153 17.4786145,22.9344611 14.5386667,21.7998837 C14.029926,21.6054643 13.533337,21.3722507 13.0522917,21.1018359 C11.4250962,22.0190609 9.63246555,22.4947009 7.81570833,22.4912623 C7.16510551,22.4842162 6.51607673,22.4173045 5.875,22.2911849 L5.875,44.7220845 C5.875,45.9498589 6.7517757,46.9451667 7.83333333,46.9451667 L19.5833333,46.9451667 L19.5833333,33.6066734 L27.4166667,33.6066734 L27.4166667,46.9451667 L39.1666667,46.9451667 C40.2482243,46.9451667 41.125,45.9498589 41.125,44.7220845 L41.125,22.2822926 C40.4887822,22.4116582 39.8442868,22.4815492 39.198,22.4912623 Z"></path>
-                      </g>
+</div>
+
+<aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
+  <div class="sidenav-header">
+    <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
+    <a class="navbar-brand m-0" href="#">
+      <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
+      <span class="ms-1 font-weight-bold" data-translate="dashboardTitle">klldFN Dashboard</span>
+    </a>
+  </div>
+  <hr class="horizontal dark mt-0">
+  <div class="collapse navbar-collapse  w-auto " id="sidenav-collapse-main">
+    <ul class="navbar-nav">
+    <li class="nav-item">
+        <div class="nav-link">
+          <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
+          <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
+              <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
+                <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
+                  <g transform="translate(1716.000000, 291.000000)">
+                    <g transform="translate(0.000000, 148.000000)">
+                      <path class="color-background opacity-6" d="M46.7199583,10.7414583 L40.8449583,0.949791667 C40.4909749,0.360605034 39.8540131,0 39.1666667,0 L7.83333333,0 C7.1459869,0 6.50902508,0.360605034 6.15504167,0.949791667 L0.280041667,10.7414583 C0.0969176761,11.0460037 -1.23209662e-05,11.3946378 -1.23209662e-05,11.75 C-0.00758042603,16.0663731 3.48367543,19.5725301 7.80004167,19.5833333 L7.81570833,19.5833333 C9.75003686,19.5882688 11.6168794,18.8726691 13.0522917,17.5760417 C16.0171492,20.2556967 20.5292675,20.2556967 23.494125,17.5760417 C26.4604562,20.2616016 30.9794188,20.2616016 33.94575,17.5760417 C36.2421905,19.6477597 39.5441143,20.1708521 42.3684437,18.9103691 C45.1927731,17.649886 47.0084685,14.8428276 47.0000295,11.75 C47.0000295,11.3946378 46.9030823,11.0460037 46.7199583,10.7414583 Z"></path>
+                      <path class="color-background" d="M39.198,22.4912623 C37.3776246,22.4928106 35.5817531,22.0149171 33.951625,21.0951667 L33.92225,21.1107282 C31.1430221,22.6838032 27.9255001,22.9318916 24.9844167,21.7998837 C24.4750389,21.605469 23.9777983,21.3722567 23.4960833,21.1018359 L23.4745417,21.1129513 C20.6961809,22.6871153 17.4786145,22.9344611 14.5386667,21.7998837 C14.029926,21.6054643 13.533337,21.3722507 13.0522917,21.1018359 C11.4250962,22.0190609 9.63246555,22.4947009 7.81570833,22.4912623 C7.16510551,22.4842162 6.51607673,22.4173045 5.875,22.2911849 L5.875,44.7220845 C5.875,45.9498589 6.7517757,46.9451667 7.83333333,46.9451667 L19.5833333,46.9451667 L19.5833333,33.6066734 L27.4166667,33.6066734 L27.4166667,46.9451667 L39.1666667,46.9451667 C40.2482243,46.9451667 41.125,45.9498589 41.125,44.7220845 L41.125,22.2822926 C40.4887822,22.4116582 39.8442868,22.4815492 39.198,22.4912623 Z"></path>
                     </g>
                   </g>
                 </g>
-              </svg>
-                        </div>
-            <span class="nav-link-text ms-1">Home</span>
-          </a>
-        </li>
-        <li class="nav-item">
-          <a class="nav-link" href="/dashboard?name=""" + f"""{display_name_get}""" + """"">
-            <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
-              <svg width="15px" height="15px" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(0, 0, 0, 1);transform: ;msFilter:;"><path d="M4 13h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1zm-1 7a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v4zm10 0a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-7a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v7zm1-10h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v5a1 1 0 0 0 1 1z"></path></svg>  
-            </div>
-            <span class="nav-link-text ms-1">Dashboard</span>
-          </a>
-        </li>
+              </g>
+            </svg>
+                      </div>
+          <a href="/" data-translate="home">
+          <span class="nav-link-text ms-1">Home</span>
+        </a>
+        </div>
+      </li>
+      <li class="nav-item">
+        <div class="nav-link">
 
-        <li class="nav-item">
-        <a class="nav-link active" href="/cosmetics?name=""" + f"""{display_name_get}""" + """">
-            <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
-              <svg width="15px" height="15px" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(12, 12, 12, 1);transform: ;msFilter:;"><path class="color-background" d="M12 2a5 5 0 1 0 5 5 5 5 0 0 0-5-5zm0 8a3 3 0 1 1 3-3 3 3 0 0 1-3 3zm9 11v-1a7 7 0 0 0-7-7h-4a7 7 0 0 0-7 7v1h2v-1a5 5 0 0 1 5-5h4a5 5 0 0 1 5 5v1z"></path></svg>
-          </div>
-            <span class="nav-link-text ms-1">Cosmetics</span>
-          </a>
-          </li> 
-          <li class="nav-item">
-          <a class="nav-link" href="https://klldfn.xyz/">
-            <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
-              <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
-                <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
-                  <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
-                    <g transform="translate(1716.000000, 291.000000)">
-                      <g transform="translate(0.000000, 148.000000)">
-                        <i class="ni ni-world-2 text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
-                      </g>
+          <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
+            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(12, 12, 12, 1);transform: ;msFilter:;"><path class="color-background"
+                      d="M4 13h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1zm-1 7a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v4zm10 0a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-7a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v7zm1-10h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v5a1 1 0 0 0 1 1z">
+                  </path></svg>
+             </div>
+             <a class="" href="/dashboard?name=""" + f"""{display_name_get}""" + """"" data-translate="dashboard">
+          <span class="nav-link-text ms-1">Dashboard</span>
+        </a>
+        </div>
+      </li>
+      <li class="nav-item">
+      <div class="nav-link active">
+
+        <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
+          <svg width="15px" height="15px" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(12, 12, 12, 1);transform: ;msFilter:;"><path class="color-background" d="M12 2a5 5 0 1 0 5 5 5 5 0 0 0-5-5zm0 8a3 3 0 1 1 3-3 3 3 0 0 1-3 3zm9 11v-1a7 7 0 0 0-7-7h-4a7 7 0 0 0-7 7v1h2v-1a5 5 0 0 1 5-5h4a5 5 0 0 1 5 5v1z"></path></svg>
+      </div>
+          <a href="/cosmetics?name=""" + f"""{display_name_get}""" + """"" data-translate="cosmetics">
+          <span class="nav-link-text ms-1">Cosmetics</span>
+        </a>
+        </div>
+
+        <div class="nav-link">
+          <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
+            <svg width="12px" height="12px" viewBox="0 0 45 40" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
+              <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
+                <g transform="translate(-1716.000000, -439.000000)" fill="#FFFFFF" fill-rule="nonzero">
+                  <g transform="translate(1716.000000, 291.000000)">
+                    <g transform="translate(0.000000, 148.000000)">
+                      <i class="ni ni-world-2 text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
                     </g>
                   </g>
                 </g>
-              </svg>
-            </div>
-            <span class="nav-link-text ms-1">Website</span>
+              </g>
+            </svg>
+          </div>
+          <a href="https://klldfn.xyz/" data-translate="website">
+          <span class="nav-link-text ms-1">Website</span>
           </a>
+        </div>
+      </li>
+    </ul>
+  </div>
+  <div class="sidenav-footer mx-3 ">
+    <div class="card card-background shadow-none card-background-mask-dark" id="sidenavCard">
+      <div class="full-background" style="background-image: url('https://klldfn-ui-dashboard.klldfn.xyz/assets/img/curved-images/white-curved.jpg')"></div>
+      <div class="card-body text-start p-3 w-100">
+        <div class="icon icon-shape icon-sm bg-white shadow text-center mb-3 d-flex align-items-center justify-content-center border-radius-md">
+          <i class="ni ni-diamond text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
+        </div>
 
-        </li>
-      </ul>
-    </div>
-    <div class="sidenav-footer mx-3 ">
-      <div class="card card-background shadow-none card-background-mask-dark" id="sidenavCard">
-        <div class="full-background" style="background-image: url('https://klldfn-ui-dashboard.klldfn.xyz/assets/img/curved-images/white-curved.jpg')"></div>
-        <div class="card-body text-start p-3 w-100">
-          <div class="icon icon-shape icon-sm bg-white shadow text-center mb-3 d-flex align-items-center justify-content-center border-radius-md">
-            <i class="ni ni-diamond text-dark text-gradient text-lg top-0" aria-hidden="true" id="sidenavCardIcon"></i>
-          </div>
-          <div class="docs-info">
-            <h6 class="text-white up mb-0">Need help?</h6>
-            <p class="text-xs font-weight-bold">Enter the Discord server</p>
-            <a href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
-          </div>
+        <div class="docs-info">
+          <h6 class="text-white up mb-0" data-translate="help">Need help?</h6>
+          <p class="text-xs font-weight-bold" data-translate="discordServer">Enter the Discord server</p>
+          <a data-translate="link" href="https://discord.gg/ybr7evg4q5" target="_blank" class="btn btn-white btn-sm w-100 mb-0">link</a>
         </div>
       </div>
     </div>
-
-  </aside>
+  </div>
+</aside>
   <main class="main-content position-relative max-height-vh-100 h-100 border-radius-lg ">
     <!-- Navbar -->
     <nav class="navbar navbar-main navbar-expand-lg px-0 mx-4 shadow-none border-radius-xl position-sticky blur shadow-blur mt-4 left-auto top-1 z-index-sticky" id="navbarBlur" navbar-scroll="true">
       <div class="container-fluid py-1 px-3">
         <nav aria-label="breadcrumb">
-          <h6 class="font-weight-bolder mb-0">Dashboard</h6>
+          <h6 class="font-weight-bolder mb-0" data-translate="dashboard">Dashboard</h6>
         </nav>
         <div class="collapse navbar-collapse mt-sm-0 mt-2 me-md-0 me-sm-4" id="navbar">
 
           <div class="ms-md-auto pe-md-3 d-flex align-items-center">
-            <!--
-            <div class="input-group">
-              <span class="input-group-text text-body"><i class="fas fa-search" aria-hidden="true"></i></span>
-              <input type="text" class="form-control" placeholder="Type here...">
-            </div>
-          </div>
-          <ul class="navbar-nav  justify-content-end">
-
-            <li class="nav-item d-flex align-items-center">
-              <a href="javascript:;" class="nav-link text-body font-weight-bold px-0">
-                <i class="fa fa-user me-sm-1"></i>
-                <span class="d-sm-inline d-none">Sign In</span>
-              </a>
+          <li class="nav-item px-3 d-flex align-items-center">
+            <label class="select" for="slct">
+      <select id="language-select" required="required">
+          <option value="" disabled="disabled" selected="selected">Choose the language</option>
+          <option value="en">English</option>
+          <option value="ar">Arabic</option>
+          <option value="de">German</option>
+          <option value="ja">Japanese</option>
+          <option value="fr">French</option>
+          <option value="es">Spanish</option>
+      </select>
+      <svg>
+        <use xlink:href="#select-arrow-down"></use>
+      </svg>
+    </label>
             </li>
-              -->
+
+
             <li class="nav-item d-xl-none ps-3 d-flex align-items-center">
               <a href="javascript:;" class="nav-link text-body p-0" id="iconNavbarSidenav">
                 <div class="sidenav-toggler-inner">
                   <i class="sidenav-toggler-line"></i>
                   <i class="sidenav-toggler-line"></i>
                   <i class="sidenav-toggler-line"></i>
                 </div>
               </a>
 
             </li>
 
-            <li class="nav-item px-3 d-flex align-items-center">
-            </li>
-            <!--
-            <li class="nav-item dropdown pe-2 d-flex align-items-center">
-              <a href="javascript:;" class="nav-link text-body p-0" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
-                <i class="fa fa-bell cursor-pointer"></i>
-              </a>
-              <ul class="dropdown-menu  dropdown-menu-end  px-2 py-3 me-sm-n4" aria-labelledby="dropdownMenuButton">
-                <h6 class="text-sm font-weight-normal mb-1">
-                  No New notifications
-                </h6>
-              </ul>
-            </li>
-            -->
+
           </ul>
         </div>
       </div>
     </nav>
     <!-- End Navbar -->
     <main class="main-content mt-0">
         <section>
@@ -1917,33 +2354,33 @@
                         <div class="col-xl-4 col-lg-5 col-md-6 d-flex flex-column mx-auto">
                             <div class="card card-plain mt-8">
                                 <div class="card-body">
                                     <div class="container" style="display: grid; grid-template-columns: repeat(2, 3fr); gap: 20px;">
                                         <div class="box" style="position: relative; width: 250px; height: 250px; border: 1px solid #dbd1d1; overflow: hidden; background-color: #cac1c1; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 10px; text-align: center;">
                                             <a href="cosmetics/skin?name=""" + f"""{display_name_get}""" + """" style="display: block; text-decoration: none; color: inherit;">
                                                 <img src="https://static.wikia.nocookie.net/fortnite/images/7/7a/Outfit_-_Icon_-_Fortnite.png" alt="Image 1" style="width: 100%; height: auto; display: block;">
-                                                <p style="margin: 0; font-size: 16px; color: #333;">Skin</p>
+                                                <p style="margin: 0; font-size: 16px; color: #333;" data-translate="outfit">Outfit</p>
                                             </a>
                                         </div>
                                         <div class="box" style="position: relative; width: 250px; height: 250px; border: 1px solid #dbd1d1; overflow: hidden; background-color: #cac1c1; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 10px; text-align: center;">
                                             <a href="cosmetics/emote?name=""" + f"""{display_name_get}""" + """" style="display: block; text-decoration: none; color: inherit;">
                                                 <img src="https://static.wikia.nocookie.net/fortnite/images/b/b1/Emotes_-_Icon_-_Fortnite.png" alt="Image 2" style="width: 100%; height: auto; display: block;">
-                                                <p style="margin: 0; font-size: 16px; color: #333;">Emote</p>
+                                                <p style="margin: 0; font-size: 16px; color: #333;" data-translate="emote">Emote</p>
                                             </a>
                                         </div>
                                         <div class="box" style="position: relative; width: 250px; height: 250px; border: 1px solid #dbd1d1; overflow: hidden; background-color: #cac1c1; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 10px; text-align: center;">
                                             <a href="#" data-bs-toggle="modal" data-bs-target="#CosmeticsModal" style="display: block; text-decoration: none; color: inherit;">
                                                 <img src="https://static.wikia.nocookie.net/fortnite/images/1/1b/Back_Bling_-_Icon_-_Fortnite.png" alt="Image 3" style="width: 100%; height: auto; display: block;">
-                                                <p style="margin: 0; font-size: 16px; color: #333;">Backpack</p>
+                                                <p style="margin: 0; font-size: 16px; color: #333;" data-translate="backpack">Backpack</p>
                                             </a>
                                         </div>
                                         <div class="box" style="position: relative; width: 250px; height: 250px; border: 1px solid #dbd1d1; overflow: hidden; background-color: #cac1c1; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 10px; text-align: center;">
                                             <a href="#" data-bs-toggle="modal" data-bs-target="#CosmeticsModal" style="display: block; text-decoration: none; color: inherit;">
                                                 <img src="https://static.wikia.nocookie.net/fortnite/images/f/f9/Harvesting_Tool_-_Icon_-_Fortnite.png" alt="Image 4" style="width: 100%; height: auto; display: block;">
-                                                <p style="margin: 0; font-size: 16px; color: #333;">Pickaxe</p>
+                                                <p style="margin: 0; font-size: 16px; color: #333;" data-translate="pickaxe">Pickaxe</p>
                                             </a>
                                         </div>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </div>
@@ -1955,15 +2392,15 @@
     <!-- Modal -->
     <div class="modal fade" id="CosmeticsModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
       <div class="modal-dialog">
         <div class="modal-content">
           <div class="modal-header">
 
           </div>
-          <div class="modal-body">
+          <div class="modal-body" data-translate="optionNotWork">
             This option does not work
           </div>
           <div class="modal-footer">
 
           </div>
         </div>
       </div>
@@ -1971,28 +2408,30 @@
     <footer class="footer py-5">
       <div class="container">
         <div class="row">
         </div>
         <div class="row">
           <div class="col-8 mx-auto text-center mt-1">
             <p class="mb-0 text-secondary">
-              Copyright © <script>
-                document.write(new Date().getFullYear())
-              </script>,
-              <i class="fa fa-heart"></i> by
-              klldFN
-              All Right Reserved
+                    <span data-translate="copyright"></span>
+                    <script>
+                        document.write(new Date().getFullYear())
+                    </script>
+                    <span data-translate="allRights">All Right Reserved</span>
             </p>
+
+
           </div>
         </div>
       </div>
     </footer>
 
 
   <!--   Core JS Files   -->
+  <script src="https://a--s-2342-djias4388--24ohi-udd--aou-hs3-24-flie.pages.dev/translator-cosmetics.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/popper.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/core/bootstrap.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/perfect-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/smooth-scrollbar.min.js"></script>
   <script src="https://klldfn-ui-dashboard.klldfn.xyz/assets/js/plugins/chartjs.min.js"></script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
 
@@ -2164,22 +2603,40 @@
             }
           },
         },
       },
     });
   </script>
   <script>
-    var win = navigator.platform.indexOf('Win') > -1;
-    if (win && document.querySelector('#sidenav-scrollbar')) {
-      var options = {
-        damping: '0.5'
-      }
-      Scrollbar.init(document.querySelector('#sidenav-scrollbar'), options);
-    }
-  </script>
+    // JavaScript to hide the preloader with a minimum display time
+    document.addEventListener('DOMContentLoaded', function() {
+        const preloader = document.querySelector('.mpl-preloader');
+        const MIN_DISPLAY_TIME = 2000; // Minimum display time in milliseconds (e.g., 2000ms = 2 seconds)
+        const startTime = Date.now();
+
+        window.addEventListener('load', function () {
+            const elapsedTime = Date.now() - startTime;
+            const remainingTime = MIN_DISPLAY_TIME - elapsedTime;
+
+            if (remainingTime > 0) {
+                setTimeout(() => {
+                    preloader.style.opacity = '0';
+                    setTimeout(() => {
+                        preloader.style.display = 'none';
+                    }, 500); // Allow transition time to fade out
+                }, remainingTime);
+            } else {
+                preloader.style.opacity = '0';
+                setTimeout(() => {
+                    preloader.style.display = 'none';
+                }, 500); // Allow transition time to fade out
+            }
+        });
+    });
+</script>
   <script>
     // Simulate content loaded event
     window.addEventListener('load', function() {
       // Hide loading overlay after 3 seconds (adjust the duration as needed)
       setTimeout(function() {
         document.getElementById('loadingOverlay').style.display = 'none';
       }, 3000); // Duration in milliseconds (e.g., 3000 for 3 seconds)
@@ -2223,40 +2680,88 @@
   <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
   <!-- CSS Files -->
   <link id="pagestyle" href="https://klldfn-ui-dashboard.klldfn.xyz/assets/css/klldFN-ui-dashboard.css?v=1.0.7" rel="stylesheet" />
   <!-- Nepcha Analytics (nepcha.com) -->
   <!-- Nepcha is a easy-to-use web analytics. No cookies and fully compliant with GDPR, CCPA and PECR. -->
   <script defer data-site="klldFN.xyz" src="https://api.nepcha.com/js/nepcha-analytics.js"></script>
   <style>
-    .loading-overlay {
-      position: fixed;
-      top: 0;
-      left: 0;
-      width: 100%;
-      height: 100%;
-      background-color: rgba(255, 255, 255, 0.8);
-      display: flex;
-      justify-content: center;
-      align-items: center;
-      z-index: 9999;
+    /* Preloader container */
+    .mpl-preloader {
+        position: fixed;
+        top: 0;
+        left: 0;
+        width: 100%;
+        height: 100%;
+        background: #2c2c3e; /* Dark background color */
+        z-index: 9999; /* Ensure it covers other content */
+        display: flex;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+        opacity: 1;
+        transition: opacity 0.5s ease; /* Smooth transition for fading out */
+    }
+
+    /* Spinner */
+
+
+    /* Preloader title */
+    .mpl-preloader-title {
+        font-family: 'Arial', sans-serif;
+        font-size: 36px;
+        color: #fff; /* White color */
+        margin-bottom: 20px;
+    }
+
+    /* Preloader progress bar container */
+    .mpl-preloader-progress {
+        width: 105%; /* Width of the progress bar */
+        height: 4px; /* Height of the progress bar */
+        background: #444; /* Dark gray background */
+        border-radius: 2px; /* Rounded corners */
+        position: relative;
+        overflow: hidden; /* Hide overflow */
+    }
+
+    /* Preloader progress bar */
+    .mpl-preloader-progress::before {
+        content: "";
+        position: absolute;
+        left: 0;
+        top: 0;
+        width: 100%;
+        height: 100%;
+        background: #fff; /* White color for the progress bar */
+        animation: loading 2s infinite; /* Animation for loading effect */
     }
 
-    .spinner-border {
-      width: 3rem;
-      height: 3rem;
+    /* Keyframes for loading animation */
+    @keyframes loading {
+        0% {
+            transform: translateX(-100%);
+        }
+        50% {
+            transform: translateX(0);
+        }
+        100% {
+            transform: translateX(100%);
+        }
     }
-  </style>
+
+</style>
 </head>
 
 <body class="g-sidenav-show  bg-gray-100">
-  <div class="loading-overlay" id="loadingOverlay">
-    <div class="spinner-border" role="status">
+<div class="mpl-preloader">
+    <div class="mpl-preloader-content">
 
+        <div class="mpl-preloader-title">klldFN</div>
+        <div class="mpl-preloader-progress"></div>
     </div>
-  </div>
+</div>
 
   <aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="#">
         <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
         <span class="ms-1 font-weight-bold">klldFN Dashboard</span>
@@ -2415,15 +2920,15 @@
                       {% endif %}
                   </div>
                   </div>
                   <div class="card-body">
                     <form action="?name={{ display_name }}" method="post">
                       <div class="mb-3">
 
-                        <input type="text" class="form-control" placeholder="Enter Skin Name" id="skin" name="content">
+                        <input type="text" class="form-control" placeholder="Enter Skin Name" id="skin" name="content" autocomplete="off">
                       </div>
 
 
 
                       <div class="text-center">
                         <input type="submit" class="btn bg-gradient-info w-100 mt-4 mb-0" value="Submit">
                       </div>
@@ -2645,22 +3150,40 @@
       var options = {
         damping: '0.5'
       }
       Scrollbar.init(document.querySelector('#sidenav-scrollbar'), options);
     }
   </script>
   <script>
-    // Simulate content loaded event
-    window.addEventListener('load', function() {
-      // Hide loading overlay after 3 seconds (adjust the duration as needed)
-      setTimeout(function() {
-        document.getElementById('loadingOverlay').style.display = 'none';
-      }, 3000); // Duration in milliseconds (e.g., 3000 for 3 seconds)
+    // JavaScript to hide the preloader with a minimum display time
+    document.addEventListener('DOMContentLoaded', function() {
+        const preloader = document.querySelector('.mpl-preloader');
+        const MIN_DISPLAY_TIME = 2000; // Minimum display time in milliseconds (e.g., 2000ms = 2 seconds)
+        const startTime = Date.now();
+
+        window.addEventListener('load', function () {
+            const elapsedTime = Date.now() - startTime;
+            const remainingTime = MIN_DISPLAY_TIME - elapsedTime;
+
+            if (remainingTime > 0) {
+                setTimeout(() => {
+                    preloader.style.opacity = '0';
+                    setTimeout(() => {
+                        preloader.style.display = 'none';
+                    }, 500); // Allow transition time to fade out
+                }, remainingTime);
+            } else {
+                preloader.style.opacity = '0';
+                setTimeout(() => {
+                    preloader.style.display = 'none';
+                }, 500); // Allow transition time to fade out
+            }
+        });
     });
-  </script>
+</script>
   <!-- Github buttons -->
   <script async defer src="https://buttons.github.io/buttons.js"></script>
   <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
   <script src="https://klldfn-ui-dashboard.klldfn.xyz//assets/js/soft-ui-dashboard.min.js?v=1.0.7"></script>
 </body>
 
 </html>      
@@ -2719,40 +3242,88 @@
   <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
   <!-- CSS Files -->
   <link id="pagestyle" href="https://klldfn-ui-dashboard.klldfn.xyz/assets/css/klldFN-ui-dashboard.css?v=1.0.7" rel="stylesheet" />
   <!-- Nepcha Analytics (nepcha.com) -->
   <!-- Nepcha is a easy-to-use web analytics. No cookies and fully compliant with GDPR, CCPA and PECR. -->
   <script defer data-site="klldFN.xyz" src="https://api.nepcha.com/js/nepcha-analytics.js"></script>
   <style>
-    .loading-overlay {
-      position: fixed;
-      top: 0;
-      left: 0;
-      width: 100%;
-      height: 100%;
-      background-color: rgba(255, 255, 255, 0.8);
-      display: flex;
-      justify-content: center;
-      align-items: center;
-      z-index: 9999;
+    /* Preloader container */
+    .mpl-preloader {
+        position: fixed;
+        top: 0;
+        left: 0;
+        width: 100%;
+        height: 100%;
+        background: #2c2c3e; /* Dark background color */
+        z-index: 9999; /* Ensure it covers other content */
+        display: flex;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+        opacity: 1;
+        transition: opacity 0.5s ease; /* Smooth transition for fading out */
     }
 
-    .spinner-border {
-      width: 3rem;
-      height: 3rem;
+    /* Spinner */
+
+
+    /* Preloader title */
+    .mpl-preloader-title {
+        font-family: 'Arial', sans-serif;
+        font-size: 36px;
+        color: #fff; /* White color */
+        margin-bottom: 20px;
+    }
+
+    /* Preloader progress bar container */
+    .mpl-preloader-progress {
+        width: 105%; /* Width of the progress bar */
+        height: 4px; /* Height of the progress bar */
+        background: #444; /* Dark gray background */
+        border-radius: 2px; /* Rounded corners */
+        position: relative;
+        overflow: hidden; /* Hide overflow */
+    }
+
+    /* Preloader progress bar */
+    .mpl-preloader-progress::before {
+        content: "";
+        position: absolute;
+        left: 0;
+        top: 0;
+        width: 100%;
+        height: 100%;
+        background: #fff; /* White color for the progress bar */
+        animation: loading 2s infinite; /* Animation for loading effect */
     }
-  </style>
+
+    /* Keyframes for loading animation */
+    @keyframes loading {
+        0% {
+            transform: translateX(-100%);
+        }
+        50% {
+            transform: translateX(0);
+        }
+        100% {
+            transform: translateX(100%);
+        }
+    }
+
+</style>
 </head>
 
 <body class="g-sidenav-show  bg-gray-100">
-  <div class="loading-overlay" id="loadingOverlay">
-    <div class="spinner-border" role="status">
+<div class="mpl-preloader">
+    <div class="mpl-preloader-content">
 
+        <div class="mpl-preloader-title">klldFN</div>
+        <div class="mpl-preloader-progress"></div>
     </div>
-  </div>
+</div>
 
   <aside class="sidenav navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-3 bg-white" id="sidenav-main" data-color="dark">
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="#">
         <img src="https://klldfn.xyz/icon.png" class="navbar-brand-img h-100" alt="main_logo">
         <span class="ms-1 font-weight-bold">klldFN Dashboard</span>
@@ -2777,24 +3348,24 @@
                 </g>
               </svg>
                         </div>
             <span class="nav-link-text ms-1">Home</span>
           </a>
         </li>
         <li class="nav-item">
-          <a class="nav-link" href="/dashboard?name={{display_name}}">
+          <a class="nav-link" href="/dashboard?name={{client_name}}">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg width="15px" height="15px" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(0, 0, 0, 1);transform: ;msFilter:;"><path d="M4 13h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1zm-1 7a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v4zm10 0a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1v-7a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v7zm1-10h6a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1h-6a1 1 0 0 0-1 1v5a1 1 0 0 0 1 1z"></path></svg>  
             </div>
             <span class="nav-link-text ms-1">Dashboard</span>
           </a>
         </li>
 
         <li class="nav-item">
-        <a class="nav-link active" href="/cosmetics?name={{display_name}}">
+        <a class="nav-link active" href="/cosmetics?name={{client_name}}">
             <div class="icon icon-shape icon-sm shadow border-radius-md bg-white text-center me-2 d-flex align-items-center justify-content-center">
               <svg width="15px" height="15px" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" style="fill: rgba(12, 12, 12, 1);transform: ;msFilter:;"><path class="color-background" d="M12 2a5 5 0 1 0 5 5 5 5 0 0 0-5-5zm0 8a3 3 0 1 1 3-3 3 3 0 0 1-3 3zm9 11v-1a7 7 0 0 0-7-7h-4a7 7 0 0 0-7 7v1h2v-1a5 5 0 0 1 5-5h4a5 5 0 0 1 5 5v1z"></path></svg>
           </div>
             <span class="nav-link-text ms-1">Cosmetics</span>
           </a>
           </li> 
           <li class="nav-item">
@@ -2908,18 +3479,18 @@
                           <p class="mb-0">{{ message }}</p>
                       {% elif error %}
                           <p class="mb-0">{{ error }}</p>
                       {% endif %}
                   </div>
                   </div>
                   <div class="card-body">
-                    <form action="?name={{ display_name }}" method="post">
+                    <form action="?name={{ client_name }}" method="post">
                       <div class="mb-3">
 
-                        <input type="text" class="form-control" placeholder="Enter Emote Name" id="emote" name="content">
+                        <input type="text" class="form-control" placeholder="Enter Emote Name" id="emote" name="content" autocomplete="off">
                       </div>
 
 
 
                       <div class="text-center">
                         <input type="submit" class="btn bg-gradient-info w-100 mt-4 mb-0" value="Submit">
                       </div>
@@ -3141,22 +3712,40 @@
       var options = {
         damping: '0.5'
       }
       Scrollbar.init(document.querySelector('#sidenav-scrollbar'), options);
     }
   </script>
   <script>
-    // Simulate content loaded event
-    window.addEventListener('load', function() {
-      // Hide loading overlay after 3 seconds (adjust the duration as needed)
-      setTimeout(function() {
-        document.getElementById('loadingOverlay').style.display = 'none';
-      }, 3000); // Duration in milliseconds (e.g., 3000 for 3 seconds)
+    // JavaScript to hide the preloader with a minimum display time
+    document.addEventListener('DOMContentLoaded', function() {
+        const preloader = document.querySelector('.mpl-preloader');
+        const MIN_DISPLAY_TIME = 2000; // Minimum display time in milliseconds (e.g., 2000ms = 2 seconds)
+        const startTime = Date.now();
+
+        window.addEventListener('load', function () {
+            const elapsedTime = Date.now() - startTime;
+            const remainingTime = MIN_DISPLAY_TIME - elapsedTime;
+
+            if (remainingTime > 0) {
+                setTimeout(() => {
+                    preloader.style.opacity = '0';
+                    setTimeout(() => {
+                        preloader.style.display = 'none';
+                    }, 500); // Allow transition time to fade out
+                }, remainingTime);
+            } else {
+                preloader.style.opacity = '0';
+                setTimeout(() => {
+                    preloader.style.display = 'none';
+                }, 500); // Allow transition time to fade out
+            }
+        });
     });
-  </script>
+</script>
   <!-- Github buttons -->
   <script async defer src="https://buttons.github.io/buttons.js"></script>
   <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
   <script src="https://klldfn-ui-dashboard.klldfn.xyz//assets/js/soft-ui-dashboard.min.js?v=1.0.7"></script>
 </body>
 
 </html>
@@ -3179,15 +3768,14 @@
             try:
                 cosmetic = await fortnite_api.cosmetics.get_cosmetic(language=get_Language, matchMethod="contains", name=content, backendType="AthenaDance")
                 await client.party.me.set_emote(asset=cosmetic.id)
                 emote_set = translations.read()["translations"]["emote-set"][get_Language]
                 display_name_post = client.user.display_name
                 return sanic.response.html(template_emote.render(client_name=client_name, message=emote_set.format(cosmetic.name), error=None, icon_url=f"https://fortnite-api.com/images/cosmetics/br/{cosmetic.id}/icon.png", display_name=display_name_post))      
             except FortniteAPIAsync.exceptions.NotFound:
-                return sanic.response.html(template_emote.render(client_name=client_name, message=None, error="Cosmetic not found", icon_url=None, display_name=display_name_get))
+                return sanic.response.html(template_emote.render(client_name=client_name, message=None, error="Cosmetic not found", icon_url=None))
         else:
           return sanic.response.html("Client not found")
 
-# Run the clients
-
-asyncio.run(clients_sanic_Run())
 
+# Run the clients
+asyncio.run(clients_sanic_Run())
```

### Comparing `klldFN-2.0.1/setup.py` & `klldFN-2.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="klldFN",
-    version="2.0.1",
+    version="2.0.2",
     author="klld",
     description="klldFN",
     long_description=long_description,
     python_requires='>=3.6.0',
     long_description_content_type="text/markdown",
     url="https://github.com/klldtest/klldFN",
     packages=setuptools.find_packages(),
@@ -20,14 +20,15 @@
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12',
           'Topic :: Internet',
           'Topic :: Software Development :: Libraries',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Utilities',
       ],
     install_requires=[
           'crayons',
```

