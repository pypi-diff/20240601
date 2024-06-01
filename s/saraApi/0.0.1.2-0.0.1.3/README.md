# Comparing `tmp/saraapi-0.0.1.2.tar.gz` & `tmp/saraapi-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.1.2.tar", last modified: Sun May 26 03:42:20 2024, max compression
+gzip compressed data, was "saraapi-0.0.1.3.tar", last modified: Sat Jun  1 19:27:45 2024, max compression
```

## Comparing `saraapi-0.0.1.2.tar` & `saraapi-0.0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 03:42:20.308018 saraapi-0.0.1.2/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5324 2024-05-26 03:42:20.306018 saraapi-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4591 2024-05-26 03:37:57.000000 saraapi-0.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 03:42:20.291446 saraapi-0.0.1.2/sara/
--rw-rw-rw-   0        0        0      131 2024-05-26 03:41:27.000000 saraapi-0.0.1.2/sara/__init__.py
--rw-rw-rw-   0        0        0      740 2024-05-26 03:23:22.000000 saraapi-0.0.1.2/sara/ext.py
--rw-rw-rw-   0        0        0     2021 2024-05-26 03:22:27.000000 saraapi-0.0.1.2/sara/nsfw.py
--rw-rw-rw-   0        0        0      616 2024-05-10 05:07:28.000000 saraapi-0.0.1.2/sara/req.py
--rw-rw-rw-   0        0        0      575 2024-05-26 03:38:27.000000 saraapi-0.0.1.2/sara/rolplay.py
--rw-rw-rw-   0        0        0      268 2024-05-26 03:23:00.000000 saraapi-0.0.1.2/sara/rolplayNsfw.py
--rw-rw-rw-   0        0        0      988 2024-05-26 03:31:59.000000 saraapi-0.0.1.2/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-26 03:42:20.305389 saraapi-0.0.1.2/saraApi.egg-info/
--rw-rw-rw-   0        0        0     5324 2024-05-26 03:42:20.000000 saraapi-0.0.1.2/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 03:42:20.000000 saraapi-0.0.1.2/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 03:42:20.000000 saraapi-0.0.1.2/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 03:42:20.000000 saraapi-0.0.1.2/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 03:42:20.000000 saraapi-0.0.1.2/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 03:42:20.308018 saraapi-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-26 03:42:07.000000 saraapi-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:27:45.941590 saraapi-0.0.1.3/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5354 2024-06-01 19:27:45.940585 saraapi-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4621 2024-06-01 19:27:02.000000 saraapi-0.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 19:27:45.925588 saraapi-0.0.1.3/sara/
+-rw-rw-rw-   0        0        0      131 2024-05-26 03:41:27.000000 saraapi-0.0.1.3/sara/__init__.py
+-rw-rw-rw-   0        0        0      753 2024-06-01 19:26:33.000000 saraapi-0.0.1.3/sara/ext.py
+-rw-rw-rw-   0        0        0     2021 2024-05-26 03:22:27.000000 saraapi-0.0.1.3/sara/nsfw.py
+-rw-rw-rw-   0        0        0      616 2024-05-10 05:07:28.000000 saraapi-0.0.1.3/sara/req.py
+-rw-rw-rw-   0        0        0      575 2024-05-26 03:38:27.000000 saraapi-0.0.1.3/sara/rolplay.py
+-rw-rw-rw-   0        0        0      309 2024-06-01 19:26:12.000000 saraapi-0.0.1.3/sara/rolplayNsfw.py
+-rw-rw-rw-   0        0        0      988 2024-05-26 03:31:59.000000 saraapi-0.0.1.3/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:27:45.939578 saraapi-0.0.1.3/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     5354 2024-06-01 19:27:45.000000 saraapi-0.0.1.3/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-06-01 19:27:45.000000 saraapi-0.0.1.3/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 19:27:45.000000 saraapi-0.0.1.3/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 19:27:45.000000 saraapi-0.0.1.3/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 19:27:45.000000 saraapi-0.0.1.3/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 19:27:45.941590 saraapi-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-06-01 19:27:38.000000 saraapi-0.0.1.3/setup.py
```

### Comparing `saraapi-0.0.1.2/PKG-INFO` & `saraapi-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,14 +137,15 @@
 ---|---
 rolplayNsfw.fuck | sex 
 rolplayNsfw.anal | :0
 rolplayNsfw.happyend | happyend
 rolplayNsfw.kuni | kuni
 rolplayNsfw.spank | spank
 rolplayNsfw.suck | suck
+rolpayNsfw.feetjob | feetjob
 
 Function | Description
 ---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.2 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.3 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -49,21 +49,21 @@
 Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
 why do they look like intestines? thighs | The top part of your legs, very hot,
 isn't it? uglyBastard | The one thing most of us can all agree to hate :
 ) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
 Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
 squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
 rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
-rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
-- sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
-sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
-sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
-sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
-Bot Example ```python import discord # Import the module import sara from
-discord.ext import commands # get commands from discord.ext client =
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck rolpayNsfw.feetjob | feetjob
+Function | Description ---|--- sara.sfw.mobileWallpapers() | Fetch a random SFW
+Wallpaper! (Mobile) sara.sfw.wallpapers() | Fetch a random SFW Wallpaper!
+(Desktop) sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper!
+(Mobile) sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ##
+Discord Bot Example ```python import discord # Import the module import sara
+from discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
 decorator async def on_ready(): # on Ready event print(f"Ready as
 {client.user}") # print the bot's tag when its ready @client.command() # Make a
 isinstance for the command async def neko(ctx): # Make the function and pass in
 `ctx` as the params print(sara.sfw.neko()) client.run("token") # token here ```
 ## Any Bugs? [Open a issue](https://github.com/EverGasterXd/sara_api/issues) or
 dm evergaster
```

### Comparing `saraapi-0.0.1.2/README.md` & `saraapi-0.0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 ---|---
 rolplayNsfw.fuck | sex 
 rolplayNsfw.anal | :0
 rolplayNsfw.happyend | happyend
 rolplayNsfw.kuni | kuni
 rolplayNsfw.spank | spank
 rolplayNsfw.suck | suck
+rolpayNsfw.feetjob | feetjob
 
 Function | Description
 ---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -39,21 +39,21 @@
 Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
 why do they look like intestines? thighs | The top part of your legs, very hot,
 isn't it? uglyBastard | The one thing most of us can all agree to hate :
 ) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
 Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
 squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
 rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
-rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
-- sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
-sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
-sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
-sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
-Bot Example ```python import discord # Import the module import sara from
-discord.ext import commands # get commands from discord.ext client =
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck rolpayNsfw.feetjob | feetjob
+Function | Description ---|--- sara.sfw.mobileWallpapers() | Fetch a random SFW
+Wallpaper! (Mobile) sara.sfw.wallpapers() | Fetch a random SFW Wallpaper!
+(Desktop) sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper!
+(Mobile) sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ##
+Discord Bot Example ```python import discord # Import the module import sara
+from discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
 decorator async def on_ready(): # on Ready event print(f"Ready as
 {client.user}") # print the bot's tag when its ready @client.command() # Make a
 isinstance for the command async def neko(ctx): # Make the function and pass in
 `ctx` as the params print(sara.sfw.neko()) client.run("token") # token here ```
 ## Any Bugs? [Open a issue](https://github.com/EverGasterXd/sara_api/issues) or
 dm evergaster
```

### Comparing `saraapi-0.0.1.2/sara/ext.py` & `saraapi-0.0.1.3/sara/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 ROLPLAYNSFW:
     anal
     fuck
     happyend
     spank
     suck
     kuni
+    feetjob
 ROLPLAYSFW:
     baka
     kiss
     kill
     spank
     puch
     poke
```

### Comparing `saraapi-0.0.1.2/sara/nsfw.py` & `saraapi-0.0.1.3/sara/nsfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.1.2/sara/req.py` & `saraapi-0.0.1.3/sara/req.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.1.2/sara/rolplay.py` & `saraapi-0.0.1.3/sara/rolplay.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.1.2/sara/sfw.py` & `saraapi-0.0.1.3/sara/sfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.1.2/saraApi.egg-info/PKG-INFO` & `saraapi-0.0.1.3/saraApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,14 +137,15 @@
 ---|---
 rolplayNsfw.fuck | sex 
 rolplayNsfw.anal | :0
 rolplayNsfw.happyend | happyend
 rolplayNsfw.kuni | kuni
 rolplayNsfw.spank | spank
 rolplayNsfw.suck | suck
+rolpayNsfw.feetjob | feetjob
 
 Function | Description
 ---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.2 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.3 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -49,21 +49,21 @@
 Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
 why do they look like intestines? thighs | The top part of your legs, very hot,
 isn't it? uglyBastard | The one thing most of us can all agree to hate :
 ) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
 Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
 squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
 rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
-rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
-- sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
-sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
-sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
-sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
-Bot Example ```python import discord # Import the module import sara from
-discord.ext import commands # get commands from discord.ext client =
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck rolpayNsfw.feetjob | feetjob
+Function | Description ---|--- sara.sfw.mobileWallpapers() | Fetch a random SFW
+Wallpaper! (Mobile) sara.sfw.wallpapers() | Fetch a random SFW Wallpaper!
+(Desktop) sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper!
+(Mobile) sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ##
+Discord Bot Example ```python import discord # Import the module import sara
+from discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
 decorator async def on_ready(): # on Ready event print(f"Ready as
 {client.user}") # print the bot's tag when its ready @client.command() # Make a
 isinstance for the command async def neko(ctx): # Make the function and pass in
 `ctx` as the params print(sara.sfw.neko()) client.run("token") # token here ```
 ## Any Bugs? [Open a issue](https://github.com/EverGasterXd/sara_api/issues) or
 dm evergaster
```

### Comparing `saraapi-0.0.1.2/setup.py` & `saraapi-0.0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.1.2'
+version = '0.0.1.3'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

