# Comparing `tmp/antchain_mpaasfaceverify-1.1.8.tar.gz` & `tmp/antchain_mpaasfaceverify-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_mpaasfaceverify-1.1.8.tar", last modified: Wed May 18 06:13:21 2022, max compression
+gzip compressed data, was "dist/antchain_mpaasfaceverify-1.1.9.tar", last modified: Wed May 18 08:49:21 2022, max compression
```

## Comparing `antchain_mpaasfaceverify-1.1.8.tar` & `antchain_mpaasfaceverify-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1034 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32190 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/client.py
--rw-r--r--   0 root         (0) root         (0)    44862 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2548 2022-05-18 06:13:21.000000 antchain_mpaasfaceverify-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1034 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32190 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/client.py
+-rw-r--r--   0 root         (0) root         (0)    45434 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2548 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/setup.py
```

### Comparing `antchain_mpaasfaceverify-1.1.8/LICENSE` & `antchain_mpaasfaceverify-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_mpaasfaceverify-1.1.8/PKG-INFO` & `antchain_mpaasfaceverify-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_mpaasfaceverify
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ant Chain MPAASFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mpaasfaceverify-1.1.8/README-CN.md` & `antchain_mpaasfaceverify-1.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_mpaasfaceverify-1.1.8/README.md` & `antchain_mpaasfaceverify-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_mpaasfaceverify-1.1.8/antchain_mpaasfaceverify.egg-info/PKG-INFO` & `antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-mpaasfaceverify
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ant Chain MPAASFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/client.py` & `antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.8'
+                    'sdk_version': '1.1.9'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -231,15 +231,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.8'
+                    'sdk_version': '1.1.9'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
```

### Comparing `antchain_mpaasfaceverify-1.1.8/antchain_sdk_mpaasfaceverify/models.py` & `antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -992,14 +992,15 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         extern_info: str = None,
         result_code_sub: str = None,
         result_msg_sub: str = None,
         certify_id: str = None,
+        certify_url: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -1007,14 +1008,16 @@
         self.extern_info = extern_info
         # 产品结果明细，不影响决策
         self.result_code_sub = result_code_sub
         # result_code_sub对应的文案
         self.result_msg_sub = result_msg_sub
         # 认证单据号
         self.certify_id = certify_id
+        # 认证h5 url
+        self.certify_url = certify_url
 
     def validate(self):
         pass
 
     def to_map(self):
         result = dict()
         if self.req_msg_id is not None:
@@ -1027,14 +1030,16 @@
             result['extern_info'] = self.extern_info
         if self.result_code_sub is not None:
             result['result_code_sub'] = self.result_code_sub
         if self.result_msg_sub is not None:
             result['result_msg_sub'] = self.result_msg_sub
         if self.certify_id is not None:
             result['certify_id'] = self.certify_id
+        if self.certify_url is not None:
+            result['certify_url'] = self.certify_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -1045,14 +1050,16 @@
             self.extern_info = m.get('extern_info')
         if m.get('result_code_sub') is not None:
             self.result_code_sub = m.get('result_code_sub')
         if m.get('result_msg_sub') is not None:
             self.result_msg_sub = m.get('result_msg_sub')
         if m.get('certify_id') is not None:
             self.certify_id = m.get('certify_id')
+        if m.get('certify_url') is not None:
+            self.certify_url = m.get('certify_url')
         return self
 
 
 class InitCertifyrecordRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -1135,14 +1142,15 @@
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         extern_info: str = None,
         result_code_sub: str = None,
         result_msg_sub: str = None,
         certify_id: str = None,
+        certify_url: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -1150,14 +1158,16 @@
         self.extern_info = extern_info
         # 产品结果明细，不影响决策
         self.result_code_sub = result_code_sub
         # result_code_sub对应的文案
         self.result_msg_sub = result_msg_sub
         # 认证单据号
         self.certify_id = certify_id
+        # 认证h5 url
+        self.certify_url = certify_url
 
     def validate(self):
         pass
 
     def to_map(self):
         result = dict()
         if self.req_msg_id is not None:
@@ -1170,14 +1180,16 @@
             result['extern_info'] = self.extern_info
         if self.result_code_sub is not None:
             result['result_code_sub'] = self.result_code_sub
         if self.result_msg_sub is not None:
             result['result_msg_sub'] = self.result_msg_sub
         if self.certify_id is not None:
             result['certify_id'] = self.certify_id
+        if self.certify_url is not None:
+            result['certify_url'] = self.certify_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -1188,10 +1200,12 @@
             self.extern_info = m.get('extern_info')
         if m.get('result_code_sub') is not None:
             self.result_code_sub = m.get('result_code_sub')
         if m.get('result_msg_sub') is not None:
             self.result_msg_sub = m.get('result_msg_sub')
         if m.get('certify_id') is not None:
             self.certify_id = m.get('certify_id')
+        if m.get('certify_url') is not None:
+            self.certify_url = m.get('certify_url')
         return self
```

### Comparing `antchain_mpaasfaceverify-1.1.8/setup.py` & `antchain_mpaasfaceverify-1.1.9/setup.py`

 * *Files identical despite different names*

