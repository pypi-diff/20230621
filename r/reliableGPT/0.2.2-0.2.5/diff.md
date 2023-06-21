# Comparing `tmp/reliableGPT-0.2.2.tar.gz` & `tmp/reliableGPT-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.2.tar", last modified: Wed Jun 21 01:31:15 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.5.tar", last modified: Wed Jun 21 05:31:31 2023, max compression
```

## Comparing `reliableGPT-0.2.2.tar` & `reliableGPT-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 01:31:15.484804 reliableGPT-0.2.2/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.2/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 01:31:15.484701 reliableGPT-0.2.2/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.2/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 01:31:15.484279 reliableGPT-0.2.2/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 01:31:15.000000 reliableGPT-0.2.2/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 01:31:15.000000 reliableGPT-0.2.2/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 01:31:15.000000 reliableGPT-0.2.2/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 01:31:15.000000 reliableGPT-0.2.2/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 01:31:15.000000 reliableGPT-0.2.2/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 01:31:15.484573 reliableGPT-0.2.2/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.2/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7371 2023-06-21 01:30:39.000000 reliableGPT-0.2.2/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3905 2023-06-21 01:23:52.000000 reliableGPT-0.2.2/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 01:31:15.484838 reliableGPT-0.2.2/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 01:30:58.000000 reliableGPT-0.2.2/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 05:31:31.735675 reliableGPT-0.2.5/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.5/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 05:31:31.735578 reliableGPT-0.2.5/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.2.5/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 05:31:31.735020 reliableGPT-0.2.5/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-21 05:31:31.000000 reliableGPT-0.2.5/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-21 05:31:31.000000 reliableGPT-0.2.5/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-21 05:31:31.000000 reliableGPT-0.2.5/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       32 2023-06-21 05:31:31.000000 reliableGPT-0.2.5/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-21 05:31:31.000000 reliableGPT-0.2.5/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-21 05:31:31.735340 reliableGPT-0.2.5/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.5/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7452 2023-06-21 05:30:08.000000 reliableGPT-0.2.5/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3905 2023-06-21 01:23:52.000000 reliableGPT-0.2.5/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-21 05:31:31.735713 reliableGPT-0.2.5/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      312 2023-06-21 05:30:48.000000 reliableGPT-0.2.5/setup.py
```

### Comparing `reliableGPT-0.2.2/LICENSE` & `reliableGPT-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.2/README.md` & `reliableGPT-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.2/reliablegpt/main.py` & `reliableGPT-0.2.5/reliablegpt/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 import openai
+from termcolor import colored
 import time
 import functools
 import copy
 import requests
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 def make_LLM_request(new_kwargs):
     try:
         model = new_kwargs['model']
         if "3.5" or "4" in model: # call ChatCompletion
-            print(f"ReliableGPT: Retrying request with model CHAT {model}")
+            print(colored(f"ReliableGPT: Retrying request with model CHAT {model}", "blue"))
             return openai.ChatCompletion.create(**new_kwargs)
         else:
-            print(f"ReliableGPT: Retrying request with model TEXT {model}")
+            print(colored(f"ReliableGPT: Retrying request with model TEXT {model}", "blue"))
             new_kwargs['prompt'] = " ".join([message["content"] for message in new_kwargs['messages']])
             new_kwargs.pop('messages', None) # remove messages for completion models 
             return openai.Completion.create(**new_kwargs)
     except Exception as e:
-        print(f"ReliableGPT: Got 2nd AGAIN Error {e}")
+        print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
         return None
     return None
 
 def fallback_request(args, kwargs, fallback_strategy):
     result = None
     for model in fallback_strategy:
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
         result = make_LLM_request(new_kwargs)
         if result != None:
             return result    
     return None
 
 def api_key_handler(args, kwargs, fallback_strategy, user_email, user_token):
-    print(f"ReliableGPT: in API key handler")
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
     response = requests.get(url)
     if response.status_code == 200:
         result = response.json()
-        print(f"ReliableGPT: in API key handler: Got new fallbacks")
+        if result['status'] == 'failed':
+            print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
+            return None
+
         fallback_keys = result['response']['openai_api_keys'] # list of fallback keys
         if len(fallback_keys) == 0:
-            print(f"ReliableGPT: in API key handler: Got 0 new fallbacks")
             return None
         for fallback_key in fallback_keys:
             openai.api_key = fallback_key
-            print(f"ReliableGPT: in API key handler: trying fallback with {fallback_key}")
             result = make_LLM_request(kwargs)
-            print(f"ReliableGPT: in API key handler: trying fallback with {fallback_key} {result}")
             if result != None:
                 return result
+    else:
+        print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
     return None
 
+
 def handle_openAI_error(args, kwargs, openAI_error, fallback_strategy, graceful_string, user_email="", user_token=""):
     # Error Types from https://platform.openai.com/docs/guides/error-codes/python-library-error-types
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
     # 4. APIConnectionError - Check your network settings, proxy configuration, SSL certificates, or firewall rules.
     # 5. InvalidRequestError - User input was bad: context_length_exceeded, 
     # 6. AuthenticationError - API key not working, return default hardcoded message
     # 7. ServiceUnavailableError - retry, retry with fallback
     error_type = openAI_error['type']
     if error_type == 'invalid_request_error' or error_type == 'InvalidRequestError':
         # check if this is context window related, try with a 16k model
         if openAI_error.code == 'context_length_exceeded':
-            print("ReliableGPT: invalid request error - context_length_exceeded")
+            print(colored("ReliableGPT: invalid request error - context_length_exceeded", "red"))
             fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
             result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
             if result == None:
                 return graceful_string
             else:
                 return result
         if openAI_error.code == "invalid_api_key":
-            print("ReliableGPT: invalid request error - invalid_api_key")
+            print(colored("ReliableGPT: invalid request error - invalid_api_key", "red"))
             result = api_key_handler(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, user_email=user_email, user_token=user_token)
             if result == None:
                 return graceful_string
             else:
                 return result
 
     # todo: alert on user_email that there is now an auth error 
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
-        print("ReliableGPT: Auth error")
+        print(colored("ReliableGPT: Auth error", "red"))
         return graceful_string
 
     # catch all 
     result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
     if result == None:
         return graceful_string
     else:
@@ -109,27 +112,27 @@
     def __call__(self, *args, **kwargs):
         try:
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
             return result
         except Exception as e:
             try:
-                print(f"ReliableGPT: Error Response from openai.ChatCompletion.create()")
-                print(f"ReliableGPT: Got Exception {e}", 'red')
+                print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
+                print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
                 result = handle_openAI_error(
                     args = args,
                     kwargs = kwargs,
                     openAI_error = e.error,
                     fallback_strategy = self.fallback_strategy,
                     graceful_string = self.graceful_string,
                     user_email = self.user_email,
                     user_token=self.user_token
                 )
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e.error, 'recovered_response': result})
-                print(f"ReliableGPT: Recoverd got a successfull response {result}")
+                print(colored(f"ReliableGPT: Recoverd got a successfull response {result}", "green"))
                 return result
             except:
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': self.graceful_string})
                 return self.graceful_string
 
 
 def add_keys(user_email="", keys=[]):
```

### Comparing `reliableGPT-0.2.2/reliablegpt/tests.py` & `reliableGPT-0.2.5/reliablegpt/tests.py`

 * *Files identical despite different names*

