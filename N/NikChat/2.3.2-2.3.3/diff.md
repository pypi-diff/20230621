# Comparing `tmp/NikChat-2.3.2.tar.gz` & `tmp/NikChat-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.3.2.tar", last modified: Mon Jun 19 23:43:19 2023, max compression
+gzip compressed data, was "NikChat-2.3.3.tar", last modified: Wed Jun 21 20:35:11 2023, max compression
```

## Comparing `NikChat-2.3.2.tar` & `NikChat-2.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.109067 NikChat-2.3.2/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.084087 NikChat-2.3.2/NikChat/
--rw-rw-rw-   0        0        0     6738 2023-06-19 23:41:35.000000 NikChat-2.3.2/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.2/NikChat/results.py
--rw-rw-rw-   0        0        0     4658 2023-06-19 23:24:28.000000 NikChat-2.3.2/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.107095 NikChat-2.3.2/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1658 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1658 2023-06-19 23:43:19.109067 NikChat-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.2/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      633 2023-06-19 23:43:19.114782 NikChat-2.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.061278 NikChat-2.3.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.034357 NikChat-2.3.3/NikChat/
+-rw-rw-rw-   0        0        0     6570 2023-06-21 20:34:09.000000 NikChat-2.3.3/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.3/NikChat/results.py
+-rw-rw-rw-   0        0        0     4658 2023-06-19 23:24:28.000000 NikChat-2.3.3/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.059284 NikChat-2.3.3/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1658 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1658 2023-06-21 20:35:11.061278 NikChat-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.3/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      633 2023-06-21 20:35:11.063274 NikChat-2.3.3/setup.cfg
```

### Comparing `NikChat-2.3.2/LICENSE` & `NikChat-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.2/NikChat/__init__.py` & `NikChat-2.3.3/NikChat/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from os.path import exists
 import json
 import random
 import requests
 import pickle
 import numpy as np
 import nltk
+from textblob import TextBlob
 from nltk.stem import WordNetLemmatizer
 from tensorflow.keras.models import load_model
 from NikChat.results import ctime, weather, internet
 
 def DChat(input):
     try:
-        import nltk
-        #nltk.download('punkt')
-        #nltk.download('wordnet')
-        import json
-        import random
-        import requests
-        import pickle
-        import numpy as np
-        from nltk.stem import WordNetLemmatizer
-        from tensorflow.keras.models import load_model
-        from NikChat.results import ctime, weather, internet
+        nltk.download('punkt')
+        nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
         intents = json.loads(x.text)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
         json.dumps(intents, "training.json")
         model = load_model('Speechbot.h5')
@@ -36,14 +28,15 @@
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
             bag = [0] * len(words)
             for w in sentence_words:
                 for i, word in enumerate(words):
                     if word == w:
                         bag[i] = 1
+            print(np.array(bag))
             return np.array(bag)
         def predict_class(sentence):
             bow = bag_of_words(sentence)
             res = model.predict(np.array([bow]))[0]
             ERROR_TRESHOLD = 0.25
             results = [[i, r] for i, r in enumerate(res) if r > ERROR_TRESHOLD]
             results.sort(key=lambda x: x[1], reverse=True)
@@ -56,21 +49,22 @@
             list_of_intents = intents_json['intents']
             for i in list_of_intents:
                 if i['tag'] == tag:
                     result = random.choice(i['responses'])
                     break
             return result
         #print('THE BOT IS RUNNING')
-        message = input
+        idk = TextBlob(input)
+        message = idk.correct()
         ints = predict_class(message)
         res = get_response(ints, intents['record'])
         str1 = ''
         for elm in message.split(' '):
             str1 += elm.lower() + " "
-        #print(str1.split(' '))
+        print(str1.split(' '))
         if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
             res = weather()
         elif "day" in str1.split(' ') or "time" in str1.split(' ') or "date" in str1.split(' '):
             res = ctime()
         elif res == "bob is your dad":
             res = internet(str1)
         else:
@@ -99,16 +93,16 @@
         traning.init()
         return 'done'
     else:
         return 'done'
 
 def NChat(filePath, input):
     try:
-        #nltk.download('punkt')
-        #nltk.download('wordnet')
+        nltk.download('punkt')
+        nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         intents = {}
         with open(filePath, 'r') as f:
             intents = json.load(f)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
         model = load_model('Speechbot.h5')
@@ -139,15 +133,16 @@
             list_of_intents = intents_json['intents']
             for i in list_of_intents:
                 if i['tag'] == tag:
                     result = random.choice(i['responses'])
                     break
             return result
         #print('THE BOT IS RUNNING')
-        message = input
+        idk = TextBlob(input)
+        message = idk.correct()
         ints = predict_class(message)
         res = get_response(ints, intents['record'])
         str1 = ''
         for elm in message.split(' '):
             str1 += elm.lower() + " "
         #print(str1.split(' '))
         if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
@@ -161,7 +156,8 @@
         return res
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
             return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
+
```

### Comparing `NikChat-2.3.2/NikChat/results.py` & `NikChat-2.3.3/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.2/NikChat/training.py` & `NikChat-2.3.3/NikChat/training.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.2/NikChat.egg-info/PKG-INFO` & `NikChat-2.3.3/NikChat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.2
+Version: 2.3.3
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3.2/PKG-INFO` & `NikChat-2.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.2
+Version: 2.3.3
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3.2/README.md` & `NikChat-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.2/setup.cfg` & `NikChat-2.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 332e 320d 0a61 7574  ion = 2.3.2..aut
+00000020: 696f 6e20 3d20 322e 332e 330d 0a61 7574  ion = 2.3.3..aut
 00000030: 686f 7220 3d20 4e69 6b68 696c 2054 616d  hor = Nikhil Tam
 00000040: 7661 6461 2028 4e69 6b68 696c 6f64 656f  vada (Nikhilodeo
 00000050: 6e31 290d 0a61 7574 686f 725f 656d 6169  n1)..author_emai
 00000060: 6c20 3d20 6e69 6b68 696c 7461 6d76 6164  l = nikhiltamvad
 00000070: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
 00000080: 6372 6970 7469 6f6e 203d 2041 2066 756c  cription = A ful
 00000090: 6c2d 666c 6564 6765 6420 6368 6174 626f  l-fledged chatbo
```

