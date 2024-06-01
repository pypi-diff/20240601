# Comparing `tmp/telegramify_markdown-0.1.4.tar.gz` & `tmp/telegramify_markdown-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramify_markdown-0.1.4.tar", last modified: Sat May 25 12:04:10 2024, max compression
+gzip compressed data, was "telegramify_markdown-0.1.5.tar", last modified: Sat Jun  1 12:44:10 2024, max compression
```

## Comparing `telegramify_markdown-0.1.4.tar` & `telegramify_markdown-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/LICENSE
--rw-r--r--   0        0        0     2866 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/README.md
--rw-r--r--   0        0        0      653 2024-05-25 12:04:10.405672 telegramify_markdown-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1525 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/src/telegramify_markdown/__init__.py
--rw-r--r--   0        0        0      359 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/src/telegramify_markdown/customize.py
--rw-r--r--   0        0        0     6224 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/src/telegramify_markdown/render.py
--rw-r--r--   0        0        0     1908 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/tests/exp1.md
--rw-r--r--   0        0        0      437 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/tests/exp_test.py
--rw-r--r--   0        0        0      608 2024-05-25 12:03:59.209779 telegramify_markdown-0.1.4/tests/server.py
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 telegramify_markdown-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3454 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/README.md
+-rw-r--r--   0        0        0      653 2024-06-01 12:44:10.880460 telegramify_markdown-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1700 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/src/telegramify_markdown/__init__.py
+-rw-r--r--   0        0        0      381 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/src/telegramify_markdown/customize.py
+-rw-r--r--   0        0        0     7128 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/src/telegramify_markdown/render.py
+-rw-r--r--   0        0        0     1908 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/tests/exp1.md
+-rw-r--r--   0        0        0      445 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/tests/exp_test.py
+-rw-r--r--   0        0        0      608 2024-06-01 12:43:58.520380 telegramify_markdown-0.1.5/tests/server.py
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 telegramify_markdown-0.1.5/PKG-INFO
```

### Comparing `telegramify_markdown-0.1.4/LICENSE` & `telegramify_markdown-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramify_markdown-0.1.4/README.md` & `telegramify_markdown-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 # telegramify-markdown
 
-[![PyPI version](https://badge.fury.io/py/telegramify-markdown.svg)](https://badge.fury.io/py/telegramify-markdown)
+[![PyPI version](https://badge.fury.io/py/telegramify-markdown.svg)](https://badge.fury.io/py/telegramify-markdown)  
 [![Downloads](https://pepy.tech/badge/telegramify-markdown)](https://pepy.tech/project/telegramify-markdown)
 
-> 🪄 Python Telegram markdown Converter | No more worrying about formatting.
+> 🪄 Python Telegram Markdown Converter | No more formatting headaches.
 
-**Raw Markdown -> Telegram MarkdownV2 Style**
+**Convert Raw Markdown to Telegram's MarkdownV2 Style**
 
-Before this repo came along, when you wanted to send and render unknown Markdown content (like GitHub's Readme),
-you had to use complex parsing and reconstruction methods.
-Today, you can make it easier and customize it to achieve better results!
+Introducing a robust Python library that enhances Markdown formatting support in Telegram. This library automatically
+processes various Markdown inputs, preserving the original formatting without requiring manual escaping. It simplifies
+your Markdown interactions on Telegram with seamless auto-processing.
 
-I used a custom Render to achieve this, using a real environment server to verify the applicability of this tool.
+Before this library, sending and rendering unknown Markdown content (like GitHub's README files) required complex
+parsing and reconstruction. Now, you can easily handle this and customize it for better results!
+
+Utilizing a custom renderer, the library has been tested in a real server environment to ensure its efficacy.
+
+> For those interested, there is also a Node.js version of the library with the same
+> name: [npm:telegramify-markdown](https://www.npmjs.com/package/telegramify-markdown)
 
 ## Installation
 
+To install the library, run:
+
 ```bash
 pip install telegramify-markdown
 ```
 
-or if you use `pdm`:
+or, if you use `pdm`:
 
 ```shell
 pdm add telegramify-markdown
 ```
 
 ## Supported Input
 
-- [x] Headings (1-6)
+- [x] Headings (Levels 1-6)
 - [x] `Links [text](url)`
-- [x] `Images ![alt]`
-- [x] Lists (Ordered, Unordered)
-- [x] `Tables |-|-|`
-- [x] `Horizontal Rule ----`
-- [x] `*Text* **Styles**`
-- [x] `__Underline__` (if `customize.strict_markdown` is False)
+- [x] `Images ![alt](url)`
+- [x] Lists (Ordered and Unordered)
+- [x] Tables `|-|-|`
+- [x] Horizontal Rules `----`
+- [x] Text Styles `*Italic*` and `**Bold**`
+- [x] Underline `__Underline__` (if `customize.strict_markdown` is False)
 - [x] Code Blocks
-- [x] `Inline Code`
-- [x] `Block Quotes >`
-- [x] `~~Strikethrough~~`
+- [x] Inline Code
+- [x] Block Quotes `>`
+- [x] Strikethrough `~~Strikethrough~~`
 - [ ] Task Lists
-- [ ] `~Strikethrough~`
-- [ ] ||Spoiler||
-- [ ] Tg Emoji
-- [ ] Tg User At
-
-> [!NOTE]
-> Since mistletoe doesn't parse `- [] TODO` and Spoiler, we can't apply it.
-`~Strikethrough~` is incorrect, even if it comes from telegram official documentation, its cant be parsed as
-> strikethrough.
+- [ ] Strikethrough `~Strikethrough~`
+- [ ] Spoilers `||Spoiler||`
+- [ ] Telegram Emojis
+- [ ] Telegram User Mentions
+
+> [!NOTE]  
+> Since mistletoe doesn't parse `- [ ] TODO` or Spoilers, we can't implement them.  
+> Despite `~Strikethrough~` being mentioned in Telegram's official documentation, it can't be parsed as strikethrough.
 
 ## Use case
 
 ````python3
 import telegramify_markdown
 from telegramify_markdown import customize
 
@@ -80,15 +87,15 @@
 ```
 This is `inline code`
 1. First ordered list item
 2. Another item
     - Unordered sub-list.
 1. Actual numbers don't matter, just that it's a number
 """
-converted = telegramify_markdown.convert(markdown_text)
+converted = telegramify_markdown.markdownify(markdown_text)
 print(converted)
 # export Markdown to Telegram MarkdownV2 style.
 ````
 
 output as follows:
 
 ![.github/result.png](.github/result.png)
```

### Comparing `telegramify_markdown-0.1.4/pyproject.toml` & `telegramify_markdown-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [project]
 name = "telegramify-markdown"
-version = "0.1.4"
+version = "0.1.5"
 description = "Convert Markdown to a format usable by Telegram."
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "mistletoe==1.3.0",
-    "pytelegrambotapi>=4.16.1",
     "emoji>=2.10.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
@@ -25,11 +24,12 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "loguru>=0.7.2",
     "python-dotenv>=1.0.1",
+    "pytelegrambotapi>=4.18.1",
 ]
 
 [tool.pdm.scripts]
 test = "python -m unittest discover -s ./tests -p *_test.py"
```

### Comparing `telegramify_markdown-0.1.4/src/telegramify_markdown/__init__.py` & `telegramify_markdown-0.1.5/src/telegramify_markdown/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 from typing import Union
 
 import mistletoe
 from mistletoe.block_token import BlockToken, ThematicBreak
 from mistletoe.markdown_renderer import LinkReferenceDefinition
 from mistletoe.span_token import SpanToken
-from telebot import formatting
 
-from .render import TelegramMarkdownRenderer
+from . import customize
+from .render import TelegramMarkdownRenderer, escape_markdown
 
-
-def markdownify(text: str):
-    # '_', '*', '[', ']', '(', ')', '~', '`', '>', '#', '+', '-', '=', '|', '{', '}', '.', '!'
-    return formatting.escape_markdown(text)
+__all__ = [
+    "convert",
+    "escape_markdown",
+    "customize",
+    "markdownify"
+]
 
 
 def _update_text(token: Union[SpanToken, BlockToken]):
     """Update the text contents of a span token and its children.
     `InlineCode` tokens are left unchanged."""
     if isinstance(token, ThematicBreak):
-        token.line = formatting.escape_markdown("————————")
+        token.line = escape_markdown("————————")
         pass
     elif isinstance(token, LinkReferenceDefinition):
         pass
     else:
         assert hasattr(token, "content"), f"Token {token} has no content attribute"
-        token.content = markdownify(token.content)
+        token.content = escape_markdown(token.content, unescape_html=customize.unescape_html)
 
 
 def _update_block(token: BlockToken):
     """Update the text contents of paragraphs and headings within this block,
     and recursively within its children."""
     if hasattr(token, "children"):
-        # 解包所有的子节点
+        # Dispatch all children
         for child in token.children:
             _update_block(child)
     else:
         _update_text(token)
 
 
-def convert(content: str):
+def convert(content: str) -> str:
     with TelegramMarkdownRenderer() as renderer:
         document = mistletoe.Document(content)
         _update_block(document)
         result = renderer.render(document)
     return result
+
+
+def markdownify(content: str) -> str:
+    # '_', '*', '[', ']', '(', ')', '~', '`', '>', '#', '+', '-', '=', '|', '{', '}', '.', '!'
+    # simple warp for the markdownify function
+    return convert(content)
```

### Comparing `telegramify_markdown-0.1.4/src/telegramify_markdown/render.py` & `telegramify_markdown-0.1.5/src/telegramify_markdown/render.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,41 @@
+import html
+import re
 from typing import Iterable
 
 from mistletoe import block_token, span_token
 from mistletoe.markdown_renderer import MarkdownRenderer, LinkReferenceDefinition, Fragment
 from telebot import formatting
 
 from .customize import markdown_symbol, strict_markdown
 
 
+def escape_markdown(content: str, unescape_html: bool = True) -> str:
+    """
+    Escapes Markdown characters in a string of Markdown with optional HTML unescaping.
+
+    :param content: The string of Markdown to escape.
+    :type content: str
+    :param unescape_html: Whether to unescape HTML entities before escaping, defaults to True.
+    :type unescape_html: bool, optional
+    :return: The escaped string.
+    :rtype: str
+    """
+    if not content:
+        return ""
+    # Unescape HTML entities if specified
+    if unescape_html:
+        content = html.unescape(content)
+    # First pass to escape all markdown special characters
+    escaped_content = re.sub(r"([_*\[\]()~`>\#\+\-=|{}\.!\\])", r"\\\1", content)
+    # Second pass to remove double escaping
+    final_content = re.sub(r"\\\\([_*\[\]()~`>\#\+\-=|{}\.!\\])", r"\\\1", escaped_content)
+    return final_content
+
+
 class TelegramMarkdownRenderer(MarkdownRenderer):
 
     def render_heading(
             self, token: block_token.Heading, max_line_length: int
     ) -> Iterable[str]:
         # note: no word wrapping, because atx headings always fit on a single line.
         line = ""
```

### Comparing `telegramify_markdown-0.1.4/tests/exp1.md` & `telegramify_markdown-0.1.5/tests/exp1.md`

 * *Files identical despite different names*

### Comparing `telegramify_markdown-0.1.4/tests/server.py` & `telegramify_markdown-0.1.5/tests/server.py`

 * *Files identical despite different names*

### Comparing `telegramify_markdown-0.1.4/PKG-INFO` & `telegramify_markdown-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 Metadata-Version: 2.1
 Name: telegramify-markdown
-Version: 0.1.4
+Version: 0.1.5
 Summary: Convert Markdown to a format usable by Telegram.
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: mistletoe==1.3.0
-Requires-Dist: pytelegrambotapi>=4.16.1
 Requires-Dist: emoji>=2.10.1
 Description-Content-Type: text/markdown
 
 # telegramify-markdown
 
-[![PyPI version](https://badge.fury.io/py/telegramify-markdown.svg)](https://badge.fury.io/py/telegramify-markdown)
+[![PyPI version](https://badge.fury.io/py/telegramify-markdown.svg)](https://badge.fury.io/py/telegramify-markdown)  
 [![Downloads](https://pepy.tech/badge/telegramify-markdown)](https://pepy.tech/project/telegramify-markdown)
 
-> 🪄 Python Telegram markdown Converter | No more worrying about formatting.
+> 🪄 Python Telegram Markdown Converter | No more formatting headaches.
 
-**Raw Markdown -> Telegram MarkdownV2 Style**
+**Convert Raw Markdown to Telegram's MarkdownV2 Style**
 
-Before this repo came along, when you wanted to send and render unknown Markdown content (like GitHub's Readme),
-you had to use complex parsing and reconstruction methods.
-Today, you can make it easier and customize it to achieve better results!
+Introducing a robust Python library that enhances Markdown formatting support in Telegram. This library automatically
+processes various Markdown inputs, preserving the original formatting without requiring manual escaping. It simplifies
+your Markdown interactions on Telegram with seamless auto-processing.
 
-I used a custom Render to achieve this, using a real environment server to verify the applicability of this tool.
+Before this library, sending and rendering unknown Markdown content (like GitHub's README files) required complex
+parsing and reconstruction. Now, you can easily handle this and customize it for better results!
+
+Utilizing a custom renderer, the library has been tested in a real server environment to ensure its efficacy.
+
+> For those interested, there is also a Node.js version of the library with the same
+> name: [npm:telegramify-markdown](https://www.npmjs.com/package/telegramify-markdown)
 
 ## Installation
 
+To install the library, run:
+
 ```bash
 pip install telegramify-markdown
 ```
 
-or if you use `pdm`:
+or, if you use `pdm`:
 
 ```shell
 pdm add telegramify-markdown
 ```
 
 ## Supported Input
 
-- [x] Headings (1-6)
+- [x] Headings (Levels 1-6)
 - [x] `Links [text](url)`
-- [x] `Images ![alt]`
-- [x] Lists (Ordered, Unordered)
-- [x] `Tables |-|-|`
-- [x] `Horizontal Rule ----`
-- [x] `*Text* **Styles**`
-- [x] `__Underline__` (if `customize.strict_markdown` is False)
+- [x] `Images ![alt](url)`
+- [x] Lists (Ordered and Unordered)
+- [x] Tables `|-|-|`
+- [x] Horizontal Rules `----`
+- [x] Text Styles `*Italic*` and `**Bold**`
+- [x] Underline `__Underline__` (if `customize.strict_markdown` is False)
 - [x] Code Blocks
-- [x] `Inline Code`
-- [x] `Block Quotes >`
-- [x] `~~Strikethrough~~`
+- [x] Inline Code
+- [x] Block Quotes `>`
+- [x] Strikethrough `~~Strikethrough~~`
 - [ ] Task Lists
-- [ ] `~Strikethrough~`
-- [ ] ||Spoiler||
-- [ ] Tg Emoji
-- [ ] Tg User At
-
-> [!NOTE]
-> Since mistletoe doesn't parse `- [] TODO` and Spoiler, we can't apply it.
-`~Strikethrough~` is incorrect, even if it comes from telegram official documentation, its cant be parsed as
-> strikethrough.
+- [ ] Strikethrough `~Strikethrough~`
+- [ ] Spoilers `||Spoiler||`
+- [ ] Telegram Emojis
+- [ ] Telegram User Mentions
+
+> [!NOTE]  
+> Since mistletoe doesn't parse `- [ ] TODO` or Spoilers, we can't implement them.  
+> Despite `~Strikethrough~` being mentioned in Telegram's official documentation, it can't be parsed as strikethrough.
 
 ## Use case
 
 ````python3
 import telegramify_markdown
 from telegramify_markdown import customize
 
@@ -92,15 +98,15 @@
 ```
 This is `inline code`
 1. First ordered list item
 2. Another item
     - Unordered sub-list.
 1. Actual numbers don't matter, just that it's a number
 """
-converted = telegramify_markdown.convert(markdown_text)
+converted = telegramify_markdown.markdownify(markdown_text)
 print(converted)
 # export Markdown to Telegram MarkdownV2 style.
 ````
 
 output as follows:
 
 ![.github/result.png](.github/result.png)
```

