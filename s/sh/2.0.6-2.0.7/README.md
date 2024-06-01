# Comparing `tmp/sh-2.0.6.tar.gz` & `tmp/sh-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-2.0.6.tar", max compression
+gzip compressed data, was "sh-2.0.7.tar", max compression
```

## Comparing `sh-2.0.6.tar` & `sh-2.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    17409 2023-08-10 01:31:12.504134 sh-2.0.6/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-08-10 01:31:12.504134 sh-2.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2842 2023-08-10 01:31:12.504134 sh-2.0.6/MIGRATION.md
--rw-r--r--   0        0        0      452 2023-08-10 01:31:12.504134 sh-2.0.6/Makefile
--rw-r--r--   0        0        0     2109 2023-08-10 01:31:12.504134 sh-2.0.6/README.rst
--rw-r--r--   0        0        0    32464 2023-08-10 01:31:12.508134 sh-2.0.6/images/logo-230.png
--rw-r--r--   0        0        0   246823 2023-08-10 01:31:12.508134 sh-2.0.6/images/logo-big.png
--rw-r--r--   0        0        0     1827 2023-08-10 01:31:12.508134 sh-2.0.6/pyproject.toml
--rw-r--r--   0        0        0   126947 2023-08-10 01:31:12.508134 sh-2.0.6/sh.py
--rw-r--r--   0        0        0      962 2023-08-10 01:31:12.508134 sh-2.0.6/tests/Dockerfile
--rw-r--r--   0        0        0        0 2023-08-10 01:31:12.508134 sh-2.0.6/tests/__init__.py
--rw-r--r--   0        0        0    90975 2023-08-10 01:31:12.508134 sh-2.0.6/tests/sh_test.py
--rw-r--r--   0        0        0      548 2023-08-10 01:31:12.508134 sh-2.0.6/tox.ini
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 sh-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0    17527 2024-06-01 16:36:44.916450 sh-2.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2024-06-01 16:36:44.916450 sh-2.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     2842 2024-06-01 16:36:44.916450 sh-2.0.7/MIGRATION.md
+-rw-r--r--   0        0        0      452 2024-06-01 16:36:44.916450 sh-2.0.7/Makefile
+-rw-r--r--   0        0        0     2109 2024-06-01 16:36:44.916450 sh-2.0.7/README.rst
+-rw-r--r--   0        0        0    32464 2024-06-01 16:36:44.920450 sh-2.0.7/images/logo-230.png
+-rw-r--r--   0        0        0   246823 2024-06-01 16:36:44.920450 sh-2.0.7/images/logo-big.png
+-rw-r--r--   0        0        0     1827 2024-06-01 16:36:44.920450 sh-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0   126807 2024-06-01 16:36:44.920450 sh-2.0.7/sh.py
+-rw-r--r--   0        0        0      962 2024-06-01 16:36:44.920450 sh-2.0.7/tests/Dockerfile
+-rw-r--r--   0        0        0        0 2024-06-01 16:36:44.920450 sh-2.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    90905 2024-06-01 16:36:44.920450 sh-2.0.7/tests/sh_test.py
+-rw-r--r--   0        0        0      548 2024-06-01 16:36:44.920450 sh-2.0.7/tox.ini
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 sh-2.0.7/PKG-INFO
```

### Comparing `sh-2.0.6/CHANGELOG.md` & `sh-2.0.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 2.0.7 - 5/31/24
+
+- Fix `sh.glob` arguments [#708](https://github.com/amoffat/sh/issues/708)
+- Misc modernizations
+
 ## 2.0.6 - 8/9/23
 
 - Add back appropriate sdist files [comment](https://github.com/amoffat/sh/commit/89333ae48069a5b445b3535232195b2de6f4648f)
 
 ## 2.0.5 - 8/7/23
 
 - Allow nested `with` contexts [#690](https://github.com/amoffat/sh/issues/690)
```

### Comparing `sh-2.0.6/LICENSE.txt` & `sh-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/MIGRATION.md` & `sh-2.0.7/MIGRATION.md`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/README.rst` & `sh-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/images/logo-230.png` & `sh-2.0.7/images/logo-230.png`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/images/logo-big.png` & `sh-2.0.7/images/logo-big.png`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/pyproject.toml` & `sh-2.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sh"
-version = "2.0.6"
+version = "2.0.7"
 description = "Python subprocess replacement"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 readme = "README.rst"
 maintainers = [
     "Andrew Moffat <arwmoffat@gmail.com>",
     "Erik Cederstrand <erik@cederstrand.dk>"
 ]
```

### Comparing `sh-2.0.6/sh.py` & `sh-2.0.7/sh.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # ===============================================================================
 import asyncio
 from collections import deque
 
 try:
     from collections.abc import Mapping
 except ImportError:  # pragma: no cover
-    from collections import Mapping
+    from collections.abc import Mapping
 
 import errno
 import fcntl
 import gc
 import getpass
 import glob as glob_module
 import inspect
@@ -102,24 +102,24 @@
 PUSHD_LOCK = threading.RLock()
 
 
 def get_num_args(fn):
     return len(inspect.getfullargspec(fn).args)
 
 
-_unicode_methods = set(dir(str()))
+_unicode_methods = set(dir(""))
 
 HAS_POLL = hasattr(select, "poll")
 POLLER_EVENT_READ = 1
 POLLER_EVENT_WRITE = 2
 POLLER_EVENT_HUP = 4
 POLLER_EVENT_ERROR = 8
 
 
-class PollPoller(object):
+class PollPoller:
     def __init__(self):
         self._poll = select.poll()
         # file descriptor <-> file object bidirectional maps
         self.fd_lookup = {}
         self.fo_lookup = {}
 
     def __nonzero__(self):
@@ -187,15 +187,15 @@
             elif events & select.POLLHUP:
                 results.append((f, POLLER_EVENT_HUP))
             elif events & (select.POLLERR | select.POLLNVAL):
                 results.append((f, POLLER_EVENT_ERROR))
         return results
 
 
-class SelectPoller(object):
+class SelectPoller:
     def __init__(self):
         self.rlist = []
         self.wlist = []
         self.xlist = []
 
     def __nonzero__(self):
         return len(self.rlist) + len(self.wlist) + len(self.xlist) != 0
@@ -267,15 +267,15 @@
     subclass of ErrorReturnCode from another module.  this is mostly necessary
     in the tests, where we do assertRaises, but the ErrorReturnCode that the
     program we're testing throws may not be the same class that we pass to
     assertRaises
     """
 
     def __subclasscheck__(self, o):
-        other_bases = set([b.__name__ for b in o.__bases__])
+        other_bases = {b.__name__ for b in o.__bases__}
         return self.__name__ in other_bases or o.__name__ == self.__name__
 
 
 class ErrorReturnCode(Exception):
     __metaclass__ = ErrorReturnCodeMeta
 
     """ base class for all exceptions as a result of a command's exit status
@@ -326,15 +326,15 @@
 
         msg = (
             f"\n\n  RAN: {self.full_cmd}"
             f"\n\n  STDOUT:\n{exc_stdout.decode(DEFAULT_ENCODING, 'replace')}"
             f"\n\n  STDERR:\n{exc_stderr.decode(DEFAULT_ENCODING, 'replace')}"
         )
 
-        super(ErrorReturnCode, self).__init__(msg)
+        super().__init__(msg)
 
 
 class SignalException(ErrorReturnCode):
     pass
 
 
 class TimeoutException(Exception):
@@ -368,17 +368,17 @@
 class CommandNotFound(AttributeError):
     pass
 
 
 rc_exc_regex = re.compile(r"(ErrorReturnCode|SignalException)_((\d+)|SIG[a-zA-Z]+)")
 rc_exc_cache: Dict[str, Type[ErrorReturnCode]] = {}
 
-SIGNAL_MAPPING = dict(
-    [(v, k) for k, v in signal.__dict__.items() if re.match(r"SIG[a-zA-Z]+", k)]
-)
+SIGNAL_MAPPING = {
+    v: k for k, v in signal.__dict__.items() if re.match(r"SIG[a-zA-Z]+", k)
+}
 
 
 def get_exc_from_name(name):
     """takes an exception name, like:
 
         ErrorReturnCode_1
         SignalException_9
@@ -453,20 +453,20 @@
 
 class GlobResults(list):
     def __init__(self, path, results):
         self.path = path
         list.__init__(self, results)
 
 
-def glob(path, recursive=False):
-    expanded = GlobResults(path, _old_glob(path, recursive=recursive))
+def glob(path, *args, **kwargs):
+    expanded = GlobResults(path, _old_glob(path, *args, **kwargs))
     return expanded
 
 
-glob_module.glob = glob
+glob_module.glob = glob  # type: ignore
 
 
 def canonicalize(path):
     return os.path.abspath(os.path.expanduser(path))
 
 
 def _which(program, paths=None):
@@ -532,15 +532,15 @@
     if path:
         cmd = command_cls(path)
         if baked_args:
             cmd = cmd.bake(**baked_args)
     return cmd
 
 
-class Logger(object):
+class Logger:
     """provides a memory-inexpensive logger.  a gotcha about python's builtin
     logger is that logger objects are never garbage collected.  if you create a
     thousand loggers with unique names, they'll sit there in memory until your
     script is done.  with sh, it's easy to create loggers with unique names if
     we want our loggers to include our command arguments.  for example, these
     are all unique loggers:
 
@@ -592,15 +592,15 @@
     if pid:
         s = f"<Command {cmd!r}, pid {pid}>"
     else:
         s = f"<Command {cmd!r}>"
     return s
 
 
-class RunningCommand(object):
+class RunningCommand:
     """this represents an executing Command object.  it is returned as the
     result of __call__() being executed on a Command instance.  this creates a
     reference to a OProc instance, which is a low-level wrapper around the
     process that was exec'd
 
     this is the class that gets manipulated the most by user code, and so it
     implements various convenience methods and logical mechanisms for the
@@ -1154,15 +1154,15 @@
             invalid.append(("env", f"env key {k!r} must be a str"))
         if not isinstance(v, str):
             invalid.append(("env", f"value {v!r} of env key {k!r} must be a str"))
 
     return invalid
 
 
-class Command(object):
+class Command:
     """represents an un-run system program, like "ls" or "cd".  because it
     represents the program itself (and not a running instance of it), it should
     hold very little state.  in fact, the only state it does hold is baked
     arguments.
 
     when a Command object is called, the result that is returned is a
     RunningCommand object, which represents the Command put into an execution
@@ -1769,15 +1769,15 @@
                 raise
         else:
             break
 
     return ret
 
 
-class OProc(object):
+class OProc:
     """this class is instantiated by RunningCommand for a command to be exec'd.
     it handles all the nasty business involved with correctly setting up the
     input/output to the child process.  it gets its name for subprocess.Popen
     (process open) but we're calling ours OProc (open process)"""
 
     _default_window_size = (24, 80)
 
@@ -2084,20 +2084,20 @@
                 if close_fds:
                     pass_fds = {0, 1, 2, exc_pipe_write}
                     pass_fds.update(ca["pass_fds"])
 
                     # don't inherit file descriptors
                     try:
                         inherited_fds = os.listdir("/dev/fd")
-                    except (IOError, OSError):
+                    except OSError:
                         # Some systems don't have /dev/fd. Raises OSError in
                         # Python2, FileNotFoundError on Python3. The latter doesn't
                         # exist on Python2, but inherits from IOError, which does.
                         inherited_fds = os.listdir("/proc/self/fd")
-                    inherited_fds = set(int(fd) for fd in inherited_fds) - pass_fds
+                    inherited_fds = {int(fd) for fd in inherited_fds} - pass_fds
                     for fd in inherited_fds:
                         try:
                             os.close(fd)
                         except OSError:
                             pass
 
                 # python=3.6, locale=c will fail test_unicode_arg if we don't
@@ -2866,15 +2866,15 @@
     # or buffered by specific amount
     else:
         bufsize = bf_type
 
     return bufsize
 
 
-class StreamWriter(object):
+class StreamWriter:
     """StreamWriter reads from some input (the stdin param) and writes to a fd
     (the stream param).  the stdin may be a Queue, a callable, something with
     the "read" method, a string, or an iterable"""
 
     def __init__(self, log, stream, stdin, bufsize_type, encoding, tty_in):
         self.stream = stream
         self.stdin = stdin
@@ -3069,15 +3069,15 @@
 
     def finish():
         pass
 
     return process, finish
 
 
-class StreamReader(object):
+class StreamReader:
     """reads from some output (the stream) and sends what it just read to the
     handler."""
 
     def __init__(
         self,
         log,
         stream,
@@ -3156,15 +3156,15 @@
             return True
 
         self.log.debug("got chunk size %d: %r", len(chunk), chunk[:30])
         for chunk in self.stream_bufferer.process(chunk):
             self.write_chunk(chunk)
 
 
-class StreamBufferer(object):
+class StreamBufferer:
     """this is used for feeding in chunks of stdout/stderr, and breaking it up
     into chunks that will actually be put into the internal buffers.  for
     example, if you have two processes, one being piped to the other, and you
     want that, first process to feed lines of data (instead of the chunks
     however they come in), OProc will use an instance of this class to chop up
     the data and feed it as lines to be sent down the pipe"""
 
@@ -3502,15 +3502,15 @@
     return cmd
 
 
 @contrib("ssh")
 def ssh(orig):  # pragma: no cover
     """An ssh command for automatic password login"""
 
-    class SessionContent(object):
+    class SessionContent:
         def __init__(self):
             self.chars = deque(maxlen=50000)
             self.lines = deque(maxlen=5000)
             self.line_chars = []
             self.last_line = ""
             self.cur_char = ""
 
@@ -3527,15 +3527,15 @@
             self.cur_char = char
 
         @property
         def cur_line(self):
             line = "".join(self.line_chars)
             return line
 
-    class SSHInteract(object):
+    class SSHInteract:
         def __init__(self, prompt_match, pass_getter, out_handler, login_success):
             self.prompt_match = prompt_match
             self.pass_getter = pass_getter
             self.out_handler = out_handler
             self.login_success = login_success
             self.content = SessionContent()
 
@@ -3622,15 +3622,15 @@
 # import lookup to our Environment class
 class SelfWrapper(ModuleType):
     def __init__(self, self_module, baked_args=None):
         # this is super ugly to have to copy attributes like this,
         # but it seems to be the only way to make reload() behave
         # nicely.  if i make these attributes dynamic lookups in
         # __getattr__, reload sometimes chokes in weird ways...
-        super(SelfWrapper, self).__init__(
+        super().__init__(
             name=getattr(self_module, "__name__", None),
             doc=getattr(self_module, "__doc__", None),
         )
         for attr in ["__builtins__", "__file__", "__package__"]:
             setattr(self, attr, getattr(self_module, attr, None))
 
         # python 3.2 (2.7 and 3.3 work fine) breaks on osx (not ubuntu)
```

### Comparing `sh-2.0.6/tests/Dockerfile` & `sh-2.0.7/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/tests/sh_test.py` & `sh-2.0.7/tests/sh_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf8 -*-
 import asyncio
 import errno
 import fcntl
 import inspect
 import logging
 import os
 import platform
@@ -442,15 +441,15 @@
     sys.stdout.write(chr(ord(letter)+1))
 """
         )
 
         def inc(*args, **kwargs):
             return python("-u", inc_py.name, *args, **kwargs)
 
-        class Derp(object):
+        class Derp:
             def __init__(self):
                 self.times = []
                 self.stdout = []
                 self.last_received = None
 
             def agg(self, line):
                 self.stdout.append(line.strip())
@@ -791,15 +790,15 @@
             os.chmod(gcc_file2, int(0o755))
 
             from sh import gcc
 
             self.assertEqual(gcc._path, gcc_file2)
             self.assertEqual(
                 gcc("no-error", _return_cmd=True).stdout.strip(),
-                "no-error".encode("ascii"),
+                b"no-error",
             )
 
         finally:
             os.environ["PATH"] = save_path
             if exists(gcc_file2):
                 os.unlink(gcc_file2)
             if exists(gcc_dir1):
@@ -2304,15 +2303,15 @@
         py = create_tmp_test(
             """
 import sys
 sys.stdout.write("line1")
 """
         )
 
-        class Callable(object):
+        class Callable:
             def __init__(self):
                 self.line = None
 
             def __call__(self, line):
                 self.line = line
 
         cb = Callable()
@@ -2643,15 +2642,15 @@
         ll = ls.bake("-l")
         self.assertTrue(str(ll).endswith("/ls -l"))
 
     # https://github.com/amoffat/sh/issues/185
     def test_done_callback(self):
         import time
 
-        class Callback(object):
+        class Callback:
             def __init__(self):
                 self.called = False
                 self.exit_code = None
                 self.success = None
 
             def __call__(self, p, success, exit_code):
                 self.called = True
@@ -2788,15 +2787,15 @@
         self.assertTrue(event.is_set())
 
         event.clear()
 
     def test_done_cb_exc(self):
         from sh import ErrorReturnCode
 
-        class Callback(object):
+        class Callback:
             def __init__(self):
                 self.called = False
                 self.success = None
 
             def __call__(self, p, success, exit_code):
                 self.success = success
                 self.called = True
```

### Comparing `sh-2.0.6/tox.ini` & `sh-2.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `sh-2.0.6/PKG-INFO` & `sh-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python subprocess replacement
 Home-page: https://sh.readthedocs.io/
 License: MIT
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
 Maintainer-email: arwmoffat@gmail.com
@@ -15,14 +15,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://sh.readthedocs.io/
 Project-URL: Repository, https://github.com/amoffat/sh
```

