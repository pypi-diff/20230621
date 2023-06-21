# Comparing `tmp/GmailBox-0.0.4.tar.gz` & `tmp/GmailBox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GmailBox-0.0.4.tar", last modified: Wed Jun 21 07:53:30 2023, max compression
+gzip compressed data, was "GmailBox-0.0.5.tar", last modified: Wed Jun 21 13:00:56 2023, max compression
```

## Comparing `GmailBox-0.0.4.tar` & `GmailBox-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.494401 GmailBox-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.446445 GmailBox-0.0.4/GmailBox/
--rw-rw-rw-   0        0        0     6111 2023-06-21 07:51:22.000000 GmailBox-0.0.4/GmailBox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:53:30.490404 GmailBox-0.0.4/GmailBox.egg-info/
--rw-rw-rw-   0        0        0     1409 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 07:53:30.000000 GmailBox-0.0.4/GmailBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1409 2023-06-21 07:53:30.493467 GmailBox-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 07:53:30.495401 GmailBox-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-21 07:06:58.000000 GmailBox-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:00:56.639269 GmailBox-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-21 13:00:56.581322 GmailBox-0.0.5/GmailBox/
+-rw-rw-rw-   0        0        0     5877 2023-06-21 13:00:25.000000 GmailBox-0.0.5/GmailBox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:00:56.634274 GmailBox-0.0.5/GmailBox.egg-info/
+-rw-rw-rw-   0        0        0     1409 2023-06-21 13:00:56.000000 GmailBox-0.0.5/GmailBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-21 13:00:56.000000 GmailBox-0.0.5/GmailBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:00:56.000000 GmailBox-0.0.5/GmailBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-21 13:00:56.000000 GmailBox-0.0.5/GmailBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 13:00:56.000000 GmailBox-0.0.5/GmailBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1409 2023-06-21 13:00:56.638270 GmailBox-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:00:56.639269 GmailBox-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-21 13:00:40.000000 GmailBox-0.0.5/setup.py
```

### Comparing `GmailBox-0.0.4/GmailBox/__init__.py` & `GmailBox-0.0.5/GmailBox/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,19 +113,15 @@
             emaill = re.findall(r'<(.*?)>', sender)[0]
             try:
                 sender = re.findall(r'"(.*?)"', sender)[0]
             except:
                 sender = sender.split(f'<{emaill}>')[0]
             subject = hamoo['subject']
             timee = hamoo['time']
+            message = '\n'.join([p.text for p in soup.find_all('p')])
             try:
-                 message = soup.find('table', {'class': 'inner-body'}).text.strip()
-            except:
-                 message = '\n'.join([p.text for p in soup.find_all('p')])
-            try:
-                links = soup.find('a', {'class': 'button-primary'})['href']
-                message += f'\n links : {links}'
-            except:
                  links = '\n'.join([link.get('href') for link in soup.find_all('a')])
                  message += f'\n links : {links}'
+            except:
+                pass
             end.append({'from':sender,'email':emaill,'subject':subject,'message':message,'time':timee})
         return end
```

### Comparing `GmailBox-0.0.4/GmailBox.egg-info/PKG-INFO` & `GmailBox-0.0.5/GmailBox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.4 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.5 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.4/PKG-INFO` & `GmailBox-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.4 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.5 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.4/README.md` & `GmailBox-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `GmailBox-0.0.4/setup.py` & `GmailBox-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
 	name= "GmailBox",
-	version= "0.0.4",
+	version= "0.0.5",
 	author= "Hamo",
     keywords=["gmail","mail","GmailBox","inbox"],
     install_requires=['requests','beautifulsoup4'],
     long_description=readme,
     long_description_content_type="text/markdown",
 	description= "With this library, you can create random Gmail and receive messages",
 	packages=setuptools.find_packages(),
```

