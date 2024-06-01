# Comparing `tmp/weather_chatbot_phi3-0.1.1.tar.gz` & `tmp/weather_chatbot_phi3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_chatbot_phi3-0.1.1.tar", max compression
+gzip compressed data, was "weather_chatbot_phi3-0.1.2.tar", max compression
```

## Comparing `weather_chatbot_phi3-0.1.1.tar` & `weather_chatbot_phi3-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-06-01 13:36:28.802748 weather_chatbot_phi3-0.1.1/README.md
--rw-r--r--   0        0        0      624 2024-06-01 19:23:20.665655 weather_chatbot_phi3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       94 2024-06-01 19:12:51.845137 weather_chatbot_phi3-0.1.1/weather_chatbot/__init__.py
--rw-r--r--   0        0        0     2938 2024-06-01 19:13:13.282549 weather_chatbot_phi3-0.1.1/weather_chatbot/app.py
--rw-r--r--   0        0        0      423 2024-06-01 19:12:34.753201 weather_chatbot_phi3-0.1.1/weather_chatbot/download_model.py
--rw-r--r--   0        0        0     1094 2024-06-01 18:29:15.517301 weather_chatbot_phi3-0.1.1/weather_chatbot/push_model.py
--rw-r--r--   0        0        0       34 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.1/weather_chatbot/requirements.txt
--rw-r--r--   0        0        0      196 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.1/weather_chatbot/style.css
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 weather_chatbot_phi3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-06-01 13:36:28.802748 weather_chatbot_phi3-0.1.2/README.md
+-rw-r--r--   0        0        0      695 2024-06-01 19:58:55.547837 weather_chatbot_phi3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-06-01 19:12:51.845137 weather_chatbot_phi3-0.1.2/weather_chatbot/__init__.py
+-rw-r--r--   0        0        0     2991 2024-06-01 19:55:47.671834 weather_chatbot_phi3-0.1.2/weather_chatbot/app.py
+-rw-r--r--   0        0        0      423 2024-06-01 19:12:34.753201 weather_chatbot_phi3-0.1.2/weather_chatbot/download_model.py
+-rw-r--r--   0        0        0     1094 2024-06-01 18:29:15.517301 weather_chatbot_phi3-0.1.2/weather_chatbot/push_model.py
+-rw-r--r--   0        0        0       34 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.2/weather_chatbot/requirements.txt
+-rw-r--r--   0        0        0      196 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.2/weather_chatbot/style.css
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 weather_chatbot_phi3-0.1.2/PKG-INFO
```

### Comparing `weather_chatbot_phi3-0.1.1/weather_chatbot/app.py` & `weather_chatbot_phi3-0.1.2/weather_chatbot/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,9 +78,12 @@
             ["Tell me the weather forecast for Tokyo."],
             ["What's the temperature in London?"]
         ],
         inputs=message
     )
 
 # Launch the Gradio interface
-demo.launch(share=True, debug=True)
+def main():
+    demo.launch(share=True, debug=True)
 
+if __name__ == "__main__":
+    main()
```

### Comparing `weather_chatbot_phi3-0.1.1/weather_chatbot/push_model.py` & `weather_chatbot_phi3-0.1.2/weather_chatbot/push_model.py`

 * *Files identical despite different names*

### Comparing `weather_chatbot_phi3-0.1.1/PKG-INFO` & `weather_chatbot_phi3-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-chatbot-phi3
-Version: 0.1.1
+Version: 0.1.2
 Summary: An LLM Chatbot integrated with Open Weather API for Real-Time Weather Information.
 License: CC-BY-NC-SA-4.0
 Author: Vatsal Patel
 Author-email: vatsal1804@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

