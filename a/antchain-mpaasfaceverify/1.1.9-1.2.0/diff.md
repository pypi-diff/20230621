# Comparing `tmp/antchain_mpaasfaceverify-1.1.9.tar.gz` & `tmp/antchain_mpaasfaceverify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_mpaasfaceverify-1.1.9.tar", last modified: Wed May 18 08:49:21 2022, max compression
+gzip compressed data, was "dist/antchain_mpaasfaceverify-1.2.0.tar", last modified: Wed Jun 21 07:26:30 2023, max compression
```

## Comparing `antchain_mpaasfaceverify-1.1.9.tar` & `antchain_mpaasfaceverify-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1034 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32190 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/client.py
--rw-r--r--   0 root         (0) root         (0)    45434 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2548 2022-05-18 08:49:21.000000 antchain_mpaasfaceverify-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/antchain_sdk_mpaasfaceverify/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/antchain_sdk_mpaasfaceverify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45426 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/antchain_sdk_mpaasfaceverify/client.py
+-rw-r--r--   0 root         (0) root         (0)    69141 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/antchain_sdk_mpaasfaceverify/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-21 07:26:30.000000 antchain_mpaasfaceverify-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-21 07:26:29.000000 antchain_mpaasfaceverify-1.2.0/setup.py
```

### Comparing `antchain_mpaasfaceverify-1.1.9/LICENSE` & `antchain_mpaasfaceverify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_mpaasfaceverify-1.1.9/PKG-INFO` & `antchain_mpaasfaceverify-1.2.0/antchain_mpaasfaceverify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_mpaasfaceverify
-Version: 1.1.9
+Name: antchain-mpaasfaceverify
+Version: 1.2.0
 Summary: Ant Chain MPAASFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_mpaasfaceverify
-        pip install antchain_sdk_mpaasfaceverify
+        # Install the antchain-mpaasfaceverify
+        pip install antchain-mpaasfaceverify
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_mpaasfaceverify-1.1.9/README-CN.md` & `antchain_mpaasfaceverify-1.2.0/README-CN.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_mpaasfaceverify
-pip install antchain_sdk_mpaasfaceverify
+# 安装 antchain-mpaasfaceverify
+pip install antchain-mpaasfaceverify
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_mpaasfaceverify-1.1.9/README.md` & `antchain_mpaasfaceverify-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_mpaasfaceverify
-pip install antchain_sdk_mpaasfaceverify
+# Install the antchain-mpaasfaceverify
+pip install antchain-mpaasfaceverify
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_mpaasfaceverify-1.1.9/antchain_mpaasfaceverify.egg-info/PKG-INFO` & `antchain_mpaasfaceverify-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-mpaasfaceverify
-Version: 1.1.9
+Name: antchain_mpaasfaceverify
+Version: 1.2.0
 Summary: Ant Chain MPAASFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_mpaasfaceverify
-        pip install antchain_sdk_mpaasfaceverify
+        # Install the antchain-mpaasfaceverify
+        pip install antchain-mpaasfaceverify
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_mpaasfaceverify-1.1.9/antchain_sdk_mpaasfaceverify/client.py` & `antchain_mpaasfaceverify-1.2.0/antchain_sdk_mpaasfaceverify/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,26 +94,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
-            'ignoreSSL': runtime.ignore_ssl
+            'ignoreSSL': runtime.ignore_ssl,
+            # 单据计费信息，包括单据号和是否计费
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -130,15 +131,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.9'
+                    'sdk_version': '1.2.0',
+                    '_prod_code': 'MPAASFACEVERIFY',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -195,26 +198,27 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
-            'ignoreSSL': runtime.ignore_ssl
+            'ignoreSSL': runtime.ignore_ssl,
+            # 单据计费信息，包括单据号和是否计费
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -231,15 +235,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.9'
+                    'sdk_version': '1.2.0',
+                    '_prod_code': 'MPAASFACEVERIFY',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -265,14 +271,70 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def query_certify_analysis(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyAnalysisRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyAnalysisResponse:
+        """
+        Description: 人脸认证问题自动化排查接口
+        Summary: 人脸认证问题自动化排查接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_certify_analysis_ex(request, headers, runtime)
+
+    async def query_certify_analysis_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyAnalysisRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyAnalysisResponse:
+        """
+        Description: 人脸认证问题自动化排查接口
+        Summary: 人脸认证问题自动化排查接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_certify_analysis_ex_async(request, headers, runtime)
+
+    def query_certify_analysis_ex(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyAnalysisRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyAnalysisResponse:
+        """
+        Description: 人脸认证问题自动化排查接口
+        Summary: 人脸认证问题自动化排查接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyAnalysisResponse(),
+            self.do_request('1.0', 'antfin.mpaasfaceverify.certify.analysis.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_certify_analysis_ex_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyAnalysisRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyAnalysisResponse:
+        """
+        Description: 人脸认证问题自动化排查接口
+        Summary: 人脸认证问题自动化排查接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyAnalysisResponse(),
+            await self.do_request_async('1.0', 'antfin.mpaasfaceverify.certify.analysis.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def init_faceauth(
         self,
         request: mpaasfaceverify_models.InitFaceauthRequest,
     ) -> mpaasfaceverify_models.InitFaceauthResponse:
         """
         Description: 调用“实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: 实人认证初始化
@@ -300,30 +362,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitFaceauthResponse:
         """
         Description: 调用“实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: 实人认证初始化
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitFaceauthResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitFaceauthResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.faceauth.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_ex_async(
         self,
         request: mpaasfaceverify_models.InitFaceauthRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitFaceauthResponse:
         """
         Description: 调用“实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: 实人认证初始化
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitFaceauthResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitFaceauthResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.faceauth.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth(
         self,
         request: mpaasfaceverify_models.QueryFaceauthRequest,
     ) -> mpaasfaceverify_models.QueryFaceauthResponse:
@@ -354,30 +418,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceauthResponse:
         """
         Description: 调用“实人认证结果查询”接口可以通过zimId查询当次认证的结果
         Summary: 实人认证查询
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceauthResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceauthResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.faceauth.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_ex_async(
         self,
         request: mpaasfaceverify_models.QueryFaceauthRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceauthResponse:
         """
         Description: 调用“实人认证结果查询”接口可以通过zimId查询当次认证的结果
         Summary: 实人认证查询
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceauthResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceauthResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.faceauth.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceplus(
         self,
         request: mpaasfaceverify_models.InitFaceplusRequest,
     ) -> mpaasfaceverify_models.InitFaceplusResponse:
@@ -408,30 +474,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitFaceplusResponse:
         """
         Description: 人脸双因子认证服务端初始化
         Summary: 人脸双因子认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitFaceplusResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.faceplus.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceplus_ex_async(
         self,
         request: mpaasfaceverify_models.InitFaceplusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitFaceplusResponse:
         """
         Description: 人脸双因子认证服务端初始化
         Summary: 人脸双因子认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitFaceplusResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.faceplus.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceplus(
         self,
         request: mpaasfaceverify_models.QueryFaceplusRequest,
     ) -> mpaasfaceverify_models.QueryFaceplusResponse:
@@ -462,30 +530,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceplusResponse:
         """
         Description: 人脸双因子认证服务端查询
         Summary: 人脸双因子认证服务端查询
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceplusResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.faceplus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceplus_ex_async(
         self,
         request: mpaasfaceverify_models.QueryFaceplusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceplusResponse:
         """
         Description: 人脸双因子认证服务端查询
         Summary: 人脸双因子认证服务端查询
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceplusResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.faceplus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_file(
         self,
         request: mpaasfaceverify_models.QueryFaceauthFileRequest,
     ) -> mpaasfaceverify_models.QueryFaceauthFileResponse:
@@ -516,30 +586,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceauthFileResponse:
         """
         Description: zoloz提供具备权限控制的人脸图片获取接口，提供于支付宝会员等上游，控制数据风险
         Summary: 获取认证资料
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceauthFileResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceauthFileResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.faceauth.file.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_file_ex_async(
         self,
         request: mpaasfaceverify_models.QueryFaceauthFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.QueryFaceauthFileResponse:
         """
         Description: zoloz提供具备权限控制的人脸图片获取接口，提供于支付宝会员等上游，控制数据风险
         Summary: 获取认证资料
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.QueryFaceauthFileResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryFaceauthFileResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.faceauth.file.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def certify_servermode(
         self,
         request: mpaasfaceverify_models.CertifyServermodeRequest,
     ) -> mpaasfaceverify_models.CertifyServermodeResponse:
@@ -570,30 +642,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.CertifyServermodeResponse:
         """
         Description: 调用”实人认证核验源服务“接口，可获取权威源的人脸比对结果，认证链路不依赖客户端
         Summary: 实人认证核验源服务
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.CertifyServermodeResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.CertifyServermodeResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.servermode.certify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def certify_servermode_ex_async(
         self,
         request: mpaasfaceverify_models.CertifyServermodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.CertifyServermodeResponse:
         """
         Description: 调用”实人认证核验源服务“接口，可获取权威源的人脸比对结果，认证链路不依赖客户端
         Summary: 实人认证核验源服务
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.CertifyServermodeResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.CertifyServermodeResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.servermode.certify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_certifyrecord_realperson(
         self,
         request: mpaasfaceverify_models.InitCertifyrecordRealpersonRequest,
     ) -> mpaasfaceverify_models.InitCertifyrecordRealpersonResponse:
@@ -624,30 +698,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitCertifyrecordRealpersonResponse:
         """
         Description: 调用”实人认证单据初始化服务“接口，生成业务认证单据，返回单据号
         Summary: 实人认证单据初始化服务
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitCertifyrecordRealpersonResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitCertifyrecordRealpersonResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.certifyrecord.realperson.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_certifyrecord_realperson_ex_async(
         self,
         request: mpaasfaceverify_models.InitCertifyrecordRealpersonRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitCertifyrecordRealpersonResponse:
         """
         Description: 调用”实人认证单据初始化服务“接口，生成业务认证单据，返回单据号
         Summary: 实人认证单据初始化服务
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitCertifyrecordRealpersonResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitCertifyrecordRealpersonResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.certifyrecord.realperson.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_certifyrecord(
         self,
         request: mpaasfaceverify_models.InitCertifyrecordRequest,
     ) -> mpaasfaceverify_models.InitCertifyrecordResponse:
@@ -678,25 +754,251 @@
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitCertifyrecordResponse:
         """
         Description: 调用”认证单据初始化服务“接口，生成业务认证单据，返回单据号
         Summary: 认证单据初始化服务(无身份)
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitCertifyrecordResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitCertifyrecordResponse(),
             self.do_request('1.0', 'antfin.mpaasfaceverify.certifyrecord.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_certifyrecord_ex_async(
         self,
         request: mpaasfaceverify_models.InitCertifyrecordRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> mpaasfaceverify_models.InitCertifyrecordResponse:
         """
         Description: 调用”认证单据初始化服务“接口，生成业务认证单据，返回单据号
         Summary: 认证单据初始化服务(无身份)
         """
         UtilClient.validate_model(request)
-        return mpaasfaceverify_models.InitCertifyrecordResponse().from_map(
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitCertifyrecordResponse(),
             await self.do_request_async('1.0', 'antfin.mpaasfaceverify.certifyrecord.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_certifyrecord(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordResponse:
+        """
+        Description: 调用“实人认证结果查询(certifyId)”接口可以通过certifyId查询当次认证的结果
+        Summary: 实人认证查询(certifyId)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_certifyrecord_ex(request, headers, runtime)
+
+    async def query_certifyrecord_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordResponse:
+        """
+        Description: 调用“实人认证结果查询(certifyId)”接口可以通过certifyId查询当次认证的结果
+        Summary: 实人认证查询(certifyId)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_certifyrecord_ex_async(request, headers, runtime)
+
+    def query_certifyrecord_ex(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordResponse:
+        """
+        Description: 调用“实人认证结果查询(certifyId)”接口可以通过certifyId查询当次认证的结果
+        Summary: 实人认证查询(certifyId)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyrecordResponse(),
+            self.do_request('1.0', 'antfin.mpaasfaceverify.certifyrecord.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_certifyrecord_ex_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordResponse:
+        """
+        Description: 调用“实人认证结果查询(certifyId)”接口可以通过certifyId查询当次认证的结果
+        Summary: 实人认证查询(certifyId)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyrecordResponse(),
+            await self.do_request_async('1.0', 'antfin.mpaasfaceverify.certifyrecord.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_ocr_servermode(
+        self,
+        request: mpaasfaceverify_models.UploadOcrServermodeRequest,
+    ) -> mpaasfaceverify_models.UploadOcrServermodeResponse:
+        """
+        Description: 调用”纯服务端OCR数据上传“接口，存储OCR数据，返回计费单据号
+        Summary: OCR数据上传接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_ocr_servermode_ex(request, headers, runtime)
+
+    async def upload_ocr_servermode_async(
+        self,
+        request: mpaasfaceverify_models.UploadOcrServermodeRequest,
+    ) -> mpaasfaceverify_models.UploadOcrServermodeResponse:
+        """
+        Description: 调用”纯服务端OCR数据上传“接口，存储OCR数据，返回计费单据号
+        Summary: OCR数据上传接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_ocr_servermode_ex_async(request, headers, runtime)
+
+    def upload_ocr_servermode_ex(
+        self,
+        request: mpaasfaceverify_models.UploadOcrServermodeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.UploadOcrServermodeResponse:
+        """
+        Description: 调用”纯服务端OCR数据上传“接口，存储OCR数据，返回计费单据号
+        Summary: OCR数据上传接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.UploadOcrServermodeResponse(),
+            self.do_request('1.0', 'antfin.mpaasfaceverify.ocr.servermode.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_ocr_servermode_ex_async(
+        self,
+        request: mpaasfaceverify_models.UploadOcrServermodeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.UploadOcrServermodeResponse:
+        """
+        Description: 调用”纯服务端OCR数据上传“接口，存储OCR数据，返回计费单据号
+        Summary: OCR数据上传接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.UploadOcrServermodeResponse(),
+            await self.do_request_async('1.0', 'antfin.mpaasfaceverify.ocr.servermode.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_certifyrecord_charge(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordChargeRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordChargeResponse:
+        """
+        Description: 调用“计费信息查询”接口可以通过certifyId查询当次认证的计费信息，并且支持批量certifyId查询
+        Summary: 计费信息查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_certifyrecord_charge_ex(request, headers, runtime)
+
+    async def query_certifyrecord_charge_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordChargeRequest,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordChargeResponse:
+        """
+        Description: 调用“计费信息查询”接口可以通过certifyId查询当次认证的计费信息，并且支持批量certifyId查询
+        Summary: 计费信息查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_certifyrecord_charge_ex_async(request, headers, runtime)
+
+    def query_certifyrecord_charge_ex(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordChargeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordChargeResponse:
+        """
+        Description: 调用“计费信息查询”接口可以通过certifyId查询当次认证的计费信息，并且支持批量certifyId查询
+        Summary: 计费信息查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyrecordChargeResponse(),
+            self.do_request('1.0', 'antfin.mpaasfaceverify.certifyrecord.charge.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_certifyrecord_charge_ex_async(
+        self,
+        request: mpaasfaceverify_models.QueryCertifyrecordChargeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.QueryCertifyrecordChargeResponse:
+        """
+        Description: 调用“计费信息查询”接口可以通过certifyId查询当次认证的计费信息，并且支持批量certifyId查询
+        Summary: 计费信息查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.QueryCertifyrecordChargeResponse(),
+            await self.do_request_async('1.0', 'antfin.mpaasfaceverify.certifyrecord.charge.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def init_onelogin(
+        self,
+        request: mpaasfaceverify_models.InitOneloginRequest,
+    ) -> mpaasfaceverify_models.InitOneloginResponse:
+        """
+        Description: 调用”一键登录初始化服务“接口，生成业务认证单据，返回单据号
+        Summary: 一键登录初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_onelogin_ex(request, headers, runtime)
+
+    async def init_onelogin_async(
+        self,
+        request: mpaasfaceverify_models.InitOneloginRequest,
+    ) -> mpaasfaceverify_models.InitOneloginResponse:
+        """
+        Description: 调用”一键登录初始化服务“接口，生成业务认证单据，返回单据号
+        Summary: 一键登录初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_onelogin_ex_async(request, headers, runtime)
+
+    def init_onelogin_ex(
+        self,
+        request: mpaasfaceverify_models.InitOneloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.InitOneloginResponse:
+        """
+        Description: 调用”一键登录初始化服务“接口，生成业务认证单据，返回单据号
+        Summary: 一键登录初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitOneloginResponse(),
+            self.do_request('1.0', 'antfin.mpaasfaceverify.onelogin.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_onelogin_ex_async(
+        self,
+        request: mpaasfaceverify_models.InitOneloginRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mpaasfaceverify_models.InitOneloginResponse:
+        """
+        Description: 调用”一键登录初始化服务“接口，生成业务认证单据，返回单据号
+        Summary: 一键登录初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mpaasfaceverify_models.InitOneloginResponse(),
+            await self.do_request_async('1.0', 'antfin.mpaasfaceverify.onelogin.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_mpaasfaceverify-1.1.9/setup.py` & `antchain_mpaasfaceverify-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_mpaasfaceverify.
 
-Created on 18/05/2022
+Created on 21/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_mpaasfaceverify"
 NAME = "antchain_mpaasfaceverify" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain MPAASFACEVERIFY SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

