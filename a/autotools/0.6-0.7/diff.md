# Comparing `tmp/autotools-0.6.tar.gz` & `tmp/autotools-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotools-0.6.tar", last modified: Wed Jun 21 08:55:14 2023, max compression
+gzip compressed data, was "autotools-0.7.tar", last modified: Wed Jun 21 10:19:47 2023, max compression
```

## Comparing `autotools-0.6.tar` & `autotools-0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:55:14.820135 autotools-0.6/
--rw-rw-rw-   0        0        0      195 2023-06-21 08:55:14.820135 autotools-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 08:55:14.728340 autotools-0.6/autotools/
--rw-rw-rw-   0        0        0      157 2023-06-20 18:04:02.000000 autotools-0.6/autotools/__init__.py
--rw-rw-rw-   0        0        0     1802 2023-06-20 17:55:20.000000 autotools-0.6/autotools/audio.py
--rw-rw-rw-   0        0        0     2403 2023-06-20 18:11:14.000000 autotools-0.6/autotools/chatgpt.py
--rw-rw-rw-   0        0        0     3472 2023-06-20 18:09:15.000000 autotools-0.6/autotools/chatgpt_presets.py
--rw-rw-rw-   0        0        0     2221 2023-06-20 18:11:43.000000 autotools-0.6/autotools/chats.py
--rw-rw-rw-   0        0        0      899 2023-06-20 18:03:35.000000 autotools-0.6/autotools/img.py
--rw-rw-rw-   0        0        0     1103 2023-06-21 08:15:15.000000 autotools-0.6/autotools/module_get.py
--rw-rw-rw-   0        0        0      380 2023-06-20 17:42:44.000000 autotools-0.6/autotools/to_ipv4.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:55:14.809883 autotools-0.6/autotools.egg-info/
--rw-rw-rw-   0        0        0      195 2023-06-21 08:55:14.000000 autotools-0.6/autotools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-21 08:55:14.000000 autotools-0.6/autotools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:55:14.000000 autotools-0.6/autotools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-21 08:55:14.000000 autotools-0.6/autotools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-21 08:55:14.000000 autotools-0.6/autotools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 08:55:14.820135 autotools-0.6/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-06-21 08:55:00.000000 autotools-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:19:46.994645 autotools-0.7/
+-rw-rw-rw-   0        0        0      193 2023-06-21 10:19:46.952663 autotools-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 10:19:46.795424 autotools-0.7/autotools/
+-rw-rw-rw-   0        0        0      185 2023-06-21 09:39:24.000000 autotools-0.7/autotools/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-06-21 10:12:35.000000 autotools-0.7/autotools/audio.py
+-rw-rw-rw-   0        0        0     2393 2023-06-21 10:10:51.000000 autotools-0.7/autotools/chatgpt.py
+-rw-rw-rw-   0        0        0     3472 2023-06-20 18:09:15.000000 autotools-0.7/autotools/chatgpt_presets.py
+-rw-rw-rw-   0        0        0     2189 2023-06-21 10:07:53.000000 autotools-0.7/autotools/chats.py
+-rw-rw-rw-   0        0        0      897 2023-06-21 10:07:05.000000 autotools-0.7/autotools/img.py
+-rw-rw-rw-   0        0        0     1485 2023-06-21 10:03:49.000000 autotools-0.7/autotools/module_get.py
+-rw-rw-rw-   0        0        0      409 2023-06-21 10:03:27.000000 autotools-0.7/autotools/temp_download.py
+-rw-rw-rw-   0        0        0      380 2023-06-21 10:11:17.000000 autotools-0.7/autotools/to_ipv4.py
+drwxrwxrwx   0        0        0        0 2023-06-21 10:19:46.947572 autotools-0.7/autotools.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-06-21 10:19:45.000000 autotools-0.7/autotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-06-21 10:19:46.000000 autotools-0.7/autotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 10:19:45.000000 autotools-0.7/autotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-21 10:19:45.000000 autotools-0.7/autotools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-21 10:19:46.000000 autotools-0.7/autotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 10:19:47.007349 autotools-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-21 10:04:59.000000 autotools-0.7/setup.py
```

### Comparing `autotools-0.6/autotools/audio.py` & `autotools-0.7/autotools/audio.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     This function uses SpeechRecognition library to convert user's speech to text in Russian language.
     It initializes a Recognizer object and a Microphone object to capture the audio. Then, it waits for user's speech input.
     If the speech is successfully recognised, it returns the text. If not, it returns an empty string.
     :return: str - the recognized text
     """
     r = sr.Recognizer()
     with sr.Microphone() as source:
-        print("Говорите!")
+        print("Say something!")
         audio = r.listen(source)
     try:
         text = r.recognize_google(audio, language=language)
-        print(f"Вы сказали: {text}")
+        print(f"You said: {text}")
         return text
     except sr.UnknownValueError:
-        print("Извините, я не понял, что вы сказали.")
+        print("Google Speech Recognition could not understand audio.")
         return ''
     except sr.RequestError as e:
-        print(f"Произошла ошибка {e}")
+        print(f"Could not request results from Google Speech Recognition service {e}")
         return ''
 
 
 def string_to_speech(text: str, lang: str = 'ru') -> None:
     """
     Convert a given `text` string to speech in the specified `lang` language using Google's Text-to-Speech (gTTS) API.
     If `text` is empty, raise a `ValueError`. 
@@ -36,11 +36,11 @@
     :type text: str
     :param lang: The language in which the speech output should be generated. Default is 'ru'.
     :type lang: str
     :return: None
     :rtype: None
     """
     if not text:
-        raise ValueError('text is empty!')
+        raise ValueError('Text is empty!')
     tts = gTTS(text=text, lang=lang)
     tts.save("response.mp3")
     playsound("response.mp3")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autotools-0.6/autotools/chatgpt.py` & `autotools-0.7/autotools/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Returns:
         None.
     
     Raises:
         ValueError: If the new_temperature value is not between 0 and 1.
     """
     if 0 > new_temperature > 1:
-        raise ValueError('new_temperature must be between 0 and 1')
+        raise ValueError('New_temperature must be between 0 and 1')
 
     global temperature
     temperature = new_temperature
 
 
 def set_max_tokens(new_max_tokens: int) -> None:
     """
@@ -74,9 +74,9 @@
     - behaviour (str): The behaviour to be logged.
     
     Returns:
     - response (str): The response received using the logged data.
     """
     message_log = [{"role": "system", "content": behaviour}, {"role": "user", "content": message}]
     response = _get_response(message_log)
-    print("\n" + f"AI assistant: {response}" + "\n")
+    print("\n" + f"AI: {response}" + "\n")
     return response
```

### Comparing `autotools-0.6/autotools/chatgpt_presets.py` & `autotools-0.7/autotools/chatgpt_presets.py`

 * *Files identical despite different names*

### Comparing `autotools-0.6/autotools/chats.py` & `autotools-0.7/autotools/chats.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     """
     message_log = [
         {"role": "system", "content": behaviour}
     ]
 
     while True:
         user_input = speech_to_text()
-        if user_input.lower() == "выход":
-            print("До свидания!")
+        if user_input.lower() == "exit":
+            print("Goodbye!")
             break
         message_log.append({"role": "user", "content": user_input})
         response = _get_response(message_log)
         message_log.append({"role": "assistant", "content": response})
         string_to_speech(response)
-        print(f"ИИ: {response}")
+        print(f"AI: {response}")
 
         if 'exit' in response.lower():
             print('ChatGPT has exited the program')
             break
 
 
 def chat(behaviour: str) -> None:
@@ -59,8 +59,8 @@
             return
 
         message_log.append({"role": "user", "content": user_input})
 
         response = _get_response(message_log)
 
         message_log.append({"role": "assistant", "content": response})
-        print(f"AI assistant: {response}")
+        print(f"AI: {response}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autotools-0.6/autotools/img.py` & `autotools-0.7/autotools/img.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 
     Returns:
         None
     """
     formatted_prompt = urllib.parse.quote_plus(prompt)
     resp = requests.get('https://image.pollinations.ai/prompt/{}'.format(formatted_prompt))
     if resp.status_code != 200:
-        raise Exception('request error. try again later')
+        raise Exception('Bad request. Try again later')
     with open('img.png', 'wb') as f:
         for chunk in resp:
             f.write(chunk)
     if open_img:
         open_image('img.png').show()
```

### Comparing `autotools-0.6/setup.py` & `autotools-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 description = 'Just save your time'
-long_description = 'Simple module for realisate simple tasks'
+long_description = 'Simple module for realize simple tasks'
 
 setup(
     name='autotools',
-    version='0.6',
+    version='0.7',
     description=description,
     long_description=long_description,
     author='automatic, ebu sobak',
     author_email='',
     license='OpenSource',
     packages=['autotools'],
     install_requires=[
```

