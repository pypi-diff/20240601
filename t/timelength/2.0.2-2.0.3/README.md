# Comparing `tmp/timelength-2.0.2.tar.gz` & `tmp/timelength-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelength-2.0.2.tar", max compression
+gzip compressed data, was "timelength-2.0.3.tar", max compression
```

## Comparing `timelength-2.0.2.tar` & `timelength-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1082 2024-04-25 11:57:51.204519 timelength-2.0.2/LICENSE
--rw-r--r--   0        0        0     5563 2024-04-25 11:57:51.204519 timelength-2.0.2/README.md
--rw-r--r--   0        0        0     1023 2024-04-25 11:57:51.204519 timelength-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      172 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/__init__.py
--rw-r--r--   0        0        0     2235 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/dataclasses.py
--rw-r--r--   0        0        0      884 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/enums.py
--rw-r--r--   0        0        0      392 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/errors.py
--rw-r--r--   0        0        0     9457 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales/english.json
--rw-r--r--   0        0        0    12113 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales/spanish.json
--rw-r--r--   0        0        0     8170 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/locales.py
--rw-r--r--   0        0        0    16803 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/parsers/parser_one.py
--rw-r--r--   0        0        0     8755 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/timelength.py
--rw-r--r--   0        0        0     1254 2024-04-25 11:57:51.204519 timelength-2.0.2/timelength/utils.py
--rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 timelength-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-06-01 11:44:52.587577 timelength-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5563 2024-06-01 11:44:52.587577 timelength-2.0.3/README.md
+-rw-r--r--   0        0        0     1023 2024-06-01 11:44:52.587577 timelength-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      172 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/__init__.py
+-rw-r--r--   0        0        0     2235 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/dataclasses.py
+-rw-r--r--   0        0        0     1573 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/enums.py
+-rw-r--r--   0        0        0      392 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/errors.py
+-rw-r--r--   0        0        0     9419 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/locales/english.json
+-rw-r--r--   0        0        0    13738 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/locales/spanish.json
+-rw-r--r--   0        0        0     8362 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/locales.py
+-rw-r--r--   0        0        0    22135 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/parsers/parser_one.py
+-rw-r--r--   0        0        0     8755 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/timelength.py
+-rw-r--r--   0        0        0     1254 2024-06-01 11:44:52.587577 timelength-2.0.3/timelength/utils.py
+-rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 timelength-2.0.3/PKG-INFO
```

### Comparing `timelength-2.0.2/LICENSE` & `timelength-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timelength-2.0.2/README.md` & `timelength-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timelength-2.0.2/pyproject.toml` & `timelength-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timelength"
-version = "2.0.2"
+version = "2.0.3"
 description = "A Python package to parse human readable lengths of time."
 authors = ["Etorix <admin@etorix.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/timelength/"
 repository = "https://github.com/EtorixDev/timelength/"
 keywords = ["timelength", "duration", "python", "parsing", "time"]
```

### Comparing `timelength-2.0.2/timelength/dataclasses.py` & `timelength-2.0.3/timelength/dataclasses.py`

 * *Files identical despite different names*

### Comparing `timelength-2.0.2/timelength/locales/english.json` & `timelength-2.0.3/timelength/locales/english.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703705%*

 * *Differences: {"'numerals'": "{'zero': {'type': 'DIGIT'}, 'one': {'type': 'DIGIT'}, 'two': {'type': 'DIGIT'}, "*

 * *               "'three': {'type': 'DIGIT'}, 'four': {'type': 'DIGIT'}, 'five': {'type': 'DIGIT'}, "*

 * *               "'six': {'type': 'DIGIT'}, 'seven': {'type': 'DIGIT'}, 'eight': {'type': 'DIGIT'}, "*

 * *               "'nine': {'type': 'DIGIT'}, 'ten': {'type': 'TEEN'}, 'eleven': {'type': 'TEEN'}, "*

 * *               "'twelve': {'type': 'TEEN'}, 'thirteen': {'type': 'TEEN'}, 'fourteen': {'type': "*

 * *               "'TE […]*

```diff
@@ -22,99 +22,99 @@
                 "billion",
                 "Billion",
                 "BILLION",
                 "billions",
                 "Billions",
                 "BILLIONS"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000000000.0
         },
         "eight": {
             "terms": [
                 "eight",
                 "Eight",
                 "EIGHT",
                 "eights",
                 "Eights",
                 "EIGHTS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 8.0
         },
         "eighteen": {
             "terms": [
                 "eighteen",
                 "Eighteen",
                 "EIGHTEEN",
                 "eighteens",
                 "Eighteens",
                 "EIGHTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 18.0
         },
         "eighty": {
             "terms": [
                 "eighty",
                 "Eighty",
                 "EIGHTY",
                 "eighties",
                 "Eighties",
                 "EIGHTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 80.0
         },
         "eleven": {
             "terms": [
                 "eleven",
                 "Eleven",
                 "ELEVEN",
                 "elevens",
                 "Elevens",
                 "ELEVENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 11.0
         },
         "fifteen": {
             "terms": [
                 "fifteen",
                 "Fifteen",
                 "FIFTEEN",
                 "fifteens",
                 "Fifteens",
                 "FIFTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 15.0
         },
         "fifty": {
             "terms": [
                 "fifty",
                 "Fifty",
                 "FIFTY",
                 "fifties",
                 "Fifties",
                 "FIFTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 50.0
         },
         "five": {
             "terms": [
                 "five",
                 "Five",
                 "FIVE",
                 "fives",
                 "Fives",
                 "FIVES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 5.0
         },
         "forty": {
             "terms": [
                 "forty",
                 "Forty",
                 "FORTY",
@@ -124,132 +124,132 @@
                 "fourty",
                 "Fourty",
                 "FOURTY",
                 "fourties",
                 "Fourties",
                 "FOURTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 40.0
         },
         "four": {
             "terms": [
                 "four",
                 "Four",
                 "FOUR",
                 "fours",
                 "Fours",
                 "FOURS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 4.0
         },
         "fourteen": {
             "terms": [
                 "fourteen",
                 "Fourteen",
                 "FOURTEEN",
                 "fourteens",
                 "Fourteens",
                 "FOURTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 14.0
         },
         "full": {
             "terms": [
                 "full",
                 "Full",
                 "FULL",
                 "whole",
                 "Whole",
                 "WHOLE"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 1.0
         },
         "half": {
             "terms": [
                 "half",
                 "Half",
                 "HALF",
                 "halves",
                 "Halves",
                 "HALVES"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 0.5
         },
         "hundred": {
             "terms": [
                 "hundred",
                 "Hundred",
                 "HUNDRED",
                 "hundreds",
                 "Hundreds",
                 "HUNDREDS"
             ],
-            "type": "thousands",
+            "type": "HUNDRED",
             "value": 100.0
         },
         "million": {
             "terms": [
                 "million",
                 "Million",
                 "MILLION",
                 "millions",
                 "Millions",
                 "MILLIONS"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000000.0
         },
         "multiplier": {
             "terms": [
                 "of",
                 "Of",
                 "OF"
             ],
-            "type": "multiplier",
+            "type": "MULTIPLIER",
             "value": -1.0
         },
         "nine": {
             "terms": [
                 "nine",
                 "Nine",
                 "NINE",
                 "nines",
                 "Nines",
                 "NINES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 9.0
         },
         "nineteen": {
             "terms": [
                 "nineteen",
                 "Nineteen",
                 "NINETEEN",
                 "nineteens",
                 "Nineteens",
                 "NINETEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 19.0
         },
         "ninety": {
             "terms": [
                 "ninety",
                 "Ninety",
                 "NINETY",
                 "nineties",
                 "Nineties",
                 "NINETIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 90.0
         },
         "one": {
             "terms": [
                 "one",
                 "One",
                 "ONE",
@@ -258,234 +258,234 @@
                 "ONES",
                 "a",
                 "A",
                 "an",
                 "An",
                 "AN"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 1.0
         },
         "quarter": {
             "terms": [
                 "quarter",
                 "Quarter",
                 "QUARTER",
                 "quarters",
                 "Quarters",
                 "QUARTERS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 0.25
         },
         "seven": {
             "terms": [
                 "seven",
                 "Seven",
                 "SEVEN",
                 "sevens",
                 "Sevens",
                 "SEVENS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 7.0
         },
         "seventeen": {
             "terms": [
                 "seventeen",
                 "Seventeen",
                 "SEVENTEEN",
                 "seventeens",
                 "Seventeens",
                 "SEVENTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 17.0
         },
         "seventy": {
             "terms": [
                 "seventy",
                 "Seventy",
                 "SEVENTY",
                 "seventies",
                 "Seventies",
                 "SEVENTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 70.0
         },
         "six": {
             "terms": [
                 "six",
                 "Six",
                 "SIX",
                 "sixes",
                 "Sixes",
                 "SIXES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 6.0
         },
         "sixteen": {
             "terms": [
                 "sixteen",
                 "Sixteen",
                 "SIXTEEN",
                 "sixteens",
                 "Sixteens",
                 "SIXTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 16.0
         },
         "sixty": {
             "terms": [
                 "sixty",
                 "Sixty",
                 "SIXTY",
                 "sixties",
                 "Sixties",
                 "SIXTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 60.0
         },
         "ten": {
             "terms": [
                 "ten",
                 "Ten",
                 "TEN",
                 "tens",
                 "Tens",
                 "TENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 10.0
         },
         "third": {
             "terms": [
                 "third",
                 "Third",
                 "THIRD",
                 "thirds",
                 "Thirds",
                 "THIRDS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": "1/3"
         },
         "thirteen": {
             "terms": [
                 "thirteen",
                 "Thirteen",
                 "THIRTEEN",
                 "thirteens",
                 "Thirteens",
                 "THIRTEENS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 13.0
         },
         "thirty": {
             "terms": [
                 "thirty",
                 "Thirty",
                 "THIRTY",
                 "thirties",
                 "Thirties",
                 "THIRTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 30.0
         },
         "thousand": {
             "terms": [
                 "thousand",
                 "Thousand",
                 "THOUSAND",
                 "thousands",
                 "Thousands",
                 "THOUSANDS"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000.0
         },
         "three": {
             "terms": [
                 "three",
                 "Three",
                 "THREE",
                 "threes",
                 "Threes",
                 "THREES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 3.0
         },
         "trillion": {
             "terms": [
                 "trillion",
                 "Trillion",
                 "TRILLION",
                 "trillions",
                 "Trillions",
                 "TRILLIONS"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000000000000.0
         },
         "twelve": {
             "terms": [
                 "twelve",
                 "Twelve",
                 "TWELVE",
                 "twelves",
                 "Twelves",
                 "TWELVES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 12.0
         },
         "twenty": {
             "terms": [
                 "twenty",
                 "Twenty",
                 "TWENTY",
                 "twenties",
                 "Twenties",
                 "TWENTIES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 20.0
         },
         "two": {
             "terms": [
                 "two",
                 "Two",
                 "TWO",
                 "twos",
                 "Twos",
                 "TWOS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 2.0
         },
         "zero": {
             "terms": [
                 "zero",
                 "Zero",
                 "ZERO",
                 "zeroes",
                 "Zeroes",
                 "ZEROES",
                 "zeros",
                 "Zeros",
                 "ZEROS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 0.0
         }
     },
     "parser_file": "parser_one.py",
     "scales": {
         "century": {
             "plural": "centuries",
```

### Comparing `timelength-2.0.2/timelength/locales/spanish.json` & `timelength-2.0.3/timelength/locales/spanish.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878086419753086%*

 * *Differences: {"'numerals'": "{'zero': {'type': 'DIGIT'}, 'one': {'type': 'DIGIT'}, 'two': {'type': 'DIGIT'}, "*

 * *               "'three': {'type': 'DIGIT'}, 'four': {'type': 'DIGIT'}, 'five': {'type': 'DIGIT'}, "*

 * *               "'six': {'type': 'DIGIT'}, 'seven': {'type': 'DIGIT'}, 'eight': {'type': 'DIGIT'}, "*

 * *               "'nine': {'type': 'DIGIT'}, 'ten': {'type': 'TEEN'}, 'eleven': {'type': 'TEEN'}, "*

 * *               "'twelve': {'type': 'TEEN'}, 'thirteen': {'type': 'TEEN'}, 'fourteen': {'type': "*

 * *               "'TE […]*

```diff
@@ -28,123 +28,159 @@
                 "ocho",
                 "Ocho",
                 "OCHO",
                 "ochos",
                 "Ochos",
                 "OCHOS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 8.0
         },
+        "eight_hundred": {
+            "terms": [
+                "ochociento",
+                "Ochociento",
+                "OCHOCIENTO",
+                "ochocientos",
+                "Ochocientos",
+                "OCHOCIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 800.0
+        },
         "eighteen": {
             "terms": [
                 "dieciocho",
                 "Dieciocho",
                 "DIECIOCHO",
                 "dieciochos",
                 "Dieciochos",
                 "DIECIOCHOS"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 18.0
         },
         "eighty": {
             "terms": [
                 "ochenta",
                 "Ochenta",
                 "OCHENTA",
                 "ochentas",
                 "Ochentas",
                 "OCHENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 80.0
         },
         "eleven": {
             "terms": [
                 "once",
                 "Once",
                 "ONCE",
                 "onces",
                 "Onces",
                 "ONCES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 11.0
         },
         "fifteen": {
             "terms": [
                 "quince",
                 "Quince",
                 "QUINCE",
                 "quinces",
                 "Quinces",
                 "QUINCES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 15.0
         },
         "fifty": {
             "terms": [
                 "cincuenta",
                 "Cincuenta",
                 "CINCUENTA",
                 "cincuentas",
                 "Cincuentas",
                 "CINCUENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 50.0
         },
         "five": {
             "terms": [
                 "cinco",
                 "Cinco",
                 "CINCO",
                 "cincos",
                 "Cincos",
                 "CINCOS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 5.0
         },
+        "five_hundred": {
+            "terms": [
+                "quiniento",
+                "Quiniento",
+                "QUINIENTO",
+                "quinientos",
+                "Quinientos",
+                "QUINIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 500.0
+        },
         "forty": {
             "terms": [
                 "cuarenta",
                 "Cuarenta",
                 "CUARENTA",
                 "cuarentas",
                 "Cuarentas",
                 "CUARENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 40.0
         },
         "four": {
             "terms": [
                 "cuatro",
                 "Cuatro",
                 "CUATRO",
                 "cuatros",
                 "Cuatros",
                 "CUATROS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 4.0
         },
+        "four_hundred": {
+            "terms": [
+                "cuatrociento",
+                "Cuatrociento",
+                "CUATROCIENTO",
+                "cuatrocientos",
+                "Cuatrocientos",
+                "CUATROCIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 400.0
+        },
         "fourteen": {
             "terms": [
                 "catorce",
                 "Catorce",
                 "CATORCE",
                 "catorces",
                 "Catorces",
                 "CATORCES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 14.0
         },
         "full": {
             "terms": [
                 "completo",
                 "Completo",
                 "COMPLETO",
@@ -196,15 +232,15 @@
                 "toda",
                 "Toda",
                 "TODA",
                 "todas",
                 "Todas",
                 "TODAS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 1.0
         },
         "half": {
             "terms": [
                 "medio",
                 "Medio",
                 "MEDIO",
@@ -220,93 +256,108 @@
                 "mitad",
                 "Mitad",
                 "MITAD",
                 "mitads",
                 "Mitads",
                 "MITADS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 0.5
         },
         "hundred": {
             "terms": [
                 "cien",
                 "Cien",
                 "CIEN",
                 "ciens",
                 "Ciens",
                 "CIENS",
                 "cienes",
                 "Cienes",
                 "CIENES",
+                "ciento",
+                "Ciento",
+                "CIENTO",
                 "cientos",
                 "Cientos",
                 "CIENTOS"
             ],
-            "type": "thousands",
+            "type": "HUNDRED",
             "value": 100.0
         },
         "million": {
             "terms": [
                 "millon",
                 "Millon",
                 "MILLON",
                 "millons",
                 "Millons",
                 "MILLONS",
                 "millones",
                 "Millones",
                 "MILLONES"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000000.0
         },
         "multiplier": {
             "terms": [
                 "de",
                 "De",
                 "DE"
             ],
-            "type": "multiplier",
+            "type": "MULTIPLIER",
             "value": -1.0
         },
         "nine": {
             "terms": [
                 "nueve",
                 "Nueve",
                 "NUEVE",
                 "nueves",
                 "Nueves",
                 "NUEVES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 9.0
         },
+        "nine_hundred": {
+            "terms": [
+                "noveciento",
+                "Noveciento",
+                "NOVECIENTO",
+                "novecientos",
+                "Novecientos",
+                "NOVECIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 900.0
+        },
         "nineteen": {
             "terms": [
                 "diecinueve",
                 "Diecinueve",
                 "DIECINUEVE",
                 "diecinueves",
                 "Diecinueves",
                 "DIECINUEVES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 19.0
         },
         "ninety": {
             "terms": [
                 "noventa",
                 "Noventa",
                 "NOVENTA",
                 "noventas",
                 "Noventas",
                 "NOVENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 90.0
         },
         "one": {
             "terms": [
                 "uno",
                 "Uno",
                 "UNO",
@@ -322,99 +373,123 @@
                 "una",
                 "Una",
                 "UNA",
                 "unas",
                 "Unas",
                 "UNAS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 1.0
         },
         "quarter": {
             "terms": [
                 "cuarto",
                 "Cuarto",
                 "CUARTO",
                 "cuartos",
                 "Cuartos",
                 "CUARTOS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": 0.25
         },
         "seven": {
             "terms": [
                 "siete",
                 "Siete",
                 "SIETE",
                 "sietes",
                 "Sietes",
                 "SIETES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 7.0
         },
+        "seven_hundred": {
+            "terms": [
+                "seteciento",
+                "Seteciento",
+                "SETECIENTO",
+                "setecientos",
+                "Setecientos",
+                "SETECIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 700.0
+        },
         "seventeen": {
             "terms": [
                 "diecisiete",
                 "Diecisiete",
                 "DIECISIETE",
                 "diecisietes",
                 "Diecisietes",
                 "DIECISIETES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 17.0
         },
         "seventy": {
             "terms": [
                 "setenta",
                 "Setenta",
                 "SETENTA",
                 "setentas",
                 "Setentas",
                 "SETENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 70.0
         },
         "six": {
             "terms": [
                 "seis",
                 "Seis",
                 "SEIS",
                 "seises",
                 "Seises",
                 "SEISES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 6.0
         },
+        "six_hundred": {
+            "terms": [
+                "seisciento",
+                "Seisciento",
+                "SEISCIENTO",
+                "seiscientos",
+                "Seiscientos",
+                "SEISCIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 600.0
+        },
         "sixteen": {
             "terms": [
                 "dieciseis",
                 "Dieciseis",
                 "DIECISEIS",
                 "dieciseises",
                 "Dieciseises",
                 "DIECISEISES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 16.0
         },
         "sixty": {
             "terms": [
                 "sesenta",
                 "Sesenta",
                 "SESENTA",
                 "sesentas",
                 "Sesentas",
                 "SESENTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 60.0
         },
         "ten": {
             "terms": [
                 "diez",
                 "Diez",
                 "DIEZ",
@@ -430,15 +505,15 @@
                 "dieses",
                 "Dieses",
                 "DIESES",
                 "dieces",
                 "Dieces",
                 "DIECES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 10.0
         },
         "third": {
             "terms": [
                 "tercio",
                 "Tercio",
                 "TERCIO",
@@ -454,153 +529,165 @@
                 "tercera",
                 "Tercera",
                 "TERCERA",
                 "terceras",
                 "Terceras",
                 "TERCERAS"
             ],
-            "type": "modifiers",
+            "type": "MODIFIER",
             "value": "1/3"
         },
         "thirteen": {
             "terms": [
                 "trece",
                 "Trece",
                 "TRECE",
                 "treces",
                 "Treces",
                 "TRECES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 13.0
         },
         "thirty": {
             "terms": [
                 "treinta",
                 "Treinta",
                 "TREINTA",
                 "treintas",
                 "Treintas",
                 "TREINTAS"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 30.0
         },
         "thousand": {
             "terms": [
                 "mil",
                 "Mil",
                 "MIL",
                 "mils",
                 "Mils",
                 "MILS",
                 "miles",
                 "Miles",
                 "MILES"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000.0
         },
         "three": {
             "terms": [
                 "tres",
                 "Tres",
                 "TRES",
                 "treses",
                 "Treses",
                 "TRESES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 3.0
         },
+        "three_hundred": {
+            "terms": [
+                "tresciento",
+                "Tresciento",
+                "TRESCIENTO",
+                "trescientos",
+                "Trescientos",
+                "TRESCIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 300.0
+        },
         "trillion": {
             "terms": [
                 "billon",
                 "Billon",
                 "BILLON",
                 "billons",
                 "Billons",
                 "BILLONS",
                 "billones",
                 "Billones",
                 "BILLONES"
             ],
-            "type": "thousands",
+            "type": "THOUSAND",
             "value": 1000000000000.0
         },
         "twelve": {
             "terms": [
                 "doce",
                 "Doce",
                 "DOCE",
                 "doces",
                 "Doces",
                 "DOCES"
             ],
-            "type": "teens",
+            "type": "TEEN",
             "value": 12.0
         },
         "twenty": {
             "terms": [
                 "veinte",
                 "Veinte",
                 "VEINTE",
                 "veintes",
                 "Veintes",
                 "VEINTES"
             ],
-            "type": "tens",
+            "type": "TEN",
             "value": 20.0
         },
         "twenty-eight": {
             "terms": [
                 "veintiocho",
                 "Veintiocho",
                 "VEINTIOCHO",
                 "veintiochos",
                 "Veintiochos",
                 "VEINTIOCHOS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 28.0
         },
         "twenty-five": {
             "terms": [
                 "veinticinco",
                 "Veinticinco",
                 "VEINTICINCO",
                 "veinticincos",
                 "Veinticincos",
                 "VEINTICINCOS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 25.0
         },
         "twenty-four": {
             "terms": [
                 "veinticuatro",
                 "Veinticuatro",
                 "VEINTICUATRO",
                 "veinticuatros",
                 "Veinticuatros",
                 "VEINTICUATROS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 24.0
         },
         "twenty-nine": {
             "terms": [
                 "veintinueve",
                 "Veintinueve",
                 "VEINTINUEVE",
                 "veintinueves",
                 "Veintinueves",
                 "VEINTINUEVES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 29.0
         },
         "twenty-one": {
             "terms": [
                 "veintiuno",
                 "Veintiuno",
                 "VEINTIUNO",
@@ -610,87 +697,99 @@
                 "veintiuna",
                 "Veintiuna",
                 "VEINTIUNA",
                 "veintiunas",
                 "Veintiunas",
                 "VEINTIUNAS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 21.0
         },
         "twenty-seven": {
             "terms": [
                 "veintisiete",
                 "Veintisiete",
                 "VEINTISIETE",
                 "veintisietes",
                 "Veintisietes",
                 "VEINTISIETES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 27.0
         },
         "twenty-six": {
             "terms": [
                 "veintiseis",
                 "Veintiseis",
                 "VEINTISEIS",
                 "veintiseises",
                 "Veintiseises",
                 "VEINTISEISES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 26.0
         },
         "twenty-three": {
             "terms": [
                 "veintitres",
                 "Veintitres",
                 "VEINTITRES",
                 "veintitreses",
                 "Veintitreses",
                 "VEINTITRESES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 23.0
         },
         "twenty-two": {
             "terms": [
                 "veintidos",
                 "Veintidos",
                 "VEINTIDOS",
                 "veintidoses",
                 "Veintidoses",
                 "VEINTIDOSES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 22.0
         },
         "two": {
             "terms": [
                 "dos",
                 "Dos",
                 "DOS",
                 "doses",
                 "Doses",
                 "DOSES"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 2.0
         },
+        "two_hundred": {
+            "terms": [
+                "dosciento",
+                "Dosciento",
+                "DOSCIENTO",
+                "doscientos",
+                "Doscientos",
+                "DOSCIENTOS"
+            ],
+            "type": "HUNDRED",
+            "value": 200.0
+        },
         "zero": {
             "terms": [
                 "cero",
                 "Cero",
                 "CERO",
                 "ceros",
                 "Ceros",
                 "CEROS"
             ],
-            "type": "digits",
+            "type": "DIGIT",
             "value": 0.0
         }
     },
     "parser_file": "parser_one.py",
     "scales": {
         "century": {
             "plural": "siglos",
```

### Comparing `timelength-2.0.2/timelength/locales.py` & `timelength-2.0.3/timelength/locales.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 
         self._connectors = self._get_config_or_raise("connectors")
         self._segmentors = self._get_config_or_raise("segmentors")
         if set(self._connectors).intersection(self._segmentors):
             raise LocaleConfigError(
                 "Connectors and Segmentors may not have overlap in config."
             )
+        if not self._connectors or not self._segmentors:
+            raise LocaleConfigError(
+                "Connectors and Segmentors must have at least one value in config."
+            )
 
         # _allowed_terms may appear ONCE in a row in the input while strict is enabled.
         self._allowed_terms = self._get_config_or_raise("allowed_terms")
         self._decimal_separators = self._get_config_or_raise("decimal_separators")
         self._thousand_separators = self._get_config_or_raise("thousand_separators")
         if set(self._decimal_separators).intersection(self._thousand_separators):
             raise LocaleConfigError(
```

### Comparing `timelength-2.0.2/timelength/parsers/parser_one.py` & `timelength-2.0.3/timelength/parsers/parser_one.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fractions import Fraction
 
 from timelength.dataclasses import ParsedTimeLength, Scale
-from timelength.enums import BufferType, CharacterType
+from timelength.enums import BufferType, CharacterType, NumeralType
 from timelength.locales import Locale
 from timelength.utils import buffer_type, character_type, remove_diacritics
 
 
 def parser_one(
     content: str,
     strict: bool,
@@ -33,20 +33,27 @@
                     term
                     for numeral in numerals
                     if "terms" in numerals[numeral]
                     for term in numerals[numeral]["terms"]
                 ],
                 locale._connectors + locale._segmentors + locale._allowed_terms,
             )
+
+            numeral_type = None
+            if buffer_alphanum is BufferType.NUMERAL:
+                numeral_type = NumeralType(locale._get_numeral(buffer)["type"])
+
             buffer_values.append(
                 (
-                    float(buffer) if buffer_alphanum == BufferType.NUMBER else buffer,
+                    float(buffer) if buffer_alphanum is BufferType.NUMBER else buffer,
                     buffer_alphanum,
+                    numeral_type,
                 )
             )
+
             buffer = ""
 
     def check_next(
         next_index: int,
         target_chartype: CharacterType,
         decimal_only: bool = False,
     ):
@@ -170,15 +177,15 @@
     skip_buffer = 0
     for index, item in enumerate(buffer_values):
         if skip_buffer:
             skip_buffer -= 1
             continue
         if not item:
             continue
-        if item[1] == BufferType.UNKNOWN:
+        if item[1] is BufferType.UNKNOWN:
             result.invalid.append((item[0], "UNKNOWN_TERM"))
             if (
                 index + 1 < len(buffer_values)
                 and buffer_values[index + 1][0] in locale._connectors
             ):
                 skip_buffer += 1
         else:
@@ -193,67 +200,70 @@
     current_value_type_converted = None
     previous_value_type = None
     previous_value_type_converted = None
     current_numeral_type = None
     previous_numeral_type = None
     larger_numeral = False
     starts_with_modifier = False
+    skip_potential = 0
+    numeral_segment_tier = None
 
     def handle_multiplier(text: str, index: int):
         nonlocal parsed_value, segment_value
         previous_numeric = False
         next_numeric = False
         next_term = False
         previous_value = 0.0
         next_value = 0.0
         if (index - 2) >= 0:
             previous_type = potential_values[index - 2][1]
-            if previous_type == BufferType.NUMERAL:
+            if previous_type is BufferType.NUMERAL:
                 previous_numeric = True
                 previous_value = locale._get_numeral(potential_values[index - 2][0])[
                     "value"
                 ]
                 if isinstance(previous_value, str):
                     previous_value = float(Fraction(previous_value))
-            elif previous_type == BufferType.NUMBER:
+            elif previous_type is BufferType.NUMBER:
                 previous_numeric = True
                 previous_value = potential_values[index - 2][0]
         if (index + 2) < len(potential_values):
             next_type = potential_values[index + 2][1]
-            if next_type == BufferType.NUMERAL:
+            if next_type is BufferType.NUMERAL:
                 next_numeric = True
                 next_value = locale._get_numeral(potential_values[index + 2][0])[
                     "value"
                 ]
                 if isinstance(next_value, str):
                     next_value = float(Fraction(next_value))
-            elif next_type == BufferType.NUMBER:
+            elif next_type is BufferType.NUMBER:
                 next_numeric = True
                 next_value = potential_values[index + 2][0]
-            elif next_type == BufferType.SCALE:
+            elif next_type is BufferType.SCALE:
                 next_term = True
         if previous_numeric and next_numeric:
             potential_values[index + 2] = (
                 previous_value * next_value,
                 BufferType.NUMBER,
+                potential_values[index + 2][2],
             )
         else:
             if (not previous_numeric and not next_numeric) or not next_term:
                 result.invalid.append((text, "UNUSED_MULTIPLIER"))
 
     def handle_special(symbol: str):
         if symbol in previous_specials:
             result.invalid.append((symbol, "CONSECUTIVE_SPECIALS"))
         previous_specials.append(symbol)
 
     def handle_float(number: float):
         nonlocal parsed_value, segment_value
 
         if (
-            previous_value_type_converted == BufferType.NUMBER
+            previous_value_type_converted is BufferType.NUMBER
             and not starts_with_modifier
         ):
             if segment_value:
                 result.invalid.append((segment_value, "LONELY_VALUE"))
                 segment_value = None
             result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
         parsed_value = number
@@ -261,77 +271,167 @@
     def handle_numeral(text: str, index: int):
         nonlocal \
             parsed_value, \
             current_numeral_type, \
             current_value_type_converted, \
             starts_with_modifier, \
             segment_value, \
-            larger_numeral
+            larger_numeral, \
+            skip_potential, \
+            numeral_segment_tier
 
         numeral = locale._get_numeral(text)
         numeral_value = (
             float(Fraction(numeral["value"]))
             if isinstance(numeral["value"], str)
             else float(numeral["value"])
         )
-        current_numeral_type = numeral["type"]
         current_value_type_converted = BufferType.NUMBER
 
         if parsed_value is None:
             parsed_value = 0.0
             if (
-                current_numeral_type == "modifiers"
+                current_numeral_type is NumeralType.MODIFIER
                 and index + 2 < len(potential_values)
                 and potential_values[index + 2][1]
                 in [BufferType.NUMBER, BufferType.NUMERAL]
             ):
-                if potential_values[index + 2][1] == BufferType.NUMERAL:
-                    numeral = locale._get_numeral(potential_values[index + 2][0])
-                    if numeral["type"] == "multiplier":
+                if potential_values[index + 2][1] is BufferType.NUMERAL:
+                    next_numeral = locale._get_numeral(potential_values[index + 2][0])
+                    if NumeralType(next_numeral["type"]) is NumeralType.MULTIPLIER:
                         parsed_value = numeral_value
                     else:
                         potential_values[index + 2] = (
-                            numeral["value"] * numeral_value,
+                            next_numeral["value"] * numeral_value,
                             BufferType.NUMBER,
+                            potential_values[index + 2][2],
                         )
                 else:
                     potential_values[index + 2] = (
                         potential_values[index + 2][0] * numeral_value,
                         BufferType.NUMBER,
+                        potential_values[index + 2][2],
                     )
                 starts_with_modifier = True
             else:
                 parsed_value = numeral_value
-        elif current_numeral_type in ["modifiers", "thousands"]:
-            parsed_value *= numeral_value
-        elif current_numeral_type == "digits" and previous_numeral_type == "tens":
+        elif current_numeral_type == previous_numeral_type and segment_value:
+            segment_value += parsed_value
+            result.invalid.append((segment_value, "CONSECUTIVE_VALUES"))
+            segment_value = None
+            parsed_value = numeral_value
+        elif current_numeral_type in [
+            NumeralType.MODIFIER,
+            NumeralType.THOUSAND,
+            NumeralType.HUNDRED,
+        ]:
+            if current_numeral_type is NumeralType.THOUSAND:
+                next_non_special = None
+                trimmed_potential_values = potential_values[index + 1 :]
+                for item in trimmed_potential_values:
+                    if not next_non_special and item[1] is not BufferType.SPECIAL:
+                        next_non_special = item[2]
+                    if item[1] not in [BufferType.SPECIAL, BufferType.NUMERAL]:
+                        break
+                if next_non_special in [
+                    NumeralType.HUNDRED,
+                    NumeralType.DIGIT,
+                    NumeralType.TEEN,
+                    NumeralType.TEN,
+                ]:
+                    parsed_value *= numeral_value
+                    if segment_value:
+                        if (
+                            numeral_segment_tier
+                            and numeral_segment_tier > numeral_value
+                        ):
+                            segment_value += parsed_value
+                        else:
+                            result.invalid.append((segment_value, "LONELY_VALUE"))
+                            segment_value = parsed_value
+                    else:
+                        segment_value = parsed_value
+                    parsed_value = None
+                else:
+                    if (segment_value and not numeral_segment_tier) or (
+                        segment_value and numeral_segment_tier < numeral_value
+                    ):
+                        segment_value += parsed_value
+                        segment_value *= numeral_value
+                        parsed_value = None
+                    else:
+                        parsed_value *= numeral_value
+                numeral_segment_tier = numeral_value
+            elif current_numeral_type is NumeralType.HUNDRED:
+                if numeral_value == 100:
+                    parsed_value *= numeral_value
+                    if segment_value:
+                        if (
+                            numeral_segment_tier
+                            and numeral_segment_tier > numeral_value
+                        ):
+                            pass
+                        else:
+                            result.invalid.append((segment_value, "LONELY_VALUE"))
+                            segment_value = None
+                    else:
+                        next_non_special = None
+                        skip_potential = 0
+                        for item in potential_values[index + 1 :]:
+                            if item[1] is not BufferType.SPECIAL:
+                                next_non_special = item[2]
+                                break
+                            else:
+                                skip_potential += 1
+                        if next_non_special not in [
+                            NumeralType.DIGIT,
+                            NumeralType.TEEN,
+                            NumeralType.TEN,
+                        ]:
+                            skip_potential = 0
+                else:
+                    parsed_value += numeral_value
+            else:
+                parsed_value *= numeral_value
+        elif (
+            current_numeral_type is NumeralType.DIGIT
+            and previous_numeral_type is NumeralType.TEN
+        ):
             larger_numeral = True
             parsed_value = parsed_value + numeral_value
         elif (
-            current_numeral_type == "digits"
-            and previous_numeral_type == "digits"
+            current_numeral_type is NumeralType.DIGIT
+            and previous_numeral_type is NumeralType.DIGIT
             and not larger_numeral
         ):
             parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
-        elif current_numeral_type in ["teens", "tens"] and previous_numeral_type in [
-            "digits",
-            "teens",
-            "tens",
+        elif current_numeral_type in [
+            NumeralType.TEEN,
+            NumeralType.TEN,
+        ] and previous_numeral_type in [
+            NumeralType.DIGIT,
+            NumeralType.TEEN,
+            NumeralType.TEN,
         ]:
             parsed_value = float(f"{int(parsed_value)}{int(numeral_value)}")
-        elif (
-            current_numeral_type in ["tens", "teens", "digits"]
-            and previous_numeral_type == "thousands"
-        ):
+        elif current_numeral_type in [
+            NumeralType.TEN,
+            NumeralType.TEEN,
+            NumeralType.DIGIT,
+        ] and previous_numeral_type in [NumeralType.THOUSAND, NumeralType.HUNDRED]:
             parsed_value = parsed_value + numeral_value
             larger_numeral = True
         elif (
-            previous_value_type_converted == BufferType.NUMBER
-            or previous_numeral_type == "modifiers"
-        ) and current_numeral_type not in ["thousands", "modifiers"]:
+            previous_value_type_converted is BufferType.NUMBER
+            or previous_numeral_type is NumeralType.MODIFIER
+        ) and current_numeral_type not in [
+            NumeralType.THOUSAND,
+            NumeralType.HUNDRED,
+            NumeralType.MODIFIER,
+        ]:
             if segment_value:
                 result.invalid.append((segment_value, "LONELY_VALUE"))
                 segment_value = None
             result.invalid.append((parsed_value, "CONSECUTIVE_VALUES"))
             larger_numeral = False
             parsed_value = numeral_value
         else:
@@ -339,15 +439,15 @@
             parsed_value = numeral_value
 
     def handle_scale(text: str):
         nonlocal parsed_value, segment_value, result, parsed_scale, current_numeral_type
 
         if index == 0:
             result.invalid.append((text, "LEADING_SCALE"))
-        elif previous_value_type == BufferType.SCALE:
+        elif previous_value_type is BufferType.SCALE:
             result.invalid.append((text, "CONSECUTIVE_SCALES"))
         elif parsed_value is None and segment_value is None:
             result.invalid.append((text, "LONELY_SCALE"))
 
         if parsed_value is not None or segment_value is not None:
             scale: Scale
             scale = locale._get_scale(text)
@@ -355,38 +455,62 @@
                 if not parsed_value:
                     parsed_value = 0.0
                 if not segment_value:
                     segment_value = 0.0
                 result.seconds += (parsed_value + segment_value) * scale.scale
                 parsed_scale = scale
 
+    skip_numeral_check = 0
+    for index, element in enumerate(potential_values):
+        if skip_numeral_check > 0:
+            skip_numeral_check -= 1
+            continue
+        if element[1] is BufferType.NUMERAL:
+            idx = index + 1
+            while idx < len(potential_values) and potential_values[idx][1] in [
+                BufferType.SPECIAL,
+                BufferType.NUMERAL,
+            ]:
+                skip_numeral_check += 1
+                if potential_values[idx][0] in locale._segmentors:
+                    potential_values[idx] = (None, None, None)
+                    if potential_values[idx + 1][0] in locale._connectors:
+                        potential_values[idx + 1] = (None, None, None)
+                        skip_numeral_check += 1
+                idx += 1
+
+    potential_values = [item for item in potential_values if item[0] is not None]
+
     for index, element in enumerate(potential_values):
+        if skip_potential > 0:
+            skip_potential -= 1
+            continue
         current_value = element[0]
+        if current_value is None:
+            continue
         current_value_type = element[1]
         current_value_type_converted = current_value_type
+        current_numeral_type = element[2]
 
-        multiplier = False
-        if current_value_type == BufferType.NUMERAL:
-            multiplier = locale._get_numeral(current_value)
-            multiplier = True if multiplier["type"] == "multiplier" else False
-        if multiplier:
-            if parsed_value is not None:
-                handle_multiplier(current_value, index)
+        if current_value_type is BufferType.NUMERAL:
+            if current_numeral_type is NumeralType.MULTIPLIER:
+                if parsed_value is not None:
+                    handle_multiplier(current_value, index)
+                else:
+                    result.invalid.append((current_value, "UNUSED_MULTIPLIER"))
+                    segment_value = None
+                    parsed_value = None
+                    handle_special(current_value)
             else:
-                result.invalid.append((current_value, "UNUSED_MULTIPLIER"))
-                segment_value = None
-                parsed_value = None
-                handle_special(current_value)
-        elif current_value_type == BufferType.SPECIAL:
+                handle_numeral(current_value, index)
+        elif current_value_type is BufferType.SPECIAL:
             handle_special(current_value)
-        elif current_value_type == BufferType.NUMBER:
+        elif current_value_type is BufferType.NUMBER:
             handle_float(current_value)
-        elif current_value_type == BufferType.NUMERAL:
-            handle_numeral(current_value, index)
-        elif current_value_type == BufferType.SCALE:
+        elif current_value_type is BufferType.SCALE:
             handle_scale(current_value)
 
         if (
             current_value_type != BufferType.SPECIAL
             or current_value in locale._segmentors
         ):
             previous_value_type = current_value_type
@@ -423,15 +547,18 @@
 
     if (parsed_value is not None or segment_value is not None) and not parsed_scale:
         if not parsed_value:
             parsed_value = 0.0
         if not segment_value:
             segment_value = 0.0
         selected_value = parsed_value + segment_value
-        if not strict and len(potential_values) == 1:
+        if not strict and (
+            len(potential_values) == 1
+            or (len(result.valid) == 0 and len(result.invalid) == 0)
+        ):
             result.valid.append((parsed_value + segment_value, locale._second))
             result.seconds += parsed_value + segment_value
         else:
             result.invalid.append(
                 (
                     selected_value,
                     "LONELY_VALUE",
```

### Comparing `timelength-2.0.2/timelength/timelength.py` & `timelength-2.0.3/timelength/timelength.py`

 * *Files identical despite different names*

### Comparing `timelength-2.0.2/timelength/utils.py` & `timelength-2.0.3/timelength/utils.py`

 * *Files identical despite different names*

### Comparing `timelength-2.0.2/PKG-INFO` & `timelength-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelength
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python package to parse human readable lengths of time.
 Home-page: https://pypi.org/project/timelength/
 License: MIT
 Keywords: timelength,duration,python,parsing,time
 Author: Etorix
 Author-email: admin@etorix.dev
 Requires-Python: >=3.8,<4.0
```

