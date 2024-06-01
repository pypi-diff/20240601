# Comparing `tmp/distyll_info-0.2.4.tar.gz` & `tmp/distyll_info-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distyll_info-0.2.4.tar", max compression
+gzip compressed data, was "distyll_info-0.3.0.tar", max compression
```

## Comparing `distyll_info-0.2.4.tar` & `distyll_info-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-03-05 21:09:40.618601 distyll_info-0.2.4/README.md
--rw-r--r--   0        0        0      588 2024-05-18 12:00:57.234361 distyll_info-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      109 2024-05-18 11:51:33.424409 distyll_info-0.2.4/src/distyll/__init__.py
--rw-r--r--   0        0        0      141 2024-05-18 11:47:11.878086 distyll_info-0.2.4/src/distyll/config.py
--rw-r--r--   0        0        0     5237 2024-05-18 12:00:46.189295 distyll_info-0.2.4/src/distyll/db.py
--rw-r--r--   0        0        0      186 2024-03-05 19:57:41.677116 distyll_info-0.2.4/src/distyll/loggerconfig.py
--rw-r--r--   0        0        0       89 2024-03-05 21:28:53.227286 distyll_info-0.2.4/src/distyll/text/__init__.py
--rw-r--r--   0        0        0     2938 2024-03-05 20:52:11.237125 distyll_info-0.2.4/src/distyll/text/text.py
--rw-r--r--   0        0        0      104 2024-03-05 21:28:53.229015 distyll_info-0.2.4/src/distyll/transcripts/__init__.py
--rw-r--r--   0        0        0     2617 2024-03-05 20:53:15.041741 distyll_info-0.2.4/src/distyll/transcripts/transcripts.py
--rw-r--r--   0        0        0    11674 2024-03-05 21:28:53.292900 distyll_info-0.2.4/src/distyll/utils.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 distyll_info-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-31 23:24:35.426663 distyll_info-0.3.0/README.md
+-rw-r--r--   0        0        0      607 2024-06-01 00:51:26.883818 distyll_info-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-06-01 00:07:11.558957 distyll_info-0.3.0/src/distyll/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-31 23:24:35.427286 distyll_info-0.3.0/src/distyll/config.py
+-rw-r--r--   0        0        0     2143 2024-05-31 23:24:35.427426 distyll_info-0.3.0/src/distyll/db.py
+-rw-r--r--   0        0        0       90 2024-06-01 00:10:44.875692 distyll_info-0.3.0/src/distyll/llm/__init__.py
+-rw-r--r--   0        0        0     1950 2024-06-01 00:39:59.270298 distyll_info-0.3.0/src/distyll/llm/utils.py
+-rw-r--r--   0        0        0      186 2024-03-03 21:51:47.002643 distyll_info-0.3.0/src/distyll/loggerconfig.py
+-rw-r--r--   0        0        0       89 2024-05-31 23:24:35.427572 distyll_info-0.3.0/src/distyll/text/__init__.py
+-rw-r--r--   0        0        0     2938 2024-05-31 23:24:35.427679 distyll_info-0.3.0/src/distyll/text/text.py
+-rw-r--r--   0        0        0      104 2024-05-31 23:24:35.427815 distyll_info-0.3.0/src/distyll/transcripts/__init__.py
+-rw-r--r--   0        0        0     2617 2024-05-31 23:24:35.427932 distyll_info-0.3.0/src/distyll/transcripts/transcripts.py
+-rw-r--r--   0        0        0    12867 2024-06-01 00:42:05.256965 distyll_info-0.3.0/src/distyll/utils.py
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 distyll_info-0.3.0/PKG-INFO
```

### Comparing `distyll_info-0.2.4/README.md` & `distyll_info-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.4/pyproject.toml` & `distyll_info-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "distyll-info"
-version = "0.2.4"
+version = "0.3.0"
 description = "Information parsing assistant"
 authors = ["JP Hwang <61258750+databyjp@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "distyll", from="src"}]
 
 [tool.poetry.dependencies]
@@ -12,14 +12,15 @@
 pypdf = "^4.1.0"
 openai = "^1.13.3"
 pydub = "^0.25.1"
 yt-dlp = "^2023.12.30"
 moviepy = "^1.0.3"
 beautifulsoup4 = "^4.12.3"
 weaviate-client = "^4.5.0"
+jupyter = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `distyll_info-0.2.4/src/distyll/text/text.py` & `distyll_info-0.3.0/src/distyll/text/text.py`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.4/src/distyll/transcripts/transcripts.py` & `distyll_info-0.3.0/src/distyll/transcripts/transcripts.py`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.4/src/distyll/utils.py` & `distyll_info-0.3.0/src/distyll/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bs4 import BeautifulSoup
 from typing import Union, List, Dict, Any, Literal
 import requests
 import logging
-from typing import Union
 from pathlib import Path
 from openai import OpenAI
 import yt_dlp
 import os
 
 
 OPENAI_APIKEY = None
@@ -84,21 +83,22 @@
         return title_element["content"]
     else:
         logging.info("Failed to find the title element")
         return None
 
 
 def chunk_text_by_num_words(
-    source_text: str, max_chunk_words: int = 100, overlap_fraction: float = 0.25
+    source_text: str, max_chunk_words: int = 100, overlap_fraction: float = 0.25, prevent_short_last_chunks: bool = True
 ) -> List[str]:
     """
     Chunk text input into a list of strings, using a number of words
     :param source_text: Input string to be chunked
     :param max_chunk_words: Maximum length of chunk, in words
     :param overlap_fraction: Overlap as a percentage of chunk_words. The overlap is prepended to each chunk.
+    :param prevent_short_last_chunks: Prevent very short last chunks
     :return: return a list of words
     """
     logging.info(f"Chunking text of {len(source_text)} chars by number of words.")
     sep = " "
     overlap_words = int(max_chunk_words * overlap_fraction)
 
     source_text = source_text.strip()
@@ -106,15 +106,33 @@
     chunks_list = list()
 
     n_chunks = ((len(word_list) - 1 + overlap_words) // max_chunk_words) + 1
     for i in range(n_chunks):
         window_words = word_list[
             max(max_chunk_words * i - overlap_words, 0) : max_chunk_words * (i + 1)
         ]
-        chunks_list.append(sep.join(window_words))
+        if prevent_short_last_chunks:
+            # Conditional logic to handle the last two chunks and prevent very short chunks
+            if i < n_chunks - 2:
+                chunks_list.append(sep.join(window_words))
+            else:  # Second to last chunk onwards
+                remaining_words = word_list[max(max_chunk_words * i - overlap_words, 0) :]
+                if len(remaining_words) <= max_chunk_words:
+                    chunks_list.append(sep.join(remaining_words))
+                    break
+                second_last_chunk = remaining_words[
+                    : len(remaining_words) // 2 + overlap_words
+                ]
+                last_chunk = remaining_words[len(remaining_words) // 2 :]
+                chunks_list.append(sep.join(second_last_chunk))
+                chunks_list.append(sep.join(last_chunk))
+                break
+        else:
+            chunks_list.append(sep.join(window_words))
+
     return chunks_list
 
 
 def chunk_text_by_num_chars(
     source_text: str, max_chunk_chars: int = 300, overlap_fraction: float = 0.25
 ) -> List[str]:
     """
@@ -150,43 +168,49 @@
     return source_text
 
 
 def chunk_text(
     source_text: str,
     method: Literal["words", "chars"] = "words",
     token_length: Union[None, int] = 100,
+    overlap_fraction: float = 0.25,
 ) -> List[str]:
     """
     Chunk longer text
     :param source_text: Input text
     :param method: "words" or "chars"
     :param token_length: Number of tokens to chunk by
+    :param overlap_fraction: Overlap as a percentage of chunk
     :return:
     """
     logging.info(
         f"Chunking text of {len(source_text)} characters with {method} method."
     )
     source_text = remove_multiple_whitespaces(source_text)
     if method == "words":
-        return chunk_text_by_num_words(source_text, max_chunk_words=token_length)
+        return chunk_text_by_num_words(
+            source_text, max_chunk_words=token_length, overlap_fraction=overlap_fraction
+        )
     elif method == "chars":
-        return chunk_text_by_num_chars(source_text, max_chunk_chars=token_length)
+        return chunk_text_by_num_chars(
+            source_text, max_chunk_chars=token_length, overlap_fraction=overlap_fraction
+        )
     else:
         raise ValueError(f"Unsupported method: {method}")
 
 
 def extract_metadata(video_info: Dict[str, Any]) -> Dict[str, Any]:
     metadata = dict()
     for k in ["title", "upload_date", "channel", "uploader"]:
         if k in video_info:
             metadata[k] = video_info[k]
     return metadata
 
 
-def download_youtube(youtube_url: str, path_out: Path) -> str:
+def download_youtube(youtube_url: str, path_out: Path) -> Dict[str, Any]:
     """
     Download a YouTube video's audio and return its title
     :param youtube_url: URL of the YouTube video
     :param path_out: Path where the audio file will be saved
     :return: Video title
     """
     path_template = str(path_out.absolute())
```

### Comparing `distyll_info-0.2.4/PKG-INFO` & `distyll_info-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: distyll-info
-Version: 0.2.4
+Version: 0.3.0
 Summary: Information parsing assistant
 License: MIT
 Author: JP Hwang
 Author-email: 61258750+databyjp@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: weaviate-client (>=4.5.0,<5.0.0)
 Requires-Dist: yt-dlp (>=2023.12.30,<2024.0.0)
 Description-Content-Type: text/markdown
```

