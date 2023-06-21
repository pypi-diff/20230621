# Comparing `tmp/abaxai-speech-client-0.1.1.tar.gz` & `tmp/abaxai-speech-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abaxai-speech-client-0.1.1.tar", last modified: Fri Mar 24 03:27:21 2023, max compression
+gzip compressed data, was "abaxai-speech-client-0.1.2.tar", last modified: Wed Jun 21 07:27:14 2023, max compression
```

## Comparing `abaxai-speech-client-0.1.1.tar` & `abaxai-speech-client-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/
--rwxrwxr-x   0 ly        (1000) ly        (1000)     1074 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.1/LICENSE
--rw-rw-r--   0 ly        (1000) ly        (1000)     3439 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/PKG-INFO
--rwxrwxr-x   0 ly        (1000) ly        (1000)     2873 2023-03-24 03:26:24.000000 abaxai-speech-client-0.1.1/README.md
--rwxrwxr-x   0 ly        (1000) ly        (1000)       85 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.1/pyproject.toml
--rwxrwxr-x   0 ly        (1000) ly        (1000)      691 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/setup.cfg
-drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/src/
-drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/src/abaxai_sdk/
--rwxrwxr-x   0 ly        (1000) ly        (1000)        0 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.1/src/abaxai_sdk/__init__.py
--rwxrwxr-x   0 ly        (1000) ly        (1000)    10309 2023-03-23 08:22:28.000000 abaxai-speech-client-0.1.1/src/abaxai_sdk/streaming.py
--rw-rw-r--   0 ly        (1000) ly        (1000)    11578 2023-03-23 09:18:05.000000 abaxai-speech-client-0.1.1/src/abaxai_sdk/transcribing.py
-drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-03-24 03:27:21.203808 abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/
--rw-rw-r--   0 ly        (1000) ly        (1000)     3439 2023-03-24 03:27:21.000000 abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/PKG-INFO
--rw-rw-r--   0 ly        (1000) ly        (1000)      320 2023-03-24 03:27:21.000000 abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ly        (1000) ly        (1000)        1 2023-03-24 03:27:21.000000 abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ly        (1000) ly        (1000)       11 2023-03-24 03:27:21.000000 abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/top_level.txt
+drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-06-21 07:27:14.639122 abaxai-speech-client-0.1.2/
+-rwxrwxr-x   0 ly        (1000) ly        (1000)     1074 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.2/LICENSE
+-rw-rw-r--   0 ly        (1000) ly        (1000)     3439 2023-06-21 07:27:14.639122 abaxai-speech-client-0.1.2/PKG-INFO
+-rwxrwxr-x   0 ly        (1000) ly        (1000)     2873 2023-03-24 03:26:24.000000 abaxai-speech-client-0.1.2/README.md
+-rwxrwxr-x   0 ly        (1000) ly        (1000)       85 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.2/pyproject.toml
+-rwxrwxr-x   0 ly        (1000) ly        (1000)      691 2023-06-21 07:27:14.639122 abaxai-speech-client-0.1.2/setup.cfg
+drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-06-21 07:27:14.635122 abaxai-speech-client-0.1.2/src/
+drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-06-21 07:27:14.635122 abaxai-speech-client-0.1.2/src/abaxai_sdk/
+-rwxrwxr-x   0 ly        (1000) ly        (1000)        0 2022-11-02 02:29:43.000000 abaxai-speech-client-0.1.2/src/abaxai_sdk/__init__.py
+-rwxrwxr-x   0 ly        (1000) ly        (1000)    10306 2023-06-21 07:25:53.000000 abaxai-speech-client-0.1.2/src/abaxai_sdk/streaming.py
+-rw-rw-r--   0 ly        (1000) ly        (1000)    11575 2023-06-21 07:26:10.000000 abaxai-speech-client-0.1.2/src/abaxai_sdk/transcribing.py
+drwxrwxr-x   0 ly        (1000) ly        (1000)        0 2023-06-21 07:27:14.639122 abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/
+-rw-rw-r--   0 ly        (1000) ly        (1000)     3439 2023-06-21 07:27:14.000000 abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ly        (1000) ly        (1000)      320 2023-06-21 07:27:14.000000 abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ly        (1000) ly        (1000)        1 2023-06-21 07:27:14.000000 abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ly        (1000) ly        (1000)       11 2023-06-21 07:27:14.000000 abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/top_level.txt
```

### Comparing `abaxai-speech-client-0.1.1/LICENSE` & `abaxai-speech-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abaxai-speech-client-0.1.1/PKG-INFO` & `abaxai-speech-client-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abaxai-speech-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python3 client to connect and use Abax.AI Speech services
 Home-page: https://github.com/ntuspeechlab/asr-client-scripts
 Author: AbaxAI Developer
 Author-email: tlvu@ntu.edu.sg
 Project-URL: Bug Tracker, https://github.com/ntuspeechlab/asr-client-scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abaxai-speech-client-0.1.1/README.md` & `abaxai-speech-client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `abaxai-speech-client-0.1.1/setup.cfg` & `abaxai-speech-client-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = abaxai-speech-client
-version = 0.1.1
+version = 0.1.2
 author = AbaxAI Developer
 author_email = tlvu@ntu.edu.sg
 description = A Python3 client to connect and use Abax.AI Speech services
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ntuspeechlab/asr-client-scripts
 project_urls =
```

### Comparing `abaxai-speech-client-0.1.1/src/abaxai_sdk/streaming.py` & `abaxai-speech-client-0.1.2/src/abaxai_sdk/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     def closed(self, code, reason=None):
         # logger.debug("Websocket closed() called with code %s and reason: %s" % (code, reason))
         self.final_hyp_queue.put(" ".join(self.final_hyps))
 
 
 class SpeechClient(WebSocketClient):
-    SPEECH_SERVER_URL = "wss://gatewayapi.speechlab.sg/client/ws/speech"
+    SPEECH_SERVER_URL = "wss://gateway.speechlab.sg/client/ws/speech"
     
     def __init__(self):
         #logger.info("Welcome to Abax.AI Speech Services!")
         pass
   
     def streaming_recognize(self, config, requests):
         encoded_content_type = urllib.parse.urlencode([("content-type", config.getContentType())])
```

### Comparing `abaxai-speech-client-0.1.1/src/abaxai_sdk/transcribing.py` & `abaxai-speech-client-0.1.2/src/abaxai_sdk/transcribing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 __version__ = "1.0.0"
 __author__  = "AISpeechlab - NTU"
 __status__  = "Release"
 __all__     = ['get_audio_length', 'send_audio', 'check_status', 'get_transcription']
 
 
 class SpeechClient(object):
-    _SPEECH_URL = 'https://gatewayapi.speechlab.sg'
+    _SPEECH_URL = 'https://gateway.speechlab.sg'
 
     def __init__(self):
         #logger.info("Welcome to Abax.AI Speech Services!")
         self.request_token = ""
         self.request_header = {'accept': 'application/json', 'Authorization': ""}
         self.request_queue = 'normal'
```

### Comparing `abaxai-speech-client-0.1.1/src/abaxai_speech_client.egg-info/PKG-INFO` & `abaxai-speech-client-0.1.2/src/abaxai_speech_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abaxai-speech-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python3 client to connect and use Abax.AI Speech services
 Home-page: https://github.com/ntuspeechlab/asr-client-scripts
 Author: AbaxAI Developer
 Author-email: tlvu@ntu.edu.sg
 Project-URL: Bug Tracker, https://github.com/ntuspeechlab/asr-client-scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

