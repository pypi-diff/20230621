# Comparing `tmp/refractio-2.0.5.5.tar.gz` & `tmp/refractio-2.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.5.tar", last modified: Thu Jun 15 18:11:03 2023, max compression
+gzip compressed data, was "refractio-2.0.5.6.tar", last modified: Wed Jun 21 14:06:26 2023, max compression
```

## Comparing `refractio-2.0.5.5.tar` & `refractio-2.0.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.984468 refractio-2.0.5.5/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-15 18:11:03.984468 refractio-2.0.5.5/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-14 14:53:40.000000 refractio-2.0.5.5/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.982468 refractio-2.0.5.5/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-14 13:25:53.000000 refractio-2.0.5.5/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-15 18:10:28.000000 refractio-2.0.5.5/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16632 2023-06-15 18:10:28.000000 refractio-2.0.5.5/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.984468 refractio-2.0.5.5/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-15 18:11:03.984468 refractio-2.0.5.5/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-15 18:10:28.000000 refractio-2.0.5.5/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.134051 refractio-2.0.5.6/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-21 14:06:26.133051 refractio-2.0.5.6/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-21 14:05:47.000000 refractio-2.0.5.6/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.132051 refractio-2.0.5.6/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16632 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-21 14:05:36.000000 refractio-2.0.5.6/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-21 14:05:47.000000 refractio-2.0.5.6/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-21 14:06:26.133051 refractio-2.0.5.6/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-21 14:06:26.000000 refractio-2.0.5.6/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-21 14:06:26.134051 refractio-2.0.5.6/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-21 14:05:47.000000 refractio-2.0.5.6/setup.py
```

### Comparing `refractio-2.0.5.5/PKG-INFO` & `refractio-2.0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.5
+Version: 2.0.5.6
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.5/README.md` & `refractio-2.0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/amazons3.py` & `refractio-2.0.5.6/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/azure.py` & `refractio-2.0.5.6/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/hive.py` & `refractio-2.0.5.6/refractio/hive.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,26 @@
             print(output)
             return False
         return True
 
     def _get_connection(self, user_id):
         try:
             os.environ['USER'] = user_id
-            command = "echo '{1}' | kinit {0}".format(
-                self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
-                self.__connection_details["params"]["READER"].get("userPrincipalPassword")
-            )
             if self.__connection_details["params"]["READER"].get("kerberosEnable"):
                 print("Connecting to HIVE using Kerberos")
+                if self.__connection_details["params"]["READER"].get("keytabFilePath"):
+                    command = "kinit -kt {0} {1}".format(
+                        self.__connection_details["params"]["READER"].get("keytabFilePath"),
+                        self.__connection_details["params"]["READER"].get("userPrincipal")
+                    )
+                else:
+                    command = "echo '{1}' | kinit {0}".format(
+                        self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
+                        self.__connection_details["params"]["READER"].get("userPrincipalPassword")
+                    )
                 if Hive._run_os_level_command(command):
                     from pyhive import hive
                     os.environ["HIVE_HOSTNAME"] = self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress")
                     ssl_enabled = self.__connection_details["params"]["READER"]["ssl_enable"] if self.__connection_details["params"]["READER"].get("ssl_enable") else self.__connection_details["params"]["READER"].get("sslEnable")
                     self.con_obj = hive.connect(
                         # todo: To update the keys here, once we have the connection manager API created for refractio.
                         host=self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress"),
```

### Comparing `refractio-2.0.5.5/refractio/manager.py` & `refractio-2.0.5.6/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/mysql.py` & `refractio-2.0.5.6/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/postgres.py` & `refractio-2.0.5.6/refractio/postgres.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/refractio.py` & `refractio-2.0.5.6/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/sftp.py` & `refractio-2.0.5.6/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/snowflake.py` & `refractio-2.0.5.6/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio/sqlserver.py` & `refractio-2.0.5.6/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.6/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.5
+Version: 2.0.5.6
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.5/refractio.egg-info/requires.txt` & `refractio-2.0.5.6/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.5/setup.py` & `refractio-2.0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.5'
+VERSION = '2.0.5.6'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

