# Comparing `tmp/cobble-0.1.3.tar.gz` & `tmp/cobble-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cobble-0.1.3.tar", last modified: Wed May 24 20:33:50 2017, max compression
+gzip compressed data, was "cobble-0.1.4.tar", last modified: Sat Jun  1 18:11:06 2024, max compression
```

## Comparing `cobble-0.1.3.tar` & `cobble-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2017-05-24 20:33:50.000000 cobble-0.1.3/
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2017-05-24 20:33:50.000000 cobble-0.1.3/cobble.egg-info/
--rw-r--r--   0 mick      (1000) mick      (1000)        7 2017-05-24 20:33:49.000000 cobble-0.1.3/cobble.egg-info/top_level.txt
--rw-r--r--   0 mick      (1000) mick      (1000)      193 2017-05-24 20:33:50.000000 cobble-0.1.3/cobble.egg-info/SOURCES.txt
--rw-r--r--   0 mick      (1000) mick      (1000)        1 2017-05-24 20:33:49.000000 cobble-0.1.3/cobble.egg-info/dependency_links.txt
--rw-r--r--   0 mick      (1000) mick      (1000)     3276 2017-05-24 20:33:49.000000 cobble-0.1.3/cobble.egg-info/PKG-INFO
--rw-r--r--   0 mick      (1000) mick      (1000)     1770 2015-08-09 10:19:10.000000 cobble-0.1.3/README.rst
-drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2017-05-24 20:33:50.000000 cobble-0.1.3/cobble/
--rw-r--r--   0 mick      (1000) mick      (1000)    30097 2015-08-08 10:59:54.000000 cobble-0.1.3/cobble/six.py
--rw-r--r--   0 mick      (1000) mick      (1000)     5177 2017-05-24 20:32:00.000000 cobble-0.1.3/cobble/__init__.py
--rw-r--r--   0 mick      (1000) mick      (1000)      799 2015-08-08 12:32:57.000000 cobble-0.1.3/cobble/inflection.py
--rw-r--r--   0 mick      (1000) mick      (1000)       59 2017-05-24 20:33:50.000000 cobble-0.1.3/setup.cfg
--rw-r--r--   0 mick      (1000) mick      (1000)     1117 2017-05-24 20:32:06.000000 cobble-0.1.3/setup.py
--rw-r--r--   0 mick      (1000) mick      (1000)     3276 2017-05-24 20:33:50.000000 cobble-0.1.3/PKG-INFO
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2024-06-01 18:11:06.153825 cobble-0.1.4/
+-rw-r--r--   0 mick      (1000) mick      (1000)     2698 2024-06-01 18:11:06.153825 cobble-0.1.4/PKG-INFO
+-rw-r--r--   0 mick      (1000) mick      (1000)     1770 2015-08-09 10:19:10.000000 cobble-0.1.4/README.rst
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2024-06-01 18:11:06.149825 cobble-0.1.4/cobble/
+-rw-r--r--   0 mick      (1000) mick      (1000)     4807 2024-06-01 18:04:31.000000 cobble-0.1.4/cobble/__init__.py
+-rw-r--r--   0 mick      (1000) mick      (1000)      799 2015-08-08 12:32:57.000000 cobble-0.1.4/cobble/inflection.py
+drwxr-xr-x   0 mick      (1000) mick      (1000)        0 2024-06-01 18:11:06.153825 cobble-0.1.4/cobble.egg-info/
+-rw-r--r--   0 mick      (1000) mick      (1000)     2698 2024-06-01 18:11:06.000000 cobble-0.1.4/cobble.egg-info/PKG-INFO
+-rw-r--r--   0 mick      (1000) mick      (1000)      179 2024-06-01 18:11:06.000000 cobble-0.1.4/cobble.egg-info/SOURCES.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)        1 2024-06-01 18:11:06.000000 cobble-0.1.4/cobble.egg-info/dependency_links.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)        7 2024-06-01 18:11:06.000000 cobble-0.1.4/cobble.egg-info/top_level.txt
+-rw-r--r--   0 mick      (1000) mick      (1000)       38 2024-06-01 18:11:06.153825 cobble-0.1.4/setup.cfg
+-rw-r--r--   0 mick      (1000) mick      (1000)     1189 2024-06-01 18:10:23.000000 cobble-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cobble-0.1.3/cobble.egg-info/PKG-INFO` & `cobble-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cobble
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create data objects
 Home-page: http://github.com/mwilliamson/python-cobble
 Author: Michael Williamson
 Author-email: mike@zwobble.org
-License: UNKNOWN
-Description: Cobble
-        ======
-        
-        Cobble is a Python library that allows easy creation of data objects,
-        including implementations of common methods such as ``__eq__`` and ``__repr__``.
-        
-        Examples
-        --------
-        
-        .. code-block:: python
-        
-            import cobble
-        
-            @cobble.data
-            class Song(object):
-                name = cobble.field()
-                artist = cobble.field()
-                album = cobble.field(default=None)
-        
-        
-            song = Song("MFEO", artist="Jack's Mannequin")
-        
-            print(song) # Prints "Song(name='MFEO', artist="Jack's Mannequin", album=None)"
-        
-        .. code-block:: python
-        
-            class Expression(object):
-                pass
-        
-            @cobble.data
-            class Literal(Expression):
-                value = cobble.field()
-        
-            @cobble.data
-            class Add(Expression):
-                left = cobble.field()
-                right = cobble.field()
-            
-            class Evaluator(cobble.visitor(Expression)):
-                def visit_literal(self, literal):
-                    return literal.value
-                
-                def visit_add(self, add):
-                    return self.visit(add.left) + self.visit(add.right)
-        
-            Evaluator().visit(Add(Literal(2), Literal(4))) # 6
-        
-        .. code-block:: python
-        
-            class Expression(object):
-                pass
-        
-            @cobble.visitable
-            class Literal(Expression):
-                def __init__(self, value):
-                    self.value = value
-        
-            @cobble.visitable
-            class Add(Expression):
-                def __init__(self, left, right):
-                    self.left = left
-                    self.right = right
-            
-            class Evaluator(cobble.visitor(Expression)):
-                def visit_literal(self, literal):
-                    return literal.value
-                
-                def visit_add(self, add):
-                    return self.visit(add.left) + self.visit(add.right)
-        
-            Evaluator().visit(Add(Literal(2), Literal(4))) # 6
-        
-        License
-        -------
-        
-        `2-Clause BSD <http://opensource.org/licenses/BSD-2-Clause>`_
-        
 Keywords: data object case class
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+
+Cobble
+======
+
+Cobble is a Python library that allows easy creation of data objects,
+including implementations of common methods such as ``__eq__`` and ``__repr__``.
+
+Examples
+--------
+
+.. code-block:: python
+
+    import cobble
+
+    @cobble.data
+    class Song(object):
+        name = cobble.field()
+        artist = cobble.field()
+        album = cobble.field(default=None)
+
+
+    song = Song("MFEO", artist="Jack's Mannequin")
+
+    print(song) # Prints "Song(name='MFEO', artist="Jack's Mannequin", album=None)"
+
+.. code-block:: python
+
+    class Expression(object):
+        pass
+
+    @cobble.data
+    class Literal(Expression):
+        value = cobble.field()
+
+    @cobble.data
+    class Add(Expression):
+        left = cobble.field()
+        right = cobble.field()
+    
+    class Evaluator(cobble.visitor(Expression)):
+        def visit_literal(self, literal):
+            return literal.value
+        
+        def visit_add(self, add):
+            return self.visit(add.left) + self.visit(add.right)
+
+    Evaluator().visit(Add(Literal(2), Literal(4))) # 6
+
+.. code-block:: python
+
+    class Expression(object):
+        pass
+
+    @cobble.visitable
+    class Literal(Expression):
+        def __init__(self, value):
+            self.value = value
+
+    @cobble.visitable
+    class Add(Expression):
+        def __init__(self, left, right):
+            self.left = left
+            self.right = right
+    
+    class Evaluator(cobble.visitor(Expression)):
+        def visit_literal(self, literal):
+            return literal.value
+        
+        def visit_add(self, add):
+            return self.visit(add.left) + self.visit(add.right)
+
+    Evaluator().visit(Add(Literal(2), Literal(4))) # 6
+
+License
+-------
+
+`2-Clause BSD <http://opensource.org/licenses/BSD-2-Clause>`_
```

### Comparing `cobble-0.1.3/README.rst` & `cobble-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `cobble-0.1.3/cobble/__init__.py` & `cobble-0.1.4/cobble/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import itertools
 import functools
 import abc
-import inspect
 
-from .six import exec_, iteritems
-from . import six
 from .inflection import underscore
 
 
 def data(cls):
     fields = sorted(
         filter(
             None,
@@ -19,17 +16,17 @@
     _add_methods(cls, _methods(cls, fields))
     visitable(cls)
     cls._cobble_fields = fields
     return cls
 
 def _add_methods(cls, methods):
     definitions = _compile_definitions(methods, {cls.__name__: cls})
-    for key, value in iteritems(definitions):
+    for key, value in definitions.items():
         setattr(cls, key, value)
-    
+
 
 def _methods(cls, fields):
     names = [name for name, field in fields]
     return [
         _make_init(cls, fields),
         _make_repr(cls, names),
         _make_eq(cls, names),
@@ -40,15 +37,15 @@
 
 def _make_init(cls, fields):
     def make_arg(name, field):
         if field.default == _undefined:
             return name
         else:
             return "{0}={1}".format(name, field.default)
-    
+
     args_source = ", ".join(make_arg(name, field) for name, field in fields)
     assignments_source = "".join(
         "\n    self.{0} = {0}".format(name)
         for name, field in fields
     )
     return "def __init__(self, {0}):{1}\n    super({2}, self).__init__()\n".format(args_source, assignments_source, cls.__name__)
 
@@ -113,51 +110,41 @@
     _visitables.add(cls)
     return cls
 
 
 def visitor(cls, args=None):
     if args is None:
         args = 0
-    
+
     subclasses = set(filter(
         lambda subclass: subclass in _visitables,
         _subclasses(cls)
     ))
     for subclass in subclasses:
         _add_methods(subclass, [_make_accept(subclass, args=args)])
-    
+
     abstract_method_template = """
     @abc.abstractmethod
     def {0}(self, value):
         pass
 """
     abstract_methods = (
         abstract_method_template.format(_visit_method_name(subclass))
         for subclass in subclasses
     )
-    
-    if six.PY2:
-        py2_metaclass = "__metaclass__ = abc.ABCMeta"
-        py3_metaclass = ""
-    else:
-        py2_metaclass = ""
-        py3_metaclass = ", metaclass=abc.ABCMeta"
-    
+
     source = """
-class {name}Visitor(object{py3_metaclass}):
-    {py2_metaclass}
+class {name}Visitor(metaclass=abc.ABCMeta):
 
     def visit(self, value{args_signature}):
         return value._accept{args}(self{args_signature})
-    
+
 {abstract_methods}
 """.format(
     name=cls.__name__,
-    py3_metaclass=py3_metaclass,
-    py2_metaclass=py2_metaclass,
     args_signature=_args_signature(args),
     args=args,
     abstract_methods="\n".join(abstract_methods),
 )
     definition = _compile_definitions([source], {abc: abc})
     return next(iter(definition.values()))
 
@@ -165,15 +152,15 @@
 def _args_signature(args):
     return "".join(", arg{0}".format(arg_index) for arg_index in range(0, args))
 
 def _compile_definitions(definitions, bindings):
     definition_globals = {"abc": abc}
     definition_globals.update(bindings)
     stash = {}
-    exec_("\n".join(definitions), definition_globals, stash)
+    exec("\n".join(definitions), definition_globals, stash)
     return stash
 
 def _visit_method_name(cls):
     return "visit_" + underscore(cls.__name__)
 
 
 def _subclasses(cls):
```

### Comparing `cobble-0.1.3/cobble/inflection.py` & `cobble-0.1.4/cobble/inflection.py`

 * *Files identical despite different names*

### Comparing `cobble-0.1.3/setup.py` & `cobble-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #!/usr/bin/env python
 
 import os
 from setuptools import setup
-import sys
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='cobble',
-    version='0.1.3',
+    version='0.1.4',
     description='Create data objects',
     long_description=read("README.rst"),
     author='Michael Williamson',
     author_email='mike@zwobble.org',
     url='http://github.com/mwilliamson/python-cobble',
     keywords="data object case class",
     packages=['cobble'],
+    python_requires='>=3.5',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `cobble-0.1.3/PKG-INFO` & `cobble-0.1.4/cobble.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cobble
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create data objects
 Home-page: http://github.com/mwilliamson/python-cobble
 Author: Michael Williamson
 Author-email: mike@zwobble.org
-License: UNKNOWN
-Description: Cobble
-        ======
-        
-        Cobble is a Python library that allows easy creation of data objects,
-        including implementations of common methods such as ``__eq__`` and ``__repr__``.
-        
-        Examples
-        --------
-        
-        .. code-block:: python
-        
-            import cobble
-        
-            @cobble.data
-            class Song(object):
-                name = cobble.field()
-                artist = cobble.field()
-                album = cobble.field(default=None)
-        
-        
-            song = Song("MFEO", artist="Jack's Mannequin")
-        
-            print(song) # Prints "Song(name='MFEO', artist="Jack's Mannequin", album=None)"
-        
-        .. code-block:: python
-        
-            class Expression(object):
-                pass
-        
-            @cobble.data
-            class Literal(Expression):
-                value = cobble.field()
-        
-            @cobble.data
-            class Add(Expression):
-                left = cobble.field()
-                right = cobble.field()
-            
-            class Evaluator(cobble.visitor(Expression)):
-                def visit_literal(self, literal):
-                    return literal.value
-                
-                def visit_add(self, add):
-                    return self.visit(add.left) + self.visit(add.right)
-        
-            Evaluator().visit(Add(Literal(2), Literal(4))) # 6
-        
-        .. code-block:: python
-        
-            class Expression(object):
-                pass
-        
-            @cobble.visitable
-            class Literal(Expression):
-                def __init__(self, value):
-                    self.value = value
-        
-            @cobble.visitable
-            class Add(Expression):
-                def __init__(self, left, right):
-                    self.left = left
-                    self.right = right
-            
-            class Evaluator(cobble.visitor(Expression)):
-                def visit_literal(self, literal):
-                    return literal.value
-                
-                def visit_add(self, add):
-                    return self.visit(add.left) + self.visit(add.right)
-        
-            Evaluator().visit(Add(Literal(2), Literal(4))) # 6
-        
-        License
-        -------
-        
-        `2-Clause BSD <http://opensource.org/licenses/BSD-2-Clause>`_
-        
 Keywords: data object case class
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+
+Cobble
+======
+
+Cobble is a Python library that allows easy creation of data objects,
+including implementations of common methods such as ``__eq__`` and ``__repr__``.
+
+Examples
+--------
+
+.. code-block:: python
+
+    import cobble
+
+    @cobble.data
+    class Song(object):
+        name = cobble.field()
+        artist = cobble.field()
+        album = cobble.field(default=None)
+
+
+    song = Song("MFEO", artist="Jack's Mannequin")
+
+    print(song) # Prints "Song(name='MFEO', artist="Jack's Mannequin", album=None)"
+
+.. code-block:: python
+
+    class Expression(object):
+        pass
+
+    @cobble.data
+    class Literal(Expression):
+        value = cobble.field()
+
+    @cobble.data
+    class Add(Expression):
+        left = cobble.field()
+        right = cobble.field()
+    
+    class Evaluator(cobble.visitor(Expression)):
+        def visit_literal(self, literal):
+            return literal.value
+        
+        def visit_add(self, add):
+            return self.visit(add.left) + self.visit(add.right)
+
+    Evaluator().visit(Add(Literal(2), Literal(4))) # 6
+
+.. code-block:: python
+
+    class Expression(object):
+        pass
+
+    @cobble.visitable
+    class Literal(Expression):
+        def __init__(self, value):
+            self.value = value
+
+    @cobble.visitable
+    class Add(Expression):
+        def __init__(self, left, right):
+            self.left = left
+            self.right = right
+    
+    class Evaluator(cobble.visitor(Expression)):
+        def visit_literal(self, literal):
+            return literal.value
+        
+        def visit_add(self, add):
+            return self.visit(add.left) + self.visit(add.right)
+
+    Evaluator().visit(Add(Literal(2), Literal(4))) # 6
+
+License
+-------
+
+`2-Clause BSD <http://opensource.org/licenses/BSD-2-Clause>`_
```

