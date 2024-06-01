# Comparing `tmp/etm-dgraham-6.3.0.tar.gz` & `tmp/etm-dgraham-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.3.0.tar", last modified: Fri May 31 12:30:19 2024, max compression
+gzip compressed data, was "etm-dgraham-6.3.1.tar", last modified: Sat Jun  1 17:44:28 2024, max compression
```

## Comparing `etm-dgraham-6.3.0.tar` & `etm-dgraham-6.3.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.632781 etm-dgraham-6.3.0/
--rw-r--r--   0 dag        (501) staff       (20)     5351 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   146330 2024-05-31 12:30:19.632408 etm-dgraham-6.3.0/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144761 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.3.0/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.3.0/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.624845 etm-dgraham-6.3.0/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.628239 etm-dgraham-6.3.0/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-23 14:53:47.000000 etm-dgraham-6.3.0/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    27073 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29418 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.3.0/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   338742 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.3.0/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.3.0/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)     1512 2024-05-30 19:08:07.000000 etm-dgraham-6.3.0/etm/rrule-test.py
--rw-r--r--   0 dag        (501) staff       (20)     1284 2024-05-30 10:36:15.000000 etm-dgraham-6.3.0/etm/rruleset-test.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126430 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.630507 etm-dgraham-6.3.0/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   146330 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      921 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.3.0/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.3.0/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/namedcolors.py
--rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.3.0/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-31 12:30:19.632826 etm-dgraham-6.3.0/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.3.0/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.630639 etm-dgraham-6.3.0/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.3.0/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.631893 etm-dgraham-6.3.0/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.3.0/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.3.0/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.3.0/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.412205 etm-dgraham-6.3.1/
+-rw-r--r--   0 dag        (501) staff       (20)     4792 2024-06-01 17:44:24.000000 etm-dgraham-6.3.1/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.3.1/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   145410 2024-06-01 17:44:28.411937 etm-dgraham-6.3.1/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   143841 2024-06-01 17:44:24.000000 etm-dgraham-6.3.1/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.3.1/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.3.1/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.406330 etm-dgraham-6.3.1/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.3.1/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.3.1/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.3.1/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.408522 etm-dgraham-6.3.1/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.3.1/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-23 14:53:47.000000 etm-dgraham-6.3.1/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-06-01 17:44:24.000000 etm-dgraham-6.3.1/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    27073 2024-05-31 12:30:12.000000 etm-dgraham-6.3.1/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29418 2024-05-31 12:30:12.000000 etm-dgraham-6.3.1/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    10177 2024-06-01 17:44:24.000000 etm-dgraham-6.3.1/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   338982 2024-06-01 17:44:24.000000 etm-dgraham-6.3.1/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.3.1/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.3.1/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     1512 2024-05-30 19:08:07.000000 etm-dgraham-6.3.1/etm/rrule-test.py
+-rw-r--r--   0 dag        (501) staff       (20)     2678 2024-05-31 19:35:05.000000 etm-dgraham-6.3.1/etm/rruleset-test.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     2764 2024-05-31 16:28:12.000000 etm-dgraham-6.3.1/etm/simulate_time_passage.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126430 2024-05-31 12:30:12.000000 etm-dgraham-6.3.1/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.410590 etm-dgraham-6.3.1/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   145410 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      950 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-06-01 17:44:28.000000 etm-dgraham-6.3.1/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.3.1/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.3.1/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.3.1/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.3.1/namedcolors.py
+-rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.3.1/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.3.1/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-06-01 17:44:28.412243 etm-dgraham-6.3.1/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.3.1/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.410696 etm-dgraham-6.3.1/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.3.1/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-06-01 17:44:28.411400 etm-dgraham-6.3.1/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.3.1/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.3.1/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.3.1/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.3.1/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.3.0/CHANGES.txt` & `etm-dgraham-6.3.1/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,37 @@
-2024-05-31 3cfe871 Daniel Graham
+2024-06-01 b60f926 Daniel Graham
+    Tagged version 6.3.1.
+
+2024-06-01 d13c107 Daniel Graham
+    Updated goal.png
+
+2024-06-01 7b944c5 Daniel Graham
+    Tweaks for make_examples, goals.png and README
+
+2024-06-01 b70e39a Daniel Graham
+    README tweaks
+
+2024-06-01 0fa5a1d Daniel Graham
+    README tweaks
+
+2024-06-01 7e1be56 Daniel Graham
+    Fixed bug in processing yearly goals
+
+2024-06-01 0ae3c60 Daniel Graham
+    Use lorem phrase for goals. In item.get_repetititons, only update
+    hash if modified.
+
+2024-06-01 d2daf8d Daniel Graham
+    Added goals and dst tests to make_examples. Fixed bug in yearly
+    fraction.
+
+2024-06-01 37adfc3 Daniel Graham
+    README tweaks
+
+2024-05-31 16cb122 Daniel Graham
     Tagged version 6.3.0. Added goal period options for year, quarter
     and month. Added caching for non-weekly views. Fixed timezone
     issues associated with the transistions between daylight saving
     and standard time.
 
 2024-05-31 98f34e5 Daniel Graham
     Fixed timezone issues associated with daylight/standard time
@@ -157,44 +186,7 @@
 
 2024-05-04 6ffaa2f Daniel Graham
     Tagged version 6.2.0. Added a new item type, goal, and a
     corresponding goal view.
 
 2024-05-04 bd93aab Daniel Graham
     Merge branch 'working' into goals
-
-2024-05-04 9aa9c5f Daniel Graham
-    Tagged version 6.1.27.
-
-2024-05-04 eebce81 Daniel Graham
-    Fixed bug in including s as a possible pastdue in a task with an r
-    entry.
-
-2024-05-03 893a055 Daniel Graham
-    Cleaned up comments
-
-2024-05-03 c6021f9 Daniel Graham
-    Cleaned up comments. Changed min width for weekday in statusbar to
-    50. Fixed regex for quota and goal history. Include weekday 0
-    (Mon) in active but don't warn about 0 completions. Removed
-    show_active_view from alarm loop. Removed show_message
-    confirmation for toggle active and increment count.
-
-2024-05-03 e6e4a65 Daniel Graham
-    Show completions needed to get on schedule in goals instead of
-    days remaining and the average number of completions instead of
-    the total.
-
-2024-05-02 fadef79 Daniel Graham
-    Added type characters and colors for goals. Sort active/inactive
-    goals by done/quota.
-
-2024-05-02 feab252 Daniel Graham
-    Added goal view and removed goal counts from agenda view. Color
-    active goals according to progress. Added commands to toggle
-    active/paused and to end goal.
-
-2024-05-01 41242dd Daniel Graham
-    Changed binding for goto link from g to G
-
-2024-05-01 f1c68f0 Daniel Graham
-    Corrected typo
```

### Comparing `etm-dgraham-6.3.0/PKG-INFO` & `etm-dgraham-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.3.0
+Version: 6.3.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -618,37 +618,28 @@
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
 [↺ contents](#contents)
 
 ### Goals View {#goals-view}
 
-This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+This is a dedicated view that *only displays goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current period (week, month, quarter or year)*.  This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
 
-This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+Here is an illustrative screenshot from *Goals View*:
 
-Consider this illustrative screenshot from *Goals View*:
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/goals.png" alt="new" title="goals view" width="600px" hspace="20px"/>
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+In this screen shot the first goal in "Active" is selected and its details panel is displayed. The leading "1/5q" in the main window indicates that 1 instance of the goal of 5 has been completed for the current (q)uarter. The trailing (2) means that 2 more completions are currently needed to get back on schedule.  The other active goals "0/4y", "0/1w" and "0/2m" have similar interpretations but correspond to goals for (y)ear, (w)eek and (m)onth periods, respectively.
 
-Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+Active goals are sorted in descending order by the fraction of the relevant period that has passed and are given a color indicating number of completions needed to be on schedule: red for 2 or more, yellow for 1 and blue otherwise. 
 
-In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
-
-In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
-- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
-- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
-- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
-
-This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
-- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
-- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
-
-A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+All the normal commands are available and, additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current period (by incrementing the count for the current period in @h).
+- ^a: toggle the active/paused status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *paused* and are displayed in a separate category. 
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of periods that has expired) are regarded as *ended* and are also displayed in a separate category. A *goal* could, of course, be deleted but this would also delete the history of completions. 
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
@@ -1904,14 +1895,15 @@
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
+*  @q: quota. Used to specify the attributes of a goal. E.g., @q 3m, 2 would specify a goal of 3 completions per (m)onth for 2 months. Other period options include (y)ear, (q)uarter and (w)eek. Week is the default. The default for the number of periods is 0 which entails repeating indefinitely.
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
```

### Comparing `etm-dgraham-6.3.0/README.md` & `etm-dgraham-6.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -575,37 +575,28 @@
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
 [↺ contents](#contents)
 
 ### Goals View {#goals-view}
 
-This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+This is a dedicated view that *only displays goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current period (week, month, quarter or year)*.  This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
 
-This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+Here is an illustrative screenshot from *Goals View*:
 
-Consider this illustrative screenshot from *Goals View*:
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/goals.png" alt="new" title="goals view" width="600px" hspace="20px"/>
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+In this screen shot the first goal in "Active" is selected and its details panel is displayed. The leading "1/5q" in the main window indicates that 1 instance of the goal of 5 has been completed for the current (q)uarter. The trailing (2) means that 2 more completions are currently needed to get back on schedule.  The other active goals "0/4y", "0/1w" and "0/2m" have similar interpretations but correspond to goals for (y)ear, (w)eek and (m)onth periods, respectively.
 
-Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+Active goals are sorted in descending order by the fraction of the relevant period that has passed and are given a color indicating number of completions needed to be on schedule: red for 2 or more, yellow for 1 and blue otherwise. 
 
-In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
-
-In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
-- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
-- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
-- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
-
-This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
-- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
-- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
-
-A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+All the normal commands are available and, additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current period (by incrementing the count for the current period in @h).
+- ^a: toggle the active/paused status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *paused* and are displayed in a separate category. 
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of periods that has expired) are regarded as *ended* and are also displayed in a separate category. A *goal* could, of course, be deleted but this would also delete the history of completions. 
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
@@ -1861,14 +1852,15 @@
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
+*  @q: quota. Used to specify the attributes of a goal. E.g., @q 3m, 2 would specify a goal of 3 completions per (m)onth for 2 months. Other period options include (y)ear, (q)uarter and (w)eek. Week is the default. The default for the number of periods is 0 which entails repeating indefinitely.
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
```

### Comparing `etm-dgraham-6.3.0/bump.py` & `etm-dgraham-6.3.1/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/docs/index_konnections.md` & `etm-dgraham-6.3.1/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/docs/index_usedtime.md` & `etm-dgraham-6.3.1/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/docs/multiple_timers.md` & `etm-dgraham-6.3.1/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/__main__.py` & `etm-dgraham-6.3.1/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/common.py` & `etm-dgraham-6.3.1/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/data.py` & `etm-dgraham-6.3.1/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/make_examples.py` & `etm-dgraham-6.3.1/etm/make_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,14 +114,26 @@
 @j purchase materials &e 1d &i a
 @j cut pieces &s 1d &e 1d &i b &p a
 @j assemble &s 2d &e 1d &i c &p b
 @j sand &s 3d &e 1d &i d &p c
 @j paint &s 4d &e 1d &i e &p d 
 """
 
+    goal_examples = f"""\
+~ {phrase()} @s {now.strftime('%Y-%m-%d')} @q 1w @t lorem
+~ {phrase()} @s {now.strftime('%Y-%m-%d')} @q 2m @t lorem
+~ {phrase()} @s {now.strftime('%Y-%m-%d')} @q 3q @t lorem
+~ {phrase()} @s {now.strftime('%Y-%m-%d')} @q 4y @t lorem
+""".split('\n')
+
+    dst_examples = f"""\
+* fall daylight -> standard time  @s {now.strftime('%Y-%m-%d')} @r y &M 11 &w 1SU &h 0, 1, 2, 3 &n 30 @t lorem
+* spring standard -> daylight time  @s {now.strftime('%Y-%m-%d')} @r y &M 3 &w 2SU &h 0, 1, 2, 3 &n 30 @t lorem
+""".split('\n')
+
     alerts = [f'@a {random.choice([0, 15, 30])}m: d' for x in range(10)]
 
     types = ['-', '*', '%']
     clients = ['A', 'B', 'C', 'D']
     client_name = {
         'A': names[0],
         'B': names[1],
@@ -147,15 +159,15 @@
     dates = [0, 0, 0, 1, 0, 0, 0]   # dates 1/7 of the time
     minutes = range(15, 110, 5)   # for used times (test rounding)
     # days = range(7)
     extent = [x for x in range(30, 210, 15)]
 
     # client_contacts = {}
     # client_id = {}
-    examples = [doghouse_example,]
+    examples = []
 
     for i in range(4):
         examples.append(
             f'- {phrase()} {beg()} {random.choice(freq)} {random.choice(stop)} {cnt()} @t lorem'
         )
 
     for client in clients:
@@ -210,15 +222,15 @@
 
         if t == '%' and start <= now:
             summary = start.strftime('%Y-%m-%d')
             if summary not in daily:
                 daily.append(summary)
                 description = start.strftime('%A, %B %-d %Y')
                 examples.append(
-                    f'{t} {summary} @i #daily @t lorem @d {description}\n\n* {note_time()}\n  - {phrase()}'
+                    f'{t} {summary} @i #daily @t lorem @d {description}\n\n  * {note_time()}\n    - {phrase()}'
                 )
 
         elif t == '*':
             if date:      # an event
                 examples.append(
                     f'{t} {summary} @s {s} @t {random.choice(tags)} @t lorem'
                 )
@@ -264,17 +276,23 @@
     children = random.choices(indices, k=40)
     for p in parents:
         n = random.choice([x for x in range(3, 8)])
         samp = random.choices(children, k=n)
         entry = ' '.join([f'@k {x}' for x in samp if x != p])
         examples[p - last_id] += f' {entry}'
 
+    
+    examples.append(doghouse_example)
+    examples.extend(goal_examples)
+    examples.extend(dst_examples)
+    
     if egfile:
         with open(egfile, 'w') as fo:
             fo.writelines('\n'.join(examples))
+    
     return examples
 
 
 if __name__ == '__main__':
     if len(sys.argv) > 2:
         egfile = sys.argv.pop(1)
         num_items = sys.argv.pop(1)
```

### Comparing `etm-dgraham-6.3.0/etm/model.py` & `etm-dgraham-6.3.1/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,14 +862,16 @@
     def get_repetitions(self):
         """
         Called with a row, we should have an doc_id and can use relevant
         as aft_dt. Called while editing, we won't have a row or doc_id
         and can use '@s' as aft_dt
         """
         num = self.settings['num_repetitions']
+        if self.is_modified:
+            self.update_item_hsh(False)
         # self.update_item_hsh()
         item = self.item_hsh
         showing = 'Repetitions'
         if 's' not in item and ('r' not in item or '+' not in item):
             return showing, 'not a repeating item'
         logger.debug(f"{item['s'] = }; {item = }")
         relevant = date_to_datetime(item['s'])
@@ -1907,21 +1909,21 @@
         all_ok = True
         rep_lst = []
         bad_lst = []
         completions = []
         if self.item_hsh['itemtype'] == '~':
             obj = {}
             # arg list will be a list of year:weeknum num_done
-            rx = re.compile(r'^\s*\d{4}[:#-]\d{1,2}\s+\d+\s*$')
+            rx = re.compile(r'^\s*\d{4}([:#-]\d{1,2})?\s+\d+\s*$')
             for arg in args:
                 match = rx.match(arg.strip())
                 if match:
-                    yearweek, done = arg.split()
-                    obj[yearweek] = int(done)
-                    rep_lst.append(f"{yearweek}: {done}")
+                    period, done = arg.split()
+                    obj[period] = int(done)
+                    rep_lst.append(f"{period}: {done}")
                 else:
                     all_ok = False
                     bad_lst.append(arg)
             obj = obj if all_ok else None
             rep = f"done: {', '.join(rep_lst)}"
             if bad_lst:
                 rep += f"\nincomplete or invalid completions: {', '.join(bad_lst)}"
@@ -8204,15 +8206,15 @@
     #     input_date = datetime.strptime(input_date, '%Y-%m-%d')
     # elif isinstance(input_date, datetime):
     #     input_date = input_date.replace(hour=0, minute=0, microsecond=0)
     # else:
     #     input_date = date_to_datetime(input_date)
 
     today = datetime.now().astimezone().replace(
-        hour=0, minute=0, second=0, microsecond=0
+        hour=0, minute=0, second=0, microsecond=0, tzinfo=None
         )
 
     # Helper function to calculate fraction of the week passed
     def fraction_of_week_passed():
         this_period_tup = today.isocalendar()[:2] # yyyy, weeknum
         this_period = f"{this_period_tup[0]}:{this_period_tup[1]:02}"
         return this_period, today.weekday() / 6
@@ -8221,25 +8223,25 @@
     def fraction_of_month_passed():
         this_period = f"{today.year}-{today.month:02}"
         return this_period, (today.day - 1) / (calendar.monthrange(today.year, today.month)[1] - 1)
 
     # Helper function to calculate fraction of the quarter passed
     def fraction_of_quarter_passed():
         quarter_start_month = 3 * ((today.month - 1) // 3) + 1
-        quarter_start_date = datetime(today.year, quarter_start_month, 1).astimezone()
+        quarter_start_date = datetime(today.year, quarter_start_month, 1).astimezone().replace(tzinfo=None)
         quarter_end_month = quarter_start_month + 2
-        quarter_end_date = datetime(today.year, quarter_end_month, calendar.monthrange(today.year, quarter_end_month)[1]).astimezone()
+        quarter_end_date = datetime(today.year, quarter_end_month, calendar.monthrange(today.year, quarter_end_month)[1]).astimezone().replace(tzinfo=None)
         this_period = f"{today.year}#{(today.month - 1) // 3 + 1}"
         return this_period, (today - quarter_start_date).days / (quarter_end_date - quarter_start_date).days
 
     # Helper function to calculate fraction of the year passed
     def fraction_of_year_passed():
-        start_of_year = datetime(today.year, 1, 1)
-        end_of_year = datetime(today.year, 12, 31)
-        return (today - start_of_year).days / (end_of_year - start_of_year).days
+        start_of_year = datetime(today.year, 1, 1).replace(tzinfo=None)
+        end_of_year = datetime(today.year, 12, 31, 23, 59).replace(tzinfo=None)
+        return f"{today.year}", (today - start_of_year).days / (end_of_year - start_of_year).days
 
     if period == 'd':
         return 0.0
     elif period == 'w':
         return fraction_of_week_passed()
     elif period == 'm':
         return fraction_of_month_passed()
@@ -8254,16 +8256,15 @@
     # Ensure input_date is a datetime object
     if isinstance(input_date, str):
         input_date = datetime.strptime(input_date, '%Y-%m-%d')
     elif isinstance(input_date, datetime):
         input_date = input_date.replace(hour=0, minute=0, microsecond=0)
     else:
         input_date = date_to_datetime(input_date)
-    input_date = input_date.astimezone()
-    
+    input_date = input_date.astimezone(local_tz)
 
     if period == 'w':
         return input_date - timedelta(days=input_date.weekday())
     
     elif period == 'm':
         return input_date.replace(day=1)
 
@@ -8310,16 +8311,14 @@
     elif period == 'y': 
         # Calculate the last day of the year periods_ahead years from input_date
         return datetime(input_date.year + periods_ahead - 1, 12, 31).astimezone() + timedelta(days=1, seconds=-1)
 
     else:
         return None
     
-    return ret
-    
 # # Example usage
 # input_date = '2024-05-26'
 # period = 'm'
 # periods_ahead = 3
 # for period in ['w', 'm', 'q', 'y']:
 #     result = get_period_end_date(input_date, period, periods_ahead)
 #     print(f"{input_date = }, {period = }, end_date = {result}")  # (fatetime.date(2024, 6, 8), datetime.date(2024, 7, 31), datetime.date(2024, 9, 30), datetime.date(2025, 12, 31))
@@ -8342,15 +8341,15 @@
     rows = []
     path2sort = {
         'Active': 1,
         'Paused': 2,
         'Upcoming': 3,
         'Ended': 4,
     }
-    today = datetime.today().astimezone()
+    today = datetime.today().astimezone(local_tz)
     current_weekday = today.weekday()         # 0, 1, ..., 6
     # weekdays_remaining = 7 - current_weekday  # 7, 6, ..., 1 
     for item in db:
         itemtype = item.get('itemtype')
         if itemtype != '~':
             continue
         doc_id = item.doc_id
@@ -8370,30 +8369,30 @@
         if not s or q is None:
             logger.error(f"bad goal: {item = }")
             continue
         quota = int(q[0]) 
         period = q[1] if len(q) > 1 else 'w'
         periods = q[2] if len(q) > 2 else 0
 
-        begin_date = get_period_begin_date(item['s'], period)
+        begin_date = get_period_begin_date(item['s'], period) # active if today >= begin_date 
         fraction_used = 0.0
 
         if periods:
-            end_date = get_period_end_date(item['s'], period, periods)
+            end_date = get_period_end_date(item['s'], period, periods) # active if end_date <= today
 
         if quota == 0 or (
             periods and end_date and today > end_date
             ):
             path = 'Ended'
             # goal = f'{average}/{quota}{period}'
             goal = f'{period}'
             itemtype = EtmChar.ENDED_CHAR
         else:
             this_period, fraction_used = get_fraction_of_period_passed(period)
-            # logger.debug(f"{begin_date = }; {this_period = }; {fraction_used = }")
+            logger.debug(f"{begin_date = }; {this_period = }; {fraction_used = }")
             # period = f"{fraction_used:.2}{period}"
 
             # this_week = today.isocalendar()[:2] 
             # this_week_str = f"{this_week[0]}:{this_week[1]:02}"
             done = int(h.get(this_period, 0))
             if quota < 0:
                 path = 'Paused'
```

### Comparing `etm-dgraham-6.3.0/etm/options.py` & `etm-dgraham-6.3.1/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/report.py` & `etm-dgraham-6.3.1/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/rrule-test.py` & `etm-dgraham-6.3.1/etm/rrule-test.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm/view.py` & `etm-dgraham-6.3.1/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.3.1/etm_dgraham.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.3.0
+Version: 6.3.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -618,37 +618,28 @@
 
 One final useful context is 'waiting for'. E.g., completing a task might depend upon getting something from Joe. Add `@l waiting for/Joe` to the task and it will be listed in the subgroup 'Joe' under 'waiting for'.
 
 [↺ contents](#contents)
 
 ### Goals View {#goals-view}
 
-This is a dedicated view *only for goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current week*. 
+This is a dedicated view that *only displays goals*. Goals are also displayed in *History View*, *Index View* and so forth, but are **not** displayed in *Agenda View* since goals apply *only to the current period (week, month, quarter or year)*.  This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
 
-This view can be selected in *etm* either by pressing "g" or by selecting *goals* from the *view* menu.
+Here is an illustrative screenshot from *Goals View*:
 
-Consider this illustrative screenshot from *Goals View*:
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/goals.png" alt="new" title="goals view" width="600px" hspace="20px"/>
 
-<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/walk_the_dog.png" alt="new" title="goals view" width="600px" hspace="20px"/>
+In this screen shot the first goal in "Active" is selected and its details panel is displayed. The leading "1/5q" in the main window indicates that 1 instance of the goal of 5 has been completed for the current (q)uarter. The trailing (2) means that 2 more completions are currently needed to get back on schedule.  The other active goals "0/4y", "0/1w" and "0/2m" have similar interpretations but correspond to goals for (y)ear, (w)eek and (m)onth periods, respectively.
 
-Notice first that there is no heading displaying a date or week since *goal view* displays the status of *all* goals at the *current time*. 
+Active goals are sorted in descending order by the fraction of the relevant period that has passed and are given a color indicating number of completions needed to be on schedule: red for 2 or more, yellow for 1 and blue otherwise. 
 
-In this screen shot "walk the dog" is selected and its details panel is displayed. The leading "3/7+2 (4.8)" in the main window indicates that 3 instances of the goal of 7 have been completed in the current week, that 2 more completions today are needed to get back on schedule for the week and that 4.8 is the current average number of the entire history completions per week for this goal. This history is displayed in the details panel.
-
-In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
-- walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
-- wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
-- interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
-
-This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
-- F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
-- ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
-
-A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
+All the normal commands are available and, additionally, these commands are available when a goal is selected:
+- F:  increment the completion count for the current period (by incrementing the count for the current period in @h).
+- ^a: toggle the active/paused status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *paused* and are displayed in a separate category. 
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of periods that has expired) are regarded as *ended* and are also displayed in a separate category. A *goal* could, of course, be deleted but this would also delete the history of completions. 
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and the elapsed time and *state* of the associated timer.
 
@@ -1904,14 +1895,15 @@
 *  @j*: job summary. string, optionally followed by job &key entries
 *  @k*: doc_id. connect this reminder to the one corresponding to doc_id.
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep. Defaults to (k) keep.
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
+*  @q: quota. Used to specify the attributes of a goal. E.g., @q 3m, 2 would specify a goal of 3 completions per (m)onth for 2 months. Other period options include (y)ear, (q)uarter and (w)eek. Week is the default. The default for the number of periods is 0 which entails repeating indefinitely.
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
 *  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
```

### Comparing `etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.3.1/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.3.1/etm_dgraham.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 etm/data.py
 etm/make_examples.py
 etm/model.py
 etm/options.py
 etm/report.py
 etm/rrule-test.py
 etm/rruleset-test.py
+etm/simulate_time_passage.py
 etm/view.py
 etm_dgraham.egg-info/PKG-INFO
 etm_dgraham.egg-info/PKG-INFO [conflicted]
 etm_dgraham.egg-info/SOURCES [conflicted].txt
 etm_dgraham.egg-info/SOURCES.txt
 etm_dgraham.egg-info/dependency_links.txt
 etm_dgraham.egg-info/entry_points.txt
```

### Comparing `etm-dgraham-6.3.0/etmlogo.png` & `etm-dgraham-6.3.1/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etmlogo_small.png` & `etm-dgraham-6.3.1/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/etmview_agenda.png` & `etm-dgraham-6.3.1/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/namedcolors.py` & `etm-dgraham-6.3.1/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/new.png` & `etm-dgraham-6.3.1/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/setup.py` & `etm-dgraham-6.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/test/test_parser.py` & `etm-dgraham-6.3.1/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/utilities/colons_to_slashes.py` & `etm-dgraham-6.3.1/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/utilities/etm_in` & `etm-dgraham-6.3.1/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/utilities/inbasket` & `etm-dgraham-6.3.1/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.3.0/utilities/open_in_mutt` & `etm-dgraham-6.3.1/utilities/open_in_mutt`

 * *Files identical despite different names*

