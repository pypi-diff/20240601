# Comparing `tmp/beaker_gantry-1.2.0.tar.gz` & `tmp/beaker_gantry-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaker_gantry-1.2.0.tar", last modified: Fri May 31 03:08:17 2024, max compression
+gzip compressed data, was "beaker_gantry-1.3.0.tar", last modified: Fri May 31 18:33:42 2024, max compression
```

## Comparing `beaker_gantry-1.2.0.tar` & `beaker_gantry-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/beaker_gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 03:08:17.000000 beaker_gantry-1.2.0/beaker_gantry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/gantry/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:08:17.026273 beaker_gantry-1.2.0/gantry/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/follow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/commands/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/gantry/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-31 03:07:56.000000 beaker_gantry-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:08:17.030273 beaker_gantry-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:33:42.791047 beaker_gantry-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-05-31 18:33:42.787047 beaker_gantry-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:33:42.787047 beaker_gantry-1.3.0/beaker_gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27368 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 18:33:42.000000 beaker_gantry-1.3.0/beaker_gantry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:33:42.787047 beaker_gantry-1.3.0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:33:42.787047 beaker_gantry-1.3.0/gantry/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/follow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/commands/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/gantry/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-31 18:33:14.000000 beaker_gantry-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:33:42.791047 beaker_gantry-1.3.0/setup.cfg
```

### Comparing `beaker_gantry-1.2.0/LICENSE` & `beaker_gantry-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/PKG-INFO` & `beaker_gantry-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.2.0
+Version: 1.3.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beaker-py<2.0,>=1.26.13
+Requires-Dist: beaker-py<2.0,>=1.27.0
 Requires-Dist: GitPython<4.0,>=3.0
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: click-help-colors
 Requires-Dist: petname<3.0,>=2.6
 Requires-Dist: requests
 Requires-Dist: packaging
```

### Comparing `beaker_gantry-1.2.0/README.md` & `beaker_gantry-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/beaker_gantry.egg-info/PKG-INFO` & `beaker_gantry-1.3.0/beaker_gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 1.2.0
+Version: 1.3.0
 Summary: Gantry streamlines running Python experiments in Beaker by managing containers and boilerplate for you
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Pete Walsh <petew@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,15 +210,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beaker-py<2.0,>=1.26.13
+Requires-Dist: beaker-py<2.0,>=1.27.0
 Requires-Dist: GitPython<4.0,>=3.0
 Requires-Dist: rich
 Requires-Dist: click
 Requires-Dist: click-help-colors
 Requires-Dist: petname<3.0,>=2.6
 Requires-Dist: requests
 Requires-Dist: packaging
```

### Comparing `beaker_gantry-1.2.0/beaker_gantry.egg-info/SOURCES.txt` & `beaker_gantry-1.3.0/beaker_gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/commands/cluster.py` & `beaker_gantry-1.3.0/gantry/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/commands/config.py` & `beaker_gantry-1.3.0/gantry/commands/config.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/commands/list.py` & `beaker_gantry-1.3.0/gantry/commands/list.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/commands/main.py` & `beaker_gantry-1.3.0/gantry/commands/main.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/commands/run.py` & `beaker_gantry-1.3.0/gantry/commands/run.py`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/entrypoint.sh` & `beaker_gantry-1.3.0/gantry/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `beaker_gantry-1.2.0/gantry/util.py` & `beaker_gantry-1.3.0/gantry/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import tempfile
 import time
-from datetime import datetime
+from datetime import datetime, timedelta
 from enum import Enum
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Optional, Tuple, Union, cast
+from typing import Optional, Tuple, cast
 
 import requests
 import rich
 from beaker import (
     Beaker,
     Dataset,
     DatasetConflict,
     DatasetNotFound,
     Digest,
     Experiment,
     Job,
-    JobTimeoutError,
     SecretNotFound,
     WorkspaceNotSet,
 )
 from rich import print, prompt
 from rich.console import Console
 
 from . import constants
 from .constants import GITHUB_TOKEN_SECRET
 from .exceptions import *
 from .version import VERSION
 
-if TYPE_CHECKING:
-    from datetime import timedelta
-
 
 class StrEnum(str, Enum):
     def __str__(self) -> str:
         return self.value
 
 
 def unique_name() -> str:
@@ -70,87 +66,50 @@
             .split("/")
         )
     except ValueError:
         raise InvalidRemoteError(f"Failed to parse GitHub repo path from remote '{url}'")
     return account, repo
 
 
-def display_logs(logs: Iterable[bytes], ignore_timestamp: Optional[str] = None) -> Optional[str]:
+def follow_experiment(
+    beaker: Beaker, experiment: Experiment, timeout: int = 0, tail: bool = False
+) -> Job:
     console = rich.get_console()
-    latest_timestamp: Optional[str] = None
-
-    def print_line(line: str):
-        if not line:
-            return
-        nonlocal latest_timestamp
-        # Remove timestamp
-        try:
-            timestamp, line = line.split("Z ", maxsplit=1)
-            latest_timestamp = f"{timestamp}Z"
-            if ignore_timestamp is not None and latest_timestamp == ignore_timestamp:
-                return
-        except ValueError:
-            pass
-        console.print(line, highlight=False, markup=False)
-
-    line_buffer = ""
-    for bytes_chunk in logs:
-        chunk = line_buffer + bytes_chunk.decode(errors="ignore")
-        chunk = chunk.replace("\r", "\n")
-        lines = chunk.split("\n")
-        if chunk.endswith("\n"):
-            line_buffer = ""
-        else:
-            # Last line chunk is probably incomplete.
-            lines, line_buffer = lines[:-1], lines[-1]
-        for line in lines:
-            print_line(line)
-
-    print_line(line_buffer)
-    return latest_timestamp
-
-
-def follow_experiment(beaker: Beaker, experiment: Experiment, timeout: int = 0) -> Job:
-    start = time.monotonic()
 
     # Wait for job to start...
     job: Optional[Job] = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
     if job is None:
         print("Waiting for job to launch..", end="")
         while job is None:
             time.sleep(1.0)
             print(".", end="")
             job = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
 
     exit_code: Optional[int] = job.status.exit_code
 
-    stream_logs = exit_code is None
+    stream_logs = exit_code is None and not job.is_finalized
     if stream_logs:
         print()
         rich.get_console().rule("Logs")
-
-    last_timestamp: Optional[str] = None
-    since: Optional[Union[str, datetime]] = datetime.utcnow()
-    while stream_logs and exit_code is None and not job.is_finalized:
-        job = beaker.experiment.tasks(experiment.id)[0].latest_job  # type: ignore
-        assert job is not None
-        exit_code = job.status.exit_code
-        last_timestamp = display_logs(
-            beaker.job.logs(job, quiet=True, since=since),
-            ignore_timestamp=last_timestamp,
-        )
-        since = last_timestamp or since
-        time.sleep(2.0)
-        if timeout > 0 and time.monotonic() - start >= timeout:
-            raise JobTimeoutError(f"Job did not finish within {timeout} seconds")
-
-    if stream_logs:
+        for line_bytes in beaker.job.follow(
+            job,
+            timeout=timeout if timeout > 0 else None,
+            include_timestamps=False,
+            since=datetime.utcnow() - timedelta(seconds=5) if tail else None,
+        ):
+            line = line_bytes.decode(errors="ignore")
+            if line.endswith("\n"):
+                line = line[:-1]
+            console.print(line, highlight=False, markup=False)
         rich.get_console().rule("End logs")
         print()
 
+        # Refresh the job.
+        job = beaker.job.get(job.id)
+
     return job
 
 
 def display_results(beaker: Beaker, experiment: Experiment, job: Job):
     exit_code = job.status.exit_code
     if exit_code is None:
         raise ExperimentFailedError("Experiment failed")
```

### Comparing `beaker_gantry-1.2.0/pyproject.toml` & `beaker_gantry-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 authors = [
     { name = "Allen Institute for Artificial Intelligence", email = "contact@allenai.org" },
     { name = "Pete Walsh", email = "petew@allenai.org" },
 ]
 license = {file = "LICENSE"}
 requires-python = ">3.7"
 dependencies = [
-    "beaker-py>=1.26.13,<2.0",
+    "beaker-py>=1.27.0,<2.0",
     "GitPython>=3.0,<4.0",
     "rich",
     "click",
     "click-help-colors",
     "petname>=2.6,<3.0",
     "requests",
     "packaging",
```

