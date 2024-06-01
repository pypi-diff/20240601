# Comparing `tmp/atpbar-2.0.1.tar.gz` & `tmp/atpbar-2.0.2.tar.gz`

## Comparing `atpbar-2.0.1.tar` & `atpbar-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/__about__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/__init__.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/funcs.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/machine.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/py.typed
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/stream.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/__init__.py
--rwxr-xr-x   0        0        0     3692 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/barjupyter.py
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/bartty.py
--rwxr-xr-x   0        0        0     3140 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/base.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/create.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/txtprint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/jupy.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/spy.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/__init__.py
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/complement.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/pickup.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/report.py
--rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/reporter.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 atpbar-2.0.1/.gitignore
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 atpbar-2.0.1/LICENSE
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 atpbar-2.0.1/README.md
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 atpbar-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 atpbar-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/__about__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/funcs.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/machine.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/py.typed
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/stream.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/__init__.py
+-rwxr-xr-x   0        0        0     3758 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/barjupyter.py
+-rwxr-xr-x   0        0        0     3503 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/bartty.py
+-rwxr-xr-x   0        0        0     3185 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/base.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/create.py
+-rwxr-xr-x   0        0        0     1637 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/txtprint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/detect/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/detect/jupy.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/presentation/detect/spy.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/progress_report/__init__.py
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/progress_report/complement.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/progress_report/pickup.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/progress_report/report.py
+-rwxr-xr-x   0        0        0     2894 2020-02-02 00:00:00.000000 atpbar-2.0.2/atpbar/progress_report/reporter.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 atpbar-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 atpbar-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 atpbar-2.0.2/README.md
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 atpbar-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 atpbar-2.0.2/PKG-INFO
```

### Comparing `atpbar-2.0.1/atpbar/funcs.py` & `atpbar-2.0.2/atpbar/funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import atexit
 import contextlib
 import multiprocessing
 from collections.abc import Iterator
 
 from .machine import StateMachine
-from .progressreport import ProgressReporter
+from .progress_report import ProgressReporter
 
 _machine = StateMachine()
 
 
 def find_reporter() -> ProgressReporter | None:
-    """returns the progress reporter
+    '''returns the progress reporter
 
     This function is to be called in the main process of a
     multiprocessing program. The reporter should be registered in
     sub-processes with the function `register_reporter()`
 
     Returns
     -------
     object
         The progress reporter
 
-    """
+    '''
     return _machine.find_reporter()
 
 
 def register_reporter(reporter: ProgressReporter) -> None:
-    """registers a reporter
+    '''registers a reporter
 
     This function is to be called in sub-processes of a
     multiprocessing program.
 
     Parameters
     ----------
     reporter : object
@@ -38,63 +38,63 @@
         `find_reporter()`
 
 
     Returns
     -------
     None
 
-    """
+    '''
     _machine.register_reporter(reporter)
 
 
 def flush() -> None:
-    """flushes progress bars
+    '''flushes progress bars
 
     This function flushes all active progress bars. It returns when
     the progress bars finish updating.
 
     Returns
     -------
     None
 
-    """
+    '''
     _machine.flush()
 
 
 @contextlib.contextmanager
 def flushing() -> Iterator[None]:
     '''Flushes progress bars on exit'''
     try:
         yield
     finally:
         flush()
 
 
 def disable() -> None:
-    """disables progress bars
+    '''disables progress bars
 
     This function needs to be called in the main process before
     `atpbar()` or `find_reporter()` is used.
 
     Returns
     -------
     None
 
-    """
+    '''
     _machine.disable()
 
 
 def shutdown() -> None:
-    """shutdowns the progress bars
+    '''shutdowns the progress bars
 
     Returns
     -------
     None
 
-    """
+    '''
     _machine.shutdown()
 
 
 # This import prevents the issue
 # https://github.com/alphatwirl/atpbar/issues/4
 import multiprocessing.queues  # noqa: E402 F401
```

### Comparing `atpbar-2.0.1/atpbar/machine.py` & `atpbar-2.0.2/atpbar/machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterator
 from multiprocessing import Queue
 from threading import Lock, current_thread, main_thread
 
 from .presentation import create_presentation
-from .progressreport import ProgressReporter, ProgressReportPickup, Report
+from .progress_report import ProgressReporter, ProgressReportPickup, Report
 from .stream import StreamQueue, StreamRedirection, register_stream_queue
 
 
 class StateMachine:
     def __init__(self) -> None:
         self.lock = Lock()
         self.state: State = Initial()
@@ -34,15 +34,15 @@
     def fetch_reporter(self) -> Iterator[ProgressReporter | None]:
         with self.lock:
             self.state = self.state.prepare_reporter()
         yield from self.state.fetch_reporter(lock=self.lock)
 
 
 class State:
-    """The base class of the states"""
+    '''The base class of the states'''
 
     def __init__(self) -> None:
         self.reporter: ProgressReporter | None = None
 
     def prepare_reporter(self) -> 'State':
         return self
 
@@ -59,18 +59,18 @@
         return self
 
     def shutdown(self) -> 'State':
         return self
 
 
 class Initial(State):
-    """Initial state
+    '''Initial state
 
     The pickup is not running.
-    """
+    '''
 
     def __init__(self) -> None:
         self.reporter = None
 
     def prepare_reporter(self) -> State:
         return Active()
 
@@ -78,18 +78,18 @@
         yield self.reporter
 
     def flush(self) -> State:
         return Active()
 
 
 class Active(State):
-    """Active state
+    '''Active state
 
     The pickup started and is running, typically, in the main process
-    """
+    '''
 
     def __init__(self) -> None:
 
         self.queue: Queue[Report] = Queue()
         self.notices_from_sub_processes: Queue[bool] = Queue()
         self.stream_queue: StreamQueue = Queue()
         self.reporter = ProgressReporter(
@@ -99,15 +99,15 @@
         )
 
         self.reporter_yielded = False
 
         self._start_pickup()
 
         if self.stream_redirection.disabled:
-            self.reporter.stream_redirection_enablaed = False
+            self.reporter.stream_redirection_enabled = False
 
     def _start_pickup(self) -> None:
         presentation = create_presentation()
         self.pickup = ProgressReportPickup(self.queue, presentation)
 
         self.stream_redirection = StreamRedirection(
             queue=self.stream_queue, presentation=presentation
@@ -162,39 +162,39 @@
 
     def shutdown(self) -> State:
         self._end_pickup()
         return Initial()
 
 
 class Registered(State):
-    """Registered state
+    '''Registered state
 
     Typically, in a sub-process. The reporter, which has been created
     in the main process, is registered in the sub-process
-    """
+    '''
 
     def __init__(self, reporter: ProgressReporter | None) -> None:
         self.reporter = reporter
         if reporter is None:
             return
-        if reporter.stream_redirection_enablaed:
+        if reporter.stream_redirection_enabled:
             register_stream_queue(reporter.stream_queue)
 
     def fetch_reporter(self, lock: Lock) -> Iterator[ProgressReporter | None]:
         if self.reporter is None:
             yield self.reporter
             return
 
         self.reporter.notices_from_sub_processes.put(True)
         yield self.reporter
 
 
 class Disabled(State):
-    """Disabled state"""
+    '''Disabled state'''
 
     def __init__(self) -> None:
         self.reporter = None
 
 
 def in_main_thread() -> bool:
-    """test if in the main thread"""
+    '''test if in the main thread'''
     return current_thread() == main_thread()
```

### Comparing `atpbar-2.0.1/atpbar/main.py` & `atpbar-2.0.2/atpbar/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import contextlib
 import logging
 import uuid
 from collections.abc import Iterable, Iterator
 from typing import Generic, Optional, TypeVar
 
 from .funcs import fetch_reporter
-from .progressreport import Report
+from .progress_report import Report
 
 T = TypeVar('T')
 
 
 def atpbar(iterable: Iterable[T], /, name: Optional[str] = None) -> Iterable[T]:
-    """returns an instance of `Atpbar`
+    '''returns an instance of `Atpbar`
 
     Parameters
     ----------
     iterable : iterable
         An iterable whose progress of the iterations is to be shown
     name : str
         A label to be shown on the progress bar
 
     Returns
     -------
     iterable
         An instance of `Atpbar` if successfully instantiated.
         Otherwise, the object received as the parameter `iterable`.
 
-    """
+    '''
     try:
         len_ = len(iterable)  # type: ignore
     except TypeError:
         logger = logging.getLogger(__name__)
-        logger.warning("length is unknown: {!r}".format(iterable))
-        logger.warning("atpbar is turned off")
+        logger.warning('length is unknown: {!r}'.format(iterable))
+        logger.warning('atpbar is turned off')
         return iterable
 
     if name is None:
         name = repr(iterable)
 
     return Atpbar(iterable, name=name, len_=len_)
 
 
 class Atpbar(Generic[T]):
-    """Progress bar
+    '''Progress bar
 
     An iterable that wraps another iterable and shows the progress
     bars for the iterations. The class is usually instantiated by the
     function `atpbar`.
 
     Parameters
     ----------
     iterable : iterable
         An iterable whose progress of the iterations is to be shown
     name : str
         A label to be shown on the progress bar
     len_ : int
         The length of the iterable
 
-    """
+    '''
 
     def __init__(self, iterable: Iterable[T], name: str, len_: int):
         self.iterable = iterable
         self.name = name
         self.len_ = len_
         self.id_ = uuid.uuid4()
 
@@ -94,21 +94,21 @@
             self.reporter.report(report)
         except BaseException:
             pass
 
 
 @contextlib.contextmanager
 def report_last(pbar: Atpbar[T]) -> Iterator[None]:
-    """send a last report
+    '''send a last report
 
     This function sends the last report of the task when the loop ends
     with `break` or an exception so that the progress bar will be
     updated with the last complete iteration.
 
-    """
+    '''
     try:
         yield
     finally:
         if pbar.loop_complete:
             return
         if pbar.reporter is None:
             return
```

### Comparing `atpbar-2.0.1/atpbar/stream.py` & `atpbar-2.0.2/atpbar/stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 StreamQueue: TypeAlias = 'Queue[tuple[str, FD] | None]'
 
 
 class StreamRedirection:
     def __init__(self, queue: StreamQueue, presentation: Presentation) -> None:
-        self.disabled = not presentation.stdout_stderr_redrection
+        self.disabled = not presentation.stdout_stderr_redirection
         if self.disabled:
             return
 
         self.queue = queue
         self.presentation = presentation
 
         self.stdout = Stream(self.queue, FD.STDOUT)
@@ -61,22 +61,22 @@
     sys.stderr = Stream(queue, FD.STDERR)  # type: ignore
 
 
 class Stream(TextIOBase):
     def __init__(self, queue: StreamQueue, fd: FD) -> None:
         self.fd = fd
         self.queue = queue
-        self.buffer = ""
+        self.buffer = ''
 
     def write(self, s: str) -> int:
         # sys.__stdout__.write(repr(s))
         # sys.__stdout__.write('\n')
 
         try:
-            endswith_n = s.endswith("\n")
+            endswith_n = s.endswith('\n')
         except:
             self.flush()
             self.queue.put((s, self.fd))
             return len(s)
 
         if endswith_n:
             self.buffer += s
@@ -86,15 +86,15 @@
         self.buffer += s
         return len(s)
 
     def flush(self) -> None:
         if not self.buffer:
             return
         self.queue.put((self.buffer, self.fd))
-        self.buffer = ""
+        self.buffer = ''
 
 
 class StreamPickup(threading.Thread):
     def __init__(
         self,
         queue: StreamQueue,
         stdout_write: Callable[[str], Any],
@@ -113,11 +113,11 @@
                     break
                 s, f = m
                 if f == FD.STDOUT:
                     self.stdout_write(s)
                 elif f == FD.STDERR:
                     self.stderr_write(s)
                 else:
-                    raise ValueError("unknown fd: {!r}".format(f))
+                    raise ValueError('unknown fd: {!r}'.format(f))
 
         except EOFError:
             pass
```

### Comparing `atpbar-2.0.1/atpbar/presentation/barjupyter.py` & `atpbar-2.0.2/atpbar/presentation/barjupyter.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,89 +15,90 @@
         self.active_box_list = list[widgets.HBox]()
         self.complete_box_list = list[widgets.HBox]()
         self.widget_dict = dict[
             UUID, tuple[widgets.HBox, widgets.IntProgress, widgets.HTML]
         ]()
 
     def __repr__(self) -> str:
-        return "{}()".format(self.__class__.__name__)
+        return '{}()'.format(self.__class__.__name__)
 
-    def _present(self) -> None:
+    def _present(self, report: Report) -> None:
         self._create_widgets()
         self._update_widgets()
 
     def _create_widgets(self) -> None:
         if self.container_widget is None:
             self.container_widget = widgets.VBox()
             display(self.container_widget)
 
-        for taskid in self._new_taskids:
+        for taskid in self._new_task_ids:
             report = self._report_dict[taskid]
             self._create_widget(report)
 
     def _create_widget(self, report: Report) -> None:
         bar = widgets.IntProgress(
-            value=report["done"],
+            value=report['done'],
             min=0,
-            max=report["total"],
-            description="",
-            bar_style="",  # 'success', 'info', 'warning', 'danger' or ''
-            orientation="horizontal",
+            max=report['total'],
+            description='',
+            bar_style='',  # 'success', 'info', 'warning', 'danger' or ''
+            orientation='horizontal',
         )
-        label = widgets.HTML(value="")
+        label = widgets.HTML(value='')
         box = widgets.HBox([bar, label])
         self.active_box_list.append(box)
         if self.container_widget is not None:
             self.container_widget.children = (
                 self.complete_box_list + self.active_box_list
             )
-        self.widget_dict[report["taskid"]] = (box, bar, label)
+        self.widget_dict[report['taskid']] = (box, bar, label)
 
     def _update_widgets(self) -> None:
         for taskid in (
-            self._finishing_taskids + self._active_taskids + self._new_taskids
+            self._finishing_task_ids + self._active_task_ids + self._new_task_ids
         ):
             report = self._report_dict[taskid]
             self._update_widget(report)
 
         self._reorder_widgets(report)
 
-        if not self._new_taskids and not self._active_taskids:
+        if not self._new_task_ids and not self._active_task_ids:
             self.container_widget = None
             self.active_box_list[:] = []
             self.complete_box_list[:] = []
             self.widget_dict.clear()
 
     def _update_widget(self, report: Report) -> None:
 
-        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
+        percent = float(report['done']) / report['total'] if report['total'] > 0 else 1
         percent = round(percent * 100, 2)
-        percent_fmt = "{:6.2f}%".format(percent)
+        percent_fmt = '{:6.2f}%'.format(percent)
 
-        box = self.widget_dict[report["taskid"]][0]
+        box = self.widget_dict[report['taskid']][0]
+        box  # to silence not-used warning
 
-        bar = self.widget_dict[report["taskid"]][1]
-        bar.value = report["done"]
-        bar.max = report["total"]
+        bar = self.widget_dict[report['taskid']][1]
+        bar.value = report['done']
+        bar.max = report['total']
         bar.description = percent_fmt
-        if report["last"]:
-            bar.bar_style = "success"
+        if report['last']:
+            bar.bar_style = 'success'
 
-        label = self.widget_dict[report["taskid"]][2]
+        label = self.widget_dict[report['taskid']][2]
         name_field_length = 32
-        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
-        bar = (":" * int(percent * 40)).ljust(40, " ")
+        percent = float(report['done']) / report['total'] if report['total'] > 0 else 1
+        bar = (':' * int(percent * 40)).ljust(40, ' ')
         percent = round(percent * 100, 2)
-        name = report["name"][0:name_field_length]
-        label.value = "<pre> | {:8d} / {:8d} |: {:<{}s}</pre>".format(
-            report["done"], report["total"], name, name_field_length
+        name = report['name'][0:name_field_length]
+        label.value = '<pre> | {:8d} / {:8d} |: {:<{}s}</pre>'.format(
+            report['done'], report['total'], name, name_field_length
         )
 
     def _reorder_widgets(self, report: Report) -> None:
-        for taskid in self._finishing_taskids:
+        for taskid in self._finishing_task_ids:
             box, bar, label = self.widget_dict[taskid]
             if box in self.active_box_list:
                 self.active_box_list.remove(box)
                 self.complete_box_list.append(box)
                 if self.container_widget is not None:
                     self.container_widget.children = (
                         self.complete_box_list + self.active_box_list
```

### Comparing `atpbar-2.0.1/atpbar/presentation/bartty.py` & `atpbar-2.0.2/atpbar/presentation/bartty.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,109 +4,109 @@
 
 from .base import Presentation, Report
 
 MINIMUM_TERMINAL_WIDTH = 90
 
 
 class ProgressBar(Presentation):
-    stdout_stderr_redrection = True
+    stdout_stderr_redirection = True
 
     def __init__(self) -> None:
         super().__init__()
         self.interval = 0.1  # [second]
         self.width = self._get_width()
 
         self.active_bars = list[str]()
-        self.just_finised_bars = list[str]()
+        self.just_finished_bars = list[str]()
 
     def __repr__(self) -> str:
-        return "{}()".format(self.__class__.__name__)
+        return '{}()'.format(self.__class__.__name__)
 
     def _get_width(self) -> int:
         try:
             columns = shutil.get_terminal_size().columns
             return max(MINIMUM_TERMINAL_WIDTH, columns - 1)
         except AttributeError:
             return MINIMUM_TERMINAL_WIDTH
 
-    def _present(self) -> None:
+    def _present(self, report: Report) -> None:
         self._erase_active_bars()
-        self._compose_just_finised_bars()
+        self._compose_just_finished_bars()
         self._compose_active_bars()
-        self._draw_just_finised_bars()
+        self._draw_just_finished_bars()
         self._draw_active_bars()
 
     def _write(self, s: str, out: TextIO) -> None:
         if not s:
             return
         self._erase_active_bars()
         out.write(s.rstrip())
-        out.write("\n")
+        out.write('\n')
         out.flush()
         self._draw_active_bars()
 
     def _erase_active_bars(self) -> None:
-        nlines = len(self._active_taskids) + len(self._finishing_taskids)
+        n_lines = len(self._active_task_ids) + len(self._finishing_task_ids)
         # must be the same as len(self.active_bars)
 
-        if nlines == 0:
+        if n_lines == 0:
             return
 
-        code = "\033[1G" + "\033[A" * (nlines - 1) + "\033[0J"
+        code = '\033[1G' + '\033[A' * (n_lines - 1) + '\033[0J'
         # '\033[1G' move the cursor to the beginning of the line
         # '\033[A' move the cursor up
         # '\033[0J' clear from cursor to end of screen
 
         self.out.write(code)
         self.out.flush()
 
-    def _compose_just_finised_bars(self) -> None:
-        self.just_finised_bars = [
-            self._compose_bar_from_taskid(i) for i in self._finishing_taskids
+    def _compose_just_finished_bars(self) -> None:
+        self.just_finished_bars = [
+            self._compose_bar_from_taskid(i) for i in self._finishing_task_ids
         ]
 
     def _compose_active_bars(self) -> None:
         self.active_bars = [
             self._compose_bar_from_taskid(i)
-            for i in self._active_taskids + self._new_taskids
+            for i in self._active_task_ids + self._new_task_ids
         ]
 
     def _compose_bar_from_taskid(self, taskid: UUID) -> str:
         report = self._report_dict[taskid]
         return self._compose_bar_from_report(report)
 
     def _compose_bar_from_report(self, report: Report) -> str:
 
-        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
+        percent = float(report['done']) / report['total'] if report['total'] > 0 else 1
         # e.g., 0.7143369818769065
 
-        bar = (":" * int(percent * 40)).ljust(40, " ")
-        # e.g., "::::::::::::::::::::::::::::            "
+        bar = (':' * int(percent * 40)).ljust(40, ' ')
+        # e.g., '::::::::::::::::::::::::::::            '
 
         percent = round(percent * 100, 2)
         # e.g., 71.43
 
-        format = " {percent:6.2f}% {bar:s} | {done:8d} / {total:8d} |:  {name} "
+        format = ' {percent:6.2f}% {bar:s} | {done:8d} / {total:8d} |:  {name} '
 
         ret = format.format(
             percent=percent,
             bar=bar,
-            done=report["done"],
-            total=report["total"],
-            name=report["name"],
+            done=report['done'],
+            total=report['total'],
+            name=report['name'],
         )
-        # e.g., "  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task name "
+        # e.g., '  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task name '
 
-        ret = ret[: self.width].ljust(self.width, " ")
-        # e.g., "  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task na"
+        ret = ret[: self.width].ljust(self.width, ' ')
+        # e.g., '  71.43% ::::::::::::::::::::::::::::             |     3981 /     5573 |:  task na'
 
         return ret
 
-    def _draw_just_finised_bars(self) -> None:
-        if self.just_finised_bars:
-            self.out.write("\n".join(self.just_finised_bars) + "\n")
+    def _draw_just_finished_bars(self) -> None:
+        if self.just_finished_bars:
+            self.out.write('\n'.join(self.just_finished_bars) + '\n')
             self.out.flush()
 
     def _draw_active_bars(self) -> None:
         if self.active_bars:
-            self.out.write("\n".join(self.active_bars))
+            self.out.write('\n'.join(self.active_bars))
             self.out.flush()
```

### Comparing `atpbar-2.0.1/atpbar/presentation/base.py` & `atpbar-2.0.2/atpbar/presentation/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 import sys
 import threading
 import time
 from abc import ABC, abstractmethod
 from typing import TextIO
 from uuid import UUID
 
-from atpbar.progressreport import Report
+from atpbar.progress_report import Report
 
 
 class Presentation(ABC):
-    """A base class of the progress presentation.
+    '''A base class of the progress presentation.
 
     A subclass of this class should implement ``_present()``.
-    """
+    '''
 
-    stdout_stderr_redrection = False
+    stdout_stderr_redirection = False
 
     def __init__(self) -> None:
 
         self.out = sys.stdout
         self.err = sys.stderr
 
         self.lock = threading.Lock()
 
-        self._new_taskids = list[UUID]()
-        self._active_taskids = list[UUID]()  # in order of arrival
-        self._finishing_taskids = list[UUID]()
-        self._complete_taskids = list[UUID]()  # in order of completion
+        self._new_task_ids = list[UUID]()
+        self._active_task_ids = list[UUID]()  # in order of arrival
+        self._finishing_task_ids = list[UUID]()
+        self._complete_task_ids = list[UUID]()  # in order of completion
         self._report_dict = dict[UUID, Report]()
 
         self.interval = 1.0  # [second]
         self.last_time = time.time()
 
     def active(self) -> bool:
-        if self._active_taskids:
+        if self._active_task_ids:
             return True
         return False
 
     def present(self, report: Report) -> None:
         with self.lock:
             if not self._register_report(report):
                 return
             if not self._need_to_present():
                 return
-            self._present()
+            self._present(report)
             self._update_registry()
             self.last_time = time.time()
 
     @abstractmethod
-    def _present(self) -> None:
+    def _present(self, report: Report) -> None:
         pass
 
     def _register_report(self, report: Report) -> bool:
 
-        taskid = report["taskid"]
+        taskid = report['taskid']
 
-        if taskid in self._complete_taskids:
+        if taskid in self._complete_task_ids:
             return False
 
         self._report_dict[taskid] = report
 
-        if taskid in self._finishing_taskids:
+        if taskid in self._finishing_task_ids:
             return True
 
-        if report["last"]:
+        if report['last']:
             try:
-                self._active_taskids.remove(taskid)
+                self._active_task_ids.remove(taskid)
             except ValueError:
                 pass
 
             try:
-                self._new_taskids.remove(taskid)
+                self._new_task_ids.remove(taskid)
             except ValueError:
                 pass
 
-            self._finishing_taskids.append(taskid)
+            self._finishing_task_ids.append(taskid)
 
             return True
 
-        if taskid in self._active_taskids:
+        if taskid in self._active_task_ids:
             return True
 
-        if taskid in self._new_taskids:
+        if taskid in self._new_task_ids:
             return True
 
-        self._new_taskids.append(taskid)
+        self._new_task_ids.append(taskid)
         return True
 
     def _update_registry(self) -> None:
-        self._active_taskids.extend(self._new_taskids)
-        del self._new_taskids[:]
+        self._active_task_ids.extend(self._new_task_ids)
+        del self._new_task_ids[:]
 
-        self._complete_taskids.extend(self._finishing_taskids)
-        del self._finishing_taskids[:]
+        self._complete_task_ids.extend(self._finishing_task_ids)
+        del self._finishing_task_ids[:]
 
     def _need_to_present(self) -> bool:
 
-        if self._new_taskids:
+        if self._new_task_ids:
             return True
 
-        if self._finishing_taskids:
+        if self._finishing_task_ids:
             return True
 
         if time.time() - self.last_time > self.interval:
             return True
 
         return False
 
@@ -119,9 +119,9 @@
         self._write(s, out=self.out)
 
     def _stderr_write(self, s: str) -> None:
         self._write(s, out=self.err)
 
     def _write(self, s: str, out: TextIO) -> None:
         out.write(s.rstrip())
-        out.write("\n")
+        out.write('\n')
         out.flush()
```

### Comparing `atpbar-2.0.1/atpbar/presentation/create.py` & `atpbar-2.0.2/atpbar/presentation/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 try:
     from .barjupyter import ProgressBarJupyter
 except ImportError:
     pass
 
 
 def create_presentation() -> Presentation:
-    """Create a presentation of progress report, e.g., progress bars
+    '''Create a presentation of progress report, e.g., progress bars
 
     Returns
     -------
     object
         an instance of ProgressBar if on TTY
         an instance of ProgressBarJupyter if on Jupyter Notebook
         an instance of ProgressPrint otherwise
 
-    """
+    '''
 
     if sys.stdout.isatty():
         return ProgressBar()
 
     if is_jupyter_notebook():
         try:
             return ProgressBarJupyter()
```

### Comparing `atpbar-2.0.1/atpbar/presentation/txtprint.py` & `atpbar-2.0.2/atpbar/presentation/txtprint.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,57 +7,54 @@
 class ProgressPrint(Presentation):
     def __init__(self) -> None:
         super().__init__()
         self.interval = 60.0  # [second]
         self.last_time_map = dict[UUID, float]()
 
     def __repr__(self) -> str:
-        return "{}()".format(self.__class__.__name__)
+        return '{}()'.format(self.__class__.__name__)
 
     def present(self, report: Report) -> None:
 
         if not self._register_report(report):
             return
 
         if not self._need_to_present_(report):
             return
 
-        self._present_(report)
+        self._present(report)
 
-        self.last_time_map[report["taskid"]] = self._time()
-    
-    def _present(self) -> None:
-        pass
-
-    def _present_(self, report: Report) -> None:
-        time_ = time.strftime("%m/%d %H:%M", time.localtime(time.time()))
-        percent = float(report["done"]) / report["total"] if report["total"] > 0 else 1
+        self.last_time_map[report['taskid']] = self._time()
+
+    def _present(self, report: Report) -> None:
+        time_ = time.strftime('%m/%d %H:%M', time.localtime(time.time()))
+        percent = float(report['done']) / report['total'] if report['total'] > 0 else 1
         percent = round(percent * 100, 2)
-        line = "{time} : {done:8d} / {total:8d} ({percent:6.2f}%): {name} ".format(
+        line = '{time} : {done:8d} / {total:8d} ({percent:6.2f}%): {name} '.format(
             time=time_,
-            done=report["done"],
-            total=report["total"],
+            done=report['done'],
+            total=report['total'],
             percent=percent,
-            name=report["name"],
+            name=report['name'],
         )
-        line = "{}\n".format(line)
+        line = '{}\n'.format(line)
         self.out.write(line)
         self.out.flush()
 
     def _need_to_present_(self, report: Report) -> bool:
 
-        if report["first"]:
+        if report['first']:
             return True
 
-        if report["last"]:
+        if report['last']:
             return True
 
-        if report["taskid"] not in self.last_time_map:
+        if report['taskid'] not in self.last_time_map:
             return True
 
-        if self._time() - self.last_time_map[report["taskid"]] > self.interval:
+        if self._time() - self.last_time_map[report['taskid']] > self.interval:
             return True
 
         return False
 
     def _time(self) -> float:
         return time.time()
```

### Comparing `atpbar-2.0.1/atpbar/presentation/detect/spy.py` & `atpbar-2.0.2/atpbar/presentation/detect/spy.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 try:
     from IPython import get_ipython
 except ImportError:
     get_ipython = None  # type: ignore
 
 
 def is_spyder_ide() -> bool:
-    """Tests if on Spyder IDE
+    '''Tests if on Spyder IDE
 
     Returns
     -------
     bool
         True if on Spyder IDE
 
-    """
+    '''
 
     if spyder is None:
         return False
 
     try:
-        if "IPKernelApp" not in get_ipython().config:
+        if 'IPKernelApp' not in get_ipython().config:
             return False
     except:
         return False
 
-    if "SPYDER_ARGS" not in os.environ:
+    if 'SPYDER_ARGS' not in os.environ:
         return False
 
     min_n_spy_var = 15  # A possible minimum number of the environmental
-    # variables that start with "SPY_" on Spyder IDE.
-    n_spy_var = len([k for k in os.environ.keys() if k.startswith("SPY_")])
+    # variables that start with 'SPY_' on Spyder IDE.
+    n_spy_var = len([k for k in os.environ.keys() if k.startswith('SPY_')])
     if n_spy_var < min_n_spy_var:
         return False
 
     return True
```

### Comparing `atpbar-2.0.1/atpbar/progressreport/complement.py` & `atpbar-2.0.2/atpbar/progress_report/complement.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from uuid import UUID
 
 from .report import Report
 
 
 class ProgressReportComplementer:
-    """Complement progress reports
+    '''Complement progress reports
 
     Complement a progress report with the previous report for the same
     task.
 
     Parameters
     ----------
     report : Report
         A report must always include `taskid`. The first report for a task must
         include `done`, `total`, and 'name'. The `first` and `last` will be
         automatically determined if not given.
 
-    """
+    '''
 
     def __init__(self) -> None:
         self.previous_reports = dict[UUID, Report]()
 
     def __call__(self, report: Report) -> None:
-        taskid = report["taskid"]
+        taskid = report['taskid']
         if taskid in self.previous_reports:
             self._complement(taskid, report)
         self._first(report)
         self._last(report)
         self._store(taskid, report.copy())
 
     def _complement(self, taskid: UUID, report: Report) -> None:
         report_copy = report.copy()
         report.update(Report(taskid=taskid))
         report.update(self.previous_reports[taskid])
         report.update(report_copy)
 
     def _first(self, report: Report) -> None:
-        if "first" in report:
+        if 'first' in report:
             return
-        report["first"] = report["done"] == 0
+        report['first'] = report['done'] == 0
 
     def _last(self, report: Report) -> None:
-        if "last" in report:
+        if 'last' in report:
             return
-        report["last"] = report["done"] >= report["total"]
+        report['last'] = report['done'] >= report['total']
 
     def _store(self, taskid: UUID, report: Report) -> None:
         report.pop('first', None)
         report.pop('last', None)
         self.previous_reports[taskid] = report
```

### Comparing `atpbar-2.0.1/atpbar/progressreport/pickup.py` & `atpbar-2.0.2/atpbar/progress_report/pickup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 from .report import Report
 
 if TYPE_CHECKING:
     from atpbar.presentation import Presentation
 
 
 class ProgressReportPickup(threading.Thread):
-    """A pickup of progress reports.
+    '''A pickup of progress reports.
 
     This class picks up progress reports and presents them.
 
     Parameters
     ----------
     queue : multiprocessing.Queue
         The queue through which this class receives progress reports
     presentation :
         The presentation of the reports
-    """
+    '''
 
     def __init__(self, queue: 'Queue[Report]', presentation: 'Presentation') -> None:
         super().__init__(daemon=True)
         # The daemon makes the functions registered at atexit called
         # even if the pickup is still running
 
         self.queue = queue
         self.presentation = presentation
         self.last_wait_time = 1.0  # [second]
 
         self.start()
 
     def end(self) -> None:
-        """end the thread"""
+        '''end the thread'''
         self.queue.put(None)  # type: ignore
         self.join()
 
     def run(self) -> None:
         try:
             self._run_until_the_end_order_arrives()
             self._run_until_reports_stop_coming()
@@ -72,14 +72,14 @@
                 self._process_report(report)
             self._short_sleep()
 
     def _process_report(self, report: Report) -> None:
         self.presentation.present(report)
 
     def _short_sleep(self) -> None:
-        """sleep very briefly
+        '''sleep very briefly
 
         used to prevent the empty `while` loop from increasing CPU
         loads
 
-        """
+        '''
         time.sleep(0.001)
```

### Comparing `atpbar-2.0.1/atpbar/progressreport/report.py` & `atpbar-2.0.2/atpbar/progress_report/report.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.1/atpbar/progressreport/reporter.py` & `atpbar-2.0.2/atpbar/progress_report/reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if TYPE_CHECKING:
     from atpbar.stream import StreamQueue
 
 DEFAULT_INTERVAL = 0.1  # [second]
 
 
 class ProgressReporter:
-    """A progress reporter
+    '''A progress reporter
 
     This class sends progress reports. The reports will be picked up
     by the pickup (`ProgressReportPickup`), which uses the reports,
     for example, to update `ProgressBar` on the screen.
 
     An instance of this class is initialized with a message queue::
 
@@ -39,62 +39,62 @@
     of the task, will be always sent to the progress monitor
     regardless of whether it is given within the interval.
 
     Parameters
     ----------
     queue : multiprocessing.Queue
         The queue through which this class sends progress reports.
-    """
+    '''
 
     def __init__(
         self,
         queue: 'Queue[Report]',
         notices_from_sub_processes: 'Queue[bool]',
         stream_queue: 'StreamQueue',
     ) -> None:
         self.queue = queue
         self.interval = DEFAULT_INTERVAL  # [second]
         self.last_time = dict[UUID, float]()
         self.complete_report = ProgressReportComplementer()
         self.notices_from_sub_processes = notices_from_sub_processes
         self.stream_queue = stream_queue
-        self.stream_redirection_enablaed = True
+        self.stream_redirection_enabled = True
 
     def __repr__(self) -> str:
-        return "{}(queue={!r}, interval={!r})".format(
+        return '{}(queue={!r}, interval={!r})'.format(
             self.__class__.__name__, self.queue, self.interval
         )
 
     def report(self, report: Report) -> None:
-        """send ``report`` to a progress monitor
+        '''send ``report`` to a progress monitor
 
         Parameters
         ----------
         report : ProgressReport
             a progress report
 
-        """
+        '''
 
         self.complete_report(report)
 
         if not self._need_to_report(report):
             return
 
         self.queue.put(report)
 
-        self.last_time[report["taskid"]] = time.time()
+        self.last_time[report['taskid']] = time.time()
 
     def _need_to_report(self, report: Report) -> bool:
 
-        if report["first"]:
+        if report['first']:
             return True
 
-        if report["last"]:
+        if report['last']:
             return True
 
-        if report["taskid"] not in self.last_time:
+        if report['taskid'] not in self.last_time:
             return True
 
-        if time.time() - self.last_time[report["taskid"]] > self.interval:
+        if time.time() - self.last_time[report['taskid']] > self.interval:
             return True
 
         return False
```

### Comparing `atpbar-2.0.1/.gitignore` & `atpbar-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.1/README.md` & `atpbar-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.1/pyproject.toml` & `atpbar-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.1/PKG-INFO` & `atpbar-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atpbar
-Version: 2.0.1
+Version: 2.0.2
 Summary: Progress bars for threading and multiprocessing tasks
 Project-URL: Homepage, https://github.com/alphatwirl/atpbar
 Author-email: Tai Sakuma <tai.sakuma@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

