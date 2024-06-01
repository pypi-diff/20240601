# Comparing `tmp/slurmtui-0.1.5.tar.gz` & `tmp/slurmtui-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmtui-0.1.5.tar", last modified: Sat Jun  1 10:50:17 2024, max compression
+gzip compressed data, was "slurmtui-0.1.6.tar", last modified: Sat Jun  1 11:21:45 2024, max compression
```

## Comparing `slurmtui-0.1.5.tar` & `slurmtui-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:17.843505 slurmtui-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 10:50:14.000000 slurmtui-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 10:50:17.839505 slurmtui-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-06-01 10:50:14.000000 slurmtui-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:50:17.843505 slurmtui-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-01 10:50:14.000000 slurmtui-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:17.839505 slurmtui-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:17.839505 slurmtui-0.1.5/src/slurmtui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:14.000000 slurmtui-0.1.5/src/slurmtui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:17.839505 slurmtui-0.1.5/src/slurmtui/css/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-01 10:50:14.000000 slurmtui-0.1.5/src/slurmtui/css/slurmtui.css
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-06-01 10:50:14.000000 slurmtui-0.1.5/src/slurmtui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-06-01 10:50:14.000000 slurmtui-0.1.5/src/slurmtui/slurm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 10:50:14.000000 slurmtui-0.1.5/src/slurmtui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:50:17.839505 slurmtui-0.1.5/src/slurmtui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 10:50:17.000000 slurmtui-0.1.5/src/slurmtui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:45.640988 slurmtui-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 11:21:42.000000 slurmtui-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 11:21:45.640988 slurmtui-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-06-01 11:21:42.000000 slurmtui-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:21:45.640988 slurmtui-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-01 11:21:42.000000 slurmtui-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:45.636988 slurmtui-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:45.636988 slurmtui-0.1.6/src/slurmtui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:42.000000 slurmtui-0.1.6/src/slurmtui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:45.636988 slurmtui-0.1.6/src/slurmtui/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-01 11:21:42.000000 slurmtui-0.1.6/src/slurmtui/css/slurmtui.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-06-01 11:21:42.000000 slurmtui-0.1.6/src/slurmtui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-06-01 11:21:42.000000 slurmtui-0.1.6/src/slurmtui/slurm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 11:21:42.000000 slurmtui-0.1.6/src/slurmtui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:21:45.640988 slurmtui-0.1.6/src/slurmtui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 11:21:45.000000 slurmtui-0.1.6/src/slurmtui.egg-info/top_level.txt
```

### Comparing `slurmtui-0.1.5/LICENSE` & `slurmtui-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.5/PKG-INFO` & `slurmtui-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmtui
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple Terminal UI (TUI) for Slurm
 Home-page: https://github.com/WissamAntoun/SlurmTUI
 Author: Wissam Antoun
 Author-email: wissam.antoun@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `slurmtui-0.1.5/README.md` & `slurmtui-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.5/setup.py` & `slurmtui-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = f.read()
 
     return long_description
 
 
 setup(
     name="slurmtui",
-    version="0.1.5",
+    version="0.1.6",
     author="Wissam Antoun",
     author_email="wissam.antoun@gmail.com",
     description="A simple Terminal UI (TUI) for Slurm",
     long_description=get_long_description().replace(
         "./img/screenshot.png",
         "https://raw.githubusercontent.com/WissamAntoun/SlurmTUI/main/img/screenshot.png",
     ),
```

### Comparing `slurmtui-0.1.5/src/slurmtui/css/slurmtui.css` & `slurmtui-0.1.6/src/slurmtui/css/slurmtui.css`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.5/src/slurmtui/main.py` & `slurmtui-0.1.6/src/slurmtui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,20 @@
         self.action = action
         self.extra = extra
 
 
 class SlurmTUI(App[SlurmTUIReturn]):
     """A Textual UI for slurm jobs."""
 
+    DEFAULT_CSS = """
+        DataTable {
+            scrollbar-gutter: stable;
+        }
+    """
+
     CSS_PATH = "css/slurmtui.css"
 
     BINDINGS = [
         ("l", "logs_out", "Logs (STDOUT)"),
         ("e", "logs_err", "Logs (STDERR)"),
         ("c", "connect", "Connect to Node (ssh)"),
         ("i", "info", "Info"),
@@ -225,19 +231,19 @@
         old_cursor = job_table.cursor_coordinate
 
         job_table.clear()
         if self.first_display:
             job_table.cursor_type = "row"
             job_table.add_columns(
                 "Job id",
-                "Array ID",
-                "Array Index",
+                "Arr. ID",
+                "Arr. Idx",
                 "Name",
                 "Node Name",
-                "partition",
+                "Partition",
                 "Start/Sub. Time",
                 "End Time",
                 "State",
                 "State Reason",
                 "Account",
             )
             self.first_display = False
@@ -424,31 +430,35 @@
 
     def _delete_job(self, selected_job: Dict[str, Any], delete_array=False) -> None:
         if delete_array:
             self.jobs_to_be_deleted.extend(
                 [
                     job["job_id"]
                     for job in self.running_jobs_dict.values()
-                    if job["array_job_id"]["number"] == selected_job["array_job_id"]["number"]
+                    if job["array_job_id"]["number"]
+                    == selected_job["array_job_id"]["number"]
                 ]
             )
         else:
             self.jobs_to_be_deleted.append(selected_job["job_id"])
         if not self.mock:
             if delete_array:
-                os.system(f"scancel --array {selected_job["array_job_id"]["number"]}")
+                os.system(f"scancel --array {selected_job['array_job_id']['number']}")
             else:
                 os.system(f"scancel {selected_job['job_id']}")
 
     def _check_job_is_array(self, selected_job: Dict[str, Any]) -> bool:
         """Check if the selected job is an array job."""
 
         if selected_job["array_job_id"]["number"] == 0:
             return False
-        elif selected_job["array_task_id"]["number"] > 1 or selected_job["array_job_id"]["number"] != selected_job["job_id"]:
+        elif (
+            selected_job["array_task_id"]["number"] > 1
+            or selected_job["array_job_id"]["number"] != selected_job["job_id"]
+        ):
             return True
 
         return False
 
     def action_delete(self) -> None:
         """Delete the job."""
         if self._check_no_jobs():
```

### Comparing `slurmtui-0.1.5/src/slurmtui/slurm_utils.py` & `slurmtui-0.1.6/src/slurmtui/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `slurmtui-0.1.5/src/slurmtui.egg-info/PKG-INFO` & `slurmtui-0.1.6/src/slurmtui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmtui
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple Terminal UI (TUI) for Slurm
 Home-page: https://github.com/WissamAntoun/SlurmTUI
 Author: Wissam Antoun
 Author-email: wissam.antoun@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

