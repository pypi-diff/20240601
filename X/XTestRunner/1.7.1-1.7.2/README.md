# Comparing `tmp/xtestrunner-1.7.1.tar.gz` & `tmp/xtestrunner-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtestrunner-1.7.1.tar", max compression
+gzip compressed data, was "xtestrunner-1.7.2.tar", max compression
```

## Comparing `xtestrunner-1.7.1.tar` & `xtestrunner-1.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.7.1/LICENSE
--rw-r--r--   0        0        0     1207 2024-01-10 15:23:43.972430 xtestrunner-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     2348 2023-04-25 16:31:51.687169 xtestrunner-1.7.1/README.md
--rw-r--r--   0        0        0     2107 2023-04-25 16:25:31.621688 xtestrunner-1.7.1/XTestRunner/__init__.py
--rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.7.1/XTestRunner/_dingtalk.py
--rw-r--r--   0        0        0     3571 2023-04-05 03:32:24.218179 xtestrunner-1.7.1/XTestRunner/_email.py
--rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.7.1/XTestRunner/_feishu.py
--rw-r--r--   0        0        0     4251 2023-03-06 16:55:59.684323 xtestrunner-1.7.1/XTestRunner/_weixin.py
--rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.7.1/XTestRunner/config.py
--rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.7.1/XTestRunner/html/__init__.py
--rw-r--r--   0        0        0     8196 2024-01-10 14:51:29.597680 xtestrunner-1.7.1/XTestRunner/html/heading-en.html
--rw-r--r--   0        0        0     8199 2023-04-25 16:05:13.858021 xtestrunner-1.7.1/XTestRunner/html/heading-zh-CN.html
--rw-r--r--   0        0        0     3788 2023-04-25 16:05:13.859010 xtestrunner-1.7.1/XTestRunner/html/mail.html
--rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.7.1/XTestRunner/html/notice_tmp.md
--rw-r--r--   0        0        0     2366 2024-01-10 14:57:18.142618 xtestrunner-1.7.1/XTestRunner/html/report-en.html
--rw-r--r--   0        0        0     2372 2024-01-10 14:57:18.137618 xtestrunner-1.7.1/XTestRunner/html/report-zh-CN.html
--rw-r--r--   0        0        0     4761 2023-04-25 16:05:13.863034 xtestrunner-1.7.1/XTestRunner/html/stylesheet.html
--rw-r--r--   0        0        0     9782 2024-01-10 15:12:05.451794 xtestrunner-1.7.1/XTestRunner/html/template.html
--rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.7.1/XTestRunner/htmlrunner/__init__.py
--rw-r--r--   0        0        0     8914 2023-04-05 03:32:24.219167 xtestrunner-1.7.1/XTestRunner/htmlrunner/result.py
--rw-r--r--   0        0        0    19466 2024-01-10 15:08:39.042505 xtestrunner-1.7.1/XTestRunner/htmlrunner/runner.py
--rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.7.1/XTestRunner/version.py
--rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.7.1/XTestRunner/xmlrunner/__init__.py
--rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.7.1/XTestRunner/xmlrunner/result.py
--rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.7.1/XTestRunner/xmlrunner/runner.py
--rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 xtestrunner-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.7.2/LICENSE
+-rw-r--r--   0        0        0     1254 2024-06-01 08:53:25.133580 xtestrunner-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2348 2023-04-25 16:31:51.687169 xtestrunner-1.7.2/README.md
+-rw-r--r--   0        0        0     2126 2024-06-01 08:54:42.950047 xtestrunner-1.7.2/XTestRunner/__init__.py
+-rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.7.2/XTestRunner/_dingtalk.py
+-rw-r--r--   0        0        0     3608 2024-05-31 08:57:33.106682 xtestrunner-1.7.2/XTestRunner/_email.py
+-rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.7.2/XTestRunner/_feishu.py
+-rw-r--r--   0        0        0     4243 2024-05-31 08:57:33.107681 xtestrunner-1.7.2/XTestRunner/_weixin.py
+-rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.7.2/XTestRunner/config.py
+-rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.7.2/XTestRunner/html/__init__.py
+-rw-r--r--   0        0        0     8196 2024-01-10 14:51:29.597680 xtestrunner-1.7.2/XTestRunner/html/heading-en.html
+-rw-r--r--   0        0        0     8199 2023-04-25 16:05:13.858021 xtestrunner-1.7.2/XTestRunner/html/heading-zh-CN.html
+-rw-r--r--   0        0        0     3788 2023-04-25 16:05:13.859010 xtestrunner-1.7.2/XTestRunner/html/mail.html
+-rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.7.2/XTestRunner/html/notice_tmp.md
+-rw-r--r--   0        0        0     2366 2024-01-10 14:57:18.142618 xtestrunner-1.7.2/XTestRunner/html/report-en.html
+-rw-r--r--   0        0        0     2372 2024-01-10 14:57:18.137618 xtestrunner-1.7.2/XTestRunner/html/report-zh-CN.html
+-rw-r--r--   0        0        0     4761 2023-04-25 16:05:13.863034 xtestrunner-1.7.2/XTestRunner/html/stylesheet.html
+-rw-r--r--   0        0        0     9782 2024-01-10 15:12:05.451794 xtestrunner-1.7.2/XTestRunner/html/template.html
+-rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.7.2/XTestRunner/htmlrunner/__init__.py
+-rw-r--r--   0        0        0     8914 2023-04-05 03:32:24.219167 xtestrunner-1.7.2/XTestRunner/htmlrunner/result.py
+-rw-r--r--   0        0        0    19466 2024-01-10 15:08:39.042505 xtestrunner-1.7.2/XTestRunner/htmlrunner/runner.py
+-rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.7.2/XTestRunner/version.py
+-rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.7.2/XTestRunner/xmlrunner/__init__.py
+-rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.7.2/XTestRunner/xmlrunner/result.py
+-rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.7.2/XTestRunner/xmlrunner/runner.py
+-rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 xtestrunner-1.7.2/PKG-INFO
```

### Comparing `xtestrunner-1.7.1/LICENSE` & `xtestrunner-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/pyproject.toml` & `xtestrunner-1.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "XTestRunner"
-version = "1.7.1"
+version = "1.7.2"
 description = "Modern style test report based on unittest framework."
 authors = ["bugmaster <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/seldomQA/XTestRunner/"
 repository = "https://github.com/seldomQA/XTestRunner/"
 classifiers = [
@@ -15,14 +15,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     "Topic :: Software Development :: Testing",
     'Topic :: Software Development :: Version Control :: Git'
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `xtestrunner-1.7.1/README.md` & `xtestrunner-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/__init__.py` & `xtestrunner-1.7.2/XTestRunner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,13 +35,12 @@
 from .htmlrunner.runner import HTMLTestRunner
 from ._email import SMTP
 from ._dingtalk import DingTalk
 from ._feishu import FeiShu
 from ._weixin import Weinxin
 from .config import label
 
-
 __author__ = "bugmaster"
 
-__version__ = "1.7.0"
+__version__ = "1.7.2"
 
-__description__ = "Unittest-based HTML test report."
+__description__ = "Modern style test report based on unittest framework."
```

### Comparing `xtestrunner-1.7.1/XTestRunner/_dingtalk.py` & `xtestrunner-1.7.2/XTestRunner/_dingtalk.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/_email.py` & `xtestrunner-1.7.2/XTestRunner/_email.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         :param port: Email service post
         :param ssl: SMTP SSL True/False
         :param tls: TLS mode True/False
         """
         self.user = user
         self.password = password
         self.host = host
-        self.port = int(port) if port is not None else 465
+        self.port = int(port) if port is not None else (465 if ssl else 587)
         self.ssl = ssl
         self.tls = tls
 
     def sender(self, to=None, subject=None, contents=None, attachments=None):
         if to is None:
             raise ValueError("Please specify the email address to send")
 
@@ -79,19 +79,19 @@
             if "\\" in attachments:
                 att_name = attachments.split("\\")[-1]
             if "/" in attachments:
                 att_name = attachments.split("/")[-1]
 
             att = MIMEApplication(open(attachments, 'rb').read())
             att['Content-Type'] = 'application/octet-stream'
-            att["Content-Disposition"] = 'attachment; filename="{}"'.format(att_name)
+            att.add_header('Content-Disposition', 'attachment', filename=att_name)
             msg.attach(att)
 
         smtp = smtplib.SMTP_SSL(self.host, self.port) if self.ssl else smtplib.SMTP(self.host, self.port)
-        if self.tls is True:
+        if self.tls is True and self.ssl is False:
             smtp.starttls()
         try:
             smtp.login(self.user, self.password)
             smtp.sendmail(self.user, to, msg.as_string())
             print(" 📧 Email sent successfully!!")
         except BaseException as msg:
             print('❌ Email failed to send!!' + msg.__str__())
```

### Comparing `xtestrunner-1.7.1/XTestRunner/_feishu.py` & `xtestrunner-1.7.2/XTestRunner/_feishu.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/_weixin.py` & `xtestrunner-1.7.2/XTestRunner/_weixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,17 +79,17 @@
             res_text = res_text + str(append)
         if text is not None:
             res_text = text
 
         message = {"msgtype": "text", "text": {"content": res_text, "mentioned_mobile_list": self.at_mobiles}}
         resp = self._send_message(self.url, message)
         if resp["errcode"] == 0:
-            print(" 📧 dingTalk sent successfully!!")
+            print(" 📧 weixin sent successfully!!")
         else:
-            print("❌ dingTalk failed to send!!")
+            print("❌ weixin failed to send!!")
             print(resp)
         return resp
 
     def send_markdown(self, append: str = None, text: str = None):
         """
         发送markdown类型的消息
         :param append: appending sending information
@@ -101,17 +101,17 @@
             res_text = res_text + str(append)
         if text is not None:
             res_text = text
 
         message = {"msgtype": "markdown", "markdown": {"content": res_text}}
         resp = self._send_message(self.url, message)
         if resp["errcode"] == 0:
-            print(" 📧 dingTalk sent successfully!!")
+            print(" 📧 weixin sent successfully!!")
         else:
-            print("❌ dingTalk failed to send!!")
+            print("❌ weixin failed to send!!")
             print(resp)
         return resp
 
 
 if __name__ == '__main__':
     weixin = Weinxin(
         access_token="50327a8c-59c3-4be7-bf44-a7ad4ec749b59",
```

### Comparing `xtestrunner-1.7.1/XTestRunner/config.py` & `xtestrunner-1.7.2/XTestRunner/config.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/heading-en.html` & `xtestrunner-1.7.2/XTestRunner/html/heading-en.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/heading-zh-CN.html` & `xtestrunner-1.7.2/XTestRunner/html/heading-zh-CN.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/mail.html` & `xtestrunner-1.7.2/XTestRunner/html/mail.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/report-en.html` & `xtestrunner-1.7.2/XTestRunner/html/report-en.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/report-zh-CN.html` & `xtestrunner-1.7.2/XTestRunner/html/report-zh-CN.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/stylesheet.html` & `xtestrunner-1.7.2/XTestRunner/html/stylesheet.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/html/template.html` & `xtestrunner-1.7.2/XTestRunner/html/template.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/htmlrunner/result.py` & `xtestrunner-1.7.2/XTestRunner/htmlrunner/result.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/htmlrunner/runner.py` & `xtestrunner-1.7.2/XTestRunner/htmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/xmlrunner/result.py` & `xtestrunner-1.7.2/XTestRunner/xmlrunner/result.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/XTestRunner/xmlrunner/runner.py` & `xtestrunner-1.7.2/XTestRunner/xmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.7.1/PKG-INFO` & `xtestrunner-1.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xtestrunner
-Version: 1.7.1
+Name: XTestRunner
+Version: 1.7.2
 Summary: Modern style test report based on unittest framework.
 Home-page: https://github.com/seldomQA/XTestRunner/
 License: Apache-2.0
 Author: bugmaster
 Author-email: fnngj@126.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Project-URL: Repository, https://github.com/seldomQA/XTestRunner/
 Description-Content-Type: text/markdown
```

