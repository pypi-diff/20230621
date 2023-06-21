# Comparing `tmp/reliableGPT-0.2.0.tar.gz` & `tmp/reliableGPT-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.0.tar", last modified: Wed Jun 21 00:49:10 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.1.tar", last modified: Wed Jun 21 00:58:31 2023, max compression
```

## Comparing `reliableGPT-0.2.0.tar` & `reliableGPT-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001815 reliableGPT-0.2.0/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:49:10.001724 reliableGPT-0.2.0/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001027 reliableGPT-0.2.0/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 00:49:09.000000 reliableGPT-0.2.0/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:49:10.001448 reliableGPT-0.2.0/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.0/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7201 2023-06-21 00:44:15.000000 reliableGPT-0.2.0/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3469 2023-06-21 00:43:23.000000 reliableGPT-0.2.0/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 00:49:10.001845 reliableGPT-0.2.0/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 00:48:53.000000 reliableGPT-0.2.0/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:58:31.255046 reliableGPT-0.2.1/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.1/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:58:31.254947 reliableGPT-0.2.1/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.1/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:58:31.254507 reliableGPT-0.2.1/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 00:58:31.000000 reliableGPT-0.2.1/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 00:58:31.000000 reliableGPT-0.2.1/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 00:58:31.000000 reliableGPT-0.2.1/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 00:58:31.000000 reliableGPT-0.2.1/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 00:58:31.000000 reliableGPT-0.2.1/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 00:58:31.254794 reliableGPT-0.2.1/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.1/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7162 2023-06-21 00:54:46.000000 reliableGPT-0.2.1/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3469 2023-06-21 00:43:23.000000 reliableGPT-0.2.1/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 00:58:31.255091 reliableGPT-0.2.1/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 00:56:38.000000 reliableGPT-0.2.1/setup.py
```

### Comparing `reliableGPT-0.2.0/LICENSE` & `reliableGPT-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.0/README.md` & `reliableGPT-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.0/reliablegpt/main.py` & `reliableGPT-0.2.1/reliablegpt/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,20 +90,20 @@
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
 class reliableGPT:
-    def __init__(self, openai_create_function, fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], graceful_string="Sorry, the OpenAI API is currently down", account_email="", account_token=""):
+    def __init__(self, openai_create_function, fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], graceful_string="Sorry, the OpenAI API is currently down", user_email="", user_token=""):
         self.openai_create_function = openai_create_function
         self.graceful_string = graceful_string
         self.fallback_strategy = fallback_strategy
-        self.user_email = account_email
-        self.user_token = account_token
+        self.user_email = user_email
+        self.user_token = user_token
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
     def __call__(self, *args, **kwargs):
         try:
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
@@ -125,31 +125,31 @@
                 print(colored(f"ReliableGPT: Recoverd got a successfull response {result}", "green"))
                 return result
             except:
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': self.graceful_string})
                 return self.graceful_string
 
 
-def add_keys(account_email="", keys=[]):
+def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
-    if account_email == "":
+    if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
     if len(keys) == 0:
         return "reliableGPT: Please add keys to add"
-    payload = {"user_email": account_email}
+    payload = {"user_email": user_email}
     for idx, key in enumerate(keys):
         key_name = "key_" + str(idx+1)
         payload[key_name] = key
     response = requests.get(url, params=payload)
     return response.json()
 
-def delete_keys(account_email, account_token):
+def delete_keys(user_email, user_token):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/delete_keys"
-    if account_email == "":
+    if user_email == "":
         return "reliableGPT: Please add an Email to delete your keys"
-    if account_token == "":
+    if user_email == "":
         return "reliableGPT: Please add an account_token to delete your keys"
-    payload = {"user_email": account_email, "user_token": account_token}
+    payload = {"user_email": user_email, "user_token": user_token}
     response = requests.get(url, params=payload)
     return response.json()
```

### Comparing `reliableGPT-0.2.0/reliablegpt/tests.py` & `reliableGPT-0.2.1/reliablegpt/tests.py`

 * *Files identical despite different names*

