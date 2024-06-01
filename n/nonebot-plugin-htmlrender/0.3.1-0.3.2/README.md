# Comparing `tmp/nonebot_plugin_htmlrender-0.3.1.tar.gz` & `tmp/nonebot_plugin_htmlrender-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_htmlrender-0.3.1.tar", last modified: Thu Mar 14 08:47:11 2024, max compression
+gzip compressed data, was "nonebot_plugin_htmlrender-0.3.2.tar", last modified: Sat Jun  1 15:54:12 2024, max compression
```

## Comparing `nonebot_plugin_htmlrender-0.3.1.tar` & `nonebot_plugin_htmlrender-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1062 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/LICENSE
--rw-r--r--   0        0        0     4109 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/README.md
--rw-r--r--   0        0        0     1349 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/__init__.py
--rw-r--r--   0        0        0     3349 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/browser.py
--rw-r--r--   0        0        0      357 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/config.py
--rw-r--r--   0        0        0     8368 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/data_source.py
--rw-r--r--   0        0        0    17297 2024-03-14 08:47:08.845370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      630 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/markdown.html
--rw-r--r--   0        0        0     4889 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/pygments-default.css
--rw-r--r--   0        0        0      117 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/text.css
--rw-r--r--   0        0        0      220 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/text.html
--rw-r--r--   0        0        0      941 2024-03-14 08:47:11.517383 nonebot_plugin_htmlrender-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      204 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     2281 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/templates/markdown.css
--rw-r--r--   0        0        0       62 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/templates/mystyle.css
--rw-r--r--   0        0        0      406 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/templates/text.html
--rw-r--r--   0        0        0     1462 2024-03-14 08:47:08.857370 nonebot_plugin_htmlrender-0.3.1/tests/test_htmlrender.py
--rw-r--r--   0        0        0     5996 1970-01-01 00:00:00.000000 nonebot_plugin_htmlrender-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-06-01 15:54:10.010057 nonebot_plugin_htmlrender-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4109 2024-06-01 15:54:10.010057 nonebot_plugin_htmlrender-0.3.2/README.md
+-rw-r--r--   0        0        0     1349 2024-06-01 15:54:10.014057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/__init__.py
+-rw-r--r--   0        0        0     3335 2024-06-01 15:54:10.014057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/browser.py
+-rw-r--r--   0        0        0      357 2024-06-01 15:54:10.014057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/config.py
+-rw-r--r--   0        0        0     8605 2024-06-01 15:54:10.014057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/data_source.py
+-rw-r--r--   0        0        0    17297 2024-06-01 15:54:10.014057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2024-06-01 15:54:10.022057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      630 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/markdown.html
+-rw-r--r--   0        0        0     4889 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/pygments-default.css
+-rw-r--r--   0        0        0      117 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/text.css
+-rw-r--r--   0        0        0      220 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/text.html
+-rw-r--r--   0        0        0      941 2024-06-01 15:54:12.746063 nonebot_plugin_htmlrender-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      204 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     2281 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/templates/markdown.css
+-rw-r--r--   0        0        0       62 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/templates/mystyle.css
+-rw-r--r--   0        0        0      406 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/templates/text.html
+-rw-r--r--   0        0        0     1462 2024-06-01 15:54:10.026057 nonebot_plugin_htmlrender-0.3.2/tests/test_htmlrender.py
+-rw-r--r--   0        0        0     5996 1970-01-01 00:00:00.000000 nonebot_plugin_htmlrender-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_htmlrender-0.3.1/LICENSE` & `nonebot_plugin_htmlrender-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/README.md` & `nonebot_plugin_htmlrender-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/__init__.py` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/browser.py` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/browser.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 @Author         : yanyongyu
 @Date           : 2021-03-12 13:42:43
 @LastEditors    : yanyongyu
 @LastEditTime   : 2021-11-01 14:05:41
 @Description    : None
 @GitHub         : https://github.com/yanyongyu
 """
+
 __author__ = "yanyongyu"
 
 from contextlib import asynccontextmanager
 from typing import AsyncIterator, Optional
 
 from nonebot import get_plugin_config
 from nonebot.log import logger
 from playwright.async_api import Browser, Error, Page, Playwright, async_playwright
 
 from .config import Config
-import asyncio
 
 config = get_plugin_config(Config)
 
 _browser: Optional[Browser] = None
 _playwright: Optional[Playwright] = None
```

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/data_source.py` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/data_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import getcwd
 from pathlib import Path
-from typing import Literal, Optional, Union
+from typing import Any, Dict, Literal, Optional, Union
 
 import aiofiles
 import jinja2
 import markdown
 from nonebot.log import logger
 
 from .browser import get_new_page
@@ -188,41 +188,42 @@
     Returns:
         bytes: 图片, 可直接发送
     """
     # logger.debug(f"html:\n{html}")
     if "file:" not in template_path:
         raise Exception("template_path 应该为 file:///path/to/template")
     async with get_new_page(device_scale_factor, **kwargs) as page:
+        page.on("console", lambda msg: logger.debug(f"浏览器控制台: {msg.text}"))
         await page.goto(template_path)
         await page.set_content(html, wait_until="networkidle")
         await page.wait_for_timeout(wait)
         return await page.screenshot(
             full_page=True,
             type=type,
             quality=quality,
         )
 
 
 async def template_to_pic(
     template_path: str,
     template_name: str,
-    templates: dict,
-    pages: Optional[dict] = None,
+    templates: Dict[Any, Any],
+    pages: Optional[Dict[Any, Any]] = None,
     wait: int = 0,
     type: Literal["jpeg", "png"] = "png",  # noqa: A002
     quality: Union[int, None] = None,
     device_scale_factor: float = 2,
 ) -> bytes:
     """使用jinja2模板引擎通过html生成图片
 
     Args:
         template_path (str): 模板路径
         template_name (str): 模板名
-        templates (dict): 模板内参数 如: {"name": "abc"}
-        pages (dict): 网页参数 Defaults to
+        templates (Dict[Any, Any]): 模板内参数 如: {"name": "abc"}
+        pages (Optional[Dict[Any, Any]]): 网页参数 Defaults to
             {"base_url": f"file://{getcwd()}", "viewport": {"width": 500, "height": 10}}
         wait (int, optional): 网页载入等待时间. Defaults to 0.
         type (Literal["jpeg", "png"]): 图片类型, 默认 png
         quality (int, optional): 图片质量 0-100 当为`png`时无效
         device_scale_factor: 缩放比例,类型为float,值越大越清晰(真正想让图片清晰更优先请调整此选项)
     Returns:
         bytes: 图片 可直接发送
@@ -255,12 +256,13 @@
     element: str,
     timeout: float = 0,
     type: Literal["jpeg", "png"] = "png",  # noqa: A002
     quality: Union[int, None] = None,
     **kwargs,
 ) -> bytes:
     async with get_new_page(**kwargs) as page:
+        page.on("console", lambda msg: logger.debug(f"浏览器控制台: {msg.text}"))
         await page.goto(url, timeout=timeout)
         return await page.locator(element).screenshot(
             type=type,
             quality=quality,
         )
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-from os import getcwd from pathlib import Path from typing import Literal,
-Optional, Union import aiofiles import jinja2 import markdown from nonebot.log
-import logger from .browser import get_new_page TEMPLATES_PATH = str(Path
-(__file__).parent / "templates") env = jinja2.Environment( # noqa: S701
+from os import getcwd from pathlib import Path from typing import Any, Dict,
+Literal, Optional, Union import aiofiles import jinja2 import markdown from
+nonebot.log import logger from .browser import get_new_page TEMPLATES_PATH =
+str(Path(__file__).parent / "templates") env = jinja2.Environment( # noqa: S701
 extensions=["jinja2.ext.loopcontrols"], loader=jinja2.FileSystemLoader
 (TEMPLATES_PATH), enable_async=True, ) async def text_to_pic( text: str,
 css_path: str = "", width: int = 500, type: Literal["jpeg", "png"] = "png", #
 noqa: A002 quality: Union[int, None] = None, device_scale_factor: float = 2, )
 -> bytes: """å¤è¡ææ¬è½¬å¾ç Args: text (str): çº¯ææ¬, å¯å¤è¡
 css_path (str, optional): cssæä»¶ width (int, optional):
 å¾çå®½åº¦ï¼é»è®¤ä¸º 500 type (Literal["jpeg", "png"]): å¾çç±»å,
@@ -65,35 +65,37 @@
 å¾çç±»å, é»è®¤ png quality (int, optional): å¾çè´¨é 0-100
 å½ä¸º`png`æ¶æ æ device_scale_factor:
 ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
 (çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) **kwargs: ä¼ å¥ page
 çåæ° Returns: bytes: å¾ç, å¯ç´æ¥åé """ # logger.debug(f"html:\n
 {html}") if "file:" not in template_path: raise Exception("template_path
 åºè¯¥ä¸º file:///path/to/template") async with get_new_page
-(device_scale_factor, **kwargs) as page: await page.goto(template_path) await
-page.set_content(html, wait_until="networkidle") await page.wait_for_timeout
-(wait) return await page.screenshot( full_page=True, type=type,
-quality=quality, ) async def template_to_pic( template_path: str,
-template_name: str, templates: dict, pages: Optional[dict] = None, wait: int =
-0, type: Literal["jpeg", "png"] = "png", # noqa: A002 quality: Union[int, None]
-= None, device_scale_factor: float = 2, ) -> bytes:
+(device_scale_factor, **kwargs) as page: page.on("console", lambda msg:
+logger.debug(f"æµè§å¨æ§å¶å°: {msg.text}")) await page.goto(template_path)
+await page.set_content(html, wait_until="networkidle") await
+page.wait_for_timeout(wait) return await page.screenshot( full_page=True,
+type=type, quality=quality, ) async def template_to_pic( template_path: str,
+template_name: str, templates: Dict[Any, Any], pages: Optional[Dict[Any, Any]]
+= None, wait: int = 0, type: Literal["jpeg", "png"] = "png", # noqa: A002
+quality: Union[int, None] = None, device_scale_factor: float = 2, ) -> bytes:
 """ä½¿ç¨jinja2æ¨¡æ¿å¼æéè¿htmlçæå¾ç Args: template_path (str):
-æ¨¡æ¿è·¯å¾ template_name (str): æ¨¡æ¿å templates (dict): æ¨¡æ¿ååæ°
-å¦: {"name": "abc"} pages (dict): ç½é¡µåæ° Defaults to {"base_url":
-f"file://{getcwd()}", "viewport": {"width": 500, "height": 10}} wait (int,
-optional): ç½é¡µè½½å¥ç­å¾æ¶é´. Defaults to 0. type (Literal["jpeg",
-"png"]): å¾çç±»å, é»è®¤ png quality (int, optional): å¾çè´¨é 0-100
-å½ä¸º`png`æ¶æ æ device_scale_factor:
+æ¨¡æ¿è·¯å¾ template_name (str): æ¨¡æ¿å templates (Dict[Any, Any]):
+æ¨¡æ¿ååæ° å¦: {"name": "abc"} pages (Optional[Dict[Any, Any]]):
+ç½é¡µåæ° Defaults to {"base_url": f"file://{getcwd()}", "viewport":
+{"width": 500, "height": 10}} wait (int, optional): ç½é¡µè½½å¥ç­å¾æ¶é´.
+Defaults to 0. type (Literal["jpeg", "png"]): å¾çç±»å, é»è®¤ png quality
+(int, optional): å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ device_scale_factor:
 ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
 (çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) Returns: bytes: å¾ç
 å¯ç´æ¥åé """ if pages is None: pages = { "viewport": {"width": 500,
 "height": 10}, "base_url": f"file://{getcwd()}", # noqa: PTH109 } template_env
 = jinja2.Environment( # noqa: S701 loader=jinja2.FileSystemLoader
 (template_path), enable_async=True, ) template = template_env.get_template
 (template_name) return await html_to_pic( template_path=f"file://
 {template_path}", html=await template.render_async(**templates), wait=wait,
 type=type, quality=quality, device_scale_factor=device_scale_factor, **pages, )
 async def capture_element( url: str, element: str, timeout: float = 0, type:
 Literal["jpeg", "png"] = "png", # noqa: A002 quality: Union[int, None] = None,
-**kwargs, ) -> bytes: async with get_new_page(**kwargs) as page: await
+**kwargs, ) -> bytes: async with get_new_page(**kwargs) as page: page.on
+("console", lambda msg: logger.debug(f"æµè§å¨æ§å¶å°: {msg.text}")) await
 page.goto(url, timeout=timeout) return await page.locator(element).screenshot
 ( type=type, quality=quality, )
```

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/github-markdown-light.css` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/katex.min.js` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/markdown.html` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/nonebot_plugin_htmlrender/templates/pygments-default.css` & `nonebot_plugin_htmlrender-0.3.2/nonebot_plugin_htmlrender/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/pyproject.toml` & `nonebot_plugin_htmlrender-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "nonebot-plugin-htmlrender"
-version = "0.3.1"
+version = "0.3.2"
 description = "通过浏览器渲染图片"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "playwright>=1.17.2",
     "nonebot2[fastapi]>=2.2.0",
     "jinja2>=3.0.3",
     "markdown>=3.3.6",
     "Pygments>=2.10.0",
     "python-markdown-math>=0.8",
     "pymdown-extensions>=9.1",
     "aiofiles>=0.8.0",
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.9,<4.0"
 readme = "README.md"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/kexue-z/nonebot-plugin-htmlrender"
```

### Comparing `nonebot_plugin_htmlrender-0.3.1/tests/templates/markdown.css` & `nonebot_plugin_htmlrender-0.3.2/tests/templates/markdown.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/tests/test_htmlrender.py` & `nonebot_plugin_htmlrender-0.3.2/tests/test_htmlrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.3.1/PKG-INFO` & `nonebot_plugin_htmlrender-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-htmlrender
-Version: 0.3.1
+Version: 0.3.2
 Summary: 通过浏览器渲染图片
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT License
         
         Copyright (c) 2021 kexue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-htmlrender
 Project-URL: Bug tracker, https://github.com/kexue-z/nonebot-plugin-htmlrender/issues
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.9
 Requires-Dist: playwright>=1.17.2
 Requires-Dist: nonebot2[fastapi]>=2.2.0
 Requires-Dist: jinja2>=3.0.3
 Requires-Dist: markdown>=3.3.6
 Requires-Dist: Pygments>=2.10.0
 Requires-Dist: python-markdown-math>=0.8
 Requires-Dist: pymdown-extensions>=9.1
```

