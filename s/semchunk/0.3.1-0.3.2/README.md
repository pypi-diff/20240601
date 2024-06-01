# Comparing `tmp/semchunk-0.3.1.tar.gz` & `tmp/semchunk-0.3.2.tar.gz`

## Comparing `semchunk-0.3.1.tar` & `semchunk-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 semchunk-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 semchunk-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 semchunk-0.3.1/htmlcov/.gitignore
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 semchunk-0.3.1/src/semchunk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.3.1/src/semchunk/py.typed
--rw-r--r--   0        0        0    14493 2020-02-02 00:00:00.000000 semchunk-0.3.1/src/semchunk/semchunk.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 semchunk-0.3.1/tests/bench.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 semchunk-0.3.1/tests/test_semchunk.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.3.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.3.1/LICENCE
--rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 semchunk-0.3.1/README.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 semchunk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 semchunk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 semchunk-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 semchunk-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 semchunk-0.3.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/py.typed
+-rw-r--r--   0        0        0    14510 2020-02-02 00:00:00.000000 semchunk-0.3.2/src/semchunk/semchunk.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 semchunk-0.3.2/tests/bench.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 semchunk-0.3.2/tests/test_semchunk.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.3.2/LICENCE
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 semchunk-0.3.2/README.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 semchunk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 semchunk-0.3.2/PKG-INFO
```

### Comparing `semchunk-0.3.1/CHANGELOG.md` & `semchunk-0.3.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ## Changelog 🔄
 All notable changes to `semchunk` will be documented here. This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.2] - 2024-06-01
+### Fixed
+- Fixed a bug where a `DivisionByZeroError` would be raised where a token counter returned zero tokens when called from `merge_splits()`, courtesy of [@jcobol](https://github.com/jcobol) ([#5](https://github.com/umarbutler/semchunk/pull/5)) ([7fd64eb](https://github.com/umarbutler/semchunk/pull/5/commits/7fd64eb8cf51f45702c59f43795be9a00c7d0d17)), fixing [#4](https://github.com/umarbutler/semchunk/issues/4).
+
 ## [0.3.1] - 2024-05-18
 ### Fixed
 - Fixed typo in error messages in `chunkerify()` where it was referred to as `make_chunker()`.
 
 ## [0.3.0] - 2024-05-18
 ### Added
 - Introduced the `chunkerify()` function, which constructs a chunker from a tokenizer or token counter that can be reused and can also chunk multiple texts in a single call. The resulting chunker speeds up chunking by 40.4% thanks, in large part, to a token counter that avoid having to count the number of tokens in a text when the number of characters in the text exceed a certain threshold, courtesy of [@R0bk](https://github.com/R0bk) ([#3](https://github.com/umarbutler/semchunk/pull/3)) ([337a186](https://github.com/umarbutler/semchunk/pull/3/commits/337a18615f991076b076262288b0408cb162b48c)).
@@ -48,14 +52,16 @@
 - Improved chunking performance.
 - improved test coverage.
 
 ## [0.1.0] - 2023-11-05
 ### Added
 - Added the `chunk()` function, which splits text into semantically meaningful chunks of a specified size as determined by a provided token counter.
 
+[0.3.2]: https://github.com/umarbutler/semchunk/compare/v0.3.1...v0.3.2
+[0.3.1]: https://github.com/umarbutler/semchunk/compare/v0.3.0...v0.3.1
 [0.3.0]: https://github.com/umarbutler/semchunk/compare/v0.2.4...v0.3.0
 [0.2.4]: https://github.com/umarbutler/semchunk/compare/v0.2.3...v0.2.4
 [0.2.3]: https://github.com/umarbutler/semchunk/compare/v0.2.2...v0.2.3
 [0.2.2]: https://github.com/umarbutler/semchunk/compare/v0.2.1...v0.2.2
 [0.2.1]: https://github.com/umarbutler/semchunk/compare/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/umarbutler/semchunk/compare/v0.1.2...v0.2.0
 [0.1.2]: https://github.com/umarbutler/semchunk/compare/v0.1.1...v0.1.2
```

### Comparing `semchunk-0.3.1/.github/workflows/ci.yml` & `semchunk-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.1/src/semchunk/semchunk.py` & `semchunk-0.3.2/src/semchunk/semchunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from contextlib import suppress
 
 if TYPE_CHECKING:
     import tiktoken
     import tokenizers
     import transformers
 
-_memoised_token_counters = {}
-"""A map of token counters to their memoised versions."""
+_memoized_token_counters = {}
+"""A map of token counters to their memoized versions."""
 
 _NON_WHITESPACE_SEMANTIC_SPLITTERS = (
     '.', '?', '!', '*', # Sentence terminators.
     ';', ',', '(', ')', '[', ']', "“", "”", '‘', '’', "'", '"', '`', # Clause separators.
     ':', '—', '…', # Sentence interrupters.
     '/', '\\', '–', '&', '-', # Word joiners.
 )
@@ -69,15 +69,15 @@
 
     while low < high:
         i = bisect_left(cumulative_lengths[low : high + 1], chunk_size * average)
         midpoint = min(i + low, high - 1)
 
         tokens = token_counter(splitter.join(splits[:midpoint]))
 
-        average = cumulative_lengths[midpoint] / tokens if cumulative_lengths[midpoint] else average
+        average = cumulative_lengths[midpoint] / tokens if cumulative_lengths[midpoint] and tokens > 0 else average
 
         if tokens > chunk_size:
             high = midpoint
         else:
             low = midpoint + 1
 
     return low - 1, splitter.join(splits[:low - 1])
@@ -85,22 +85,22 @@
 def chunk(text: str, chunk_size: int, token_counter: Callable[[str], int], memoize: bool = True, _recursion_depth: int = 0) -> list[str]:
     """Split a text into semantically meaningful chunks of a specified size as determined by the provided token counter.
 
     Args:
         text (str): The text to be chunked.
         chunk_size (int): The maximum number of tokens a chunk may contain.
         token_counter (Callable[[str], int]): A callable that takes a string and returns the number of tokens in it.
-        memoize (bool, optional): Whether to memoise the token counter. Defaults to `True`.
+        memoize (bool, optional): Whether to memoize the token counter. Defaults to `True`.
     
     Returns:
         list[str]: A list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed."""
     
-    # If this is not a recursive call and memoization is enabled, overwrite the `token_counter` with a memoised version of itself.
+    # If this is not a recursive call and memoization is enabled, overwrite the `token_counter` with a memoized version of itself.
     if not _recursion_depth and memoize:
-        token_counter = _memoised_token_counters.setdefault(token_counter, cache(token_counter))
+        token_counter = _memoized_token_counters.setdefault(token_counter, cache(token_counter))
 
     # Split the text using the most semantically meaningful splitter possible.
     splitter, splitter_is_whitespace, splits = _split_text(text)
     
     chunks = []
     skips = set()
     """A list of indices of splits to skip because they have already been added to a chunk."""
@@ -135,15 +135,15 @@
     
     # If this is not a recursive call, remove any empty chunks.
     if not _recursion_depth:
         chunks = list(filter(None, chunks))
     
     return chunks
 
-# Memoise the `chunk` function, preserving its signature and docstring.
+# Memoize the `chunk` function, preserving its signature and docstring.
 chunk = wraps(chunk)(cache(chunk))
 
 def chunkerify(
     tokenizer_or_token_counter: str | tiktoken.Encoding | transformers.PreTrainedTokenizer \
                                 | tokenizers.Tokenizer | Callable[[str], int],
     chunk_size: int = None,
     max_token_chars: int = None,
@@ -151,15 +151,15 @@
 ): # NOTE The output of `chunkerify()` is not type hinted because it causes `vscode` to overwrite the signature and docstring of the outputted chunker with the type hint.
     """Construct a chunker that splits one or more texts into semantically meaningful chunks of a specified size as determined by the provided tokenizer or token counter.
     
     Args:
         tokenizer_or_token_counter (str | tiktoken.Encoding | transformers.PreTrainedTokenizer | tokenizers.Tokenizer | Callable[[str], int]): Either: the name of a `tiktoken` or `transformers` tokenizer (with priority given to the former); a tokenizer that possesses an `encode` attribute (eg, a `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that returns the number of tokens in a input.
         chunk_size (int, optional): The maximum number of tokens a chunk may contain. Defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
         max_token_chars (int, optional): The maximum numbers of characters a token may contain. Used to significantly speed up the token counting of long inputs. Defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
-        memoize (bool, optional): Whether to memoise the token counter. Defaults to `True`.
+        memoize (bool, optional): Whether to memoize the token counter. Defaults to `True`.
     
     Returns:
         Callable[[str | Sequence[str]], list[str] | list[list[str]]]: A function that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts."""
     
     # If the provided tokenizer is a string, try to load it with either `tiktoken` or `transformers` or raise an error if neither is available.
     if isinstance(tokenizer_or_token_counter, str):
         try:
@@ -235,15 +235,15 @@
             
             return original_token_counter(text)
 
         token_counter = faster_token_counter
     
     # Memoize the token counter if necessary.
     if memoize:
-        token_counter = _memoised_token_counters.setdefault(token_counter, cache(token_counter))
+        token_counter = _memoized_token_counters.setdefault(token_counter, cache(token_counter))
     
     # Construct and return the chunker.
     def chunker(text_or_texts: str | Sequence[str]) -> list[str] | list[list[str]]:
         """Split text or texts into semantically meaningful chunks of a specified size as determined by the provided tokenizer or token counter.
         
         Args:
             text_or_texts (str | Sequence[str]): The text or texts to be chunked.
@@ -252,8 +252,8 @@
             list[str] | list[list[str]]: If a single text has been provided, a list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts."""
                 
         if isinstance(text_or_texts, str):
             return chunk(text_or_texts, chunk_size, token_counter, memoize = False)
         
         return [chunk(text, chunk_size, token_counter, memoize = False) for text in text_or_texts]
     
-    return chunker
+    return chunker
```

### Comparing `semchunk-0.3.1/tests/bench.py` & `semchunk-0.3.2/tests/bench.py`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.1/tests/test_semchunk.py` & `semchunk-0.3.2/tests/test_semchunk.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,20 +60,23 @@
     except ValueError:
         worked = True
     
     assert worked
         
     # Test using a `tiktoken` tokenizer by name.
     chunker = semchunk.chunkerify('gpt-4', 1)
+    chunker('ThisIs\tATest.')
     
     # Test using a `transformers` tokenizer by name.
     chunker = semchunk.chunkerify('umarbutler/emubert', 1)
+    chunker('ThisIs\tATest.')
     
     # Test using a `tiktoken` encoding by name.
     chunker = semchunk.chunkerify('cl100k_base', 1)
+    chunker('ThisIs\tATest.')
 
     # Test causing a `ValueError` by passing a tokenizer by name that should not exist.
     try:
         chunker = semchunk.chunkerify('\n\f\rع\n\f\r', 1)
         worked = False
     
     except ValueError:
```

### Comparing `semchunk-0.3.1/LICENCE` & `semchunk-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `semchunk-0.3.1/README.md` & `semchunk-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 `tokenizer_or_token_counter` is either: the name of a `tiktoken` or `transformers` tokenizer (with priority given to the former); a tokenizer that possesses an `encode` attribute (eg, a `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that returns the number of tokens in a input.
 
 `chunk_size` is the maximum number of tokens a chunk may contain. It defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
 
 `max_token_chars` is the maximum numbers of characters a token may contain. It is used to significantly speed up the token counting of long inputs. It defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
 
-`memoize` flags whether to memoise the token counter. It defaults to `True`.
+`memoize` flags whether to memoize the token counter. It defaults to `True`.
 
 This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
 
 ### Chunk
 ```python
 def chunk(
     text: str,
@@ -75,15 +75,15 @@
 
 `text` is the text to be chunked.
 
 `chunk_size` is the maximum number of tokens a chunk may contain.
 
 `token_counter` is a callable that takes a string and returns the number of tokens in it.
 
-`memoize` flags whether to memoise the token counter. It defaults to `True`.
+`memoize` flags whether to memoize the token counter. It defaults to `True`.
 
 This function returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed.
 
 ## How It Works 🔍
 `semchunk` works by recursively splitting texts until all resulting chunks are equal to or less than a specified chunk size. In particular, it:
 1. Splits text using the most semantically meaningful splitter possible;
 1. Recursively splits the resulting chunks until a set of chunks equal to or less than the specified chunk size is produced;
@@ -99,13 +99,13 @@
 1. Sentence interrupters (`:`, `—` and `…`);
 1. Word joiners (`/`, `\`, `–`, `&` and `-`); and
 1. All other characters.
 
 `semchunk` also relies on memoization to cache the results of token counters and the `chunk()` function, thereby improving performance.
 
 ## Benchmarks 📊
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same texts into 512-token-long chunks — a difference of 92.84%.
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same texts into 512-token-long chunks — a difference of 92.84%.
 
 The code used to benchmark `semchunk` and `semantic-text-splitter` is available [here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py).
 
 ## Licence 📄
 This library is licensed under the [MIT License](https://github.com/umarbutler/semchunk/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -48,27 +48,27 @@
 the number of tokens returned by attempting to tokenize an empty string) if
 possible otherwise a `ValueError` will be raised. `max_token_chars` is the
 maximum numbers of characters a token may contain. It is used to significantly
 speed up the token counting of long inputs. It defaults to `None` in which case
 it will either not be used or will, if possible, be set to the numbers of
 characters in the longest token in the tokenizer's vocabulary as determined by
 the `token_byte_values` or `get_vocab` methods. `memoize` flags whether to
-memoise the token counter. It defaults to `True`. This function returns a
+memoize the token counter. It defaults to `True`. This function returns a
 callable that takes either a single text or a sequence of texts and returns, if
 a single text has been provided, a list of chunks up to `chunk_size`-tokens-
 long with any whitespace used to split the text removed, or, if multiple texts
 have been provided, a list of lists of chunks, with each inner list
 corresponding to the chunks of one of the provided input texts. ### Chunk
 ```python def chunk( text: str, chunk_size: int, token_counter: Callable,
 memoize: bool = True, ) -> list[str] ``` `chunk()` splits a text into
 semantically meaningful chunks of a specified size as determined by the
 provided token counter. `text` is the text to be chunked. `chunk_size` is the
 maximum number of tokens a chunk may contain. `token_counter` is a callable
 that takes a string and returns the number of tokens in it. `memoize` flags
-whether to memoise the token counter. It defaults to `True`. This function
+whether to memoize the token counter. It defaults to `True`. This function
 returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace
 used to split the text removed. ## How It Works ð `semchunk` works by
 recursively splitting texts until all resulting chunks are equal to or less
 than a specified chunk size. In particular, it: 1. Splits text using the most
 semantically meaningful splitter possible; 1. Recursively splits the resulting
 chunks until a set of chunks equal to or less than the specified chunk size is
 produced; 1. Merges any chunks that are under the chunk size back together
@@ -82,15 +82,15 @@
 by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
 `*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
 `â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
 1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
 `semchunk` also relies on memoization to cache the results of token counters
 and the `chunk()` function, thereby improving performance. ## Benchmarks ð
 On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it
-takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg
+takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg
 Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
 token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
 (https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the
 same texts into 512-token-long chunks â a difference of 92.84%. The code used
 to benchmark `semchunk` and `semantic-text-splitter` is available [here](https:
 //github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð
```

### Comparing `semchunk-0.3.1/pyproject.toml` & `semchunk-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semchunk"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   {name="Umar Butler", email="umar@umar.au"},
 ]
 description = "A fast and lightweight pure Python library for splitting text into semantically meaningful chunks."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
```

### Comparing `semchunk-0.3.1/PKG-INFO` & `semchunk-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: semchunk
-Version: 0.3.1
+Version: 0.3.2
 Summary: A fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 Project-URL: Homepage, https://github.com/umarbutler/semchunk
 Project-URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues
 Project-URL: Source, https://github.com/umarbutler/semchunk
 Author-email: Umar Butler <umar@umar.au>
 License: MIT
@@ -86,15 +86,15 @@
 
 `tokenizer_or_token_counter` is either: the name of a `tiktoken` or `transformers` tokenizer (with priority given to the former); a tokenizer that possesses an `encode` attribute (eg, a `tiktoken`, `transformers` or `tokenizers` tokenizer); or a token counter that returns the number of tokens in a input.
 
 `chunk_size` is the maximum number of tokens a chunk may contain. It defaults to `None` in which case it will be set to the same value as the tokenizer's `model_max_length` attribute (deducted by the number of tokens returned by attempting to tokenize an empty string) if possible otherwise a `ValueError` will be raised.
 
 `max_token_chars` is the maximum numbers of characters a token may contain. It is used to significantly speed up the token counting of long inputs. It defaults to `None` in which case it will either not be used or will, if possible, be set to the numbers of characters in the longest token in the tokenizer's vocabulary as determined by the `token_byte_values` or `get_vocab` methods.
 
-`memoize` flags whether to memoise the token counter. It defaults to `True`.
+`memoize` flags whether to memoize the token counter. It defaults to `True`.
 
 This function returns a callable that takes either a single text or a sequence of texts and returns, if a single text has been provided, a list of chunks up to `chunk_size`-tokens-long with any whitespace used to split the text removed, or, if multiple texts have been provided, a list of lists of chunks, with each inner list corresponding to the chunks of one of the provided input texts.
 
 ### Chunk
 ```python
 def chunk(
     text: str,
@@ -108,15 +108,15 @@
 
 `text` is the text to be chunked.
 
 `chunk_size` is the maximum number of tokens a chunk may contain.
 
 `token_counter` is a callable that takes a string and returns the number of tokens in it.
 
-`memoize` flags whether to memoise the token counter. It defaults to `True`.
+`memoize` flags whether to memoize the token counter. It defaults to `True`.
 
 This function returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed.
 
 ## How It Works 🔍
 `semchunk` works by recursively splitting texts until all resulting chunks are equal to or less than a specified chunk size. In particular, it:
 1. Splits text using the most semantically meaningful splitter possible;
 1. Recursively splits the resulting chunks until a set of chunks equal to or less than the specified chunk size is produced;
@@ -132,13 +132,13 @@
 1. Sentence interrupters (`:`, `—` and `…`);
 1. Word joiners (`/`, `\`, `–`, `&` and `-`); and
 1. All other characters.
 
 `semchunk` also relies on memoization to cache the results of token counters and the `chunk()` function, thereby improving performance.
 
 ## Benchmarks 📊
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same texts into 512-token-long chunks — a difference of 92.84%.
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the same texts into 512-token-long chunks — a difference of 92.84%.
 
 The code used to benchmark `semchunk` and `semantic-text-splitter` is available [here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py).
 
 ## Licence 📄
 This library is licensed under the [MIT License](https://github.com/umarbutler/semchunk/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: semchunk Version: 0.3.1 Summary: A fast and
+Metadata-Version: 2.3 Name: semchunk Version: 0.3.2 Summary: A fast and
 lightweight pure Python library for splitting text into semantically meaningful
 chunks. Project-URL: Homepage, https://github.com/umarbutler/semchunk Project-
 URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues Project-URL:
 Source, https://github.com/umarbutler/semchunk Author-email: Umar Butler
 umar.au> License: MIT License-File: LICENCE Keywords:
 chunk,chunker,chunking,chunks,nlp,split,splits,splitter,splitting,text
@@ -70,27 +70,27 @@
 the number of tokens returned by attempting to tokenize an empty string) if
 possible otherwise a `ValueError` will be raised. `max_token_chars` is the
 maximum numbers of characters a token may contain. It is used to significantly
 speed up the token counting of long inputs. It defaults to `None` in which case
 it will either not be used or will, if possible, be set to the numbers of
 characters in the longest token in the tokenizer's vocabulary as determined by
 the `token_byte_values` or `get_vocab` methods. `memoize` flags whether to
-memoise the token counter. It defaults to `True`. This function returns a
+memoize the token counter. It defaults to `True`. This function returns a
 callable that takes either a single text or a sequence of texts and returns, if
 a single text has been provided, a list of chunks up to `chunk_size`-tokens-
 long with any whitespace used to split the text removed, or, if multiple texts
 have been provided, a list of lists of chunks, with each inner list
 corresponding to the chunks of one of the provided input texts. ### Chunk
 ```python def chunk( text: str, chunk_size: int, token_counter: Callable,
 memoize: bool = True, ) -> list[str] ``` `chunk()` splits a text into
 semantically meaningful chunks of a specified size as determined by the
 provided token counter. `text` is the text to be chunked. `chunk_size` is the
 maximum number of tokens a chunk may contain. `token_counter` is a callable
 that takes a string and returns the number of tokens in it. `memoize` flags
-whether to memoise the token counter. It defaults to `True`. This function
+whether to memoize the token counter. It defaults to `True`. This function
 returns a list of chunks up to `chunk_size`-tokens-long, with any whitespace
 used to split the text removed. ## How It Works ð `semchunk` works by
 recursively splitting texts until all resulting chunks are equal to or less
 than a specified chunk size. In particular, it: 1. Splits text using the most
 semantically meaningful splitter possible; 1. Recursively splits the resulting
 chunks until a set of chunks equal to or less than the specified chunk size is
 produced; 1. Merges any chunks that are under the chunk size back together
@@ -104,15 +104,15 @@
 by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
 `*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
 `â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
 1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
 `semchunk` also relies on memoization to cache the results of token counters
 and the `chunk()` function, thereby improving performance. ## Benchmarks ð
 On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.11.4, it
-takes `semchunk` 8.34s seconds to split every sample in [NLTK's Gutenberg
+takes `semchunk` 8.34 seconds to split every sample in [NLTK's Gutenberg
 Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
 token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
 (https://pypi.org/project/semantic-text-splitter/) 116.59 seconds to chunk the
 same texts into 512-token-long chunks â a difference of 92.84%. The code used
 to benchmark `semchunk` and `semantic-text-splitter` is available [here](https:
 //github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð
```

