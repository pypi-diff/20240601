# Comparing `tmp/bipsea-0.1.3.tar.gz` & `tmp/bipsea-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.1.3.tar", last modified: Sun May 26 22:46:37 2024, max compression
+gzip compressed data, was "bipsea-0.2.0.tar", last modified: Sat Jun  1 03:25:30 2024, max compression
```

## Comparing `bipsea-0.1.3.tar` & `bipsea-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 22:46:37.762846 bipsea-0.1.3/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.1.3/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 22:46:37.762642 bipsea-0.1.3/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)     9770 2024-05-26 22:37:27.000000 bipsea-0.1.3/README.md
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 22:46:37.762882 bipsea-0.1.3/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1185 2024-05-26 22:39:38.000000 bipsea-0.1.3/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 22:46:37.759620 bipsea-0.1.3/src/
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 22:46:37.761158 bipsea-0.1.3/src/bipsea/
--rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.1.3/src/bipsea/__init__.py
--rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 22:08:44.000000 bipsea-0.1.3/src/bipsea/bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.1.3/src/bipsea/bip32types.py
--rw-r--r--   0 akarve     (501) staff       (20)     5521 2024-05-26 22:08:44.000000 bipsea-0.1.3/src/bipsea/bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7659 2024-05-26 22:08:44.000000 bipsea-0.1.3/src/bipsea/bipsea.py
--rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.1.3/src/bipsea/english.txt
--rw-r--r--   0 akarve     (501) staff       (20)     3748 2024-05-26 22:39:38.000000 bipsea-0.1.3/src/bipsea/seedwords.py
--rw-r--r--   0 akarve     (501) staff       (20)      760 2024-05-26 22:46:26.000000 bipsea-0.1.3/src/bipsea/util.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 22:46:37.762446 bipsea-0.1.3/src/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      488 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       45 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        7 2024-05-26 22:46:37.000000 bipsea-0.1.3/src/bipsea.egg-info/top_level.txt
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 22:46:37.762259 bipsea-0.1.3/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 22:36:53.000000 bipsea-0.1.3/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     2237 2024-05-26 22:39:38.000000 bipsea-0.1.3/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     4530 2024-05-26 22:36:53.000000 bipsea-0.1.3/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     6535 2024-05-26 22:36:53.000000 bipsea-0.1.3/tests/test_cli.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.089135 bipsea-0.2.0/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.2.0/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 03:25:30.088907 bipsea-0.2.0/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)     9770 2024-05-26 22:37:27.000000 bipsea-0.2.0/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-01 03:25:30.089174 bipsea-0.2.0/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.2.0/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.085508 bipsea-0.2.0/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.087234 bipsea-0.2.0/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.2.0/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     4602 2024-06-01 01:30:56.000000 bipsea-0.2.0/src/bipsea/bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6794 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7854 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.2.0/src/bipsea/english.txt
+-rw-r--r--   0 akarve     (501) staff       (20)      760 2024-06-01 03:17:12.000000 bipsea-0.2.0/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.088702 bipsea-0.2.0/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      484 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-01 03:25:30.000000 bipsea-0.2.0/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-01 03:25:30.088456 bipsea-0.2.0/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 22:36:53.000000 bipsea-0.2.0/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3138 2024-06-01 01:30:56.000000 bipsea-0.2.0/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.2.0/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7088 2024-06-01 03:17:12.000000 bipsea-0.2.0/tests/test_cli.py
```

### Comparing `bipsea-0.1.3/LICENSE.md` & `bipsea-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/PKG-INFO` & `bipsea-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.md
 Requires-Dist: click
 Requires-Dist: base58
 Requires-Dist: ecdsa
 Requires-Dist: pytest
```

### Comparing `bipsea-0.1.3/README.md` & `bipsea-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/setup.py` & `bipsea-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="Bitcoin BIP85 BIP32 cryptography",
     install_requires=[
         "click",
         "base58",
         "ecdsa",
         "pytest",
```

### Comparing `bipsea-0.1.3/src/bipsea/bip32.py` & `bipsea-0.2.0/src/bipsea/bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/src/bipsea/bip32types.py` & `bipsea-0.2.0/src/bipsea/bip32types.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/src/bipsea/bipsea.py` & `bipsea-0.2.0/src/bipsea/bipsea.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,179 +1,166 @@
 """CLI"""
 
-import hashlib
 import logging
+import math
 import re
 import select
+import string
 import sys
 import threading
+from collections import Counter
 
 import click
 
 from .bip32 import to_master_key
 from .bip32types import parse_ext_key
-from .bip85 import DRNG, PURPOSE_CODES, apply_85, derive, to_entropy
-from .seedwords import (
-    N_WORDS_ALLOWED,
-    bip39_english_words,
-    entropy_to_words,
-    to_master_seed,
-    warn_stretching,
+from .bip39 import N_WORDS_ALLOWED, entropy_to_words, to_master_seed, verify_seed_words
+from .bip85 import (
+    APPLICATIONS,
+    DRNG,
+    PURPOSE_CODES,
+    RANGES,
+    apply_85,
+    derive,
+    to_entropy,
 )
 from .util import LOGGER, __app_name__, __version__, to_hex_string
 
+MIN_ENTROPY = 256
 SEED_FROM_VALUES = [
-    "string",
     "rand",
     "words",
 ]
 SEED_TO_VALUES = [
     "words",
     "tprv",
     "xprv",
 ]
-TIMEOUT = 1
-
-APPLICATIONS = {
-    "base64": "707764'",
-    "base85": "707785'",
-    "drng": None,
-    "hex": "128169'",
-    "words": "39'",
-    "wif": "2'",
-    "xprv": "32'",
-}
-
-RANGES = {
-    "base64": (20, 86),
-    "base85": (10, 80),
-    "hex": (16, 64),
-}
+TIMEOUT = 0.1
 
 N_WORDS_ALLOWED_STR = [str(n) for n in N_WORDS_ALLOWED]
 N_WORDS_ALLOWED_HELP = "|".join(N_WORDS_ALLOWED_STR)
 
 
 logger = logging.getLogger(LOGGER)
-
-
-class InputThread(threading.Thread):
-    def run(self):
-        self.seed = click.get_text_stream("stdin").read().strip()
+logger.setLevel(logging.DEBUG)
 
 
 @click.group()
 @click.version_option(version=__version__, prog_name=__app_name__)
 def cli():
     pass
 
 
-@click.command(help="Generate a master private seed")
+@click.command(
+    name="seed", help="Generate an extended master private key (BIP-32, BIP-39)"
+)
 @click.option(
     "-f",
     "--from",
     "from_",
     type=click.Choice(SEED_FROM_VALUES, case_sensitive=True),
     required=True,
     help="|".join(SEED_FROM_VALUES),
     default="rand",
 )
-@click.option("-i", "--input", help="string in the format specified by --from")
+@click.option("-i", "--input", help="String in the format specified by --from")
 @click.option(
     "-t",
     "--to",
     type=click.Choice(SEED_TO_VALUES, case_sensitive=True),
-    default="words",
+    default="xprv",
     help="|".join(SEED_TO_VALUES),
     required=True,
 )
 @click.option(
     "-n",
     "--number",
+    default="24",
     type=click.Choice(N_WORDS_ALLOWED_STR),
 )
 @click.option("-p", "--passphrase", default="")
 @click.option(
-    "--pretty", is_flag=True, default=False, help="number and separate seed words"
+    "--pretty", is_flag=True, default=False, help="Number and separate seed words"
+)
+@click.option(
+    "--strict",
+    is_flag=True,
+    default=False,
+    help="Allow only checksummed BIP-39 English words",
 )
-def seed(from_, input, to, number, passphrase, pretty):
+def bip39_cmd(from_, input, to, number, passphrase, pretty, strict):
     if input:
         input = input.strip()
+    number = int(number)
     if (from_ == "rand" and input) or (from_ != "rand" and not input):
         raise click.BadOptionUsage(
             option_name="--from",
-            message="--input is required (unless --from rand)",
+            message="`--from words` requires `--input STRING`, `--from rand` forbids `--input`",
         )
     if from_ == "words":
-        if number:
-            raise click.BadOptionUsage(
-                option_name="--number",
-                message="omit when you specify --from words",
-            )
-        if to == "words":
-            raise click.BadOptionUsage(
-                option_name="--to", message="--from words is redundant"
-            )
         words = re.split(r"\s+", input)
         n_words = len(words)
-        if not n_words in N_WORDS_ALLOWED:
+        if strict:
+            if not verify_seed_words("english", words):
+                raise click.BadOptionUsage(
+                    option_name="--input",
+                    message=f"Non BIP-39 words from `--input` ({' '.join(words)}) or bad BIP-39 checksum",
+                )
+        else:
+            implied = implied_entropy(input)
+            if implied < MIN_ENTROPY:
+                click.secho(
+                    (
+                        f"Warning: {implied} bits of implied entropy is less than the"
+                        f"recommended {MIN_ENTROPY} bits."
+                    )
+                )
+        entropy = to_master_seed(words, passphrase)
+    else:  # from_ == "rand"
+        entropy = None
+        if strict:
             raise click.BadOptionUsage(
-                option_name="--number",
-                message=f"must be in {N_WORDS_ALLOWED_HELP}",
+                option_name="--strict",
+                message="`--strict` requires `--from words`",
             )
-    else:
-        if not number:
-            number = 24  # set here so we don't falsely trip `if number` above
-        else:
-            number = int(number)
-        if from_ == "string":
-            string_bytes = input.encode("utf-8")
-            # this is how entropy works out in BIP-39
-            target_bits = 128 + ((number - 12) // 3) * 32
-            short = len(string_bytes) * 8 - target_bits
-            if short < 0:
-                warn_stretching(short + target_bits, target_bits, True)
-            entropy = hashlib.sha256(string_bytes).digest()
-        elif from_ == "rand":
-            entropy = None
-        words = entropy_to_words(
-            n_words=int(number), user_entropy=entropy, passphrase=passphrase
-        )
+        words = entropy_to_words(n_words=number, user_entropy=entropy)
     if to == "words":
-        english_words = set(bip39_english_words())
-        if not all(w in english_words for w in words):
+        if from_ == "words":
             raise click.BadOptionUsage(
-                option_name="--input",
-                message=f"One or more words not in BIP-39 English list: {words}",
+                option_name="--to",
+                message="`--to words` incompatible with `--from words`",
             )
         output = " ".join(words)
         if pretty:
             output = "\n".join(f"{i+1}) {w}" for i, w in enumerate(words))
 
         click.echo(output)
 
     elif to in ("tprv", "xprv"):
         if pretty:
             raise click.BadOptionUsage(
-                option_name="--pretty", message="no effect with --to xprv"
+                option_name="pretty",
+                message="`--pretty` has no effect with `--to xprv`",
             )
         mainnet = to == "xprv"
         seed = to_master_seed(words, passphrase)
         kprv = to_master_key(seed, mainnet=mainnet, private=True)
 
         click.echo(kprv)
 
 
-cli.add_command(seed)
+cli.add_command(bip39_cmd)
 
 
-@click.command(name="entropy", help="Derive entropy according to BIP-85")
+@click.command(name="entropy", help="Derive secrets according to BIP-85")
 @click.option(
     "-a",
     "--application",
+    default="words",
     required=True,
     help="|".join(APPLICATIONS.keys()),
     type=click.Choice(APPLICATIONS.keys(), case_sensitive=True),
 )
 @click.option(
     "-n",
     "--number",
@@ -183,68 +170,89 @@
 @click.option(
     "-i",
     "--index",
     type=click.IntRange(0, 2**31 - 1),
     default=0,
     help="child index",
 )
-@click.option("-p", "--input", help="Use instead of pipe --input xprv12345")
-def bip85(application, number, index, input):
+@click.option(
+    "-s",
+    "--special",
+    default=10,
+    type=int,
+    help="Additional integer (e.g. for 'dice' sides)",
+)
+@click.option(
+    "-p",
+    "--input",
+    help="`--input xprv123...` can be used instead of an input pipe `bipsea seed | bipsea entropy`",
+)
+def bip85_cmd(application, number, index, special, input):
     if not input:
-        stdin, o, stderr = select.select([sys.stdin], [], [sys.stderr], TIMEOUT)
+        stdin, _, _ = select.select([sys.stdin], [], [], TIMEOUT)
         if stdin:
             prv = sys.stdin.readline().strip()
         else:
             no_prv()
     else:
         prv = input
     if number is not None:
+        number = int(number)
         if application in ("wif", "xprv"):
             raise click.BadOptionUsage(
                 option_name="--number",
-                message="--number has no effect when --application wif|xprv",
+                message="`--number` has no effect when `--application wif|xprv`",
             )
         elif number < 1:
             raise click.BadOptionUsage(
                 option_name="--number",
                 message="must be a positive integer",
             )
     else:
         number = 24
     if not prv[:4] in ("tprv", "xprv"):
         no_prv()
     master = parse_ext_key(prv)
 
     path = f"m/{PURPOSE_CODES['BIP-85']}"
-    app_value = APPLICATIONS[application]
-    path += f"/{app_value}" if app_value else ""
+    app_code = APPLICATIONS[application]
+    path += f"/{app_code}"
     if application == "words":
         if number not in N_WORDS_ALLOWED:
             raise click.BadOptionUsage(
                 option_name="--number",
-                message=f"--application wif requires --number in {N_WORDS_ALLOWED_HELP}",
+                message=f"`--application wif` requires `--number NUMBER` in {N_WORDS_ALLOWED_HELP}",
             )
         path += f"/0'/{number}'/{index}'"
     elif application in ("wif", "xprv"):
         path += f"/{index}'"
-    elif application in ("hex", "base64", "base85"):
-        path += f"/{number}'/{index}'"
+    elif application in ("base64", "base85", "hex"):
         check_range(number, application)
+        path += f"/{number}'/{index}'"
     elif application == "drng":
         path += f"/0'/{index}'"
+    elif application == "dice":
+        check_range(number, application)
+        path += f"/{special}'/{number}'/{index}'"
+    else:
+        raise click.BadOptionUsage(
+            option_name="--application",
+            message=f"unrecognized {application}",
+        )
+
     derived = derive(master, path)
     if application == "drng":
         drng = DRNG(to_entropy(derived.data[1:]))
         output = to_hex_string(drng.read(number))
     else:
         output = apply_85(derived, path)["application"]
     click.echo(output)
 
 
-cli.add_command(bip85)
+cli.add_command(bip85_cmd)
 
 
 # TODO From BIP32: In case parse256(IL) is 0 or ≥ n, the resulting key is invalid,
 # and one should proceed with the next value for i. (Note: this has probability lower than 1 in 2127.)
 # they say hard fail but does 39? i say let's hard fail in these cases because otherwise
 # you are modifying the path?
 
@@ -257,14 +265,17 @@
             message=f"out of range; try [{min}, {max}] for {application}",
         )
 
 
 def no_prv():
     raise click.BadOptionUsage(
         option_name="[incoming pipe]",
-        message="Bad input. Need xprv or tprv. Try `bipsea seed -t xprv | bipsea entropy -a base64`",
+        message="Bad input. Need xprv or tprv. Try `bipsea seed` | bipsea entropy`",
     )
-    click.echo()
+
+
+def implied_entropy(s):
+    return math.floor(math.log(len(s) ** len(string.printable), 2))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `bipsea-0.1.3/src/bipsea/english.txt` & `bipsea-0.2.0/src/bipsea/english.txt`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/src/bipsea/util.py` & `bipsea-0.2.0/src/bipsea/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """constants and utilities"""
 
 import binascii
 import logging
 from hashlib import pbkdf2_hmac
 from unicodedata import normalize as unicode_normalize
 
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 __app_name__ = "bipsea"
 
 FORMAT = "utf-8"
 NFKD = "NFKD"
 LOGGER = __app_name__
```

### Comparing `bipsea-0.1.3/src/bipsea.egg-info/PKG-INFO` & `bipsea-0.2.0/src/bipsea.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.md
 Requires-Dist: click
 Requires-Dist: base58
 Requires-Dist: ecdsa
 Requires-Dist: pytest
```

### Comparing `bipsea-0.1.3/tests/test_bip32.py` & `bipsea-0.2.0/tests/test_bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.3/tests/test_bip85.py` & `bipsea-0.2.0/tests/test_bip85.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from hashlib import sha256
 
 import base58
 import pytest
 from data.bip85_vectors import (
     BIP39,
+    DICE,
     EXT_KEY_TO_ENTROPY,
     HEX,
     PWD_BASE64,
     PWD_BASE85,
     WIF,
     XPRV,
 )
@@ -88,15 +89,15 @@
 
 @pytest.mark.parametrize("vector", XPRV)
 def test_rsa_unsupported(vector):
     """currently no support for RSA application.
     path format: m/83696968'/828365'/{key_bits}'/{key_index}'"""
     rsa_path = "m/83696968'/828365'/1024'/0'"
     master = parse_ext_key(vector["master"])
-    with pytest.raises(NotImplementedError):
+    with pytest.raises(ValueError):
         apply_85(derive(master, rsa_path), rsa_path)
 
 
 @pytest.mark.parametrize("vector", WIF)
 def test_wif(vector):
     master = parse_ext_key(vector["master"])
     path = vector["path"]
@@ -125,7 +126,20 @@
     hash1 = sha256(extended).digest()
     hash2 = sha256(hash1).digest()
     checksum = hash2[:4]
     # they say "Base58Check encoding" but that doesn't mean
     # b58encode_check because we already have a checksum apparently
     wif = base58.b58encode(extended + checksum)
     assert wif.decode("utf-8") == "5HueCGU8rMjxEXxiPuD5BDku4MkFqeZyd4dZ1jvhTVqvbTLvyTJ"
+
+
+@pytest.mark.parametrize("vector", DICE)
+def test_rsa_unsupported(vector):
+    master = parse_ext_key(vector["master"])
+    path = vector["path"]
+    output = apply_85(derive(master, path), path)
+    rolls = output["application"]
+    assert rolls == vector["derived_rolls"]
+    rolls_int = [int(r) for r in rolls.split(",")]
+    assert len(rolls_int) == 10
+    assert all(0 <= r < 10 for r in rolls_int)
+    assert to_hex_string(output["entropy"]) == vector["derived_entropy"]
```

### Comparing `bipsea-0.1.3/tests/test_cli.py` & `bipsea-0.2.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import random
+import string
 
 import pytest
 from click.testing import CliRunner
 from data.bip39_vectors import VECTORS
 from data.bip85_vectors import BIP39, HEX, PWD_BASE64, PWD_BASE85, WIF
 
 from bipsea.bipsea import N_WORDS_ALLOWED, cli
@@ -75,30 +77,42 @@
         assert testnet.exit_code == 0
         tprv = testnet.output.strip()
         assert tprv != xprv
         assert tprv.startswith("tprv")
 
 
 @pytest.mark.parametrize("n", N_WORDS_ALLOWED)
-def test_seed_command_n_words(runner, n):
-    for from_ in ("string", "rand"):
-        cmd = ["seed", "-t", "words", "-n", str(n)]
-        cmd += ["-f", from_]
-        if from_ == "string":
-            # "s"*15 is shorter than the lowest entropy of 128 bits
-            # "l"*32 is longer than the highest entropy of 256 bits
-            for input in ("s" * 15, "l" * 32):
-                cmd += ["-i", input]
-                result = runner.invoke(cli, cmd, catch_exceptions=False)
-                if "s" in input:
-                    assert "Warning" in result.output
-                else:
-                    assert "Warning" not in result.output
-                    assert len(result.output.split()) == int(n)
-                assert result.exit_code == 0
+def test_seed_command_from_rand(runner, n):
+    cmd = ["seed", "-t", "words", "-n", str(n), "-f", "rand"]
+    result = runner.invoke(cli, cmd)
+    assert len(result.output.split()) == int(n)
+    assert result.exit_code == 0
+
+
+def test_seed_command_from_words(runner):
+    lengths = {"short": 5, "enough": 6}
+    base = ["seed", "-t", "xprv", "-n", str(21), "-f", "words"]
+    for k, v in lengths.items():
+        cmd = base + ["-i", gen_custom_seed_words(v, 0)]
+        result = runner.invoke(cli, cmd)
+        assert result.exit_code == 0
+        if k == "short":
+            assert "Warning" in result.output
+        else:
+            assert "Warning" not in result.output
+        cmd += ["--strict"]
+        bad_result = runner.invoke(cli, cmd)
+        assert bad_result.exit_code != 0
+        assert "BIP-39" in bad_result.output
+
+
+def gen_custom_seed_words(length: int, seed: int):
+    """non bip-39 seeds"""
+    random.seed(seed)
+    return "".join(random.choice(string.printable) for _ in range(length))
 
 
 def test_seed_from_and_to_words(runner):
     result = runner.invoke(cli, ["seed", "--from", "words", "--to", "words"])
     assert result.exit_code != 0
     assert "--input" in result.output
     assert "--from rand" in result.output
@@ -118,28 +132,41 @@
 
 def test_seed_bad_to(runner):
     result = runner.invoke(cli, ["seed", "--to", "blah"])
     assert result.exit_code != 0
     assert "not one of" in result.output
 
 
-@pytest.mark.parametrize("vector", PWD_BASE64)
-def test_bipsea_integration(runner, vector):
+def test_bipsea_integration(runner):
     result_seed = runner.invoke(
         cli,
-        ["seed", "-f", "string", "-i", "yooooooooooooooo", "-n", "12", "-t", "xprv"],
+        [
+            "seed",
+            "-f",
+            "words",
+            "-i",
+            "punch man spread gap size struggle clean crouch cloth swear erode fan",
+            "-n",
+            "12",
+            "-t",
+            "xprv",
+        ],
     )
     xprv = result_seed.output.strip()
+    assert (
+        xprv
+        == "xprv9s21ZrQH143K417dJYmPr6Qmy2t61xrKtDCCL3Cec4NMFFFRZTF2jSbtqSXpuCz8UqgsuyrPC5wngx3dk5Gt8zQnbnHVAsMyb7bWtHZ95Jk"
+    )
     assert result_seed.exit_code == 0
     result_entropy = runner.invoke(
         cli, ["entropy", "-a", "base64", "-n", "20", "--input", xprv]
     )
     assert result_entropy.exit_code == 0
     pwd64 = result_entropy.output.strip()
-    assert pwd64 == "lGqIFs50nYCWA0DjxHRB"
+    assert pwd64 == "72zJIS7JhyR5r5NjkuE/"
     assert len(pwd64) == 20
 
 
 @pytest.mark.parametrize("vector", PWD_BASE85)
 def test_entropy_n(runner, vector):
     xprv = vector["master"]
     for app in ("base64", "base85", "hex", "drng"):
```

