# Comparing `tmp/symmetria-0.0.4.tar.gz` & `tmp/symmetria-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmetria-0.0.4.tar", last modified: Tue May 28 21:34:32 2024, max compression
+gzip compressed data, was "symmetria-0.0.5.tar", last modified: Sat Jun  1 12:30:29 2024, max compression
```

## Comparing `symmetria-0.0.4.tar` & `symmetria-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.334811 symmetria-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 21:34:20.000000 symmetria-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-28 21:34:32.334811 symmetria-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-05-28 21:34:20.000000 symmetria-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-28 21:34:20.000000 symmetria-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:34:32.334811 symmetria-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/elements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    29943 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/cycle_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/elements/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria/groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:20.000000 symmetria-0.0.4/symmetria/groups/symmetric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/symmetria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 21:34:32.000000 symmetria-0.0.4/symmetria.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:34:32.330811 symmetria-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-28 21:34:20.000000 symmetria-0.0.4/tests/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.463321 symmetria-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-01 12:30:18.000000 symmetria-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-06-01 12:30:29.463321 symmetria-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-06-01 12:30:18.000000 symmetria-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-06-01 12:30:18.000000 symmetria-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 12:30:29.463321 symmetria-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.459321 symmetria-0.0.5/symmetria/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.463321 symmetria-0.0.5/symmetria/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/elements/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/elements/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34782 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/elements/cycle_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36663 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/elements/permutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.463321 symmetria-0.0.5/symmetria/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:18.000000 symmetria-0.0.5/symmetria/groups/symmetric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.463321 symmetria-0.0.5/symmetria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 12:30:29.000000 symmetria-0.0.5/symmetria.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:30:29.463321 symmetria-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-06-01 12:30:18.000000 symmetria-0.0.5/tests/test_factory.py
```

### Comparing `symmetria-0.0.4/LICENSE.txt` & `symmetria-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symmetria-0.0.4/PKG-INFO` & `symmetria-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.4
+Version: 0.0.5
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.4 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.5 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
```

### Comparing `symmetria-0.0.4/README.md` & `symmetria-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `symmetria-0.0.4/pyproject.toml` & `symmetria-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "symmetria"
-version = "0.0.4"
+version = "0.0.5"
 description = "Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements."
 authors = [
     {name = "Vasco Schiavo"},
 ]
 maintainers = [
     {name = "Vasco Schiavo"},
 ]
```

### Comparing `symmetria-0.0.4/symmetria/__init__.py` & `symmetria-0.0.5/symmetria/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from symmetria.elements.cycle import Cycle
 from symmetria.elements.permutation import Permutation
 from symmetria.elements.cycle_decomposition import CycleDecomposition
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __all__ = ["__version__", "Permutation", "Cycle", "CycleDecomposition"]
 
 
 def _log_version() -> None:
     """Private method which take a command line argument and log the version of `symmetria`."""
     if len(sys.argv) == 0 or len(sys.argv) == 1:
         raise Exception("No command provided.")
```

### Comparing `symmetria-0.0.4/symmetria/elements/cycle.py` & `symmetria-0.0.5/symmetria/elements/cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Tuple,
     Union,
     Iterable,
 )
 
 import symmetria.elements.permutation
 import symmetria.elements.cycle_decomposition
-from symmetria.elements._interface import _Element
+from symmetria.elements._base import _Element
 
 __all__ = ["Cycle"]
 
 
 class Cycle(_Element):
     r"""The ``Cycle`` class represents the cycle elements of a symmetric group.
 
@@ -190,14 +190,24 @@
         """Check if the cycle is equal to another object.
 
         :param other: The object to compare with.
         :type other: Any
 
         :return: True if the cycle is equal to `other`, i.e., they define the same map. Otherwise, False.
         :rtype: bool
+
+        :example:
+            >>> from symmetria import Cycle
+            ...
+            >>> Cycle(1, 2, 3) == Cycle(3, 1, 2)
+            True
+            >>> Cycle(1, 3, 2) == Cycle(1, 2, 3)
+            False
+            >>> Cycle(1, 2, 3) == 13
+            False
         """
         if isinstance(other, Cycle):
             lhs_length, rhs_length = len(self), len(other)
             if lhs_length != rhs_length:
                 return False
             else:
                 # in this case we have the identity on both side
@@ -205,23 +215,33 @@
                     return True
                 return self.map == other.map
         return False
 
     def __getitem__(self, item: int) -> int:
         """Return the value of the cycle at the given index `item`.
 
-        The index corresponds to the position in the cycle, starting from 0.
+        The index corresponds to the position in the cycle in its standardize form, starting from 0.
 
         :param item: The index of the cycle.
         :type item: int
 
         :return: The value of the cycle at the specified index.
         :rtype: int
 
         :raises IndexError: If the index is out of range.
+
+        :example:
+            >>> from symmetria import Cycle
+            ...
+            >>> cycle = Cycle(1, 3, 2)
+            >>> for idx in range(len(cycle)):
+            ...    cycle[idx]
+            1
+            3
+            2
         """
         return self._cycle[item]
 
     def __int__(self) -> int:
         """Convert the cycle to its integer representation.
 
         In other words, return a numeric one line notation of the cycle.
@@ -256,51 +276,59 @@
             3
             >>> len(Cycle(1, 3, 4, 5, 2, 6))
             6
         """
         return len(self._cycle)
 
     def __mul__(self, other: "Cycle") -> "Cycle":
+        """
+        :raise NotImplementedError: Multiplication between cycles is not supported. However, composition is supported.
+            Try to call your cycle on the cycle you would like to compose.
+        """
         raise NotImplementedError(
             "Multiplication between cycles is not supported. However, composition is supported. \n"
             "Try to call your cycle on the cycle you would like to compose."
         )
 
     def __pow__(self, power: int) -> "Cycle":
         """Return the cycle object to the chosen power.
 
         :param power: the exponent for the power operation.
         :type power: int
 
         :return: the power of the cycle.
         :rtype: Cycle
 
+        :raises TypeError: If `power` is not an integer.
+
         :example:
             >>> from symmetria import Cycle
             ...
-            >>> Cycle(1, 3, 2) ** 0
+            >>> Cycle(1, 3, 2)**0
             Cycle(1, 2, 3)
-            >>> Cycle(1, 3, 2) ** 1
+            >>> Cycle(1, 3, 2)**1
             Cycle(1, 3, 2)
-            >>> Cycle(1, 3, 2) ** -1
+            >>> Cycle(1, 3, 2)**-1
+            Cycle(1, 2, 3)
+            >>> Cycle(1, 3, 2)**2
             Cycle(1, 2, 3)
         """
         if isinstance(power, int) is False:
             raise TypeError(f"Power operation for type {type(power)} not supported.")
         elif self is False or power == 0:
             return Cycle(*list(self.domain))
         elif power == 1:
             return self
         elif power <= -1:
             return self.inverse() ** abs(power)
         else:
-            return self(self ** (power - 1))
+            return Cycle(*[self.map[(self ** (power - 1)).map[idx]] for idx in self.domain])
 
     def __repr__(self) -> str:
-        r"""Return a string representation of the cycle in the format "Cycle(x, y, z, ...)",
+        r"""Return a string representation of the cycle in the format `Cycle(x, y, z, ...)`,
         where :math:`x, y, z, ... \in \mathbb{N}` are the elements of the cycle.
 
         :return: A string representation of the cycle.
         :rtype: str
 
         :example:
             >>> from symmetria import Cycle
@@ -312,15 +340,18 @@
         """
         return f"Cycle({', '.join(str(element) for element in self.elements)})"
 
     def __str__(self) -> str:
         r"""Return a string representation of the cycle in the form of cycle notation.
 
         Recall that for a cycle :math:`\sigma` of order n, its cycle notation is given by
-        :math:`(\sigma(x) \sigma^2(x), ..., \sigma^n(x))`, where x is an element in the support of the cycle.
+
+        .. math:: (\sigma(x)\quad\sigma^2(x)\quad...\quad\sigma^n(x)),
+
+        where x is an element in the support of the cycle, and :math:`n \in \mathbb{N}` is the cycle order.
 
         :return: A string representation of the cycle.
         :rtype: str
 
         :example:
             >>> from symmetria import Cycle
             ...
@@ -330,15 +361,15 @@
             (1 3 4 5 2 6)
         """
         return "(" + " ".join([str(element) for element in self.elements]) + ")"
 
     def cycle_decomposition(self) -> "CycleDecomposition":
         """Convert the cycle into its cycle decomposition, representing it as a product of disjoint cycles.
 
-        In the specific case of a cycle, it converts it from the class `Cycle` to the class `CycleDecomposition`.
+        In the specific case of a cycle, it converts it from the class ``Cycle`` to the class ``CycleDecomposition``.
 
         :return: The cycle decomposition of the permutation.
         :rtype: CycleDecomposition
 
         :example:
             >>> from symmetria import Cycle
             ...
@@ -353,15 +384,18 @@
             *([Cycle(idx) for idx in self.domain if idx not in self] + [self])
         )
 
     def cycle_notation(self) -> str:
         r"""Return a string representing the cycle notation of the cycle.
 
         Recall that for a cycle :math:`\sigma` of order n, its cycle notation is given by
-        :math:`(\sigma(x) \sigma^2(x), ..., \sigma^n(x))`, where x is an element in the support of the cycle.
+
+        .. math:: (\sigma(x)\quad\sigma^2(x)\quad...\quad\sigma^n(x)),
+
+        where x is an element in the support of the cycle, and :math:`n \in \mathbb{N}` is the cycle order.
 
         :return: The cycle notation of the cycle.
         :rtype: str
 
         :example:
             >>> from symmetria import Cycle
             ...
@@ -405,24 +439,28 @@
             >>> Cycle(1, 3, 4, 5, 2, 6).domain
             range(1, 7)
         """
         return self._domain
 
     @property
     def elements(self) -> Tuple[int]:
-        """Return a tuple containing the elements of the cycle.
+        """Return a tuple containing the elements of the cycle in its standard form.
 
         :return: The elements of the cycle.
         :rtype: Tuple[int]
 
         :example:
             >>> from symmetria import Cycle
             ...
+            >>> Cycle(1).elements
+            (1,)
             >>> Cycle(3, 1, 2).elements
             (1, 2, 3)
+            >>> Cycle(3, 4, 7, 1, 2).elements
+            (1, 2, 3, 4, 7)
         """
         return self._cycle
 
     def equivalent(self, other: Any) -> bool:
         """Check if the cycle is equivalent to the `other` object.
 
         In `symmetria`, a permutation of the symmetric group can have different representations. For example,
@@ -466,15 +504,15 @@
     def inverse(self) -> "Cycle":
         r"""Return the inverse of the cycle.
 
         Recall that the inverse of a permutation :math:`\sigma \in S_n`, for some :math:`n \in \mathbb{N}`, is the
         the only permutation :math:`\tau \in S_n` such that :math:`\sigma * \tau = \tau * \sigma = id`,
         where :math:`id` is the identity permutation.
 
-        In the case of cycles, it suffices to consider the backward cycle.
+        Note that for a cycle, its inverse is just the backward cycle.
 
         :return: The inverse of the cycle.
         :rtype: Cycle
 
         :example:
             >>> from symmetria import Cycle
             ...
@@ -630,15 +668,16 @@
         """
         return {element: self[(idx + 1) % len(self)] for idx, element in enumerate(self.elements)}
 
     def orbit(self, item: Any) -> List[Any]:
         r"""Compute the orbit of `item` object under the action of the cycle.
 
         Recall that the orbit of the action of a cycle :math:`\sigma` on an element x is given by the set
-        :math:`\{ \sigma^n(x): n \in \mathbb{N}\}`.
+
+        .. math:: \{ \sigma^n(x): n \in \mathbb{N}\}.
 
         :param item: The initial element or iterable to compute the orbit for.
         :type item: Any
 
         :return: The orbit of the specified element under the permutation.
         :rtype: List[Any]
```

### Comparing `symmetria-0.0.4/symmetria/elements/cycle_decomposition.py` & `symmetria-0.0.5/symmetria/elements/cycle_decomposition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from math import lcm, prod
 from typing import Any, Set, Dict, List, Tuple, Union, Iterable
 from itertools import combinations
 
 import symmetria.elements.cycle
 import symmetria.elements.permutation
-from symmetria.elements._interface import _Element
+from symmetria.elements._base import _Element
 
 __all__ = ["CycleDecomposition"]
 
 
 class CycleDecomposition(_Element):
     r"""The ``CycleDecomposition`` class represents the cycle decomposition of a permutation of the symmetric group.
 
@@ -169,21 +169,31 @@
         else:
             return permuted
 
     def _call_on_permutation(self, original: "Permutation") -> "Permutation":
         return symmetria.elements.permutation.Permutation.from_cycle_decomposition(self) * original
 
     def __eq__(self, other: Any) -> bool:
-        """Check if the cycle decomposition is equal to the `another` object.
+        """Check if the cycle decomposition is equal to the `other` object.
 
         :param other: The object to compare with.
         :type other: Any
 
         :return: True if the cycle decomposition is equal to `other`, i.e., they define the same map. Otherwise, False.
         :rtype: bool
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1, 2)) == CycleDecomposition(Cycle(1, 2))
+            True
+            >>> CycleDecomposition(Cycle(1), Cycle(2)) == CycleDecomposition(Cycle(1), Cycle(2))
+            True
+            >>> CycleDecomposition(Cycle(1), Cycle(2, 3)) == CycleDecomposition(Cycle(1))
+            False
         """
         if isinstance(other, CycleDecomposition):
             if len(self) != len(other):
                 return False
             else:
                 for cycle_a, cycle_b in zip(self, other):
                     if cycle_a.elements != cycle_b.elements:
@@ -287,39 +297,47 @@
 
         :param power: the exponent for the power operation.
         :type power: int
 
         :return: the power of the cycle decomposition.
         :rtype: Permutation
 
+        :raises TypeError: If `power` is not an integer.
+
         :example:
             >>> from symmetria import Cycle, CycleDecomposition
             ...
             >>> CycleDecomposition(Cycle(3), Cycle(1), Cycle(2)) ** 0
             CycleDecomposition(Cycle(1), Cycle(2), Cycle(3))
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3)) ** 1
             CycleDecomposition(Cycle(1, 2), Cycle(3))
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3)) ** -1
             CycleDecomposition(Cycle(1, 2), Cycle(3))
+            >>> CycleDecomposition(Cycle(1, 3), Cycle(2, 4))**2
+            CycleDecomposition(Cycle(1), Cycle(2), Cycle(3), Cycle(4))
         """
         if isinstance(power, int) is False:
             raise TypeError(f"Power operation for type {type(power)} not supported.")
         elif self is False or power == 0:
             return CycleDecomposition(*[symmetria.elements.cycle.Cycle(i) for i in self.domain])
         elif power == 1:
             return self
         elif power <= -1:
             return self.inverse() ** abs(power)
         else:
             return self * (self ** (power - 1))
 
     def __repr__(self) -> str:
-        r"""Return a string representation of the cycle decomposition in the format
-        'CycleDecomposition(Cycle(x, ...), Cycle(y, ...), ...)', where :math:`x, y, ... \in \mathbb{N}` are
-        the elements of the cycles.
+        r"""Return a string representation of the cycle decomposition.
+
+         The string representation is in the following format:
+
+        .. math:: 'CycleDecomposition(Cycle(x, ...), Cycle(y, ...), ...)',
+
+        where :math:`x, y, ... \in \mathbb{N}` are the elements of the cycles.
 
         :return: A string representation of the cycle decomposition.
         :rtype: str
 
         :example:
             >>> from symmetria import Cycle, CycleDecomposition
             ...
@@ -329,15 +347,15 @@
             'CycleDecomposition(Cycle(1, 3), Cycle(2))'
             >>> CycleDecomposition(Cycle(1, 3), Cycle(4, 5, 2, 6)).__repr__()
             'CycleDecomposition(Cycle(1, 3), Cycle(2, 6, 4, 5))'
         """
         return f"CycleDecomposition({', '.join([cycle.__repr__() for cycle in self])})"
 
     def __str__(self) -> str:
-        """Return a string representation of the cycle decmposition in the cycle notation.
+        """Return a string representation of the cycle decomposition in the cycle notation.
 
         :return: A string representation of the cycle decomposition.
         :rtype: str
 
         :example:
             >>> from symmetria import Cycle, CycleDecomposition
             ...
@@ -346,14 +364,36 @@
             >>> str(CycleDecomposition(Cycle(1, 3), Cycle(2)))
             '(1 3)(2)'
             >>> str(CycleDecomposition(Cycle(1, 3), Cycle(4, 5, 2, 6)))
             '(1 3)(2 6 4 5)'
         """
         return "".join([str(c) for c in self])
 
+    def ascents(self) -> List[int]:
+        r"""Return the ascents of the cycle decomposition.
+
+        Recall that an ascent of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any position
+        :math:`i<n` such that :math:`\sigma(i) < \sigma(i+1)`.
+
+        :return: The ascents of the cycle decomposition.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1, 2, 3)).ascents()
+            [1]
+            >>> CycleDecomposition(Cycle(1), Cycle(2), Cycle(3)).ascents()
+            [1, 2]
+            >>> CycleDecomposition(Cycle(2, 3), Cycle(4, 5, 1)).ascents()
+            [3]
+        """
+        permutation = symmetria.Permutation.from_cycle_decomposition(self)
+        return permutation.ascents()
+
     def cycle_decomposition(self) -> "CycleDecomposition":
         """Return the cycle decomposition of the permutation.
 
         As a cycle decomposition is already in the
         cycle decomposition, the method return the cycle decomposition itself.
 
         :return: The cycle decomposition of the permutation.
@@ -400,14 +440,36 @@
             >>> CycleDecomposition(Cycle(1, 3, 2), Cycle(4)).cycle_type()
             (1, 3)
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3, 4)).cycle_type()
             (2, 2)
         """
         return tuple(sorted(len(cycle) for cycle in self))
 
+    def descents(self) -> List[int]:
+        r"""Return the descents of the cycle decomposition.
+
+        Recall that a descent of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any position
+        :math:`i<n` such that :math:`\sigma(i) > \sigma(i+1)`.
+
+        :return: The descents of the cycle decomposition.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1, 2, 3)).descents()
+            [2]
+            >>> CycleDecomposition(Cycle(1), Cycle(2), Cycle(3)).descents()
+            []
+            >>> CycleDecomposition(Cycle(2, 3), Cycle(4, 5, 1)).descents()
+            [1, 2, 4]
+        """
+        permutation = symmetria.Permutation.from_cycle_decomposition(self)
+        return permutation.descents()
+
     @property
     def domain(self) -> Iterable[int]:
         """Return an iterable containing the elements of the domain of the cycle decomposition.
 
         The domain of a cycle decomposition is the set of indices for which the cycle decomposition is defined.
 
         :return: The domain of the cycle decomposition.
@@ -460,14 +522,43 @@
                     if len(cycle) > 1 and cycle != other:
                         return False
             return True
         elif isinstance(other, symmetria.elements.permutation.Permutation):
             return symmetria.elements.permutation.Permutation.from_cycle_decomposition(self) == other
         return False
 
+    def exceedances(self, weakly: bool = False) -> List[int]:
+        r"""Return the exceedances of the cycle decomposition.
+
+        Recall that an exceedance of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any
+        position :math:`i \in \{ 1, ..., n\}` where :math:`\sigma(i) > i`. An exceedance is called weakly if
+        :math:`\sigma(i) \geq i`.
+
+        :param weakly: `True` to return the weakly exceedances of the cycle decomposition. Default `False`.
+        :type weakly: bool
+
+        :return: The exceedances of the cycle decomposition.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1, 2), Cycle(3)).exceedances()
+            [1]
+            >>> CycleDecomposition(Cycle(1, 2), Cycle(3)).exceedances(weakly=True)
+            [1, 3]
+            >>> CycleDecomposition(Cycle(2, 3), Cycle(4, 5, 1)).exceedances()
+            [1, 2, 4]
+            >>> CycleDecomposition(Cycle(1), Cycle(2), Cycle(3)).exceedances()
+            []
+            >>> CycleDecomposition(Cycle(1), Cycle(2), Cycle(3)).exceedances(weakly=True)
+            [1, 2, 3]
+        """
+        return symmetria.Permutation.from_cycle_decomposition(self).exceedances(weakly=weakly)
+
     def inverse(self) -> "CycleDecomposition":
         r"""Return the inverse of the cycle decomposition.
 
         Recall that the inverse of a permutation :math:`\sigma \in S_n`, for some :math:`n \in \mathbb{N}`, is the
         the only permutation :math:`\tau \in S_n` such that :math:`\sigma * \tau = \tau * \sigma = id`,
         where :math:`id` is the identity permutation.
 
@@ -642,15 +733,16 @@
             _map.update(cycle.map)
         return _map
 
     def orbit(self, item: Any) -> List[Any]:
         r"""Compute the orbit of `item` object under the action of the cycle decomposition.
 
         Recall that the orbit of the action of a cycle decomposition :math:`\sigma` on an element x is given by the set
-        :math:`\{ \sigma^n(x): n \in \mathbb{N}\}`.
+
+        ..math:: \{ \sigma^n(x): n \in \mathbb{N}\}.
 
         :param item: The initial element or iterable to compute the orbit for.
         :type item: Any
 
         :return: The orbit of the specified element under the permutation.
         :rtype: List[Any]
         """
@@ -679,14 +771,39 @@
             >>> CycleDecomposition(Cycle(1, 3, 2)).order()
             3
             >>> CycleDecomposition(Cycle(1, 3, 2), Cycle(4, 5)).order()
             6
         """
         return lcm(*[len(cycle) for cycle in self])
 
+    def records(self) -> List[int]:
+        r"""Return the records of the cycle decomposition.
+
+        Recall that a record of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is a position
+        :math:`i \in \{1, ..., n\}` such that is either :math:`i=1` or :math:`\sigma(j) < \sigma(i)`
+        for all :math:`j<i`.
+
+        .. note:: There are definitions of records in the literature where the first index is not considered as a
+            record.
+
+        :return: The records of the cycle decomposition.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> CycleDecomposition(Cycle(1)).records()
+            [1]
+            >>> CycleDecomposition(Cycle(1, 2), Cycle(3)).records()
+            [1, 3]
+            >>> CycleDecomposition(Cycle(1), Cycle(2, 4, 7, 6), Cycle(3, 5)).records()
+            [1, 2, 3, 4]
+        """
+        return symmetria.Permutation.from_cycle_decomposition(self).records()
+
     def sgn(self) -> int:
         r"""Return the sign of the cycle decomposition.
 
         Recall that the sign, signature, or signum of a permutation :math:`\sigma` is defined as +1 if :math:`\sigma`
         is even, and -1 if :math:`\sigma` is odd.
 
         To compute the sign of a cycle decomposition, we use the fact that the sign is a homomorphism of groups, i.e.,
@@ -704,22 +821,25 @@
             -1
             >>> CycleDecomposition(Cycle(1), Cycle(2, 4, 7, 6), Cycle(3, 5)).sgn()
             1
         """
         return prod([cycle.sgn() for cycle in self])
 
     def support(self) -> Set[int]:
-        """Return a set containing the indices in the domain of the permutation whose images are different from
-        their respective indices, i.e., the set of :math:`n` in the permutation domain which are not mapped to itself.
+        r"""Return a set containing the indices in the domain of the permutation whose images are different from
+        their respective indices, i.e., the set of :math:`n \in \mathbb{N}` in the permutation domain which are
+        not mapped to itself.
 
         :return: The support set of the cycle decomposition.
         :rtype: Set[int]
 
         :example:
             >>> from symmetria import Cycle, CycleDecomposition
             ...
             >>> CycleDecomposition(Cycle(1)).support()
             set()
             >>> CycleDecomposition(Cycle(1), Cycle(2, 3)).support()
             {2, 3}
+            >>> CycleDecomposition(Cycle(3, 4, 5, 6), Cycle(2, 1)).support()
+            {1, 2, 3, 4, 5, 6}
         """
         return {element for cycle in self if len(cycle) != 1 for element in cycle.elements}
```

### Comparing `symmetria-0.0.4/symmetria/elements/permutation.py` & `symmetria-0.0.5/symmetria/elements/permutation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Set, Dict, List, Tuple, Union, Iterable
 
 import symmetria.elements.cycle
 import symmetria.elements.cycle_decomposition
-from symmetria.elements._interface import _Element
+from symmetria.elements._base import _Element
 
 __all__ = ["Permutation"]
 
 
 class Permutation(_Element):
     r"""The ``Permutation`` class represents an element of the symmetric group as a map, i.e., a bijective function
     from a finite set of integer :math:`\{1, ..., n\}`, for some :math:`n \in \mathbb{N}_{>0}`, to itself.
@@ -172,32 +172,54 @@
         """Check if the permutation is equal to `another` object.
 
         :param other: The object to compare with.
         :type other: Any
 
         :return: True if the permutation is equal to `other`, i.e., they define the same map. Otherwise, False.
         :rtype: bool
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3) == Permutation(1, 2, 3)
+            True
+            >>> Permutation(1, 2, 3) == Permutation(3, 2, 1)
+            False
+            >>> Permutation(1, 2, 3) == 12
+            False
         """
         if isinstance(other, Permutation):
             return self.map == other.map
         return False
 
     def __getitem__(self, item: int) -> int:
         """Return the value of the permutation at the given index `item`.
 
         In other words, it returns the image of the permutation at point `item`.
-        The index corresponds to the position in the permutation, starting from 0.
+
+        .. note:: The index corresponds to the element in the domain of the permutation, i.e.,
+            the index is a number between 1 and the length of the permutation.
 
         :param item: The index of the permutation.
         :type item: int
 
         :return: The value of the permutation at the specified index.
         :rtype: int
 
         :raises IndexError: If the index is out of range.
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> permutation = Permutation(2, 3, 1)
+            >>> for idx in range(1, len(permutation)+1):
+            ...     permutation[idx]
+            2
+            3
+            1
         """
         return self.map[item]
 
     def __int__(self) -> int:
         """Convert the permutation to its integer representation.
 
         :return: The integer representation of the permutation.
@@ -268,37 +290,41 @@
 
         :param power: the exponent for the power operation.
         :type power: int
 
         :return: the power of the permutation.
         :rtype: Permutation
 
+        :raises TypeError: If `power` is not an integer.
+
         :example:
             >>> from symmetria import Permutation
             ...
-            >>> Permutation(3, 1, 2) ** 0
+            >>> Permutation(3, 1, 2)**0
             Permutation(1, 2, 3)
-            >>> Permutation(3, 1, 2) ** 1
+            >>> Permutation(3, 1, 2)**1
             Permutation(3, 1, 2)
-            >>> Permutation(3, 1, 2) ** -1
+            >>> Permutation(3, 1, 2)**-1
+            Permutation(2, 3, 1)
+            >>> Permutation(3, 1, 2)**2
             Permutation(2, 3, 1)
         """
         if isinstance(power, int) is False:
             raise TypeError(f"Power operation for type {type(power)} not supported.")
         elif self is False or power == 0:
             return Permutation(*list(self.domain))
         elif power == 1:
             return self
         elif power <= -1:
             return self.inverse() ** abs(power)
         else:
             return self * (self ** (power - 1))
 
     def __repr__(self) -> str:
-        r"""Return a string representation of the permutation in the format "Permutation(x, y, z, ...)",
+        r"""Return a string representation of the permutation in the format `Permutation(x, y, z, ...)`,
         where :math:`x, y, z, ... \in \mathbb{N}` are the elements of the permutation.
 
         :return: A string representation of the permutation.
         :rtype: str
 
         :example:
             >>> from symmetria import Permutation
@@ -307,28 +333,51 @@
             'Permutation(3, 1, 2)'
             >>> Permutation(1, 3, 4, 5, 2, 6).__repr__()
             'Permutation(1, 3, 4, 5, 2, 6)'
         """
         return f"Permutation({', '.join([str(self._map[idx]) for idx in self.domain])})"
 
     def __str__(self) -> str:
-        """Return a string representation of the permutation in the form of tuples.
+        """Return a string representation of the permutation in the form of a tuple.
+
+        The string representation represents the image of the permutation.
 
         :return: A string representation of the permutation.
         :rtype: str
 
         :example:
             >>> from symmetria import Permutation
             ...
             >>> print(Permutation(3, 1, 2))
             (3, 1, 2)
             >>> print(Permutation(1, 3, 4, 5, 2, 6))
             (1, 3, 4, 5, 2, 6)
         """
-        return "(" + ", ".join([str(self[idx]) for idx in self.domain]) + ")"
+        return str(self.image) if len(self.image) > 1 else f"({self.image[0]})"
+
+    def ascents(self) -> List[int]:
+        r"""Return the ascents of the permutation.
+
+        Recall that an ascent of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any position
+        :math:`i<n` such that :math:`\sigma(i) < \sigma(i+1)`.
+
+        :return: The ascents of the permutation.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).ascents()
+            [1, 2]
+            >>> Permutation(3, 4, 5, 2, 1, 6, 7).ascents()
+            [1, 2, 5, 6]
+            >>> Permutation(4, 3, 2, 1).ascents()
+            []
+        """
+        return [idx + 1 for idx in range(len(self) - 1) if self.image[idx] < self.image[idx + 1]]
 
     def cycle_decomposition(self) -> "CycleDecomposition":
         """Decompose the permutation into its cycle decomposition.
 
         :return: The cycle decomposition of the permutation.
         :rtype: CycleDecomposition
 
@@ -370,15 +419,15 @@
 
     def cycle_type(self) -> Tuple[int]:
         r"""Return the cycle type of the permutation.
 
         Recall that the cycle type of the permutation :math:`\sigma` is a sequence of integer, where
         There is a 1 for every fixed point of :math:`\sigma`, a 2 for every transposition, and so on.
 
-        .. note:: Note that the resulting tuple is sorted in ascending order.
+        .. note:: The resulting tuple is sorted in ascending order.
 
         :return: The cycle type of the permutation.
         :rtype: Tuple[int]
 
         :example:
             >>> from symmetria import Permutation
             ...
@@ -389,14 +438,35 @@
             >>> Permutation(3, 1, 2, 4, 5, 6).cycle_type()
             (1, 1, 1, 3)
             >>> Permutation(1, 4, 5, 7, 3, 2, 6).cycle_type()
             (1, 2, 4)
         """
         return tuple(sorted(len(cycle) for cycle in self.cycle_decomposition()))
 
+    def descents(self) -> List[int]:
+        r"""Return the descents of the permutation.
+
+        Recall that a descent of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any position
+        :math:`i<n` such that :math:`\sigma(i) > \sigma(i+1)`.
+
+        :return: The descents of the permutation.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).descents()
+            []
+            >>> Permutation(3, 4, 5, 2, 1, 6, 7).descents()
+            [3, 4]
+            >>> Permutation(4, 3, 2, 1).descents()
+            [1, 2, 3]
+        """
+        return [idx + 1 for idx in range(len(self) - 1) if self.image[idx] > self.image[idx + 1]]
+
     @property
     def domain(self) -> Iterable[int]:
         """Return an iterable containing the elements of the domain of the permutation.
 
         The domain of a permutation is the set of indices for which the permutation is defined.
 
         :return: The domain of the permutation.
@@ -441,14 +511,45 @@
             return self == other
         elif isinstance(other, symmetria.elements.cycle.Cycle):
             return self == Permutation.from_cycle(other)
         elif isinstance(other, symmetria.elements.cycle_decomposition.CycleDecomposition):
             return self == Permutation.from_cycle_decomposition(other)
         return False
 
+    def exceedances(self, weakly: bool = False) -> List[int]:
+        r"""Return the exceedances of the permutation.
+
+        Recall that an exceedance of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is any
+        position :math:`i \in \{ 1, ..., n\}` where :math:`\sigma(i) > i`. An exceedance is called weakly if
+        :math:`\sigma(i) \geq i`.
+
+        :param weakly: `True` to return the weakly exceedances of the permutation. Default `False`.
+        :type weakly: bool
+
+        :return: The exceedances of the permutation.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).exceedances()
+            []
+            >>> Permutation(1, 2, 3).exceedances(weakly=True)
+            [1, 2, 3]
+            >>> Permutation(4, 3, 2, 1).exceedances()
+            [1, 2]
+            >>> Permutation(3, 4, 5, 2, 1, 6, 7).exceedances()
+            [1, 2, 3]
+            >>> Permutation(3, 4, 5, 2, 1, 6, 7).exceedances(weakly=True)
+            [1, 2, 3, 6, 7]
+        """
+        if weakly:
+            return [i for i, p in enumerate(self.image, 1) if p >= i]
+        return [i for i, p in enumerate(self.image, 1) if p > i]
+
     @classmethod
     def from_cycle(cls, cycle: "Cycle") -> "Permutation":
         """Return a permutation from a cycle.
 
         In other word, it converts a cycle into a permutation.
 
         :param cycle: A cycle.
@@ -511,22 +612,24 @@
         :rtype: Permutation
 
         :example:
             >>> from symmetria import Permutation
             ...
             >>> Permutation.from_dict({1: 3, 2: 1, 3: 2})
             Permutation(3, 1, 2)
+            >>> Permutation.from_dict({1: 5, 2: 3, 3: 1, 4: 2, 5:4})
+            Permutation(5, 3, 1, 2, 4)
         """
         return Permutation(*[p[idx] for idx in range(1, len(p) + 1)])
 
     @property
     def image(self) -> Tuple[int]:
         r"""Return the image of the permutation.
 
-        For example, to define the permutation :math:`\sigma \in S_3` given by :math:`\sigma(1)=3, \sigma(2)=1`, and
+        For example, consider the permutation :math:`\sigma \in S_3` given by :math:`\sigma(1)=3, \sigma(2)=1`, and
         :math:`\sigma (3)=2`, then the image of :math:`\sigma` is :math:`(3, 1, 2)` .
 
         :return: The image of the permutation.
         :rtype: Tuple[int]
 
         :example:
             >>> from symmetria import Permutation
@@ -601,24 +704,24 @@
 
         :param other: a permutation
         :type other: Permutation
 
         :return: True if self and other are conjugated, False otherwise.
         :rtype: bool
 
+        :raises TypeError: If `other` is not a permutation.
+
         :example:
             >>> from symmetria import Permutation
             ...
             >>> Permutation(1, 2, 3).is_conjugate(Permutation(1, 2, 3))
             True
             >>> Permutation(1, 2, 3).is_conjugate(Permutation(3, 2, 1))
             False
-            >>> permutation_a = Permutation(3, 2, 5, 4, 1)
-            >>> permutation_b = Permutation(5, 2, 1, 4, 3)
-            >>> permutation_a.is_conjugate(permutation_b)
+            >>> Permutation(3, 2, 5, 4, 1).is_conjugate(Permutation(5, 2, 1, 4, 3))
             True
         """
         if isinstance(other, Permutation) is False:
             raise TypeError(f"Method `is_conjugate` not implemented for type {type}.")
         return self.cycle_type() == other.cycle_type()
 
     def is_derangement(self) -> bool:
@@ -751,15 +854,16 @@
         """
         return str(int(self))
 
     def orbit(self, item: Any) -> List[Any]:
         r"""Compute the orbit of `item` object under the action of the cycle.
 
         Recall that the orbit of the action of a permutation :math:`\sigma` on an element x is given by the set
-        :math:`\{ \sigma^n(x): n \in \mathbb{N}\}`.
+
+        .. math:: \{ \sigma^n(x): n \in \mathbb{N}\}
 
         :param item: The initial element or iterable to compute the orbit for.
         :type item: Any
 
         :return: The orbit of the specified element under the permutation.
         :rtype: List[Any]
 
@@ -802,14 +906,45 @@
             >>> Permutation(3, 1, 2).order()
             3
             >>> Permutation(1, 3, 4, 5, 2, 6).order()
             4
         """
         return self.cycle_decomposition().order()
 
+    def records(self) -> List[int]:
+        r"""Return the records of the permutation.
+
+        Recall that a record of a permutation :math:`\sigma \in S_n`, where :math:`n \in \mathbb{N}`, is a position
+        :math:`i \in \{1, ..., n\}` such that is either :math:`i=1` or :math:`\sigma(j) < \sigma(i)`
+        for all :math:`j<i`.
+
+        .. note:: There are definitions of records in the literature where the first index is not considered as a
+            record.
+
+        :return: The records of the permutation.
+        :rtype: List[int]
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).records()
+            [1, 2, 3]
+            >>> Permutation(3, 1, 2).records()
+            [1]
+            >>> Permutation(1, 3, 4, 5, 2, 6).records()
+            [1, 2, 3, 4, 6]
+        """
+        records = [1]
+        tmp_max = self[1]
+        for i in self.domain:
+            if self[i] > tmp_max:
+                records.append(i)
+                tmp_max = self[i]
+        return records
+
     def sgn(self) -> int:
         r"""Return the sign of the permutation.
 
         Recall that the sign, signature, or signum of a permutation :math:`\sigma` is defined as +1 if :math:`\sigma`
         is even, and -1 if :math:`\sigma` is odd.
 
         :return: 1 if the permutation is even, -1 if the permutation is odd.
```

### Comparing `symmetria-0.0.4/symmetria.egg-info/PKG-INFO` & `symmetria-0.0.5/symmetria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.4
+Version: 0.0.5
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.4 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.5 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
```

