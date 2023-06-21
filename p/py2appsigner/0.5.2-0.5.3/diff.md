# Comparing `tmp/py2appsigner-0.5.2.tar.gz` & `tmp/py2appsigner-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2appsigner-0.5.2.tar", last modified: Tue Jun 20 03:07:28 2023, max compression
+gzip compressed data, was "py2appsigner-0.5.3.tar", last modified: Wed Jun 21 17:13:56 2023, max compression
```

## Comparing `py2appsigner-0.5.2.tar` & `py2appsigner-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682803 py2appsigner-0.5.2/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.2/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-20 03:07:28.682672 py2appsigner-0.5.2/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.2/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.680960 py2appsigner-0.5.2/py2appsigner/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.2/py2appsigner/ApplicationNotarize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6785 2023-06-19 21:47:06.000000 py2appsigner-0.5.2/py2appsigner/ApplicationSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/ApplicationStaple.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/ApplicationVerify.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-06-04 22:47:50.000000 py2appsigner-0.5.2/py2appsigner/BaseCommand.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.2/py2appsigner/CommandBasic.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/CommandExtended.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10033 2023-06-04 23:39:53.000000 py2appsigner-0.5.2/py2appsigner/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.2/py2appsigner/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.2/py2appsigner/Notary.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6225 2023-06-03 20:22:37.000000 py2appsigner-0.5.2/py2appsigner/ZipSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.2/py2appsigner/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-06-20 02:48:04.000000 py2appsigner-0.5.2/py2appsigner/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682230 py2appsigner-0.5.2/py2appsigner/environment/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.2/py2appsigner/environment/BasicEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.2/py2appsigner/environment/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.2/py2appsigner/environment/NotaryEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.2/py2appsigner/environment/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682455 py2appsigner-0.5.2/py2appsigner/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.2/py2appsigner/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.2/py2appsigner/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.681783 py2appsigner-0.5.2/py2appsigner.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-20 03:07:28.682837 py2appsigner-0.5.2/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.2/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-21 17:13:56.990612 py2appsigner-0.5.3/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.3/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-21 17:13:56.990472 py2appsigner-0.5.3/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.3/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-21 17:13:56.988691 py2appsigner-0.5.3/py2appsigner/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.3/py2appsigner/ApplicationNotarize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6785 2023-06-20 03:51:13.000000 py2appsigner-0.5.3/py2appsigner/ApplicationSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.3/py2appsigner/ApplicationStaple.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.3/py2appsigner/ApplicationVerify.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1222 2023-06-20 13:59:01.000000 py2appsigner-0.5.3/py2appsigner/BaseCommand.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.3/py2appsigner/CommandBasic.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      826 2023-06-20 03:50:35.000000 py2appsigner-0.5.3/py2appsigner/CommandExtended.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10133 2023-06-20 13:48:46.000000 py2appsigner-0.5.3/py2appsigner/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.3/py2appsigner/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.3/py2appsigner/Notary.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6233 2023-06-20 03:49:22.000000 py2appsigner-0.5.3/py2appsigner/ZipSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.3/py2appsigner/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-06-20 03:53:02.000000 py2appsigner-0.5.3/py2appsigner/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-21 17:13:56.990021 py2appsigner-0.5.3/py2appsigner/environment/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.3/py2appsigner/environment/BasicEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.3/py2appsigner/environment/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.3/py2appsigner/environment/NotaryEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.3/py2appsigner/environment/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-21 17:13:56.990209 py2appsigner-0.5.3/py2appsigner/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.3/py2appsigner/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.3/py2appsigner/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-21 17:13:56.989529 py2appsigner-0.5.3/py2appsigner.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-21 17:13:56.000000 py2appsigner-0.5.3/py2appsigner.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-21 17:13:56.990650 py2appsigner-0.5.3/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.3/setup.py
```

### Comparing `py2appsigner-0.5.2/LICENSE` & `py2appsigner-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/PKG-INFO` & `py2appsigner-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.2/README.md` & `py2appsigner-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/ApplicationNotarize.py` & `py2appsigner-0.5.3/py2appsigner/ApplicationNotarize.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/ApplicationSign.py` & `py2appsigner-0.5.3/py2appsigner/ApplicationSign.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/ApplicationStaple.py` & `py2appsigner-0.5.3/py2appsigner/ApplicationStaple.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/BaseCommand.py` & `py2appsigner-0.5.3/py2appsigner/BaseCommand.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 from logging import Logger
 from logging import getLogger
+from subprocess import CalledProcessError
 
 from sys import stdout
 
 from subprocess import run as subProcessRun
 from subprocess import check_call as subProcessCheckCall
 from subprocess import STDOUT
 
+from click import ClickException
 from click import secho
 
 
 class BaseCommand:
     def __init__(self, verbose: bool = True):
 
         self._verbose: bool   = verbose
@@ -26,14 +28,17 @@
         if self._verbose is True:
             return verboseOptions
         else:
             return quietOptions
 
     def _runCommand(self,  command: str):
 
-        if self._verbose is True:
-            secho(self._execute(command=command))
-        else:
-            subProcessRun([command], shell=True, capture_output=True, text=True, check=True)
+        try:
+            if self._verbose is True:
+                secho(self._execute(command=command))
+            else:
+                subProcessRun([command], shell=True, capture_output=True, text=True, check=True)
+        except CalledProcessError as cpe:
+            raise ClickException(message=f'Fail {cpe.cmd}')
 
     def _execute(self, command):
         subProcessCheckCall(command, shell=True, stdout=stdout, stderr=STDOUT)
```

### Comparing `py2appsigner-0.5.2/py2appsigner/CommandBasic.py` & `py2appsigner-0.5.3/py2appsigner/CommandBasic.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/CommandExtended.py` & `py2appsigner-0.5.3/py2appsigner/CommandExtended.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 class CommandExtended(CommandBasic):
     def __init__(self, environment: Environment):
 
         super().__init__(environment=environment)
         self.logger: Logger = getLogger(__name__)
 
         self._extendedEnvironment: Environment = environment
-        self._pythonVersion:       str         = self._removeDecimalSeparator(self._extendedEnvironment.pythonVersion)
+        self._pythonVersion:       str         = self._extendedEnvironment.pythonVersion
+        self._flatPythonVersion:   str         = self._removeDecimalSeparator(self._extendedEnvironment.pythonVersion)
 
     @abstractmethod
     def execute(self):
         pass
 
     def _removeDecimalSeparator(self, pythonVersion: str):
         return pythonVersion.replace('.', '')
```

### Comparing `py2appsigner-0.5.2/py2appsigner/Commands.py` & `py2appsigner-0.5.3/py2appsigner/Commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,9 +226,10 @@
     # noinspection SpellCheckingInspection
     """
     py2appSign(['--python-version', '3.10', '-d', 'pyut', '--application-name', 'pyut', 'zipsign'])
     py2appSign(['--python-version', '3.10', '-d', 'pyut', '--application-name', 'pyut', 'appsign'])
     appNotarize(['-d', 'pyut', '--application-name', 'pyut', '--verbose'])
     appStaple(['-d', 'pyut', '--application-name', 'pyut', '--verbose'])
     notaryTool(['information', '-i', '5f57fc1e-23d3-42ab-b0ad-ec1d2635c4ad'])
-    """
     notaryTool(['--keychain-profile', 'NOTARY_TOOL_APP_ID', 'history'])
+    """
+    py2appSign(['--python-version', '3.11', '-d', 'pyut', '--application-name', 'pyut', 'appsign'])
```

### Comparing `py2appsigner-0.5.2/py2appsigner/Notary.py` & `py2appsigner-0.5.3/py2appsigner/Notary.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/ZipSign.py` & `py2appsigner-0.5.3/py2appsigner/ZipSign.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         self.logger.debug(f'{self._extendedEnvironment.pythonVersion=} {self._extendedEnvironment.applicationName=}')
 
         # fullPath:        str = f'{self._environment.projectsBase}/{self._environment.projectDirectory}'
         # pythonVersion:   str = self._removeDecimalSeparator(self._environment.pythonVersion)
         # applicationName: str = f'{fullPath}{BUILD_DIR}{self._environment.applicationName}.app'
 
         originalZipDir: str = f'{self._applicationName}{ZIP_DIRECTORY_SNIPPET}'
-        unzipDir:       str = f'{TMP_DIR_PATH}/python{self._pythonVersion}'
-        zipName:        str = f'python{self._pythonVersion}.zip'
+        unzipDir:       str = f'{TMP_DIR_PATH}/python{self._flatPythonVersion}'
+        zipName:        str = f'python{self._flatPythonVersion}.zip'
 
         self._cleanupTemporaryDirectory(unzipDir=unzipDir, zipName=zipName)
         self._getUnsignedZipCopy(originalZipDir=originalZipDir, zipName=zipName)
         self._unzipCopy(unzipDir=unzipDir, zipName=zipName)
         self._signLibs(unzipDir=unzipDir)
         self._removeOldUnSignedZip(zipName=zipName)
         self._recreateSignedZip(unzipDir=unzipDir, zipName=zipName)
```

### Comparing `py2appsigner-0.5.2/py2appsigner/environment/BasicEnvironment.py` & `py2appsigner-0.5.3/py2appsigner/environment/BasicEnvironment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/environment/Environment.py` & `py2appsigner-0.5.3/py2appsigner/environment/Environment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner/resources/loggingConfiguration.json` & `py2appsigner-0.5.3/py2appsigner/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/py2appsigner.egg-info/PKG-INFO` & `py2appsigner-0.5.3/py2appsigner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.2/py2appsigner.egg-info/SOURCES.txt` & `py2appsigner-0.5.3/py2appsigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.2/setup.py` & `py2appsigner-0.5.3/setup.py`

 * *Files identical despite different names*

