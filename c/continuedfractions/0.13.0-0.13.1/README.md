# Comparing `tmp/continuedfractions-0.13.0.tar.gz` & `tmp/continuedfractions-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.13.0.tar", last modified: Fri May 31 08:07:12 2024, max compression
+gzip compressed data, was "continuedfractions-0.13.1.tar", last modified: Fri May 31 19:19:06 2024, max compression
```

## Comparing `continuedfractions-0.13.0.tar` & `continuedfractions-0.13.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.13.0/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.13.0/LICENSE
--rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.13.0/README.md
--rw-r--r--   0        0        0     3436 2024-05-16 21:48:47.164813 continuedfractions-0.13.0/README.md
--rw-r--r--   0        0        0     3506 2024-05-31 08:07:12.531507 continuedfractions-0.13.0/pyproject.toml
--rw-r--r--   0        0        0    32416 2024-05-30 21:10:36.891568 continuedfractions-0.13.0/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15740 2024-05-31 08:01:57.322632 continuedfractions-0.13.0/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    35383 2024-05-17 21:03:20.372072 continuedfractions-0.13.0/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.13.0/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-30 21:20:30.848875 continuedfractions-0.13.0/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24420 1970-01-01 00:00:00.000000 continuedfractions-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.13.1/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.13.1/LICENSE
+-rw-r--r--   0        0        0     3463 2024-05-31 19:13:19.818920 continuedfractions-0.13.1/README.md
+-rw-r--r--   0        0        0     3463 2024-05-31 19:13:19.818920 continuedfractions-0.13.1/README.md
+-rw-r--r--   0        0        0     3506 2024-05-31 19:19:06.218063 continuedfractions-0.13.1/pyproject.toml
+-rw-r--r--   0        0        0    32416 2024-05-30 21:10:36.891568 continuedfractions-0.13.1/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15740 2024-05-31 19:03:16.066740 continuedfractions-0.13.1/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    35383 2024-05-17 21:03:20.372072 continuedfractions-0.13.1/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.13.1/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-31 19:03:31.107758 continuedfractions-0.13.1/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24447 1970-01-01 00:00:00.000000 continuedfractions-0.13.1/PKG-INFO
```

### Comparing `continuedfractions-0.13.0/LICENSE` & `continuedfractions-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.13.0/README.md` & `continuedfractions-0.13.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
-* working with (finite) continued fractions as Python objects
+* working with (finite) continued fractions as Python objects, in an object-oriented way
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
 * supporting approximations of and experimental computations for irrational numbers
 * exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
 Currently, it does **not** support the following features:
```

#### html2text {}

```diff
@@ -27,19 +27,19 @@
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are
 beautiful and interesting mathematical objects, with many connections in
 [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very
 useful practical applications, including the [rational approximation of real
 numbers](https://en.wikipedia.org/wiki/
 Continued_fraction#Best_rational_approximations). The `continuedfractions`
 package is designed for: * working with (finite) continued fractions as Python
-objects * exploring their key properties, such as elements/coefficients,
-convergents, segments, remainders, and others * operating on them as rationals
-and instances of the standard library [`fractions.Fraction`](https://
-docs.python.org/3/library/fractions.html#fractions.Fraction) class * supporting
-approximations of and experimental computations for irrational numbers *
-exploring other related objects, such as mediants, and special sequences of
-rational numbers such as Farey sequences Currently, it does **not** support the
-following features: * infinite and generalised continued fractions * symbolic
-computations These are [planned](https://github.com/sr-murthy/
-continuedfractions/issues) for future releases. The project is [licensed]
-(LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/
-licenses/MPL-2.0).
+objects, in an object-oriented way * exploring their key properties, such as
+elements/coefficients, convergents, segments, remainders, and others *
+operating on them as rationals and instances of the standard library
+[`fractions.Fraction`](https://docs.python.org/3/library/
+fractions.html#fractions.Fraction) class * supporting approximations of and
+experimental computations for irrational numbers * exploring other related
+objects, such as mediants, and special sequences of rational numbers such as
+Farey sequences Currently, it does **not** support the following features: *
+infinite and generalised continued fractions * symbolic computations These are
+[planned](https://github.com/sr-murthy/continuedfractions/issues) for future
+releases. The project is [licensed](LICENSE) under the [Mozilla Public License
+2.0](https://opensource.org/licenses/MPL-2.0).
```

### Comparing `continuedfractions-0.13.0/pyproject.toml` & `continuedfractions-0.13.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.13.0"
+version = "0.13.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.13.0/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.13.1/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.13.0/src/continuedfractions/lib.py` & `continuedfractions-0.13.1/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.13.0/src/continuedfractions/sequences.py` & `continuedfractions-0.13.1/src/continuedfractions/sequences.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.13.0/src/continuedfractions/utils.py` & `continuedfractions-0.13.1/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.13.0/PKG-INFO` & `continuedfractions-0.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.13.0
+Version: 0.13.1
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -424,15 +424,15 @@
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
-* working with (finite) continued fractions as Python objects
+* working with (finite) continued fractions as Python objects, in an object-oriented way
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
 * supporting approximations of and experimental computations for irrational numbers
 * exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
 Currently, it does **not** support the following features:
```

