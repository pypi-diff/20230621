# Comparing `tmp/fastweixin-0.0.5.tar.gz` & `tmp/fastweixin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastweixin-0.0.5.tar", last modified: Thu Jun 16 06:54:04 2022, max compression
+gzip compressed data, was "fastweixin-0.0.6.tar", last modified: Wed Jun 21 08:16:59 2023, max compression
```

## Comparing `fastweixin-0.0.5.tar` & `fastweixin-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-06-16 06:54:04.647132 fastweixin-0.0.5/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2022-04-06 07:25:53.000000 fastweixin-0.0.5/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)      410 2022-06-16 06:54:04.646743 fastweixin-0.0.5/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      579 2022-06-16 06:53:25.000000 fastweixin-0.0.5/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-06-16 06:54:04.641942 fastweixin-0.0.5/fastweixin/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       65 2022-04-06 07:27:16.000000 fastweixin-0.0.5/fastweixin/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6452 2022-06-16 06:50:40.000000 fastweixin-0.0.5/fastweixin/fastweixin.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-06-16 06:54:04.646094 fastweixin-0.0.5/fastweixin.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      410 2022-06-16 06:54:04.000000 fastweixin-0.0.5/fastweixin.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      243 2022-06-16 06:54:04.000000 fastweixin-0.0.5/fastweixin.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2022-06-16 06:54:04.000000 fastweixin-0.0.5/fastweixin.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       17 2022-06-16 06:54:04.000000 fastweixin-0.0.5/fastweixin.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       11 2022-06-16 06:54:04.000000 fastweixin-0.0.5/fastweixin.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2022-06-16 06:54:04.647385 fastweixin-0.0.5/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      878 2022-06-16 06:52:07.000000 fastweixin-0.0.5/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-21 08:16:59.748509 fastweixin-0.0.6/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-06-21 06:19:14.000000 fastweixin-0.0.6/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      365 2023-06-21 08:16:59.748377 fastweixin-0.0.6/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      579 2023-06-21 06:19:14.000000 fastweixin-0.0.6/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-21 08:16:59.747366 fastweixin-0.0.6/fastweixin/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       65 2023-06-21 06:19:14.000000 fastweixin-0.0.6/fastweixin/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8665 2023-06-21 08:16:34.000000 fastweixin-0.0.6/fastweixin/fastweixin.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-21 08:16:59.748211 fastweixin-0.0.6/fastweixin.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      365 2023-06-21 08:16:59.000000 fastweixin-0.0.6/fastweixin.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      243 2023-06-21 08:16:59.000000 fastweixin-0.0.6/fastweixin.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-21 08:16:59.000000 fastweixin-0.0.6/fastweixin.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       29 2023-06-21 08:16:59.000000 fastweixin-0.0.6/fastweixin.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       11 2023-06-21 08:16:59.000000 fastweixin-0.0.6/fastweixin.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-21 08:16:59.748552 fastweixin-0.0.6/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      900 2023-06-21 06:45:39.000000 fastweixin-0.0.6/setup.py
```

### Comparing `fastweixin-0.0.5/LICENSE` & `fastweixin-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastweixin-0.0.5/README.md` & `fastweixin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastweixin-0.0.5/fastweixin/fastweixin.py` & `fastweixin-0.0.6/fastweixin/fastweixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
 import requests
 import hashlib
 import json
 import copy
+from lxml import etree
 
 
 def login_info(
         username: str,
         password: str,
         img_code: str = None,  # 验证码
         cookie: str = None
@@ -167,7 +168,67 @@
                 new_infraction = response2_json.get('new_infraction')
                 if new_infraction is not None:
                     try:
                         return_json.update(new_infraction[0])
                     except:
                         pass
     return return_json
+
+
+def get_function_html_decode(
+        url: str
+):
+    """
+    获取文章页的 function htmlDecode(str) 脚本内容，以提取文章相关基础信息
+    :param url:
+    :return:
+
+    user_name：公众号原始ID
+    nickname： 公众号名称
+    ct：发布时间
+    msg_title：文章标题
+    msg_source_url：原文链接地址
+    """
+    headers = {
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+        "Accept-Encoding": "gzip, deflate",
+        "Accept-Language": "zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2",
+        "Connection": "keep-alive",
+        "Host": "mp.weixin.qq.com",
+        "Sec-Fetch-Dest": "document",
+        "Sec-Fetch-Mode": "navigate",
+        "Sec-Fetch-Site": "none",
+        "Sec-Fetch-User": "?1",
+        "Upgrade-Insecure-Requests": "1",
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:109.0) Gecko/20100101 Firefox/114.0"
+    }
+    response = requests.get(
+        url=url,
+        headers=headers
+    )
+    html = etree.HTML(response.content, etree.HTMLParser())
+    scripts = html.xpath('/html/body/script/text()')
+    data = dict()
+    for script in scripts:
+        if 'htmlDecode' in script:
+            script_lines = script.split('\n')
+            for script_line in script_lines:
+                if script_line[:4] == 'var ':
+                    this_line = script_line[4:-1]
+                    if ' = ' in this_line:
+                        this_line_split = this_line.split(' = ')
+                        data_key = this_line_split[0]
+                        data_value = this_line_split[1]
+                        if data_value[:1] == '"' and data_value[-1:] == '"':
+                            data_value = data_value[1:-1]
+                        elif data_value[:1] == "'" and data_value[-1:] == "'":
+                            data_value = data_value[1:-1]
+                        else:
+                            pass
+                        data[data_key] = data_value
+                    else:
+                        pass
+                else:
+                    pass
+        else:
+            pass
+    return data
```

### Comparing `fastweixin-0.0.5/setup.py` & `fastweixin-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastweixin",
-    version="0.0.5",
+    version="0.0.6",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use weixin",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastweixin",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'requests==2.27.1',
+        'lxml==4.9.0'
     ]
 )
```

