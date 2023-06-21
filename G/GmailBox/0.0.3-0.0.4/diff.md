# Comparing `tmp/GmailBox-0.0.3.tar.gz` & `tmp/GmailBox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GmailBox-0.0.3.tar", last modified: Sun Jun 18 05:18:24 2023, max compression
+gzip compressed data, was "GmailBox-0.0.4.tar", last modified: Wed Jun 21 07:53:30 2023, max compression
```

## Comparing `GmailBox-0.0.3.tar` & `GmailBox-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.692305 GmailBox-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.636148 GmailBox-0.0.3/GmailBox/
--rw-rw-rw-   0        0        0     5708 2023-06-18 05:04:32.000000 GmailBox-0.0.3/GmailBox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.685311 GmailBox-0.0.3/GmailBox.egg-info/
--rw-rw-rw-   0        0        0     1409 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1409 2023-06-18 05:18:24.688308 GmailBox-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 05:18:24.692305 GmailBox-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-18 05:17:01.000000 GmailBox-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.494401 GmailBox-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.446445 GmailBox-0.0.4/GmailBox/
+-rw-rw-rw-   0        0        0     6111 2023-06-21 07:51:22.000000 GmailBox-0.0.4/GmailBox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.490404 GmailBox-0.0.4/GmailBox.egg-info/
+-rw-rw-rw-   0        0        0     1409 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1409 2023-06-21 07:53:30.493467 GmailBox-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:53:30.495401 GmailBox-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-21 07:06:58.000000 GmailBox-0.0.4/setup.py
```

### Comparing `GmailBox-0.0.3/GmailBox/__init__.py` & `GmailBox-0.0.4/GmailBox/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
             'x-requested-with': 'XMLHttpRequest',
             'x-xsrf-token': f'{self.token}',
         }
 
         json_data = {
             'email': [
-                'plusGmail',
                 'dotGmail',
             ],
         }
 
         response = self.request.post('https://www.emailnator.com/generate-email', headers=headers, json=json_data).json()
         email = response['email'][0]
         return {'email':email}
@@ -114,10 +113,19 @@
             emaill = re.findall(r'<(.*?)>', sender)[0]
             try:
                 sender = re.findall(r'"(.*?)"', sender)[0]
             except:
                 sender = sender.split(f'<{emaill}>')[0]
             subject = hamoo['subject']
             timee = hamoo['time']
-            message = '\n'.join([p.text for p in soup.find_all('p')])
+            try:
+                 message = soup.find('table', {'class': 'inner-body'}).text.strip()
+            except:
+                 message = '\n'.join([p.text for p in soup.find_all('p')])
+            try:
+                links = soup.find('a', {'class': 'button-primary'})['href']
+                message += f'\n links : {links}'
+            except:
+                 links = '\n'.join([link.get('href') for link in soup.find_all('a')])
+                 message += f'\n links : {links}'
             end.append({'from':sender,'email':emaill,'subject':subject,'message':message,'time':timee})
         return end
```

### Comparing `GmailBox-0.0.3/GmailBox.egg-info/PKG-INFO` & `GmailBox-0.0.4/GmailBox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.3
+Version: 0.0.4
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.3 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.4 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.3/PKG-INFO` & `GmailBox-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.3
+Version: 0.0.4
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.3 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.4 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.3/README.md` & `GmailBox-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `GmailBox-0.0.3/setup.py` & `GmailBox-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
 	name= "GmailBox",
-	version= "0.0.3",
+	version= "0.0.4",
 	author= "Hamo",
     keywords=["gmail","mail","GmailBox","inbox"],
     install_requires=['requests','beautifulsoup4'],
     long_description=readme,
     long_description_content_type="text/markdown",
 	description= "With this library, you can create random Gmail and receive messages",
 	packages=setuptools.find_packages(),
```

