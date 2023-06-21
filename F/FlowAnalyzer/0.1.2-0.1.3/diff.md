# Comparing `tmp/FlowAnalyzer-0.1.2.tar.gz` & `tmp/FlowAnalyzer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.1.2.tar", last modified: Tue Jun 20 05:45:56 2023, max compression
+gzip compressed data, was "FlowAnalyzer-0.1.3.tar", last modified: Tue Jun 20 17:16:19 2023, max compression
```

## Comparing `FlowAnalyzer-0.1.2.tar` & `FlowAnalyzer-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.948942 FlowAnalyzer-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.944941 FlowAnalyzer-0.1.2/FlowAnalyzer/
--rw-rw-rw-   0        0        0     6796 2023-06-20 05:45:06.000000 FlowAnalyzer-0.1.2/FlowAnalyzer/FlowAnalyzer.py
--rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.2/FlowAnalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.947441 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     6271 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6271 2023-06-20 05:45:56.948441 FlowAnalyzer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 05:45:56.948942 FlowAnalyzer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-20 05:45:55.000000 FlowAnalyzer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:19.215024 FlowAnalyzer-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:19.213025 FlowAnalyzer-0.1.3/FlowAnalyzer/
+-rw-rw-rw-   0        0        0     7182 2023-06-20 17:10:48.000000 FlowAnalyzer-0.1.3/FlowAnalyzer/FlowAnalyzer.py
+-rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.3/FlowAnalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:19.215024 FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     6271 2023-06-20 17:16:19.000000 FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-20 17:16:19.000000 FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:16:19.000000 FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 17:16:19.000000 FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6271 2023-06-20 17:16:19.215024 FlowAnalyzer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 17:16:19.215024 FlowAnalyzer-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-20 17:11:46.000000 FlowAnalyzer-0.1.3/setup.py
```

### Comparing `FlowAnalyzer-0.1.2/FlowAnalyzer/FlowAnalyzer.py` & `FlowAnalyzer-0.1.3/FlowAnalyzer/FlowAnalyzer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import gzip
 import subprocess
 from typing import Tuple
 
 
 class FlowAnalyzer:
     """FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件"""
-    
-    def __init__(self, jsonPath : str):
+
+    def __init__(self, jsonPath: str):
         """初始化FlowAnalyzer对象
 
         Parameters
         ----------
         jsonPath : str
             tshark导出的JSON文件路径
         """
@@ -28,74 +28,78 @@
         ------
         FileNotFoundError
             当JSON文件不存在时抛出异常
         ValueError
             当JSON文件内容为空时抛出异常
         """
         if not os.path.exists(self.jsonPath):
-            raise FileNotFoundError(f"您的tshark导出的JSON文件没有找到！JSON路径：%s" % self.jsonPath)
-        
+            raise FileNotFoundError(
+                f"您的tshark导出的JSON文件没有找到！JSON路径：%s" % self.jsonPath)
+
         if os.path.getsize(self.jsonPath) == 0:
             raise ValueError("您的tshark导出的JSON文件内容为空！JSON路径：%s" % self.jsonPath)
 
     def parse_http_json(self) -> Tuple[dict, list]:
         """解析JSON数据文件中的HTTP请求和响应信息
 
         Returns
         -------
         tuple
             包含请求字典和响应列表的元组
         """
         with open(self.jsonPath, "r") as f:
             data = json.load(f)
-            
+
         request, response = {}, []
         for packet in data:
             packet = packet["_source"]["layers"]
-            file_data = packet.get("tcp.reassembled.data") or packet["tcp.payload"]
+            time_epoch = packet.get("frame.time_epoch")
+            full_request = packet.get(
+                "tcp.reassembled.data") or packet["tcp.payload"]
+
             if packet.get("http.request_in"):
-                response.append({"response_num": packet["frame.number"][0], "request_in": packet["http.request_in"][0], "full_request": file_data[0]})
+                response.append({"response_num": packet["frame.number"][0], "request_in": packet["http.request_in"]
+                                [0], "full_request": full_request[0], "time_epoch": float(time_epoch[0])})
             else:
-                request[packet["frame.number"][0]] = file_data[0]
+                request[packet["frame.number"][0]] = {
+                    "full_request": full_request[0], "time_epoch": float(time_epoch[0])}
         return request, response
-    
-    def generate_http_dict_pairs(self, save_http_header=False):
+
+    def generate_http_dict_pairs(self, http_header=False, time_epoch=False):
         """生成HTTP请求和响应信息的字典对
 
         Parameters
         ----------
-        save_http_header : bool, optional
+        http_header : bool, optional
             指是否提取HTTP请求的全部，默认为False，表示只提取请求体，否则返回整个HTTP请求，如下结构：
             请求行：请求方法、请求目标和 HTTP 协议版本组成，例如 POST /login.php HTTP/1.1。
             请求头：包含了各种请求的元数据，比如 Host、Content-Length、User-Agent 等。每个请求头都由一个字段名和对应的值组成，以冒号分隔，例如 Host: 192.168.52.176。
             空行：用于分隔请求头和请求体，由两个连续的回车换行符组成。
             请求体：包含了请求的实际数据，对于 POST 请求来说，请求体通常包含表单数据或其他数据，以便发送给服务器进行处理。
-            
+        time_epoch : bool, optional
+            指是否提取HTTP请求的时间，指的是开始时间
+
         Yields
         ------
         Iterator[dict]
             包含请求和响应信息的字典迭代器
         """
         request, response = self.parse_http_json()
         for resp in response:
             frame_num = resp["response_num"]
             request_num = resp["request_in"]
-            full_request = request.get(request_num)
-            yield {
-                "response": [
-                    frame_num,
-                    self.extract_http_file_data(resp['full_request'], save_http_header)
-                ],
-                "request": [
-                    request_num,
-                    self.extract_http_file_data(full_request, save_http_header)
-                ]
-                if full_request
-                else None,
-            }
+            requ = request.get(request_num)
+            
+            dic = {"response": [frame_num, self.extract_http_file_data(resp['full_request'], http_header)]}
+            dic["request"] = [request_num, self.extract_http_file_data(requ["full_request"], http_header)] if requ else None
+
+            if time_epoch:
+                dic["response"].append(resp["time_epoch"])
+                dic["request"].append(requ["time_epoch"]) if requ else None
+            yield dic
 
     @staticmethod
     def get_json_data(filePath, display_filter):
         """获取JSON数据并保存至文件
 
         Parameters
         ----------
@@ -108,49 +112,52 @@
         -------
         str
             保存JSON数据的文件路径
         """
         # sourcery skip: use-fstring-for-formatting
         # jsonPath = os.path.join(os.path.dirname(filePath), "output.json")
         jsonPath = os.path.join(os.getcwd(), "output.json")
-        command = 'tshark -r {} -Y "{}" -T json -e http.request_in -e tcp.reassembled.data -e frame.number -e tcp.payload > {}'.format(filePath, display_filter, jsonPath)
-        proc = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        command = 'tshark -r {} -Y "{}" -T json -e http.request_in -e tcp.reassembled.data -e frame.number -e tcp.payload -e frame.time_epoch > {}'.format(
+            filePath, display_filter, jsonPath)
+        proc = subprocess.Popen(command, shell=True,
+                                stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         proc.communicate()
         return jsonPath
 
     @staticmethod
-    def extract_http_file_data(full_request, save_http_header=False):
+    def extract_http_file_data(full_request, http_header=False):
         # sourcery skip: merge-else-if-into-elif, swap-if-else-branches
         """提取HTTP请求或响应中的文件数据
 
         Parameters
         ----------
         full_request : str
             HTTP请求或响应的消息体
-        save_http_header : bool, optional
+        http_header : bool, optional
             指是否提取HTTP请求的全部，默认为False，表示只提取请求体，否则返回整个HTTP请求，如下结构：
             请求行：请求方法、请求目标和 HTTP 协议版本组成，例如 POST /login.php HTTP/1.1。
             请求头：包含了各种请求的元数据，比如 Host、Content-Length、User-Agent 等。每个请求头都由一个字段名和对应的值组成，以冒号分隔，例如 Host: 192.168.52.176。
             空行：用于分隔请求头和请求体，由两个连续的回车换行符组成。
             请求体：包含了请求的实际数据，对于 POST 请求来说，请求体通常包含表单数据或其他数据，以便发送给服务器进行处理。
 
         Returns
         -------
         bytes
             解压缩后的文件数据
         """
         full_request = bytes.fromhex(full_request)
         if not full_request.endswith(b"\r\n\r\n"):
-            if not save_http_header:
+            if not http_header:
                 num = full_request.find(b"\r\n\r\n")
                 full_request = full_request[num+4:]
         else:
-            if not save_http_header:
+            if not http_header:
                 num = full_request.find(b"\r\n\r\n")
-                full_request = re.findall(b'^\r\n\r\n.*?\r\n(.*)\r\n.*?\r\n\r\n$', full_request[num:], flags=re.DOTALL)[0]
-            full_request = re.sub(b"\r\n.{4}\r\n", b"", full_request) # 由于是多个tcp所以需要去除应该是长度的字节 不确定是不是4个字节 后期可能出现bug
-            
+                full_request = re.findall(
+                    b'^\r\n\r\n.*?\r\n(.*)\r\n.*?\r\n\r\n$', full_request[num:], flags=re.DOTALL)[0]
+            # 由于是多个tcp所以需要去除应该是长度的字节 不确定是不是4个字节 后期可能出现bug
+            full_request = re.sub(b"\r\n.{4}\r\n", b"", full_request)
+
         try:
             return gzip.decompress(full_request)
         except Exception:
             return full_request
-
```

### Comparing `FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/PKG-INFO` & `FlowAnalyzer-0.1.3/FlowAnalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.2
+Version: 0.1.3
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.2/LICENSE` & `FlowAnalyzer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.2/PKG-INFO` & `FlowAnalyzer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.2
+Version: 0.1.3
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.2/README.md` & `FlowAnalyzer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.2/setup.py` & `FlowAnalyzer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="FlowAnalyzer",
-    version="0.1.2",
+    version="0.1.3",
     description="FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件",
     author="Byxs20",
     author_email="97766819@qq.com",
     packages=find_packages(exclude=["tests", "*.egg-info"]),
     package_data={
         '': ['LICENSE', 'README.md', 'setup.py'],
     },
```

