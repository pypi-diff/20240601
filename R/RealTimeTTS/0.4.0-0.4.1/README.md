# Comparing `tmp/RealTimeTTS-0.4.0.tar.gz` & `tmp/RealTimeTTS-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.4.0.tar", last modified: Fri May 17 22:02:55 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.4.1.tar", last modified: Sat Jun  1 17:25:23 2024, max compression
```

## Comparing `RealTimeTTS-0.4.0.tar` & `RealTimeTTS-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.864385 RealTimeTTS-0.4.0/
--rw-rw-rw-   0        0        0    21039 2024-05-17 22:02:55.863385 RealTimeTTS-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    19894 2024-05-17 21:59:46.000000 RealTimeTTS-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.862384 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    21039 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      193 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 22:02:55.000000 RealTimeTTS-0.4.0/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.590479 RealTimeTTS-0.4.0/RealtimeTTS/
--rw-rw-rw-   0        0        0      466 2024-05-17 21:40:58.000000 RealTimeTTS-0.4.0/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.812388 RealTimeTTS-0.4.0/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      459 2024-05-17 21:41:03.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9413 2024-05-16 19:46:11.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    38627 2024-05-16 19:46:15.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10661 2024-05-16 20:09:01.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0     3878 2024-05-17 22:00:29.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/gtts_engine.py
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     4834 2024-05-17 20:58:34.000000 RealTimeTTS-0.4.0/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.4.0/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.4.0/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.0/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-05-17 22:02:55.864385 RealTimeTTS-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1294 2024-05-17 21:59:14.000000 RealTimeTTS-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 22:02:55.860382 RealTimeTTS-0.4.0/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.4.0/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.4.0/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:25:23.679263 RealTimeTTS-0.4.1/
+-rw-rw-rw-   0        0        0    21425 2024-06-01 17:25:23.678263 RealTimeTTS-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20274 2024-06-01 17:01:17.000000 RealTimeTTS-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 17:25:23.677264 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    21425 2024-06-01 17:25:23.000000 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-06-01 17:25:23.000000 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:25:23.000000 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      199 2024-06-01 17:25:23.000000 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 17:25:23.000000 RealTimeTTS-0.4.1/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:25:23.660263 RealTimeTTS-0.4.1/RealtimeTTS/
+-rw-rw-rw-   0        0        0      466 2024-05-17 21:40:58.000000 RealTimeTTS-0.4.1/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:25:23.673262 RealTimeTTS-0.4.1/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      459 2024-05-17 21:41:03.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0    11928 2024-06-01 16:18:56.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    38212 2024-06-01 16:32:49.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10845 2024-06-01 16:23:37.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0     4558 2024-06-01 16:47:12.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/gtts_engine.py
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     4834 2024-05-17 20:58:34.000000 RealTimeTTS-0.4.1/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10568 2024-06-01 16:49:40.000000 RealTimeTTS-0.4.1/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.4.1/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.4.1/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:25:23.679263 RealTimeTTS-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-06-01 17:25:05.000000 RealTimeTTS-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:25:23.675262 RealTimeTTS-0.4.1/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.4.1/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.4.1/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.4.0/PKG-INFO` & `RealTimeTTS-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.4.0
+Version: 0.4.1
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.3
 Requires-Dist: PyAudio==0.2.14
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: stream2sentence==0.2.3
-Requires-Dist: azure-cognitiveservices-speech==1.36.0
+Requires-Dist: azure-cognitiveservices-speech==1.37.0
 Requires-Dist: elevenlabs==1.2.2
-Requires-Dist: TTS==0.22.0
-Requires-Dist: tqdm==4.66.2
+Requires-Dist: tqdm==4.66.4
 Requires-Dist: pydub==0.25.1
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.30.5
 Requires-Dist: gtts==2.5.1
+Requires-Dist: coqui_tts==0.24.1
 
 # RealtimeTTS
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
@@ -53,15 +53,19 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.4.0 (added GTTS engine)
+Latest Version: v0.4.1 
+- switched coquiengine to [Idiap Research Institute](https://github.com/idiap)'s maintained [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS) (thank you)
+- added emotions to Azure engine
+- added speed to GTTS engine
+- bugfix for ElevenlabsEngine get_voices method
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -274,27 +278,29 @@
   
 - **PyAudio**: to create an output audio stream
   
 - **stream2sentence**: to split the incoming text stream into sentences 
 
 - **pyttsx3**: System text-to-speech conversion engine
 
-- **tqdm (>=4.66.2)**: to display progress bars in the command line
+- **tqdm**: to display progress bars in the command line
 
-- **pydub (>=0.25.1)**: to convert audio chunk formats
+- **pydub**: to convert audio chunk formats
 
 - **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
 - **elevenlabs**: Elevenlabs text-to-speech conversion engine
 
-- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+- **coqui-TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+  Shoutout to [Idiap Research Institute](https://github.com/idiap) for maintaining a [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS).
 
 - **openai**: to interact with OpenAI's TTS API
 
-- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
+- **gtts**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
```

### Comparing `RealTimeTTS-0.4.0/README.md` & `RealTimeTTS-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.4.0 (added GTTS engine)
+Latest Version: v0.4.1 
+- switched coquiengine to [Idiap Research Institute](https://github.com/idiap)'s maintained [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS) (thank you)
+- added emotions to Azure engine
+- added speed to GTTS engine
+- bugfix for ElevenlabsEngine get_voices method
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -249,27 +253,29 @@
   
 - **PyAudio**: to create an output audio stream
   
 - **stream2sentence**: to split the incoming text stream into sentences 
 
 - **pyttsx3**: System text-to-speech conversion engine
 
-- **tqdm (>=4.66.2)**: to display progress bars in the command line
+- **tqdm**: to display progress bars in the command line
 
-- **pydub (>=0.25.1)**: to convert audio chunk formats
+- **pydub**: to convert audio chunk formats
 
 - **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
 - **elevenlabs**: Elevenlabs text-to-speech conversion engine
 
-- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+- **coqui-TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+  Shoutout to [Idiap Research Institute](https://github.com/idiap) for maintaining a [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS).
 
 - **openai**: to interact with OpenAI's TTS API
 
-- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
+- **gtts**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
```

### Comparing `RealTimeTTS-0.4.0/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.4.1/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.4.0
+Version: 0.4.1
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.3
 Requires-Dist: PyAudio==0.2.14
 Requires-Dist: pyttsx3==2.90
 Requires-Dist: stream2sentence==0.2.3
-Requires-Dist: azure-cognitiveservices-speech==1.36.0
+Requires-Dist: azure-cognitiveservices-speech==1.37.0
 Requires-Dist: elevenlabs==1.2.2
-Requires-Dist: TTS==0.22.0
-Requires-Dist: tqdm==4.66.2
+Requires-Dist: tqdm==4.66.4
 Requires-Dist: pydub==0.25.1
-Requires-Dist: openai==1.13.3
+Requires-Dist: openai==1.30.5
 Requires-Dist: gtts==2.5.1
+Requires-Dist: coqui_tts==0.24.1
 
 # RealtimeTTS
 
 *Easy to use, low-latency text-to-speech library for realtime applications*
 
 ## About the Project
 
@@ -53,15 +53,19 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.4.0 (added GTTS engine)
+Latest Version: v0.4.1 
+- switched coquiengine to [Idiap Research Institute](https://github.com/idiap)'s maintained [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS) (thank you)
+- added emotions to Azure engine
+- added speed to GTTS engine
+- bugfix for ElevenlabsEngine get_voices method
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -274,27 +278,29 @@
   
 - **PyAudio**: to create an output audio stream
   
 - **stream2sentence**: to split the incoming text stream into sentences 
 
 - **pyttsx3**: System text-to-speech conversion engine
 
-- **tqdm (>=4.66.2)**: to display progress bars in the command line
+- **tqdm**: to display progress bars in the command line
 
-- **pydub (>=0.25.1)**: to convert audio chunk formats
+- **pydub**: to convert audio chunk formats
 
 - **azure-cognitiveservices-speech**: Azure text-to-speech conversion engine
   
 - **elevenlabs**: Elevenlabs text-to-speech conversion engine
 
-- **TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+- **coqui-TTS**: Coqui's XTTS text-to-speech library for high-quality local neural TTS
+
+  Shoutout to [Idiap Research Institute](https://github.com/idiap) for maintaining a [fork of coqui tts](https://github.com/idiap/coqui-ai-TTS).
 
 - **openai**: to interact with OpenAI's TTS API
 
-- **gtts (>=2.5.1)**: Google translate text-to-speech conversion
+- **gtts**: Google translate text-to-speech conversion
 
 
 ## Configuration
 
 ### Initialization Parameters for `TextToAudioStream`
 
 When you initialize the `TextToAudioStream` class, you have various options to customize its behavior. Here are the available parameters:
```

### Comparing `RealTimeTTS-0.4.0/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.4.1/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/azure_engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,18 +44,18 @@
         # Extracts the language from the locale string
         end_index = locale.find("-")
         return locale[:end_index]
 
 
 class AzureEngine(BaseEngine):
 
-    def __init__(self, 
+    def __init__(self,
                  speech_key: str = "", 
                  service_region: str = "", 
-                 voice: str = "en-US-AshleyNeural", 
+                 voice: str = "en-US-AshleyNeural",
                  rate: float = 0.0,
                  pitch: float = 0.0):
         """
         Initializes an azure voice realtime text to speech engine object.
 
         Args:
             speech_key (str): Azure subscription key. (TTS API key)
@@ -67,14 +67,38 @@
 
         self.speech_key = speech_key
         self.service_region = service_region
         self.language = voice[:5]
         self.voice_name = voice
         self.rate = rate
         self.pitch = pitch
+        self.emotion = "neutral"
+        self.emotion_degree = 1.0
+        self.emotion_role = "YoungAdultFemale"
+        self.emotion_roles = [
+            "Girl",
+            "Boy",
+            "YoungAdultFemale",
+            "YoungAdultMale",
+            "OlderAdultFemale",
+            "OlderAdultMale",
+            "SeniorFemale",
+            "SeniorMale"
+        ]
+        self.emotions = [
+            "advertisement_upbeat", "affectionate", "angry", "assistant",
+            "calm", "chat", "cheerful", "customerservice", "depressed",
+            "disgruntled", "documentary-narration", "embarrassed",
+            "empathetic", "envious", "excited", "fearful", "friendly",
+            "gentle", "hopeful", "lyrical", "narration-professional",
+            "narration-relaxed", "neutral", "newscast", "newscast-casual",
+            "newscast-formal", "poetry-reading", "sad", "serious", "shouting",
+            "sports_commentary", "sports_commentary_excited", "whispering",
+            "terrified", "unfriendly"
+        ]
 
     def post_init(self):
         self.engine_name = "azure"
 
     def get_stream_info(self):
         """
         Returns the PyAudio stream configuration information suitable for Azure Engine.
@@ -99,21 +123,28 @@
         # Set up the Azure TTS configuration
         speech_config = tts.SpeechConfig(subscription=self.speech_key, region=self.service_region)
         stream_callback = PushAudioOutputStreamSampleCallback(self.queue)
         push_stream = tts.audio.PushAudioOutputStream(stream_callback)
         stream_config = tts.audio.AudioOutputConfig(stream=push_stream)
         speech_synthesizer = tts.SpeechSynthesizer(speech_config=speech_config, audio_config=stream_config)
 
-        # Construct the SSML string
+        emotion_start_tag = f'<mstts:express-as style="{self.emotion}" styledegree="{self.emotion_degree}" role="{self.emotion_role}">'
+        emotion_end_tag = "</mstts:express-as>"
+        if self.emotion not in self.emotions or self.emotion == "neutral":
+            emotion_start_tag = ""
+            emotion_end_tag = ""
+
         ssml_string = f"""
-        <speak version="1.0" xmlns="http://www.w3.org/2001/10/synthesis" xml:lang="{self.language}">
+        <speak version="1.0" xmlns="http://www.w3.org/2001/10/synthesis" xmlns:mstts="https://www.w3.org/2001/mstts" xml:lang="{self.language}">
             <voice name="{self.voice_name}">
-                <prosody rate="{self.rate}%" pitch="{self.pitch}%">
-                    {text}
-                </prosody>
+                {emotion_start_tag}
+                    <prosody rate="{self.rate}%" pitch="{self.pitch}%">
+                        {text}
+                    </prosody>
+                {emotion_end_tag}
             </voice>
         </speak>
         """
 
         logging.debug(f"SSML:\n{ssml_string}")
 
         # Convert the SSML to audio stream
@@ -129,15 +160,43 @@
             print("SSLM:")
             print(ssml_string)
             if cancellation_details.reason == tts.CancellationReason.Error:
                 print("Error details: {}".format(cancellation_details.error_details))        
         else:
             print(f"Speech synthesis failed: {result.reason}")
             print(f"Result: {result}")
-        
+
+    def set_emotion(
+            self,
+            emotion: str,
+            emotion_role: str = "YoungAdultFemale",
+            emotion_degree: float = 1.0,
+            ):
+        """
+        Sets the emotion to be used for speech synthesis.
+
+        Args:
+            emotion (str): The emotion to be used for speech synthesis.
+            emotion_degree (float, optional): The degree of the emotion. Defaults to 1.0.
+            emotion_role (str, optional): The role of the emotion. Defaults to "YoungAdultFemale".
+        """
+        # https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-synthesis-markup-voice
+        self.emotion = emotion
+        self.emotion_degree = emotion_degree
+        self.emotion_role = emotion_role
+
+    def get_emotions(self):
+        """
+        Retrieves the available emotions for the Azure Speech engine.
+
+        Returns:
+            list[str]: A list containing the available emotions for the Azure Speech engine.
+        """
+        return self.emotions
+
     def set_speech_key(self, speech_key: str):
         """
         Sets the azure subscription key. 
 
         Args:
             speech_key (str): Azure subscription key. (TTS API key)
         """
```

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/coqui_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,21 +508,21 @@
 
         ready_event.set()
 
         logging.info('Coqui text to speech synthesize model initialized successfully')
 
         try:
             while True:
-                message = conn.recv()  
+                message = conn.recv()
                 command = message['command']
                 data = message['data']
 
                 if command == 'update_reference':
                     new_wav_path = data['cloning_reference_wav']
-                    logging.info(f'Updating reference WAV to {new_wav_path}')                    
+                    logging.info(f'Updating reference WAV to {new_wav_path}')
                     gpt_cond_latent, speaker_embedding = get_conditioning_latents(new_wav_path, tts)
                     conn.send(('success', 'Reference updated successfully'))
 
                 elif command == 'set_speed':
                     speed = data['speed']
                     conn.send(('success', 'Speed updated successfully'))
 
@@ -540,15 +540,14 @@
                 elif command == 'synthesize':
 
                     text = data['text']
                     language = data['language']
 
                     logging.debug(f'Starting inference for text: {text}')
 
-                    print(f"XTTS Synthesizing: {text}")
                     time_start = time.time()
                     seconds_to_first_chunk = 0.0
                     full_generated_seconds = 0.0
                     raw_inference_start = 0.0
                     first_chunk_length_seconds = 0.0
 
                     chunks = tts.inference_stream(
@@ -604,23 +603,14 @@
 
                     if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
 
                         realtime_factor = seconds / full_generated_seconds
                         raw_inference_time = seconds - seconds_to_first_chunk
                         raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
 
-                        # print(
-                        #     f"XTTS synthesized {full_generated_seconds:.2f}s"
-                        #     f" audio in {seconds:.2f}s"
-                        #     f" realtime factor: {realtime_factor:.2f}x"
-                        # )
-                        # print(
-                        #     f"seconds to first chunk: {seconds_to_first_chunk:.2f}s"
-                        #     f" raw_inference_factor: {raw_inference_factor:.2f}x"
-                        # )
 
                     # Send silent audio
                     sample_rate = config.audio.sample_rate
 
                     end_sentence_delimeters = ".!?…。¡¿"
                     mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
 
@@ -948,12 +938,16 @@
             local_models_path = self.local_models_path
         else:
             local_models_path = os.path.join(
                 os.getcwd(), 'models', f'{self.specific_model}')
 
         speaker_file_path = os.path.join(
             local_models_path, "speakers_xtts.pth")
+        if not os.path.exists(speaker_file_path):
+            speaker_file_path = os.path.join(
+                local_models_path, self.specific_model, "speakers_xtts.pth")
+
         speaker_manager = SpeakerManager(speaker_file_path)
         self.voices_list = []
         for speaker_name in speaker_manager.name_to_id:
             self.voices_list.append(speaker_name)
         return self.voices_list
```

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,20 +219,29 @@
 
         Note:
             This method relies on the `voices()` function to obtain the raw voice data. Ensure that the 
             `voices()` function is accessible and functional before calling this method.
         """
         fetched_voices = self.client.voices.get_all()
 
+        voices_list = fetched_voices.voices
+
         voice_objects = []
-        for voice in fetched_voices:
-            voice_object = ElevenlabsVoice(voice.name, voice.voice_id, voice.category, voice.description, voice.labels)
+        for voice in voices_list:
+            voice_object = ElevenlabsVoice(
+                name=voice.name,
+                voice_id=voice.voice_id,
+                category=voice.category,
+                description=voice.description,
+                labels=voice.labels
+            )
             voice_objects.append(voice_object)
+
         return voice_objects
-    
+
     def set_voice(self, voice: Union[str, ElevenlabsVoice]):
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, ElevenlabsVoice]): The voice to be used for speech synthesis.
         """
```

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/gtts_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/gtts_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,28 @@
 from gtts import gTTS
 import gtts.lang
 
 SYNTHESIS_FILE = 'gtts_speech_synthesis.wav'
 
 
 class GTTSVoice:
-    def __init__(self, language: str, tld: str = 'com'):
+    def __init__(self, 
+                 language: str = 'en',
+                 tld: str = 'com',
+                 chunk_length: int = 100,
+                 crossfade_length: int = 10,
+                 speed_increase: float = 1.0):
         self.language = language
         self.tld = tld
+        self.chunk_length = chunk_length
+        self.crossfade_length = crossfade_length
+        self.speed_increase = speed_increase
 
     def __repr__(self):
-        return f"{self.language} ({self.tld})"
+        return f"{self.language} ({self.tld}), Chunk: {self.chunk_length}, Crossfade: {self.crossfade_length}, Speedup: {self.speed_increase}"
 
 
 class GTTSEngine(BaseEngine):
     def __init__(self,
                  voice: Union[str, GTTSVoice] = GTTSVoice("en", "com"),
                  print_installed_voices: bool = False):
         """
@@ -60,20 +68,29 @@
 
         Args:
             text (str): Text to synthesize.
         """
         try:
             # Generate audio with gTTS
             with io.BytesIO() as f:
-                tts = gTTS(text=text, lang=self.language, tld=self.tld)
+                tts = gTTS(
+                    text=text,
+                    lang=self.voice.language,
+                    tld=self.voice.tld)
                 tts.write_to_fp(f)
                 f.seek(0)
-                # Load the audio into Pydub
+                
                 audio = AudioSegment.from_file(f, format="mp3")
-                # Export as WAV
+
+                if self.voice.speed_increase != 1.0:
+                    audio = audio.speedup(
+                        playback_speed=self.voice.speed_increase,
+                        chunk_size=self.voice.chunk_length,
+                        crossfade=self.voice.crossfade_length)
+
                 audio.export(self.file_path, format="wav")
 
             # Now open the WAV file and read the chunks
             with wave.open(self.file_path, 'rb') as wf:
                 audio_data = wf.readframes(wf.getnframes())
                 self.queue.put(audio_data)
                 return True
@@ -103,12 +120,10 @@
         """
         Sets the voice to be used for speech synthesis.
 
         Args:
             voice (Union[str, GTTSVoice]): The voice to be used for speech synthesis.
         """
         if isinstance(voice, GTTSVoice):
-            self.language = voice.language
-            self.tld = voice.tld
+            self.voice = voice
         else:
-            self.language = voice
-            self.tld = 'com'
+            self.voice = GTTSVoice(language=voice, tld = 'com')
```

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.4.1/RealtimeTTS/engines/system_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.4.1/RealtimeTTS/stream_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,17 @@
 
         # check for mpeg format
         pyChannels = self.config.channels
         pySampleRate = self.config.rate
         pyOutput_device_index = self.config.output_device_index
 
         if self.config.muted:
-            print("Muted mode, no opening stream")
             logging.debug("Muted mode, no opening stream")
 
         else:
-            print("Opening stream")
             if self.config.format == pyaudio.paCustomFormat:
                 pyFormat = self.pyaudio_instance.get_format_from_width(2)
                 logging.debug("Opening stream for mpeg audio chunks, "
                             f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
                             f"pySampleRate: {pySampleRate}")
             else:
                 pyFormat = self.config.format
```

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.4.1/RealtimeTTS/text_to_stream.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.4.1/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/setup.py` & `RealTimeTTS-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.4.0",
+    version="0.4.1",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.4.0/tests/test_callbacks.py` & `RealTimeTTS-0.4.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.4.0/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.4.1/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

