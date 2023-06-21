# Comparing `tmp/p-ttauto-crawler-0.0.9.tar.gz` & `tmp/p-ttauto-crawler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.9.tar", last modified: Mon Apr 17 03:50:15 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.1.0.tar", last modified: Wed Jun 21 05:12:29 2023, max compression
```

## Comparing `p-ttauto-crawler-0.0.9.tar` & `p-ttauto-crawler-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.529398 p-ttauto-crawler-0.0.9/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      397 2023-04-17 03:50:15.528397 p-ttauto-crawler-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.524398 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 03:50:15.000000 p-ttauto-crawler-0.0.9/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 03:50:15.529398 p-ttauto-crawler-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-04-17 03:49:54.000000 p-ttauto-crawler-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.526398 p-ttauto-crawler-0.0.9/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:50:15.527398 p-ttauto-crawler-0.0.9/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0    16773 2023-04-17 03:49:47.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0    10733 2023-04-17 03:37:59.000000 p-ttauto-crawler-0.0.9/ttauto_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.742390 p-ttauto-crawler-0.1.0/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-06-21 05:12:29.742390 p-ttauto-crawler-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.726390 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 05:12:29.000000 p-ttauto-crawler-0.1.0/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:12:29.743391 p-ttauto-crawler-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-06-20 10:32:11.000000 p-ttauto-crawler-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.740391 p-ttauto-crawler-0.1.0/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/__init__.py
+-rw-rw-rw-   0        0        0     9462 2023-06-21 05:10:39.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/auto_crawler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:12:29.741390 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-06-21 02:38:00.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0      711 2023-04-01 07:26:14.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/bin/print_md5.py
+-rw-rw-rw-   0        0        0     4084 2023-06-21 05:12:20.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/binary.py
+-rw-rw-rw-   0        0        0    10986 2023-06-20 10:58:46.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/downloader.py
+-rw-rw-rw-   0        0        0     2041 2023-06-20 03:32:56.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0     4058 2023-06-20 03:44:32.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/mecord_downloader.py
+-rw-rw-rw-   0        0        0     9064 2023-06-21 05:10:22.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/processing.py
+-rw-rw-rw-   0        0        0     3934 2023-06-20 07:22:50.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/task.py
+-rw-rw-rw-   0        0        0     2208 2023-06-21 04:26:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/ttsUtils.py
+-rw-rw-rw-   0        0        0    10318 2023-06-21 05:10:31.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/txt2proj.py
+-rw-rw-rw-   0        0        0     2926 2023-06-20 08:53:22.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/uploading.py
+-rw-rw-rw-   0        0        0    10914 2023-06-20 08:47:18.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/utils.py
+-rw-rw-rw-   0        0        0     4537 2023-06-20 09:30:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/video_merge.py
+-rw-rw-rw-   0        0        0     7846 2023-06-20 06:23:09.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/video_random_cutter.py
+-rw-rw-rw-   0        0        0     1247 2023-05-12 13:00:44.000000 p-ttauto-crawler-0.1.0/ttauto_crawler/ytdlp_downloader.py
```

### Comparing `p-ttauto-crawler-0.0.9/LICENSE` & `p-ttauto-crawler-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.9/setup.py` & `p-ttauto-crawler-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.0.9",
+    version="0.1.0",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -18,16 +18,20 @@
     ],
     py_modules=[],
     install_requires=[
         'requests',
         'oss2',
         'Image',
         'Pillow',
-        'p-template-generator',
-        'fake_useragent'
+        'p-template-generator>=0.1.67',
+        'fake_useragent',
+        'mutagen',
+        'yt-dlp==2023.3.4',
+        'moviepy',
+        'urlparser'
     ],
     dependency_links=[],
     entry_points={
         'console_scripts':[
             'ttauto_crawler = ttauto_crawler.main:main'
         ]
     },
```

### Comparing `p-ttauto-crawler-0.0.9/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.1.0/ttauto_crawler/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,171 +4,100 @@
 import time
 import oss2
 import http.client
 import json
 import logging
 import calendar
 from pathlib import Path
+from ttauto_crawler import binary
 import shutil
 import zipfile
 import platform
 import requests
 import hashlib
 import ftplib
 from PIL import Image
 from io import BytesIO
+from threading import Thread, current_thread, Lock
 
-def getOssResource(rootDir, url, md5, name):
-    localFile = os.path.join(rootDir, name)
-    localFileIsRemote = False
-    if os.path.exists(localFile):
-        with open(localFile, 'rb') as fp:
-                file_data = fp.read()
-        file_md5 = hashlib.md5(file_data).hexdigest()
-        if file_md5 == md5:
-            localFileIsRemote = True
-
-    if localFileIsRemote == False: #download
-        if os.path.exists(localFile):
-            os.remove(localFile)
-        s = requests.session()
-        s.headers.update({'Connection':'close'})
-        print(f"download {url} ")
-        file = s.get(url, verify=False)
-        with open(localFile, "wb") as c:
-            c.write(file.content)
-        s.close()
-        fname = name[0:name.index(".")]
-        fext = name[name.index("."):]
-        unzipDir = os.path.join(rootDir, fname)
-        if os.path.exists(unzipDir):
-            shutil.rmtree(unzipDir)
-        print(f"unzip {url} -> {unzipDir}")
-
-def updateBin(rootDir):
-    getOssResource(rootDir, "http://template-m.2tianxin.com/res/ffmpeg.zip", "a9e6b05ac70f6416d5629c07793b4fcf", "ffmpeg.zip.py")
-    for root,dirs,files in os.walk(rootDir):
-        for file in files:
-            if file.find(".") <= 0:
-                continue
-            name = file[0:file.index(".")]
-            ext = file[file.index("."):]
-            if ext == ".zip.py" and os.path.exists(os.path.join(root, name)) == False:
-                print(f"unzip {os.path.join(root, name)}")
-                with zipfile.ZipFile(os.path.join(root, file), "r") as zipf:
-                    zipf.extractall(os.path.join(root, name))
-        if root != files:
-            break
-
-def videoInfo(file):
-    w = 0
-    h = 0
-    bitrate = 0
-    fps = 0
-
-    ffmpeg = ffmpegBinary()
-    command = f'{ffmpeg} -i {file}'
-    try:
-        result = subprocess.run(command, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=True)
-        str = ""
-        if result.returncode == 0:
-            str = result.stdout.decode(encoding="utf8", errors="ignore")
-        else:
-            str = result.stderr.decode(encoding="utf8", errors="ignore")
-        if str.find("yuv420p") > 0 and str.find("fps") > 0:
-            s1 = str[str.find("yuv420p"):str.find("fps")+3].replace(' ', "")
-            s1_split = s1.split(",")
-            for s1_it in s1_split:
-                s2 = s1_it
-                if s2.find("[") > 0:
-                    s2 = s2[0:s2.find("[")]
-                if s2.find("(") > 0:
-                    s2 = s2[0:s2.find("[")]
-                if s2.find("x") > 0:
-                    sizes = s2.split("x")
-                    if len(sizes) > 1:
-                        w = sizes[0]
-                        h = sizes[1]
-                if s2.find("kb/s") > 0:
-                    bitrate = s2[0:s2.find("kb/s")]
-                if s2.find("fps") > 0:
-                    fps = s2[0:s2.find("fps")]
-    except subprocess.CalledProcessError as e:
-        print("====================== process error ======================")
-        print(e)
-        print("======================      end      ======================")
-    return float(w),float(h),float(bitrate),float(fps)
-
-def ffmpegBinary():
-    binDir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "bin")
-    updateBin(binDir)
+def realCommand(cmd):
+    if sys.platform != "win32":
+        return "./" + " ".join(cmd)
+    else:
+        return cmd
+    
+def ffmpegBinary(searchPath):      
     binaryFile = ""
     if sys.platform == "win32":
-        binaryFile = os.path.join(binDir, "ffmpeg", "win", "ffmpeg.exe")
+        binaryFile = os.path.join(binary.ffmpegPath(searchPath), "win", "ffmpeg.exe")
     elif sys.platform == "linux":
         machine = platform.machine().lower()
         if machine == "x86_64" or machine == "amd64":
             machine = "amd64"
         else:
             machine = "arm64"
-        binaryFile = os.path.join(binDir, "ffmpeg", "linux", machine, "ffmpeg")
+        binaryFile = os.path.join(binary.ffmpegPath(searchPath), "linux", machine, "ffmpeg")
     elif sys.platform == "darwin":
-        binaryFile = os.path.join(binDir, "ffmpeg", "darwin", "ffmpeg")
+        binaryFile = os.path.join(binary.ffmpegPath(searchPath), "darwin", "ffmpeg")
     
     if len(binaryFile) > 0 and sys.platform != "win32":
         cmd = subprocess.Popen(f"chmod 755 {binaryFile}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         while cmd.poll() is None:
-            print(cmd.stdout.readline().rstrip().decode('utf-8'))
-        
-    return binaryFile
+            logInfo(cmd.stdout.readline().rstrip().decode('utf-8'))
+
+    if os.path.exists(binaryFile):
+        return os.path.dirname(binaryFile), os.path.basename(binaryFile)
+    else:
+        return "", ""
     
 def processMoov(file):
     tmpPath = f"{file}.mp4"
-    binary = ffmpegBinary()
-    command = f'{binary} -i {file} -movflags faststart -y {tmpPath}'
-    logging.info(f"ffmpegProcess: {command}")
+    binary_dir, binary_file = ffmpegBinary("")
+    command = [binary_file, "-i", file, "-movflags", "faststart", "-y", tmpPath]
+    command = realCommand(command)
+    logInfo(f"ffmpegProcess: {command}")
     try:
         result = subprocess.run(command, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=True)
+                                stderr=subprocess.PIPE, shell=True,cwd=binary_dir)
         if result.returncode == 0:
-            logging.info(result.stdout.decode(encoding="utf8", errors="ignore"))
+            logInfo(result.stdout.decode(encoding="utf8", errors="ignore"))
             os.remove(file)
             os.rename(tmpPath, file)
         else:
-            logging.error("====================== ffmpeg error ======================")
-            logging.error(result.stderr.decode(encoding="utf8", errors="ignore"))
-            logging.error("======================     end      ======================")
+            logInfo("====================== ffmpeg error ======================")
+            logInfo(result.stderr.decode(encoding="utf8", errors="ignore"))
+            logInfo("======================     end      ======================")
     except subprocess.CalledProcessError as e:
-        logging.error("====================== process error ======================")
-        logging.error(e)
-        logging.error("======================      end      ======================")
+        logInfo("====================== process error ======================")
+        logInfo(e)
+        logInfo("======================      end      ======================")
 
 def ffmpegTest():
     binDir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "bin")
     testImage = os.path.join(binDir, "ffmpeg", "test.jpg")
-    ffmpegProcess(f"-i {testImage}")
+    ffmpegProcess(["-i", testImage])
     
 def ffmpegProcess(args):
-    binary = ffmpegBinary()
-    command = f'{binary} {args}'
-    logging.info(f"ffmpegProcess: {command}")
+    binary_dir, binary_file = ffmpegBinary("")
+    command = [binary_file] + args
+    command = realCommand(command)
+    logInfo(f"ffmpegProcess: {command}")
     try:
         result = subprocess.run(command, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=True)
+                                stderr=subprocess.PIPE, shell=True,cwd=binary_dir)
         if result.returncode == 0:
-            logging.info(result.stdout.decode(encoding="utf8", errors="ignore"))
+            logInfo(result.stdout.decode(encoding="utf8", errors="ignore"))
         else:
-            logging.error("====================== ffmpeg error ======================")
-            logging.error(result.stderr.decode(encoding="utf8", errors="ignore"))
-            logging.error("======================     end      ======================")
+            logInfo("====================== ffmpeg error ======================")
+            logInfo(result.stderr.decode(encoding="utf8", errors="ignore"))
+            logInfo("======================     end      ======================")
     except subprocess.CalledProcessError as e:
-        logging.error("====================== process error ======================")
-        logging.error(e)
-        logging.error("======================      end      ======================")
+        logInfo("====================== process error ======================")
+        logInfo(e)
+        logInfo("======================      end      ======================")
 
 def getOssImageSize(p):
     try:
         s = requests.session()
         s.headers.update({'Connection':'close'})
         res = s.get(p)
         image = Image.open(BytesIO(res.content), "r")
@@ -201,15 +130,15 @@
         with open(file, 'rb') as f:
             ftp.storbinary(f'STOR {os.path.basename(file)}', f)
         s.append(f"ftp://192.168.50.113/video/{append_dir}{os.path.basename(file)}")
     elif os.path.isdir(file):
         for filename in os.listdir(file):
             local_file = os.path.join(file, filename)
             if os.path.isfile(local_file):
-                with open(local_file, 'rb', encoding='UTF-8') as file:
+                with open(local_file, 'rb') as file:
                     ftp.storbinary(f'STOR {filename}', file)
                 s.append(f"ftp://192.168.50.113/video/{append_dir}{filename}")
             elif os.path.isdir(local_file):
                 subdir = os.path.join(remote_dir, filename)
                 s.append(ftpUpload50(local_file, ftp, subdir))
     return s
 
@@ -249,15 +178,15 @@
         with open(file, 'rb') as f:
             ftp.storbinary(f'STOR {os.path.basename(file)}', f)
         s.append(f"http://192.168.3.220/01/video/{append_dir}{os.path.basename(file)}")
     elif os.path.isdir(file):
         for filename in os.listdir(file):
             local_file = os.path.join(file, filename)
             if os.path.isfile(local_file):
-                with open(local_file, 'rb', encoding='UTF-8') as file:
+                with open(local_file, 'rb') as file:
                     ftp.storbinary(f'STOR {filename}', file)
                 s.append(f"http://192.168.3.220/01/video/{append_dir}{filename}")
             elif os.path.isdir(local_file):
                 subdir = os.path.join(remote_dir, filename)
                 s.append(ftpUpload3(local_file, ftp, subdir))
     return s
 
@@ -279,8 +208,91 @@
     ftp.quit()
     return s
 
 def ftpUpload(file):
     try:
         return ftpUpload50(file)
     except:
-        return ftpUpload3(file)
+        return ftpUpload3(file)
+
+def largeDiskPath():
+    path = ""
+    if sys.platform == "win32":
+        disk = ["c:/","d:/","e:/","f:/","g:/","h:/","i:/","j:/","k:/","l:/","m:/","n:/","o:/","p:/"]
+        for d in disk:
+            free = 0
+            try:
+                total, used, free = shutil.disk_usage(d)
+            except:
+                continue
+            if free > 0:
+                freeGB = free / 1024.0 / 1024.0 / 1024.0
+                if freeGB > 400:
+                    path = d
+                    break
+        if len(path) <= 0:
+            path = os.path.dirname(os.path.abspath(__file__))
+    elif sys.platform == "linux":
+        return "/home"
+    elif sys.platform == "darwin":
+        return "/"
+    if len(path) <= 0:
+        return ""
+    dir = os.path.join(path, "ttauto_crawler_file")
+    if os.path.exists(dir) == False:
+        os.makedirs(dir)
+    return dir
+
+def videoInfo(file):
+    w = 0
+    h = 0
+    bitrate = 0
+    fps = 0
+    duration = 0
+
+    binary_dir, binary_file = ffmpegBinary("")
+    command = [binary_file, "-i", file]
+    command = realCommand(command)
+    try:
+        result = subprocess.run(command, stdout=subprocess.PIPE,
+                                stderr=subprocess.PIPE, shell=True,cwd=binary_dir)
+        str = ""
+        if result.returncode == 0:
+            str = result.stdout.decode(encoding="utf8", errors="ignore")
+        else:
+            str = result.stderr.decode(encoding="utf8", errors="ignore")
+        if str.find("yuv420p") > 0 and str.find("fps") > 0:
+            s1 = str[str.find("yuv420p"):str.find("fps")+3].replace(' ', "")
+            s1_split = s1.split(",")
+            for s1_it in s1_split:
+                s2 = s1_it
+                if s2.find("[") > 0:
+                    s2 = s2[0:s2.find("[")]
+                if s2.find("(") > 0:
+                    s2 = s2[0:s2.find("[")]
+                if s2.find("x") > 0:
+                    sizes = s2.split("x")
+                    if len(sizes) > 1:
+                        w = sizes[0]
+                        h = sizes[1]
+                if s2.find("kb/s") > 0:
+                    bitrate = s2[0:s2.find("kb/s")]
+                if s2.find("fps") > 0:
+                    fps = s2[0:s2.find("fps")]
+        if str.find("Duration:") > 0 and str.find(", start:") > 0:
+            s2 = str[str.find("Duration:")+9:str.find(", start:")].replace(' ', "")
+            s2_split = s2.split(":")
+            if len(s2_split) > 2:
+                hour = float(s2_split[0])
+                min = float(s2_split[1])
+                second  = float(s2_split[2])
+                duration = hour*3600 + min*60 + second
+    except subprocess.CalledProcessError as e:
+        logInfo("====================== process error ======================")
+        logInfo(e)
+        logInfo("======================      end      ======================")
+    return float(w),float(h),float(bitrate),float(fps),float(duration)
+
+def logInfo(s, slient=True):
+    logging.info(f"{current_thread().name} {s}")
+    if slient:
+        print(f"{current_thread().name} {s}")
```

