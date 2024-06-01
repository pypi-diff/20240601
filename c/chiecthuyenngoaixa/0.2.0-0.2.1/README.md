# Comparing `tmp/chiecthuyenngoaixa-0.2.0.tar.gz` & `tmp/chiecthuyenngoaixa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiecthuyenngoaixa-0.2.0.tar", max compression
+gzip compressed data, was "chiecthuyenngoaixa-0.2.1.tar", max compression
```

## Comparing `chiecthuyenngoaixa-0.2.0.tar` & `chiecthuyenngoaixa-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1066 2023-09-04 02:30:44.137049 chiecthuyenngoaixa-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     2655 2023-09-04 02:30:44.137049 chiecthuyenngoaixa-0.2.0/README.md
--rwxr-xr-x   0        0        0      407 2023-09-04 02:30:44.137049 chiecthuyenngoaixa-0.2.0/ctnx/__init__.py
--rw-r--r--   0        0        0    11296 2023-09-04 02:30:44.137049 chiecthuyenngoaixa-0.2.0/ctnx/constants.py
--rw-r--r--   0        0        0     8363 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/legacy.py
--rw-r--r--   0        0        0     3436 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/misc.py
--rw-r--r--   0        0        0     4282 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/number.py
--rwxr-xr-x   0        0        0     1051 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/sort.py
--rw-r--r--   0        0        0     9433 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/syllable.py
--rw-r--r--   0        0        0    13354 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/ctnx/validation.py
--rwxr-xr-x   0        0        0      946 2023-09-04 02:30:44.141049 chiecthuyenngoaixa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 chiecthuyenngoaixa-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1066 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     4640 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/README.md
+-rwxr-xr-x   0        0        0      407 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/__init__.py
+-rw-r--r--   0        0        0    40977 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/constants.py
+-rw-r--r--   0        0        0     8363 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/legacy.py
+-rw-r--r--   0        0        0     3436 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/misc.py
+-rw-r--r--   0        0        0     4282 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/number.py
+-rwxr-xr-x   0        0        0     1068 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/sort.py
+-rw-r--r--   0        0        0    10315 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/syllable.py
+-rw-r--r--   0        0        0    13371 2024-06-01 08:32:13.604681 chiecthuyenngoaixa-0.2.1/ctnx/validation.py
+-rwxr-xr-x   0        0        0      946 2024-06-01 08:32:13.608681 chiecthuyenngoaixa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5660 1970-01-01 00:00:00.000000 chiecthuyenngoaixa-0.2.1/PKG-INFO
```

### Comparing `chiecthuyenngoaixa-0.2.0/LICENSE` & `chiecthuyenngoaixa-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/legacy.py` & `chiecthuyenngoaixa-0.2.1/ctnx/legacy.py`

 * *Files identical despite different names*

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/misc.py` & `chiecthuyenngoaixa-0.2.1/ctnx/misc.py`

 * *Files identical despite different names*

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/number.py` & `chiecthuyenngoaixa-0.2.1/ctnx/number.py`

 * *Files identical despite different names*

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/sort.py` & `chiecthuyenngoaixa-0.2.1/ctnx/sort.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from .constants import CHAR_ORDER_DICT
 
 
 class ViSortKey:
     """Vietnamese-aware sorting key class for use with the `key` parameter
-    in `sorted()` and `str.sort()` functions."""
+    in  :py:func:`sorted` and  :py:meth:`list.sort` functions."""
 
     def __init__(self, string=''):
         self.string = string
 
     def __repr__(self):
         return f"<ViSortKey '{self.string}'>"
```

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/syllable.py` & `chiecthuyenngoaixa-0.2.1/ctnx/syllable.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,47 +67,53 @@
 
 class Syllable:
     """Represent a syllable in Vietnamese language."""
 
     ONSETS = ('b', 'ch', 'c', 'd', 'đ', 'gh', 'gi', 'g', 'h', 'kh', 'k', 'l', 'm', 'ngh', 'ng', 'nh', 'ng',
     'n', 'ph', 'p', 'qu', 'r', 's', 'th', 'tr', 't', 'v', 'x', '')
     MONOPHTHONGS = ('a', 'ă', 'â', 'e', 'ê', 'i', 'o', 'ô', 'ơ', 'u', 'ư', 'y')
-    # 'oo' is not a diphthong but it's denoted using two characters
-    OPEN_DIPHTHONGS = ('iê', 'oă', 'oo', 'uâ', 'uô', 'ươ', 'yê')
+    # 'oo' and 'ôô' are not a diphthong but it's denoted using two characters
+    OPEN_DIPHTHONGS = ('iê', 'oă', 'oo', 'ôô', 'uâ', 'uô', 'ươ', 'yê')
     ROUNDED_DIPHTHONGS = ('oa', 'oe', 'uê')
     CLOSED_DIPHTHONGS = ('ai', 'ao', 'au', 'ay', 'âu', 'ây', 'eo', 'êu', 'ia', 'iu', 'oi',
-    'ôi', 'ơi', 'ua', 'ui', 'uơ', 'uy', 'ưa', 'ưi', 'ưu')
+    'ôi', 'ơi', 'ua', 'ui', 'uơ', 'uy', 'ưa', 'ưi', 'ưu', 'yu')
     DIPHTHONGS = OPEN_DIPHTHONGS + ROUNDED_DIPHTHONGS + CLOSED_DIPHTHONGS
     CLOSED_TRIPHTHONGS = ('iêu', 'oai', 'oao', 'oay', 'oeo', 'uay', 'uây', 'uôi', 'uya', 'uyu', 'ươi', 'ươu', 'yêu')
     OPEN_TRIPHTHONGS = ('uyê',)
     TRIPHTHONGS = CLOSED_TRIPHTHONGS + OPEN_TRIPHTHONGS
     OPEN_NUCLEI = OPEN_TRIPHTHONGS + OPEN_DIPHTHONGS
     CLOSED_NUCLEI = CLOSED_TRIPHTHONGS + CLOSED_DIPHTHONGS
     NUCLEI = TRIPHTHONGS + DIPHTHONGS + MONOPHTHONGS
     CODAS = ('ch', 'c', 'm', 'ng', 'nh', 'n', 'p', 't', '')
     
-    AUTO_CORRECT = True
+    AUTO_CORRECT: bool = True
     
     tone_placer = NewStyleTonePlacer
     
     def __init__(self, onset: str, nucleus: str, coda: str, tone=''):
         self.onset = onset
         self.nucleus = nucleus
         self.coda = coda
         self.tone = tone
    		
     def __repr__(self):
-       return f"Syllable({self.onset}, {self.nucleus}, {self.coda}, {self.tone})"
+        if self.tone:
+            return f"Syllable({self.onset}, {self.nucleus}, {self.coda}, {self.tone})"
+        else:
+            return f"Syllable({self.onset}, {self.nucleus}, {self.coda})"
    
     def __str__(self):
        return self.to_string()
        
     def __bool__(self):
         return True
     
+    def __eq__(self, other: Syllable):
+        return self.onset == other.onset and self.nucleus == other.nucleus and self.coda == self.coda and self.tone == other.tone
+    
     @classmethod
     @lru_cache
     def from_string(cls, string: str) -> Syllable:
         """Create a Syllable object from string."""
 
         string = normalize(string).lower()
         if ' ' in string:
@@ -124,33 +130,31 @@
             if (len(string) > 1) and (string[0] == 'ê'):
                 string = 'i' + string
         try:
             nucleus = next(filter(string.startswith, cls.NUCLEI))
             string = string[len(nucleus):]
         except StopIteration:
             if onset == 'gi':
-                if string == '':
-                    nucleus = 'i'
-                else:
-                    raise Exception(f"Invaild syllable: {original}")
+                nucleus = 'i'
+            else:
+                raise Exception(f"Invaild syllable: {original}")
         
         coda = next(filter(string.startswith, cls.CODAS))
         string = string[len(coda):]
                 
         if string != '':
             raise Exception(f"Unexpected characters '{string}' after a syllable (in '{original}'')")
                 
         return Syllable(onset, nucleus, coda, tone)
        
     def to_string(self) -> str:
         """Return the written form of the syllable."""
         onset = self.onset
         nucleus = self.nucleus
         coda = self.coda
-        tone = self.tone
         
         if (onset == 'gi') and ((nucleus == 'i') or (nucleus[:2] == 'iê')):
             onset = 'g'
         
         return ''.join((onset, self.tone_placer.place(self), coda))
 
     @property
@@ -182,15 +186,15 @@
             else:
                 self._onset = value
         else:
             raise ValueError(f"Invaild onset: {value}")
     
     @property
     def nucleus(self) -> str:
-        """The vowel part of the syllable."""
+        """The vowel part of the syllable as stored in this object, not necessarily including the semivowel."""
         
         return self._nucleus
         
     @nucleus.setter
     def nucleus(self, value: str):
         value = value.lower()
         original = value
@@ -222,14 +226,16 @@
         value = value.lower()
         original = value
         original_nucleus = self.nucleus
         if value in self.CODAS:
             if value == '':
                 if self.nucleus in self.OPEN_NUCLEI:
                     raise ValueError(f"Open syllable (nucleus: {self.nucleus}) must have a coda")
+            elif (self.nucleus == 'uy' or (self.nucleus == 'y' and self.onset == 'qu')) and value not in {'c', 'ng', ''}:
+                pass
             elif self.nucleus in self.CLOSED_NUCLEI:
                 value = ''
             else:
                 if self.nucleus == 'y':
                     if value == 'ng':
                         value = 'nh'
                     self.nucleus = 'i'
@@ -265,7 +271,22 @@
                     elif value in {'', '\\', '?'}:
                         value = '.'
                     elif value == '~':
                         value = '/'
             self._tone = value
         else:
             raise ValueError(f"Invaild tone: {value}")
+    
+    @property
+    def vowel(self) -> str:
+        """The vowel part of the syllable, including the semivowel if any."""
+
+        if self.onset == 'qu':
+            return 'u' + self.nucleus
+        else:
+            return self.nucleus
+        
+    @property
+    def rime(self) -> str:
+        """The rime of the syllable, which is the combination of the vowel and the coda."""
+
+        return self.vowel + self.coda
```

### Comparing `chiecthuyenngoaixa-0.2.0/ctnx/validation.py` & `chiecthuyenngoaixa-0.2.1/ctnx/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     92: "Cần Thơ",
     93: "Hậu Giang",
     94: "Sóc Trăng",
     95: "Bạc Liêu",
     96: "Cà Mau",
 }
 
-COUNTRY_NAME_DICT = {
+COUNTRY_ID_DICT = {
     101: 'af',
     102: 'eg',
     103: 'al',
     104: 'dz',
     105: 'ad',
     106: 'ao',
     107: 'uk',
@@ -272,15 +272,15 @@
     291: 've',
     292: 'it',
     293: 'ye',
     294: 'zm',
     295: 'zw'
 }
 
-COUNTRY_ID_DICT = {
+COUNTRY_NAME_DICT = {
     101: 'Afghanistan',
     102: 'Ai Cập',
     103: 'Albania',
     104: 'Algérie (An-giê-ri)',
     105: 'Andorra (An-đô-ra)',
     106: 'Angola (Ăng-gô-la)',
     107: 'Vương quốc Liên hiệp Anh và Bắc Ireland',
@@ -531,15 +531,15 @@
     year = 1900 + century_code * 100 + int(code[4:6])
     id = code[6:]
     if int(id) == 0:
         raise ParseError("Invalid ID", 6)
     return CccdResult(id, is_male, year, country, province)
 
 
-def is_valid_cccd(raw) -> bool:
+def is_valid_cccd(raw: Union[int, str]) -> bool:
     """Check whether a Vietnamese Citizen Identity Card
     (Căn cước công dân) number is vaild or not.
     
     Parameters
     ----------
     raw : str or int
         The ID number to be validated
```

### Comparing `chiecthuyenngoaixa-0.2.0/pyproject.toml` & `chiecthuyenngoaixa-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chiecthuyenngoaixa"
-version = "0.2.0"
+version = "0.2.1"
 description = "An utility library for processing Vietnamese texts"
 authors = ["IoeCmcomc <53734763+IoeCmcomc@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/IoeCmcomc/chiecthuyenngoaixa"
 keywords = ["Vietnamese", "text"]
 packages = [
```

