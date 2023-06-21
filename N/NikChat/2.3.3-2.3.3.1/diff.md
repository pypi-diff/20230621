# Comparing `tmp/NikChat-2.3.3.tar.gz` & `tmp/NikChat-2.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.3.3.tar", last modified: Wed Jun 21 20:35:11 2023, max compression
+gzip compressed data, was "NikChat-2.3.3.1.tar", last modified: Wed Jun 21 20:53:25 2023, max compression
```

## Comparing `NikChat-2.3.3.tar` & `NikChat-2.3.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.061278 NikChat-2.3.3/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.034357 NikChat-2.3.3/NikChat/
--rw-rw-rw-   0        0        0     6570 2023-06-21 20:34:09.000000 NikChat-2.3.3/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.3/NikChat/results.py
--rw-rw-rw-   0        0        0     4658 2023-06-19 23:24:28.000000 NikChat-2.3.3/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:35:11.059284 NikChat-2.3.3/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1658 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:35:10.000000 NikChat-2.3.3/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1658 2023-06-21 20:35:11.061278 NikChat-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.3/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      633 2023-06-21 20:35:11.063274 NikChat-2.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.128629 NikChat-2.3.3.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.3.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.093961 NikChat-2.3.3.1/NikChat/
+-rw-rw-rw-   0        0        0     6368 2023-06-21 20:51:51.000000 NikChat-2.3.3.1/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-21 20:52:17.000000 NikChat-2.3.3.1/NikChat/results.py
+-rw-rw-rw-   0        0        0     4658 2023-06-21 20:52:30.000000 NikChat-2.3.3.1/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-21 20:53:25.124140 NikChat-2.3.3.1/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1660 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 20:53:25.000000 NikChat-2.3.3.1/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1660 2023-06-21 20:53:25.128629 NikChat-2.3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.3.1/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2023-06-21 20:53:25.131626 NikChat-2.3.3.1/setup.cfg
```

### Comparing `NikChat-2.3.3/LICENSE` & `NikChat-2.3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3/NikChat/__init__.py` & `NikChat-2.3.3.1/NikChat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 from textblob import TextBlob
 from nltk.stem import WordNetLemmatizer
 from tensorflow.keras.models import load_model
 from NikChat.results import ctime, weather, internet
 
 def DChat(input):
     try:
-        nltk.download('punkt')
-        nltk.download('wordnet')
+        #nltk.download('punkt')
+        #nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
         intents = json.loads(x.text)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
         json.dumps(intents, "training.json")
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
-            sentence_words = nltk.word_tokenize(sentence)
-            sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
-            return sentence_words
+            idk = TextBlob(str(sentence))
+            return idk.correct()
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
             bag = [0] * len(words)
             for w in sentence_words:
                 for i, word in enumerate(words):
                     if word == w:
                         bag[i] = 1
@@ -93,27 +92,26 @@
         traning.init()
         return 'done'
     else:
         return 'done'
 
 def NChat(filePath, input):
     try:
-        nltk.download('punkt')
-        nltk.download('wordnet')
+        #nltk.download('punkt')
+        #nltk.download('wordnet')
         lemmatizer = WordNetLemmatizer()
         intents = {}
         with open(filePath, 'r') as f:
             intents = json.load(f)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
-            sentence_words = nltk.word_tokenize(sentence)
-            sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
-            return sentence_words
+            idk = TextBlob(str(sentence))
+            return idk.correct()
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
             bag = [0] * len(words)
             for w in sentence_words:
                 for i, word in enumerate(words):
                     if word == w:
                         bag[i] = 1
```

### Comparing `NikChat-2.3.3/NikChat/results.py` & `NikChat-2.3.3.1/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3/NikChat/training.py` & `NikChat-2.3.3.1/NikChat/training.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3/NikChat.egg-info/PKG-INFO` & `NikChat-2.3.3.1/NikChat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.3
+Version: 2.3.3.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3.3/PKG-INFO` & `NikChat-2.3.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.3
+Version: 2.3.3.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3.3/README.md` & `NikChat-2.3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.3/setup.cfg` & `NikChat-2.3.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 332e 330d 0a61 7574  ion = 2.3.3..aut
-00000030: 686f 7220 3d20 4e69 6b68 696c 2054 616d  hor = Nikhil Tam
-00000040: 7661 6461 2028 4e69 6b68 696c 6f64 656f  vada (Nikhilodeo
-00000050: 6e31 290d 0a61 7574 686f 725f 656d 6169  n1)..author_emai
-00000060: 6c20 3d20 6e69 6b68 696c 7461 6d76 6164  l = nikhiltamvad
-00000070: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
-00000080: 6372 6970 7469 6f6e 203d 2041 2066 756c  cription = A ful
-00000090: 6c2d 666c 6564 6765 6420 6368 6174 626f  l-fledged chatbo
-000000a0: 7420 6465 7369 676e 6564 2074 6f20 6265  t designed to be
-000000b0: 2069 6e63 6f72 7065 7261 7465 6420 696e   incorperated in
-000000c0: 746f 206f 7468 6572 2070 726f 6a65 6374  to other project
-000000d0: 732e 2028 5370 6565 6473 206f 6620 302e  s. (Speeds of 0.
-000000e0: 3120 7365 636f 6e64 7329 0d0a 6c6f 6e67  1 seconds)..long
-000000f0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000100: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000120: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000130: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a68  text/markdown..h
-00000140: 6f6d 655f 7061 6765 203d 2068 7474 7073  ome_page = https
-00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e69  ://github.com/Ni
-00000160: 6b68 696c 6f64 656f 6e31 2f4e 696b 4368  khilodeon1/NikCh
-00000170: 6174 0d0a 636c 6173 7369 6669 6572 7320  at..classifiers 
-00000180: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-00000190: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001a0: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
-000001b0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-000001c0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-000001d0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-000001e0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001f0: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-00000200: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-00000210: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000220: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-00000230: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000240: 6461 7461 203d 2054 7275 650d 0a0d 0a5b  data = True....[
-00000250: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000260: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000270: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000020: 696f 6e20 3d20 322e 332e 332e 310d 0a61  ion = 2.3.3.1..a
+00000030: 7574 686f 7220 3d20 4e69 6b68 696c 2054  uthor = Nikhil T
+00000040: 616d 7661 6461 2028 4e69 6b68 696c 6f64  amvada (Nikhilod
+00000050: 656f 6e31 290d 0a61 7574 686f 725f 656d  eon1)..author_em
+00000060: 6169 6c20 3d20 6e69 6b68 696c 7461 6d76  ail = nikhiltamv
+00000070: 6164 6140 676d 6169 6c2e 636f 6d0d 0a64  ada@gmail.com..d
+00000080: 6573 6372 6970 7469 6f6e 203d 2041 2066  escription = A f
+00000090: 756c 6c2d 666c 6564 6765 6420 6368 6174  ull-fledged chat
+000000a0: 626f 7420 6465 7369 676e 6564 2074 6f20  bot designed to 
+000000b0: 6265 2069 6e63 6f72 7065 7261 7465 6420  be incorperated 
+000000c0: 696e 746f 206f 7468 6572 2070 726f 6a65  into other proje
+000000d0: 6374 732e 2028 5370 6565 6473 206f 6620  cts. (Speeds of 
+000000e0: 302e 3120 7365 636f 6e64 7329 0d0a 6c6f  0.1 seconds)..lo
+000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000100: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+00000110: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000120: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000130: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+00000140: 0a68 6f6d 655f 7061 6765 203d 2068 7474  .home_page = htt
+00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000160: 4e69 6b68 696c 6f64 656f 6e31 2f4e 696b  Nikhilodeon1/Nik
+00000170: 4368 6174 0d0a 636c 6173 7369 6669 6572  Chat..classifier
+00000180: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001a0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
+000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001d0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
+000001e0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001f0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
+00000200: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
+00000210: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000220: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
+00000230: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000240: 655f 6461 7461 203d 2054 7275 650d 0a0d  e_data = True...
+00000250: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000260: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000270: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

