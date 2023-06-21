# Comparing `tmp/alibabacloud_pds_sdk-1.1.6.tar.gz` & `tmp/alibabacloud_pds_sdk-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pds_sdk-1.1.6.tar", last modified: Fri Dec  2 10:30:34 2022, max compression
+gzip compressed data, was "dist/alibabacloud_pds_sdk-1.1.7.tar", last modified: Wed Jun 21 10:08:49 2023, max compression
```

## Comparing `alibabacloud_pds_sdk-1.1.6.tar` & `alibabacloud_pds_sdk-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/
--rw-r--r--   0 root         (0) root         (0)     2018 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      923 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2637462 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/client.py
--rw-r--r--   0 root         (0) root         (0)  2100424 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2018 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2580 2022-12-02 10:30:34.000000 alibabacloud_pds_sdk-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      923 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2747364 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/client.py
+-rw-r--r--   0 root         (0) root         (0)  2203289 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-06-21 10:08:49.000000 alibabacloud_pds_sdk-1.1.7/setup.py
```

### Comparing `alibabacloud_pds_sdk-1.1.6/PKG-INFO` & `alibabacloud_pds_sdk-1.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pds_sdk
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-pds-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pds_sdk-1.1.6/README.md` & `alibabacloud_pds_sdk-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/client.py` & `alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12352,14 +12352,242 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def get_facegroups_ex(
+        self,
+        request: pds_models.GetFileFaceGroupsRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetFacegroupsModel:
+        """
+        获取文件人脸分组列表
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_facegroups')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetFacegroupsModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def get_facegroups_ex_async(
+        self,
+        request: pds_models.GetFileFaceGroupsRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetFacegroupsModel:
+        """
+        获取文件人脸分组列表
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_facegroups')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetFacegroupsModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
     def get_last_cursor_ex(
         self,
         request: pds_models.GetLastCursorRequest,
         runtime: pds_models.RuntimeOptions,
     ) -> pds_models.GetLastCursorModel:
         """
         获取drive内，增量数据最新的游标
@@ -12810,14 +13038,466 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def get_media_preview_info_ex(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayInfoRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetMediaPreviewInfoModel:
+        """
+        获取媒体文件播放信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_media_preview_info')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetMediaPreviewInfoModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def get_media_preview_info_ex_async(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayInfoRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetMediaPreviewInfoModel:
+        """
+        获取媒体文件播放信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_media_preview_info')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetMediaPreviewInfoModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    def get_media_preview_meta_ex(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayMetaRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetMediaPreviewMetaModel:
+        """
+        获取媒体文件播放元信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_media_preview_meta')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetMediaPreviewMetaModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def get_media_preview_meta_ex_async(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayMetaRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetMediaPreviewMetaModel:
+        """
+        获取媒体文件播放元信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/file/get_media_preview_meta')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetMediaPreviewMetaModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
     def get_office_edit_url_ex(
         self,
         request: pds_models.GetOfficeEditUrlRequest,
         runtime: pds_models.RuntimeOptions,
     ) -> pds_models.GetOfficeEditUrlModel:
         """
         获取文档的在线编辑地址
@@ -36554,27 +37234,25 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def update_data_process_template_ex(
+    def search_user_group_ex(
         self,
-        request: pds_models.UpdateDataProcessTemplateRequest,
+        request: pds_models.SearchUserAndGroupRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.UpdateDataProcessTemplateModel:
+    ) -> pds_models.SearchUserGroupModel:
         """
-        更新用户指定的资源的数据处理模版
-        @tags user
+        该接口将会根据条件查询用户和团队，只有管理员可以调用
+        @tags user_group
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
-        @error NotFound The resource {resource_name} cannot be found. Please check.
-        @error StateConflict User operation is not valid.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
         runtime.validate()
         _runtime = {
             'timeouted': 'retry',
@@ -36612,15 +37290,15 @@
                 accesskey_id = self.get_access_key_id()
                 access_key_secret = self.get_access_key_secret()
                 security_token = self.get_security_token()
                 access_token = self.get_access_token()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/user/update_data_process_template')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/user_group/search')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -36639,15 +37317,15 @@
                 _response = TeaCore.do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = UtilClient.read_as_json(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.UpdateDataProcessTemplateModel(),
+                        pds_models.SearchUserGroupModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -36670,27 +37348,25 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    async def update_data_process_template_ex_async(
+    async def search_user_group_ex_async(
         self,
-        request: pds_models.UpdateDataProcessTemplateRequest,
+        request: pds_models.SearchUserAndGroupRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.UpdateDataProcessTemplateModel:
+    ) -> pds_models.SearchUserGroupModel:
         """
-        更新用户指定的资源的数据处理模版
-        @tags user
+        该接口将会根据条件查询用户和团队，只有管理员可以调用
+        @tags user_group
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
-        @error NotFound The resource {resource_name} cannot be found. Please check.
-        @error StateConflict User operation is not valid.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
         runtime.validate()
         _runtime = {
             'timeouted': 'retry',
@@ -36728,15 +37404,15 @@
                 accesskey_id = await self.get_access_key_id_async()
                 access_key_secret = await self.get_access_key_secret_async()
                 security_token = await self.get_security_token_async()
                 access_token = await self.get_access_token_async()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/user/update_data_process_template')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/user_group/search')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -36755,15 +37431,15 @@
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = await UtilClient.read_as_json_async(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.UpdateDataProcessTemplateModel(),
+                        pds_models.SearchUserGroupModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -36786,22 +37462,22 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def search_user_group_ex(
+    def merge_ex(
         self,
-        request: pds_models.SearchUserAndGroupRequest,
+        request: pds_models.MergeFaceGroupRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.SearchUserGroupModel:
+    ) -> pds_models.MergeModel:
         """
-        该接口将会根据条件查询用户和团队，只有管理员可以调用
-        @tags user_group
+        该接口将会对两个人脸分组进行合并
+        @tags face_group
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
@@ -36842,15 +37518,15 @@
                 accesskey_id = self.get_access_key_id()
                 access_key_secret = self.get_access_key_secret()
                 security_token = self.get_security_token()
                 access_token = self.get_access_token()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/user_group/search')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/face_group/merge')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -36869,15 +37545,15 @@
                 _response = TeaCore.do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = UtilClient.read_as_json(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.SearchUserGroupModel(),
+                        pds_models.MergeModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -36900,22 +37576,22 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    async def search_user_group_ex_async(
+    async def merge_ex_async(
         self,
-        request: pds_models.SearchUserAndGroupRequest,
+        request: pds_models.MergeFaceGroupRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.SearchUserGroupModel:
+    ) -> pds_models.MergeModel:
         """
-        该接口将会根据条件查询用户和团队，只有管理员可以调用
-        @tags user_group
+        该接口将会对两个人脸分组进行合并
+        @tags face_group
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
@@ -36956,15 +37632,15 @@
                 accesskey_id = await self.get_access_key_id_async()
                 access_key_secret = await self.get_access_key_secret_async()
                 security_token = await self.get_security_token_async()
                 access_token = await self.get_access_token_async()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/user_group/search')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/face_group/merge')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -36983,15 +37659,15 @@
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = await UtilClient.read_as_json_async(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.SearchUserGroupModel(),
+                        pds_models.MergeModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -37014,22 +37690,22 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def merge_ex(
+    def unassign_facegroup_item_ex(
         self,
-        request: pds_models.MergeFaceGroupRequest,
+        request: pds_models.UnAssignFaceGroupItemRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.MergeModel:
+    ) -> pds_models.UnassignFacegroupItemModel:
         """
-        该接口将会对两个人脸分组进行合并
-        @tags face_group
+        该接口将会对移除人脸分组中指定的图片
+        @tags albums
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
@@ -37070,15 +37746,239 @@
                 accesskey_id = self.get_access_key_id()
                 access_key_secret = self.get_access_key_secret()
                 security_token = self.get_security_token()
                 access_token = self.get_access_token()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/face_group/merge')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/unassign_facegroup_item')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 204):
+                    return TeaCore.from_map(
+                        pds_models.UnassignFacegroupItemModel(),
+                        {
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def unassign_facegroup_item_ex_async(
+        self,
+        request: pds_models.UnAssignFaceGroupItemRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.UnassignFacegroupItemModel:
+        """
+        该接口将会对移除人脸分组中指定的图片
+        @tags albums
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/unassign_facegroup_item')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 204):
+                    return TeaCore.from_map(
+                        pds_models.UnassignFacegroupItemModel(),
+                        {
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    def get_data_process_template_ex(
+        self,
+        request: pds_models.GetDriveDataProcessTemplateRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetDataProcessTemplateModel:
+        """
+        获取 drive 的数据处理模版
+        @tags drive
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/drive/get_data_process_template')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -37097,15 +37997,15 @@
                 _response = TeaCore.do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = UtilClient.read_as_json(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.MergeModel(),
+                        pds_models.GetDataProcessTemplateModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -37128,25 +38028,27 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    async def merge_ex_async(
+    async def get_data_process_template_ex_async(
         self,
-        request: pds_models.MergeFaceGroupRequest,
+        request: pds_models.GetDriveDataProcessTemplateRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.MergeModel:
+    ) -> pds_models.GetDataProcessTemplateModel:
         """
-        该接口将会对两个人脸分组进行合并
-        @tags face_group
+        获取 drive 的数据处理模版
+        @tags drive
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
         runtime.validate()
         _runtime = {
             'timeouted': 'retry',
@@ -37184,15 +38086,15 @@
                 accesskey_id = await self.get_access_key_id_async()
                 access_key_secret = await self.get_access_key_secret_async()
                 security_token = await self.get_security_token_async()
                 access_token = await self.get_access_token_async()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/face_group/merge')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/drive/get_data_process_template')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -37211,15 +38113,15 @@
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = await UtilClient.read_as_json_async(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.MergeModel(),
+                        pds_models.GetDataProcessTemplateModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -37242,25 +38144,27 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def unassign_facegroup_item_ex(
+    def update_data_process_template_ex(
         self,
-        request: pds_models.UnAssignFaceGroupItemRequest,
+        request: pds_models.UpdateDriveDataProcessTemplateRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.UnassignFacegroupItemModel:
+    ) -> pds_models.UpdateDataProcessTemplateModel:
         """
-        该接口将会对移除人脸分组中指定的图片
-        @tags albums
+        更新 drive 的数据处理模版
+        @tags drive
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
         runtime.validate()
         _runtime = {
             'timeouted': 'retry',
@@ -37298,15 +38202,15 @@
                 accesskey_id = self.get_access_key_id()
                 access_key_secret = self.get_access_key_secret()
                 security_token = self.get_security_token()
                 access_token = self.get_access_token()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/unassign_facegroup_item')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/drive/update_data_process_template')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -37321,18 +38225,21 @@
                     string_to_sign = ROAUtilClient.get_string_to_sign(_request)
                     _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
                 _request.body = UtilClient.to_jsonstring(real_req)
                 _last_request = _request
                 _response = TeaCore.do_action(_request, _runtime)
                 resp_map = None
                 obj = None
-                if UtilClient.equal_number(_response.status_code, 204):
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.UnassignFacegroupItemModel(),
+                        pds_models.UpdateDataProcessTemplateModel(),
                         {
+                            'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
                         'data': {
                             'requestId': _response.headers.get('x-ca-request-id'),
@@ -37353,25 +38260,27 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    async def unassign_facegroup_item_ex_async(
+    async def update_data_process_template_ex_async(
         self,
-        request: pds_models.UnAssignFaceGroupItemRequest,
+        request: pds_models.UpdateDriveDataProcessTemplateRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.UnassignFacegroupItemModel:
+    ) -> pds_models.UpdateDataProcessTemplateModel:
         """
-        该接口将会对移除人脸分组中指定的图片
-        @tags albums
+        更新 drive 的数据处理模版
+        @tags drive
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         request.validate()
         runtime.validate()
         _runtime = {
             'timeouted': 'retry',
@@ -37409,15 +38318,15 @@
                 accesskey_id = await self.get_access_key_id_async()
                 access_key_secret = await self.get_access_key_secret_async()
                 security_token = await self.get_security_token_async()
                 access_token = await self.get_access_token_async()
                 real_req = UtilClient.to_map(request)
                 _request.protocol = UtilClient.default_string(self._protocol, 'https')
                 _request.method = 'POST'
-                _request.pathname = self.get_pathname(self._nickname, f'/v2/albums/unassign_facegroup_item')
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/drive/update_data_process_template')
                 _request.headers = TeaCore.merge({
                     'user-agent': self.get_user_agent(),
                     'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
                     'content-type': 'application/json; charset=utf-8'
                 }, request.httpheaders)
                 real_req['httpheaders'] = None
                 if not UtilClient.empty(access_token):
@@ -37432,18 +38341,21 @@
                     string_to_sign = ROAUtilClient.get_string_to_sign(_request)
                     _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
                 _request.body = UtilClient.to_jsonstring(real_req)
                 _last_request = _request
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 resp_map = None
                 obj = None
-                if UtilClient.equal_number(_response.status_code, 204):
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.UnassignFacegroupItemModel(),
+                        pds_models.UpdateDataProcessTemplateModel(),
                         {
+                            'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
                         'data': {
                             'requestId': _response.headers.get('x-ca-request-id'),
@@ -37924,14 +38836,246 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def create_similar_image_cluster_task_ex(
+        self,
+        request: pds_models.CreateSimilarImageClusterTaskRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.CreateSimilarImageClusterTaskModel:
+        """
+        创建相似图片聚类任务
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/create_similar_image_cluster_task')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.CreateSimilarImageClusterTaskModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def create_similar_image_cluster_task_ex_async(
+        self,
+        request: pds_models.CreateSimilarImageClusterTaskRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.CreateSimilarImageClusterTaskModel:
+        """
+        创建相似图片聚类任务
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/create_similar_image_cluster_task')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.CreateSimilarImageClusterTaskModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
     def create_story_ex(
         self,
         request: pds_models.CreateStoryRequest,
         runtime: pds_models.RuntimeOptions,
     ) -> pds_models.CreateStoryModel:
         """
         该接口将会创建故事
@@ -38154,14 +39298,244 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def delete_location_date_cluster_ex(
+        self,
+        request: pds_models.DeleteLocationDateClusterRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.DeleteLocationDateClusterModel:
+        """
+        该接口将会删除时空聚类分组
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/delete_location_date_cluster')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.DeleteLocationDateClusterModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def delete_location_date_cluster_ex_async(
+        self,
+        request: pds_models.DeleteLocationDateClusterRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.DeleteLocationDateClusterModel:
+        """
+        该接口将会删除时空聚类分组
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/delete_location_date_cluster')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.DeleteLocationDateClusterModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
     def delete_story_ex(
         self,
         request: pds_models.DeleteStoryRequest,
         runtime: pds_models.RuntimeOptions,
     ) -> pds_models.DeleteStoryModel:
         """
         该接口将会删除故事
@@ -39304,14 +40678,246 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
+    def get_task_status_ex(
+        self,
+        request: pds_models.GetTaskStatusRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetTaskStatusModel:
+        """
+        查询任务状态
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/get_task_status')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetTaskStatusModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def get_task_status_ex_async(
+        self,
+        request: pds_models.GetTaskStatusRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.GetTaskStatusModel:
+        """
+        查询任务状态
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/get_task_status')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.GetTaskStatusModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
     def list_address_groups_ex(
         self,
         request: pds_models.ListImageAddressGroupsRequest,
         runtime: pds_models.RuntimeOptions,
     ) -> pds_models.ListAddressGroupsModel:
         """
         该接口将会展示用户图片的地点分组
@@ -40222,21 +41828,21 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def delete_location_date_cluster_ex(
+    def query_location_date_cluster_ex(
         self,
-        request: pds_models.DeleteLocationDateClusterRequest,
+        request: pds_models.QueryLocationDateClustersRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.DeleteLocationDateClusterModel:
+    ) -> pds_models.QueryLocationDateClusterModel:
         """
-        该接口将会删除时空聚类分组
+        该接口将会查询时空聚类列表
         @tags image
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
@@ -40306,15 +41912,15 @@
                 _response = TeaCore.do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = UtilClient.read_as_json(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.DeleteLocationDateClusterModel(),
+                        pds_models.QueryLocationDateClusterModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -40337,21 +41943,21 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    async def delete_location_date_cluster_ex_async(
+    async def query_location_date_cluster_ex_async(
         self,
-        request: pds_models.DeleteLocationDateClusterRequest,
+        request: pds_models.QueryLocationDateClustersRequest,
         runtime: pds_models.RuntimeOptions,
-    ) -> pds_models.DeleteLocationDateClusterModel:
+    ) -> pds_models.QueryLocationDateClusterModel:
         """
-        该接口将会删除时空聚类分组
+        该接口将会查询时空聚类列表
         @tags image
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
@@ -40421,15 +42027,247 @@
                 _response = await TeaCore.async_do_action(_request, _runtime)
                 resp_map = None
                 obj = None
                 if UtilClient.equal_number(_response.status_code, 200):
                     obj = await UtilClient.read_as_json_async(_response.body)
                     resp_map = UtilClient.assert_as_map(obj)
                     return TeaCore.from_map(
-                        pds_models.DeleteLocationDateClusterModel(),
+                        pds_models.QueryLocationDateClusterModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = await UtilClient.read_as_json_async(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    def query_similar_image_clusters_ex(
+        self,
+        request: pds_models.QuerySimilarImageClusterRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.QuerySimilarImageClustersModel:
+        """
+        查询相似图片聚类
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = self.get_access_key_id()
+                access_key_secret = self.get_access_key_secret()
+                security_token = self.get_security_token()
+                access_token = self.get_access_token()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/query_similar_image_clusters')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = TeaCore.do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = UtilClient.read_as_json(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.QuerySimilarImageClustersModel(),
+                        {
+                            'body': resp_map,
+                            'headers': _response.headers
+                        }
+                    )
+                if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
+                    raise TeaException({
+                        'data': {
+                            'requestId': _response.headers.get('x-ca-request-id'),
+                            'statusCode': _response.status_code,
+                            'statusMessage': _response.status_message
+                        },
+                        'message': _response.headers.get('x-ca-error-message')
+                    })
+                obj = UtilClient.read_as_json(_response.body)
+                resp_map = UtilClient.assert_as_map(obj)
+                raise TeaException(TeaCore.merge({
+                    'data': {
+                        'requestId': _response.headers.get('x-ca-request-id'),
+                        'statusCode': _response.status_code,
+                        'statusMessage': _response.status_message
+                    }
+                }, resp_map))
+            except Exception as e:
+                if TeaCore.is_retryable(e):
+                    _last_exception = e
+                    continue
+                raise e
+        raise UnretryableException(_last_request, _last_exception)
+
+    async def query_similar_image_clusters_ex_async(
+        self,
+        request: pds_models.QuerySimilarImageClusterRequest,
+        runtime: pds_models.RuntimeOptions,
+    ) -> pds_models.QuerySimilarImageClustersModel:
+        """
+        查询相似图片聚类
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        request.validate()
+        runtime.validate()
+        _runtime = {
+            'timeouted': 'retry',
+            'readTimeout': runtime.read_timeout,
+            'connectTimeout': runtime.connect_timeout,
+            'localAddr': runtime.local_addr,
+            'httpProxy': runtime.http_proxy,
+            'httpsProxy': runtime.https_proxy,
+            'noProxy': runtime.no_proxy,
+            'maxIdleConns': runtime.max_idle_conns,
+            'socks5Proxy': runtime.socks_5proxy,
+            'socks5NetWork': runtime.socks_5net_work,
+            'retry': {
+                'retryable': runtime.autoretry,
+                'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
+            },
+            'backoff': {
+                'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
+                'period': UtilClient.default_number(runtime.backoff_period, 1)
+            },
+            'ignoreSSL': runtime.ignore_ssl
+        }
+        _last_request = None
+        _last_exception = None
+        _now = time.time()
+        _retry_times = 0
+        while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
+            if _retry_times > 0:
+                _backoff_time = TeaCore.get_backoff_time(_runtime.get('backoff'), _retry_times)
+                if _backoff_time > 0:
+                    TeaCore.sleep(_backoff_time)
+            _retry_times = _retry_times + 1
+            try:
+                _request = TeaRequest()
+                accesskey_id = await self.get_access_key_id_async()
+                access_key_secret = await self.get_access_key_secret_async()
+                security_token = await self.get_security_token_async()
+                access_token = await self.get_access_token_async()
+                real_req = UtilClient.to_map(request)
+                _request.protocol = UtilClient.default_string(self._protocol, 'https')
+                _request.method = 'POST'
+                _request.pathname = self.get_pathname(self._nickname, f'/v2/image/query_similar_image_clusters')
+                _request.headers = TeaCore.merge({
+                    'user-agent': self.get_user_agent(),
+                    'host': UtilClient.default_string(self._endpoint, f'{self._domain_id}.api.aliyunpds.com'),
+                    'content-type': 'application/json; charset=utf-8'
+                }, request.httpheaders)
+                real_req['httpheaders'] = None
+                if not UtilClient.empty(access_token):
+                    _request.headers['authorization'] = f'Bearer {access_token}'
+                elif not UtilClient.empty(accesskey_id) and not UtilClient.empty(access_key_secret):
+                    if not UtilClient.empty(security_token):
+                        _request.headers['x-acs-security-token'] = security_token
+                    _request.headers['date'] = UtilClient.get_date_utcstring()
+                    _request.headers['accept'] = 'application/json'
+                    _request.headers['x-acs-signature-method'] = 'HMAC-SHA1'
+                    _request.headers['x-acs-signature-version'] = '1.0'
+                    string_to_sign = ROAUtilClient.get_string_to_sign(_request)
+                    _request.headers['authorization'] = f'acs {accesskey_id}:{ROAUtilClient.get_signature(string_to_sign, access_key_secret)}'
+                _request.body = UtilClient.to_jsonstring(real_req)
+                _last_request = _request
+                _response = await TeaCore.async_do_action(_request, _runtime)
+                resp_map = None
+                obj = None
+                if UtilClient.equal_number(_response.status_code, 200):
+                    obj = await UtilClient.read_as_json_async(_response.body)
+                    resp_map = UtilClient.assert_as_map(obj)
+                    return TeaCore.from_map(
+                        pds_models.QuerySimilarImageClustersModel(),
                         {
                             'body': resp_map,
                             'headers': _response.headers
                         }
                     )
                 if not UtilClient.empty(_response.headers.get('x-ca-error-message')):
                     raise TeaException({
@@ -46508,14 +48346,46 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.get_download_url_ex_async(request, runtime)
 
+    def get_facegroups(
+        self,
+        request: pds_models.GetFileFaceGroupsRequest,
+    ) -> pds_models.GetFacegroupsModel:
+        """
+        获取文件人脸分组列表
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.get_facegroups_ex(request, runtime)
+
+    async def get_facegroups_async(
+        self,
+        request: pds_models.GetFileFaceGroupsRequest,
+    ) -> pds_models.GetFacegroupsModel:
+        """
+        获取文件人脸分组列表
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.get_facegroups_ex_async(request, runtime)
+
     def get_last_cursor(
         self,
         request: pds_models.GetLastCursorRequest,
     ) -> pds_models.GetLastCursorModel:
         """
         获取drive内，增量数据最新的游标
         @tags file_delta
@@ -46574,14 +48444,74 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.get_media_play_url_ex_async(request, runtime)
 
+    def get_media_preview_info(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayInfoRequest,
+    ) -> pds_models.GetMediaPreviewInfoModel:
+        """
+        获取媒体文件播放信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.get_media_preview_info_ex(request, runtime)
+
+    async def get_media_preview_info_async(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayInfoRequest,
+    ) -> pds_models.GetMediaPreviewInfoModel:
+        """
+        获取媒体文件播放信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.get_media_preview_info_ex_async(request, runtime)
+
+    def get_media_preview_meta(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayMetaRequest,
+    ) -> pds_models.GetMediaPreviewMetaModel:
+        """
+        获取媒体文件播放元信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.get_media_preview_meta_ex(request, runtime)
+
+    async def get_media_preview_meta_async(
+        self,
+        request: pds_models.CCPGetVideoPreviewPlayMetaRequest,
+    ) -> pds_models.GetMediaPreviewMetaModel:
+        """
+        获取媒体文件播放元信息
+        @tags file
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.get_media_preview_meta_ex_async(request, runtime)
+
     def get_office_edit_url(
         self,
         request: pds_models.GetOfficeEditUrlRequest,
     ) -> pds_models.GetOfficeEditUrlModel:
         """
         获取文档的在线编辑地址
         @tags file
@@ -49944,50 +51874,14 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.update_user_ex_async(request, runtime)
 
-    def update_data_process_template(
-        self,
-        request: pds_models.UpdateDataProcessTemplateRequest,
-    ) -> pds_models.UpdateDataProcessTemplateModel:
-        """
-        更新用户指定的资源的数据处理模版
-        @tags user
-        @error InvalidParameter The input parameter {parameter_name} is not valid.
-        @error AccessTokenInvalid AccessToken is invalid. {message}
-        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
-        @error NotFound The resource {resource_name} cannot be found. Please check.
-        @error StateConflict User operation is not valid.
-        @error InternalError The request has been failed due to some unknown error.
-        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
-        """
-        runtime = pds_models.RuntimeOptions()
-        return self.update_data_process_template_ex(request, runtime)
-
-    async def update_data_process_template_async(
-        self,
-        request: pds_models.UpdateDataProcessTemplateRequest,
-    ) -> pds_models.UpdateDataProcessTemplateModel:
-        """
-        更新用户指定的资源的数据处理模版
-        @tags user
-        @error InvalidParameter The input parameter {parameter_name} is not valid.
-        @error AccessTokenInvalid AccessToken is invalid. {message}
-        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
-        @error NotFound The resource {resource_name} cannot be found. Please check.
-        @error StateConflict User operation is not valid.
-        @error InternalError The request has been failed due to some unknown error.
-        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
-        """
-        runtime = pds_models.RuntimeOptions()
-        return await self.update_data_process_template_ex_async(request, runtime)
-
     def search_user_group(
         self,
         request: pds_models.SearchUserAndGroupRequest,
     ) -> pds_models.SearchUserGroupModel:
         """
         该接口将会根据条件查询用户和团队，只有管理员可以调用
         @tags user_group
@@ -50076,14 +51970,86 @@
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.unassign_facegroup_item_ex_async(request, runtime)
 
+    def get_data_process_template(
+        self,
+        request: pds_models.GetDriveDataProcessTemplateRequest,
+    ) -> pds_models.GetDataProcessTemplateModel:
+        """
+        获取 drive 的数据处理模版
+        @tags drive
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.get_data_process_template_ex(request, runtime)
+
+    async def get_data_process_template_async(
+        self,
+        request: pds_models.GetDriveDataProcessTemplateRequest,
+    ) -> pds_models.GetDataProcessTemplateModel:
+        """
+        获取 drive 的数据处理模版
+        @tags drive
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.get_data_process_template_ex_async(request, runtime)
+
+    def update_data_process_template(
+        self,
+        request: pds_models.UpdateDriveDataProcessTemplateRequest,
+    ) -> pds_models.UpdateDataProcessTemplateModel:
+        """
+        更新 drive 的数据处理模版
+        @tags drive
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.update_data_process_template_ex(request, runtime)
+
+    async def update_data_process_template_async(
+        self,
+        request: pds_models.UpdateDriveDataProcessTemplateRequest,
+    ) -> pds_models.UpdateDataProcessTemplateModel:
+        """
+        更新 drive 的数据处理模版
+        @tags drive
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.update_data_process_template_ex_async(request, runtime)
+
     def add_story_files(
         self,
         request: pds_models.AddStoryFilesRequest,
     ) -> pds_models.AddStoryFilesModel:
         """
         该接口将会在指定的故事中添加文件
         @tags image
@@ -50144,14 +52110,50 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.create_customized_story_ex_async(request, runtime)
 
+    def create_similar_image_cluster_task(
+        self,
+        request: pds_models.CreateSimilarImageClusterTaskRequest,
+    ) -> pds_models.CreateSimilarImageClusterTaskModel:
+        """
+        创建相似图片聚类任务
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.create_similar_image_cluster_task_ex(request, runtime)
+
+    async def create_similar_image_cluster_task_async(
+        self,
+        request: pds_models.CreateSimilarImageClusterTaskRequest,
+    ) -> pds_models.CreateSimilarImageClusterTaskModel:
+        """
+        创建相似图片聚类任务
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.create_similar_image_cluster_task_ex_async(request, runtime)
+
     def create_story(
         self,
         request: pds_models.CreateStoryRequest,
     ) -> pds_models.CreateStoryModel:
         """
         该接口将会创建故事
         @tags image
@@ -50178,14 +52180,48 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.create_story_ex_async(request, runtime)
 
+    def delete_location_date_cluster(
+        self,
+        request: pds_models.DeleteLocationDateClusterRequest,
+    ) -> pds_models.DeleteLocationDateClusterModel:
+        """
+        该接口将会删除时空聚类分组
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.delete_location_date_cluster_ex(request, runtime)
+
+    async def delete_location_date_cluster_async(
+        self,
+        request: pds_models.DeleteLocationDateClusterRequest,
+    ) -> pds_models.DeleteLocationDateClusterModel:
+        """
+        该接口将会删除时空聚类分组
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.delete_location_date_cluster_ex_async(request, runtime)
+
     def delete_story(
         self,
         request: pds_models.DeleteStoryRequest,
     ) -> pds_models.DeleteStoryModel:
         """
         该接口将会删除故事
         @tags image
@@ -50348,14 +52384,50 @@
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.get_story_ex_async(request, runtime)
 
+    def get_task_status(
+        self,
+        request: pds_models.GetTaskStatusRequest,
+    ) -> pds_models.GetTaskStatusModel:
+        """
+        查询任务状态
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.get_task_status_ex(request, runtime)
+
+    async def get_task_status_async(
+        self,
+        request: pds_models.GetTaskStatusRequest,
+    ) -> pds_models.GetTaskStatusModel:
+        """
+        查询任务状态
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.get_task_status_ex_async(request, runtime)
+
     def list_address_groups(
         self,
         request: pds_models.ListImageAddressGroupsRequest,
     ) -> pds_models.ListAddressGroupsModel:
         """
         该接口将会展示用户图片的地点分组
         @tags image
@@ -50482,47 +52554,83 @@
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
         return await self.parse_keywords_ex_async(request, runtime)
 
-    def delete_location_date_cluster(
+    def query_location_date_cluster(
         self,
-        request: pds_models.DeleteLocationDateClusterRequest,
-    ) -> pds_models.DeleteLocationDateClusterModel:
+        request: pds_models.QueryLocationDateClustersRequest,
+    ) -> pds_models.QueryLocationDateClusterModel:
         """
-        该接口将会删除时空聚类分组
+        该接口将会查询时空聚类列表
         @tags image
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
-        return self.delete_location_date_cluster_ex(request, runtime)
+        return self.query_location_date_cluster_ex(request, runtime)
 
-    async def delete_location_date_cluster_async(
+    async def query_location_date_cluster_async(
         self,
-        request: pds_models.DeleteLocationDateClusterRequest,
-    ) -> pds_models.DeleteLocationDateClusterModel:
+        request: pds_models.QueryLocationDateClustersRequest,
+    ) -> pds_models.QueryLocationDateClusterModel:
         """
-        该接口将会删除时空聚类分组
+        该接口将会查询时空聚类列表
         @tags image
         @error InvalidParameter The input parameter {parameter_name} is not valid.
         @error AccessTokenInvalid AccessToken is invalid. {message}
         @error ForbiddenNoPermission No Permission to access resource {resource_name}.
         @error NotFound The resource {resource_name} cannot be found. Please check.
         @error InternalError The request has been failed due to some unknown error.
         @error ServiceUnavailable The request has failed due to a temporary failure of the server.
         """
         runtime = pds_models.RuntimeOptions()
-        return await self.delete_location_date_cluster_ex_async(request, runtime)
+        return await self.query_location_date_cluster_ex_async(request, runtime)
+
+    def query_similar_image_clusters(
+        self,
+        request: pds_models.QuerySimilarImageClusterRequest,
+    ) -> pds_models.QuerySimilarImageClustersModel:
+        """
+        查询相似图片聚类
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return self.query_similar_image_clusters_ex(request, runtime)
+
+    async def query_similar_image_clusters_async(
+        self,
+        request: pds_models.QuerySimilarImageClusterRequest,
+    ) -> pds_models.QuerySimilarImageClustersModel:
+        """
+        查询相似图片聚类
+        @tags image
+        @error InvalidParameter The input parameter {parameter_name} is not valid.
+        @error AccessTokenInvalid AccessToken is invalid. {message}
+        @error ForbiddenNoPermission No Permission to access resource {resource_name}.
+        @error NotFound The resource {resource_name} cannot be found. Please check.
+        @error StateConflict User operation is not valid.
+        @error InternalError The request has been failed due to some unknown error.
+        @error ServiceUnavailable The request has failed due to a temporary failure of the server.
+        """
+        runtime = pds_models.RuntimeOptions()
+        return await self.query_similar_image_clusters_ex_async(request, runtime)
 
     def remove_story_files(
         self,
         request: pds_models.RemoveStoryFilesRequest,
     ) -> pds_models.RemoveStoryFilesModel:
         """
         该接口将会在指定的故事中移除文件
```

### Comparing `alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk/models.py` & `alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5881,14 +5881,15 @@
         owner_type: str = None,
         permission: dict = None,
         relative_path: str = None,
         status: str = None,
         store_id: str = None,
         subdomain_id: str = None,
         total_size: int = None,
+        updated_at: str = None,
         used_size: int = None,
     ):
         self.action_list = action_list
         self.category = category
         self.created_at = created_at
         # Drive 创建者
         self.creator = creator
@@ -5915,14 +5916,15 @@
         self.status = status
         # 存储 ID, domain的PathType为OSSPath时返回
         self.store_id = store_id
         # subdomain_id
         self.subdomain_id = subdomain_id
         # Drive 空间总量
         self.total_size = total_size
+        self.updated_at = updated_at
         # Drive 空间已使用量
         self.used_size = used_size
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5965,14 +5967,16 @@
             result['status'] = self.status
         if self.store_id is not None:
             result['store_id'] = self.store_id
         if self.subdomain_id is not None:
             result['subdomain_id'] = self.subdomain_id
         if self.total_size is not None:
             result['total_size'] = self.total_size
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
         if self.used_size is not None:
             result['used_size'] = self.used_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('action_list') is not None:
@@ -6009,14 +6013,16 @@
             self.status = m.get('status')
         if m.get('store_id') is not None:
             self.store_id = m.get('store_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('total_size') is not None:
             self.total_size = m.get('total_size')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
         if m.get('used_size') is not None:
             self.used_size = m.get('used_size')
         return self
 
 
 class GetDriveModel(TeaModel):
     def __init__(
@@ -6111,14 +6117,15 @@
         owner_type: str = None,
         permission: dict = None,
         relative_path: str = None,
         status: str = None,
         store_id: str = None,
         subdomain_id: str = None,
         total_size: int = None,
+        updated_at: str = None,
         used_size: int = None,
     ):
         self.action_list = action_list
         self.category = category
         self.created_at = created_at
         # Drive 创建者
         self.creator = creator
@@ -6145,14 +6152,15 @@
         self.status = status
         # 存储 ID, domain的PathType为OSSPath时返回
         self.store_id = store_id
         # subdomain_id
         self.subdomain_id = subdomain_id
         # Drive 空间总量
         self.total_size = total_size
+        self.updated_at = updated_at
         # Drive 空间已使用量
         self.used_size = used_size
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6195,14 +6203,16 @@
             result['status'] = self.status
         if self.store_id is not None:
             result['store_id'] = self.store_id
         if self.subdomain_id is not None:
             result['subdomain_id'] = self.subdomain_id
         if self.total_size is not None:
             result['total_size'] = self.total_size
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
         if self.used_size is not None:
             result['used_size'] = self.used_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('action_list') is not None:
@@ -6239,14 +6249,16 @@
             self.status = m.get('status')
         if m.get('store_id') is not None:
             self.store_id = m.get('store_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('total_size') is not None:
             self.total_size = m.get('total_size')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
         if m.get('used_size') is not None:
             self.used_size = m.get('used_size')
         return self
 
 
 class ListDriveResponse(TeaModel):
     """
@@ -6469,14 +6481,15 @@
         owner_type: str = None,
         permission: dict = None,
         relative_path: str = None,
         status: str = None,
         store_id: str = None,
         subdomain_id: str = None,
         total_size: int = None,
+        updated_at: str = None,
         used_size: int = None,
     ):
         self.action_list = action_list
         self.category = category
         self.created_at = created_at
         # Drive 创建者
         self.creator = creator
@@ -6503,14 +6516,15 @@
         self.status = status
         # 存储 ID, domain的PathType为OSSPath时返回
         self.store_id = store_id
         # subdomain_id
         self.subdomain_id = subdomain_id
         # Drive 空间总量
         self.total_size = total_size
+        self.updated_at = updated_at
         # Drive 空间已使用量
         self.used_size = used_size
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6553,14 +6567,16 @@
             result['status'] = self.status
         if self.store_id is not None:
             result['store_id'] = self.store_id
         if self.subdomain_id is not None:
             result['subdomain_id'] = self.subdomain_id
         if self.total_size is not None:
             result['total_size'] = self.total_size
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
         if self.used_size is not None:
             result['used_size'] = self.used_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('action_list') is not None:
@@ -6597,14 +6613,16 @@
             self.status = m.get('status')
         if m.get('store_id') is not None:
             self.store_id = m.get('store_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('total_size') is not None:
             self.total_size = m.get('total_size')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
         if m.get('used_size') is not None:
             self.used_size = m.get('used_size')
         return self
 
 
 class UpdateDriveModel(TeaModel):
     def __init__(
@@ -7862,14 +7880,15 @@
         encrypt_mode: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         location: str = None,
@@ -7951,14 +7970,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -8100,14 +8121,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -8229,14 +8252,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -8376,14 +8401,15 @@
         endpoint: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         meta: str = None,
@@ -8468,14 +8494,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -8620,14 +8648,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -8751,14 +8781,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -9869,14 +9901,15 @@
         encrypt_mode: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         meta: str = None,
@@ -9957,14 +9990,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -10106,14 +10141,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -10233,14 +10270,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -10376,14 +10415,15 @@
         encrypt_mode: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         meta: str = None,
@@ -10464,14 +10504,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -10613,14 +10655,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -10740,14 +10784,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -11029,116 +11075,214 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetDownloadUrlResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetLastCursorResponse(TeaModel):
+class FaceBoundary(TeaModel):
     """
-    get last file op cursor response
+    *\
     """
     def __init__(
         self,
-        cursor: str = None,
+        height: int = None,
+        left: int = None,
+        top: int = None,
+        width: int = None,
     ):
-        self.cursor = cursor
+        self.height = height
+        self.left = left
+        self.top = top
+        self.width = width
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.cursor is not None:
-            result['cursor'] = self.cursor
+        if self.height is not None:
+            result['Height'] = self.height
+        if self.left is not None:
+            result['Left'] = self.left
+        if self.top is not None:
+            result['Top'] = self.top
+        if self.width is not None:
+            result['Width'] = self.width
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cursor') is not None:
-            self.cursor = m.get('cursor')
+        if m.get('Height') is not None:
+            self.height = m.get('Height')
+        if m.get('Left') is not None:
+            self.left = m.get('Left')
+        if m.get('Top') is not None:
+            self.top = m.get('Top')
+        if m.get('Width') is not None:
+            self.width = m.get('Width')
         return self
 
 
-class GetLastCursorModel(TeaModel):
+class ImageFaceGroupResponse(TeaModel):
+    """
+    人脸分组信息
+    """
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        body: GetLastCursorResponse = None,
+        created_at: str = None,
+        group_cover_face_boundary: FaceBoundary = None,
+        group_cover_file_id: str = None,
+        group_cover_height: int = None,
+        group_cover_url: str = None,
+        group_cover_width: int = None,
+        group_id: str = None,
+        group_name: str = None,
+        image_count: int = None,
+        remarks: str = None,
+        remarks_array: List[str] = None,
+        updated_at: str = None,
     ):
-        self.headers = headers
-        self.body = body
+        # 人脸分组生成时间
+        self.created_at = created_at
+        self.group_cover_face_boundary = group_cover_face_boundary
+        # group_cover_file_id
+        self.group_cover_file_id = group_cover_file_id
+        # group_cover_height
+        self.group_cover_height = group_cover_height
+        # 人脸分组封面头像地址
+        self.group_cover_url = group_cover_url
+        # group_cover_width
+        self.group_cover_width = group_cover_width
+        # 人脸分组 ID
+        self.group_id = group_id
+        # 人脸分组名称
+        self.group_name = group_name
+        # 照片个数
+        self.image_count = image_count
+        # remarks
+        self.remarks = remarks
+        # remarks_array
+        self.remarks_array = remarks_array
+        # 人脸分组修改时间
+        self.updated_at = updated_at
 
     def validate(self):
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.group_cover_face_boundary:
+            self.group_cover_face_boundary.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.created_at is not None:
+            result['created_at'] = self.created_at
+        if self.group_cover_face_boundary is not None:
+            result['group_cover_face_boundary'] = self.group_cover_face_boundary.to_map()
+        if self.group_cover_file_id is not None:
+            result['group_cover_file_id'] = self.group_cover_file_id
+        if self.group_cover_height is not None:
+            result['group_cover_height'] = self.group_cover_height
+        if self.group_cover_url is not None:
+            result['group_cover_url'] = self.group_cover_url
+        if self.group_cover_width is not None:
+            result['group_cover_width'] = self.group_cover_width
+        if self.group_id is not None:
+            result['group_id'] = self.group_id
+        if self.group_name is not None:
+            result['group_name'] = self.group_name
+        if self.image_count is not None:
+            result['image_count'] = self.image_count
+        if self.remarks is not None:
+            result['remarks'] = self.remarks
+        if self.remarks_array is not None:
+            result['remarks_array'] = self.remarks_array
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = GetLastCursorResponse()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('created_at') is not None:
+            self.created_at = m.get('created_at')
+        if m.get('group_cover_face_boundary') is not None:
+            temp_model = FaceBoundary()
+            self.group_cover_face_boundary = temp_model.from_map(m['group_cover_face_boundary'])
+        if m.get('group_cover_file_id') is not None:
+            self.group_cover_file_id = m.get('group_cover_file_id')
+        if m.get('group_cover_height') is not None:
+            self.group_cover_height = m.get('group_cover_height')
+        if m.get('group_cover_url') is not None:
+            self.group_cover_url = m.get('group_cover_url')
+        if m.get('group_cover_width') is not None:
+            self.group_cover_width = m.get('group_cover_width')
+        if m.get('group_id') is not None:
+            self.group_id = m.get('group_id')
+        if m.get('group_name') is not None:
+            self.group_name = m.get('group_name')
+        if m.get('image_count') is not None:
+            self.image_count = m.get('image_count')
+        if m.get('remarks') is not None:
+            self.remarks = m.get('remarks')
+        if m.get('remarks_array') is not None:
+            self.remarks_array = m.get('remarks_array')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
         return self
 
 
-class GetMediaPlayURLResponse(TeaModel):
+class ImageFaceGroupsResponse(TeaModel):
     """
-    get_media_play_url response
+    人脸分组数组
     """
     def __init__(
         self,
-        url: str = None,
+        face_groups: List[ImageFaceGroupResponse] = None,
     ):
-        # url
-        self.url = url
+        self.face_groups = face_groups
 
     def validate(self):
-        pass
+        if self.face_groups:
+            for k in self.face_groups:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.url is not None:
-            result['url'] = self.url
+        result['face_groups'] = []
+        if self.face_groups is not None:
+            for k in self.face_groups:
+                result['face_groups'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('url') is not None:
-            self.url = m.get('url')
+        self.face_groups = []
+        if m.get('face_groups') is not None:
+            for k in m.get('face_groups'):
+                temp_model = ImageFaceGroupResponse()
+                self.face_groups.append(temp_model.from_map(k))
         return self
 
 
-class GetMediaPlayUrlModel(TeaModel):
+class GetFacegroupsModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetMediaPlayURLResponse = None,
+        body: ImageFaceGroupsResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -11157,69 +11301,54 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = GetMediaPlayURLResponse()
+            temp_model = ImageFaceGroupsResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetOfficeEditUrlResponse(TeaModel):
+class GetLastCursorResponse(TeaModel):
     """
-    获取office文档在线编辑地址 response
+    get last file op cursor response
     """
     def __init__(
         self,
-        edit_url: str = None,
-        office_access_token: str = None,
-        office_refresh_token: str = None,
+        cursor: str = None,
     ):
-        # EditUrl
-        self.edit_url = edit_url
-        # AccessToken
-        self.office_access_token = office_access_token
-        # RefreshToken
-        self.office_refresh_token = office_refresh_token
+        self.cursor = cursor
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.edit_url is not None:
-            result['edit_url'] = self.edit_url
-        if self.office_access_token is not None:
-            result['office_access_token'] = self.office_access_token
-        if self.office_refresh_token is not None:
-            result['office_refresh_token'] = self.office_refresh_token
+        if self.cursor is not None:
+            result['cursor'] = self.cursor
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('edit_url') is not None:
-            self.edit_url = m.get('edit_url')
-        if m.get('office_access_token') is not None:
-            self.office_access_token = m.get('office_access_token')
-        if m.get('office_refresh_token') is not None:
-            self.office_refresh_token = m.get('office_refresh_token')
+        if m.get('cursor') is not None:
+            self.cursor = m.get('cursor')
         return self
 
 
-class GetOfficeEditUrlModel(TeaModel):
+class GetLastCursorModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetOfficeEditUrlResponse = None,
+        body: GetLastCursorResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -11238,62 +11367,55 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = GetOfficeEditUrlResponse()
+            temp_model = GetLastCursorResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetOfficePreviewUrlResponse(TeaModel):
+class GetMediaPlayURLResponse(TeaModel):
     """
-    获取文档预览地址 response
+    get_media_play_url response
     """
     def __init__(
         self,
-        access_token: str = None,
-        preview_url: str = None,
+        url: str = None,
     ):
-        # AccessToken
-        self.access_token = access_token
-        # preview_url
-        self.preview_url = preview_url
+        # url
+        self.url = url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.access_token is not None:
-            result['access_token'] = self.access_token
-        if self.preview_url is not None:
-            result['preview_url'] = self.preview_url
+        if self.url is not None:
+            result['url'] = self.url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('access_token') is not None:
-            self.access_token = m.get('access_token')
-        if m.get('preview_url') is not None:
-            self.preview_url = m.get('preview_url')
+        if m.get('url') is not None:
+            self.url = m.get('url')
         return self
 
 
-class GetOfficePreviewUrlModel(TeaModel):
+class GetMediaPlayUrlModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetOfficePreviewUrlResponse = None,
+        body: GetMediaPlayURLResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -11312,187 +11434,175 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = GetOfficePreviewUrlResponse()
+            temp_model = GetMediaPlayURLResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class MediaPlayInfoTemplate(TeaModel):
+class AudioPreviewPlayInfoMetaResponse(TeaModel):
     """
-    *\
+    音频转码信息meta响应
     """
     def __init__(
         self,
-        status: str = None,
-        template_id: str = None,
-        url: str = None,
+        bitrate: int = None,
+        channels: int = None,
+        duration: float = None,
+        sample_rate: int = None,
     ):
-        # status
-        self.status = status
-        # template_id
-        self.template_id = template_id
-        # url
-        self.url = url
+        # bitrate, 码率
+        self.bitrate = bitrate
+        # channels, 声道数
+        self.channels = channels
+        # duration, 视频长度
+        self.duration = duration
+        # sample_rate, 采样率
+        self.sample_rate = sample_rate
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.status is not None:
-            result['status'] = self.status
-        if self.template_id is not None:
-            result['template_id'] = self.template_id
-        if self.url is not None:
-            result['url'] = self.url
+        if self.bitrate is not None:
+            result['bitrate'] = self.bitrate
+        if self.channels is not None:
+            result['channels'] = self.channels
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.sample_rate is not None:
+            result['sample_rate'] = self.sample_rate
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('template_id') is not None:
-            self.template_id = m.get('template_id')
-        if m.get('url') is not None:
-            self.url = m.get('url')
+        if m.get('bitrate') is not None:
+            self.bitrate = m.get('bitrate')
+        if m.get('channels') is not None:
+            self.channels = m.get('channels')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('sample_rate') is not None:
+            self.sample_rate = m.get('sample_rate')
         return self
 
 
-class GetShareLinkDownloadURLResponse(TeaModel):
+class VideoPreviewOfflineAudioTranscodingTaskResponse(TeaModel):
     """
-    获取分享中文件数据response
+    离线音频转码task响应
     """
     def __init__(
         self,
-        audio_template_list: List[MediaPlayInfoTemplate] = None,
-        download_url: str = None,
-        streams_info: dict = None,
-        streams_url: dict = None,
-        thumbnail: str = None,
+        status: str = None,
+        template_bitrate: int = None,
+        template_id: str = None,
+        template_name: str = None,
         url: str = None,
-        video_template_list: List[MediaPlayInfoTemplate] = None,
     ):
-        # audio_template_list
-        self.audio_template_list = audio_template_list
-        # download_url
-        self.download_url = download_url
-        # @Deprecated streams url info
-        self.streams_info = streams_info
-        # streams url info
-        self.streams_url = streams_url
-        # thumbnail
-        self.thumbnail = thumbnail
-        # url
+        # status, 转码状态
+        self.status = status
+        # template_bitrate, 音频码率，单位Kbps
+        self.template_bitrate = template_bitrate
+        # template_id, 转码模板id
+        self.template_id = template_id
+        # template_name, 模板文案id
+        self.template_name = template_name
+        # url, 播放地址
         self.url = url
-        # video_template_list
-        self.video_template_list = video_template_list
 
     def validate(self):
-        if self.audio_template_list:
-            for k in self.audio_template_list:
-                if k:
-                    k.validate()
-        if self.video_template_list:
-            for k in self.video_template_list:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['audio_template_list'] = []
-        if self.audio_template_list is not None:
-            for k in self.audio_template_list:
-                result['audio_template_list'].append(k.to_map() if k else None)
-        if self.download_url is not None:
-            result['download_url'] = self.download_url
-        if self.streams_info is not None:
-            result['streams_info'] = self.streams_info
-        if self.streams_url is not None:
-            result['streams_url'] = self.streams_url
-        if self.thumbnail is not None:
-            result['thumbnail'] = self.thumbnail
+        if self.status is not None:
+            result['status'] = self.status
+        if self.template_bitrate is not None:
+            result['template_bitrate'] = self.template_bitrate
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.template_name is not None:
+            result['template_name'] = self.template_name
         if self.url is not None:
             result['url'] = self.url
-        result['video_template_list'] = []
-        if self.video_template_list is not None:
-            for k in self.video_template_list:
-                result['video_template_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.audio_template_list = []
-        if m.get('audio_template_list') is not None:
-            for k in m.get('audio_template_list'):
-                temp_model = MediaPlayInfoTemplate()
-                self.audio_template_list.append(temp_model.from_map(k))
-        if m.get('download_url') is not None:
-            self.download_url = m.get('download_url')
-        if m.get('streams_info') is not None:
-            self.streams_info = m.get('streams_info')
-        if m.get('streams_url') is not None:
-            self.streams_url = m.get('streams_url')
-        if m.get('thumbnail') is not None:
-            self.thumbnail = m.get('thumbnail')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('template_bitrate') is not None:
+            self.template_bitrate = m.get('template_bitrate')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('template_name') is not None:
+            self.template_name = m.get('template_name')
         if m.get('url') is not None:
             self.url = m.get('url')
-        self.video_template_list = []
-        if m.get('video_template_list') is not None:
-            for k in m.get('video_template_list'):
-                temp_model = MediaPlayInfoTemplate()
-                self.video_template_list.append(temp_model.from_map(k))
         return self
 
 
-class GetShareLinkDownloadUrlModel(TeaModel):
+class AudioPreviewPlayInfoResponse(TeaModel):
+    """
+    音频转码信息响应
+    """
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        body: GetShareLinkDownloadURLResponse = None,
+        meta: AudioPreviewPlayInfoMetaResponse = None,
+        offline_audio_list: List[VideoPreviewOfflineAudioTranscodingTaskResponse] = None,
     ):
-        self.headers = headers
-        self.body = body
+        self.meta = meta
+        # 离线转码有效
+        self.offline_audio_list = offline_audio_list
 
     def validate(self):
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        if self.meta:
+            self.meta.validate()
+        if self.offline_audio_list:
+            for k in self.offline_audio_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.meta is not None:
+            result['meta'] = self.meta.to_map()
+        result['offline_audio_list'] = []
+        if self.offline_audio_list is not None:
+            for k in self.offline_audio_list:
+                result['offline_audio_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = GetShareLinkDownloadURLResponse()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('meta') is not None:
+            temp_model = AudioPreviewPlayInfoMetaResponse()
+            self.meta = temp_model.from_map(m['meta'])
+        self.offline_audio_list = []
+        if m.get('offline_audio_list') is not None:
+            for k in m.get('offline_audio_list'):
+                temp_model = VideoPreviewOfflineAudioTranscodingTaskResponse()
+                self.offline_audio_list.append(temp_model.from_map(k))
         return self
 
 
 class LiveTranscodingSubtitleTaskResponse(TeaModel):
     """
     *\
     """
@@ -11535,15 +11645,15 @@
         if m.get('url') is not None:
             self.url = m.get('url')
         return self
 
 
 class LiveTranscodingTaskResponse(TeaModel):
     """
-    实时转码信息task响应
+    实时转码task响应
     """
     def __init__(
         self,
         keep_original_resolution: bool = None,
         preview_url: str = None,
         stage: str = None,
         status: str = None,
@@ -11667,15 +11777,15 @@
         if m.get('ts_total_count') is not None:
             self.ts_total_count = m.get('ts_total_count')
         return self
 
 
 class VideoPreviewPlayInfoMetaResponse(TeaModel):
     """
-    获取视频转码信息meta响应
+    视频转码meta响应
     """
     def __init__(
         self,
         duration: float = None,
         height: int = None,
         live_transcoding_meta: LiveTranscodingMetaResponse = None,
         width: int = None,
@@ -11720,15 +11830,15 @@
         if m.get('width') is not None:
             self.width = m.get('width')
         return self
 
 
 class VideoPreviewOfflineVideoTranscodingTaskResponse(TeaModel):
     """
-    离线视频转码信息task响应
+    离线视频转码task响应
     """
     def __init__(
         self,
         keep_original_resolution: bool = None,
         protection_system: str = None,
         status: str = None,
         template_id: str = None,
@@ -11777,34 +11887,107 @@
         if m.get('template_id') is not None:
             self.template_id = m.get('template_id')
         if m.get('url') is not None:
             self.url = m.get('url')
         return self
 
 
+class QuickVideoTaskResponse(TeaModel):
+    """
+    快速转码task响应
+    """
+    def __init__(
+        self,
+        status: str = None,
+        template_height: int = None,
+        template_id: str = None,
+        template_name: str = None,
+        template_width: int = None,
+        url: str = None,
+    ):
+        # status, 转码状态
+        self.status = status
+        # template_height
+        self.template_height = template_height
+        # template_id, 转码模板id
+        self.template_id = template_id
+        # template_name, 模板文案id
+        self.template_name = template_name
+        # template_width
+        self.template_width = template_width
+        # url, 视频播放地址
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.template_height is not None:
+            result['template_height'] = self.template_height
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.template_name is not None:
+            result['template_name'] = self.template_name
+        if self.template_width is not None:
+            result['template_width'] = self.template_width
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('template_height') is not None:
+            self.template_height = m.get('template_height')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('template_name') is not None:
+            self.template_name = m.get('template_name')
+        if m.get('template_width') is not None:
+            self.template_width = m.get('template_width')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
 class VideoPreviewPlayInfoResponse(TeaModel):
     """
     转码信息响应
     """
     def __init__(
         self,
         category: str = None,
         live_transcoding_subtitle_task_list: List[LiveTranscodingSubtitleTaskResponse] = None,
         live_transcoding_task_list: List[LiveTranscodingTaskResponse] = None,
+        master_url: str = None,
         meta: VideoPreviewPlayInfoMetaResponse = None,
         offline_video_transcoding_list: List[VideoPreviewOfflineVideoTranscodingTaskResponse] = None,
+        quick_video_list: List[QuickVideoTaskResponse] = None,
     ):
-        # category
+        # deprecated, 使用外层Response中的同名字段替代
+        # category，此字段为保持兼容而继续存在
         self.category = category
         self.live_transcoding_subtitle_task_list = live_transcoding_subtitle_task_list
         # 边转边播有效
         self.live_transcoding_task_list = live_transcoding_task_list
+        # master playlist 播放地址
+        self.master_url = master_url
         self.meta = meta
         # 离线转码有效
         self.offline_video_transcoding_list = offline_video_transcoding_list
+        # imm边转边播
+        self.quick_video_list = quick_video_list
 
     def validate(self):
         if self.live_transcoding_subtitle_task_list:
             for k in self.live_transcoding_subtitle_task_list:
                 if k:
                     k.validate()
         if self.live_transcoding_task_list:
@@ -11813,14 +11996,18 @@
                     k.validate()
         if self.meta:
             self.meta.validate()
         if self.offline_video_transcoding_list:
             for k in self.offline_video_transcoding_list:
                 if k:
                     k.validate()
+        if self.quick_video_list:
+            for k in self.quick_video_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -11830,20 +12017,26 @@
         if self.live_transcoding_subtitle_task_list is not None:
             for k in self.live_transcoding_subtitle_task_list:
                 result['live_transcoding_subtitle_task_list'].append(k.to_map() if k else None)
         result['live_transcoding_task_list'] = []
         if self.live_transcoding_task_list is not None:
             for k in self.live_transcoding_task_list:
                 result['live_transcoding_task_list'].append(k.to_map() if k else None)
+        if self.master_url is not None:
+            result['master_url'] = self.master_url
         if self.meta is not None:
             result['meta'] = self.meta.to_map()
         result['offline_video_transcoding_list'] = []
         if self.offline_video_transcoding_list is not None:
             for k in self.offline_video_transcoding_list:
                 result['offline_video_transcoding_list'].append(k.to_map() if k else None)
+        result['quick_video_list'] = []
+        if self.quick_video_list is not None:
+            for k in self.quick_video_list:
+                result['quick_video_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('category') is not None:
             self.category = m.get('category')
         self.live_transcoding_subtitle_task_list = []
@@ -11852,64 +12045,651 @@
                 temp_model = LiveTranscodingSubtitleTaskResponse()
                 self.live_transcoding_subtitle_task_list.append(temp_model.from_map(k))
         self.live_transcoding_task_list = []
         if m.get('live_transcoding_task_list') is not None:
             for k in m.get('live_transcoding_task_list'):
                 temp_model = LiveTranscodingTaskResponse()
                 self.live_transcoding_task_list.append(temp_model.from_map(k))
+        if m.get('master_url') is not None:
+            self.master_url = m.get('master_url')
         if m.get('meta') is not None:
             temp_model = VideoPreviewPlayInfoMetaResponse()
             self.meta = temp_model.from_map(m['meta'])
         self.offline_video_transcoding_list = []
         if m.get('offline_video_transcoding_list') is not None:
             for k in m.get('offline_video_transcoding_list'):
                 temp_model = VideoPreviewOfflineVideoTranscodingTaskResponse()
                 self.offline_video_transcoding_list.append(temp_model.from_map(k))
+        self.quick_video_list = []
+        if m.get('quick_video_list') is not None:
+            for k in m.get('quick_video_list'):
+                temp_model = QuickVideoTaskResponse()
+                self.quick_video_list.append(temp_model.from_map(k))
+        return self
+
+
+class CCPGetVideoPreviewPlayInfoResponse(TeaModel):
+    """
+    获取转码信息响应
+    """
+    def __init__(
+        self,
+        audio_preview_play_info: AudioPreviewPlayInfoResponse = None,
+        category: str = None,
+        domain_id: str = None,
+        drive_id: str = None,
+        file_id: str = None,
+        share_id: str = None,
+        video_preview_play_info: VideoPreviewPlayInfoResponse = None,
+    ):
+        self.audio_preview_play_info = audio_preview_play_info
+        # category
+        self.category = category
+        # domain_id
+        self.domain_id = domain_id
+        # drive_id
+        self.drive_id = drive_id
+        # file_id
+        self.file_id = file_id
+        # share_id
+        self.share_id = share_id
+        self.video_preview_play_info = video_preview_play_info
+
+    def validate(self):
+        if self.audio_preview_play_info:
+            self.audio_preview_play_info.validate()
+        if self.domain_id is not None:
+            self.validate_pattern(self.domain_id, 'domain_id', '[a-z0-9A-Z]+')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.file_id is not None:
+            self.validate_max_length(self.file_id, 'file_id', 50)
+            self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
+        if self.video_preview_play_info:
+            self.video_preview_play_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audio_preview_play_info is not None:
+            result['audio_preview_play_info'] = self.audio_preview_play_info.to_map()
+        if self.category is not None:
+            result['category'] = self.category
+        if self.domain_id is not None:
+            result['domain_id'] = self.domain_id
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
+        if self.video_preview_play_info is not None:
+            result['video_preview_play_info'] = self.video_preview_play_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('audio_preview_play_info') is not None:
+            temp_model = AudioPreviewPlayInfoResponse()
+            self.audio_preview_play_info = temp_model.from_map(m['audio_preview_play_info'])
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('domain_id') is not None:
+            self.domain_id = m.get('domain_id')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
+        if m.get('video_preview_play_info') is not None:
+            temp_model = VideoPreviewPlayInfoResponse()
+            self.video_preview_play_info = temp_model.from_map(m['video_preview_play_info'])
+        return self
+
+
+class GetMediaPreviewInfoModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: CCPGetVideoPreviewPlayInfoResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = CCPGetVideoPreviewPlayInfoResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CCPGetVideoPreviewPlayMetaResponse(TeaModel):
+    """
+    获取播放元信息响应
+    """
+    def __init__(
+        self,
+        audio_preview_play_meta: AudioPreviewPlayInfoResponse = None,
+        category: str = None,
+        domain_id: str = None,
+        drive_id: str = None,
+        file_id: str = None,
+        share_id: str = None,
+        video_preview_play_meta: VideoPreviewPlayInfoResponse = None,
+    ):
+        self.audio_preview_play_meta = audio_preview_play_meta
+        # category
+        self.category = category
+        # domain_id
+        self.domain_id = domain_id
+        # drive_id
+        self.drive_id = drive_id
+        # file_id
+        self.file_id = file_id
+        # share_id
+        self.share_id = share_id
+        self.video_preview_play_meta = video_preview_play_meta
+
+    def validate(self):
+        if self.audio_preview_play_meta:
+            self.audio_preview_play_meta.validate()
+        if self.domain_id is not None:
+            self.validate_pattern(self.domain_id, 'domain_id', '[a-z0-9A-Z]+')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.file_id is not None:
+            self.validate_max_length(self.file_id, 'file_id', 50)
+            self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
+        if self.video_preview_play_meta:
+            self.video_preview_play_meta.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audio_preview_play_meta is not None:
+            result['audio_preview_play_meta'] = self.audio_preview_play_meta.to_map()
+        if self.category is not None:
+            result['category'] = self.category
+        if self.domain_id is not None:
+            result['domain_id'] = self.domain_id
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
+        if self.video_preview_play_meta is not None:
+            result['video_preview_play_meta'] = self.video_preview_play_meta.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('audio_preview_play_meta') is not None:
+            temp_model = AudioPreviewPlayInfoResponse()
+            self.audio_preview_play_meta = temp_model.from_map(m['audio_preview_play_meta'])
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('domain_id') is not None:
+            self.domain_id = m.get('domain_id')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
+        if m.get('video_preview_play_meta') is not None:
+            temp_model = VideoPreviewPlayInfoResponse()
+            self.video_preview_play_meta = temp_model.from_map(m['video_preview_play_meta'])
+        return self
+
+
+class GetMediaPreviewMetaModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: CCPGetVideoPreviewPlayMetaResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = CCPGetVideoPreviewPlayMetaResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetOfficeEditUrlResponse(TeaModel):
+    """
+    获取office文档在线编辑地址 response
+    """
+    def __init__(
+        self,
+        edit_url: str = None,
+        office_access_token: str = None,
+        office_refresh_token: str = None,
+    ):
+        # EditUrl
+        self.edit_url = edit_url
+        # AccessToken
+        self.office_access_token = office_access_token
+        # RefreshToken
+        self.office_refresh_token = office_refresh_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.edit_url is not None:
+            result['edit_url'] = self.edit_url
+        if self.office_access_token is not None:
+            result['office_access_token'] = self.office_access_token
+        if self.office_refresh_token is not None:
+            result['office_refresh_token'] = self.office_refresh_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('edit_url') is not None:
+            self.edit_url = m.get('edit_url')
+        if m.get('office_access_token') is not None:
+            self.office_access_token = m.get('office_access_token')
+        if m.get('office_refresh_token') is not None:
+            self.office_refresh_token = m.get('office_refresh_token')
+        return self
+
+
+class GetOfficeEditUrlModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetOfficeEditUrlResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetOfficeEditUrlResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetOfficePreviewUrlResponse(TeaModel):
+    """
+    获取文档预览地址 response
+    """
+    def __init__(
+        self,
+        access_token: str = None,
+        preview_url: str = None,
+    ):
+        # AccessToken
+        self.access_token = access_token
+        # preview_url
+        self.preview_url = preview_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        if self.preview_url is not None:
+            result['preview_url'] = self.preview_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        if m.get('preview_url') is not None:
+            self.preview_url = m.get('preview_url')
+        return self
+
+
+class GetOfficePreviewUrlModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetOfficePreviewUrlResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetOfficePreviewUrlResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class MediaPlayInfoTemplate(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        status: str = None,
+        template_id: str = None,
+        url: str = None,
+    ):
+        # status
+        self.status = status
+        # template_id
+        self.template_id = template_id
+        # url
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class GetShareLinkDownloadURLResponse(TeaModel):
+    """
+    获取分享中文件数据response
+    """
+    def __init__(
+        self,
+        audio_template_list: List[MediaPlayInfoTemplate] = None,
+        download_url: str = None,
+        streams_info: dict = None,
+        streams_url: dict = None,
+        thumbnail: str = None,
+        url: str = None,
+        video_template_list: List[MediaPlayInfoTemplate] = None,
+    ):
+        # audio_template_list
+        self.audio_template_list = audio_template_list
+        # download_url
+        self.download_url = download_url
+        # @Deprecated streams url info
+        self.streams_info = streams_info
+        # streams url info
+        self.streams_url = streams_url
+        # thumbnail
+        self.thumbnail = thumbnail
+        # url
+        self.url = url
+        # video_template_list
+        self.video_template_list = video_template_list
+
+    def validate(self):
+        if self.audio_template_list:
+            for k in self.audio_template_list:
+                if k:
+                    k.validate()
+        if self.video_template_list:
+            for k in self.video_template_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['audio_template_list'] = []
+        if self.audio_template_list is not None:
+            for k in self.audio_template_list:
+                result['audio_template_list'].append(k.to_map() if k else None)
+        if self.download_url is not None:
+            result['download_url'] = self.download_url
+        if self.streams_info is not None:
+            result['streams_info'] = self.streams_info
+        if self.streams_url is not None:
+            result['streams_url'] = self.streams_url
+        if self.thumbnail is not None:
+            result['thumbnail'] = self.thumbnail
+        if self.url is not None:
+            result['url'] = self.url
+        result['video_template_list'] = []
+        if self.video_template_list is not None:
+            for k in self.video_template_list:
+                result['video_template_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.audio_template_list = []
+        if m.get('audio_template_list') is not None:
+            for k in m.get('audio_template_list'):
+                temp_model = MediaPlayInfoTemplate()
+                self.audio_template_list.append(temp_model.from_map(k))
+        if m.get('download_url') is not None:
+            self.download_url = m.get('download_url')
+        if m.get('streams_info') is not None:
+            self.streams_info = m.get('streams_info')
+        if m.get('streams_url') is not None:
+            self.streams_url = m.get('streams_url')
+        if m.get('thumbnail') is not None:
+            self.thumbnail = m.get('thumbnail')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        self.video_template_list = []
+        if m.get('video_template_list') is not None:
+            for k in m.get('video_template_list'):
+                temp_model = MediaPlayInfoTemplate()
+                self.video_template_list.append(temp_model.from_map(k))
+        return self
+
+
+class GetShareLinkDownloadUrlModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetShareLinkDownloadURLResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetShareLinkDownloadURLResponse()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CCPGetShareLinkVideoPreviewPlayInfoResponse(TeaModel):
     """
     获取分享中媒体播放地址response
     """
     def __init__(
         self,
+        audio_preview_play_info: AudioPreviewPlayInfoResponse = None,
+        category: str = None,
         file_id: str = None,
         share_id: str = None,
         video_preview_play_info: VideoPreviewPlayInfoResponse = None,
     ):
+        self.audio_preview_play_info = audio_preview_play_info
+        # category
+        self.category = category
         # file_id
         self.file_id = file_id
         # share_id
         self.share_id = share_id
         self.video_preview_play_info = video_preview_play_info
 
     def validate(self):
+        if self.audio_preview_play_info:
+            self.audio_preview_play_info.validate()
         if self.file_id is not None:
             self.validate_max_length(self.file_id, 'file_id', 50)
             self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
         if self.video_preview_play_info:
             self.video_preview_play_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.audio_preview_play_info is not None:
+            result['audio_preview_play_info'] = self.audio_preview_play_info.to_map()
+        if self.category is not None:
+            result['category'] = self.category
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.video_preview_play_info is not None:
             result['video_preview_play_info'] = self.video_preview_play_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('audio_preview_play_info') is not None:
+            temp_model = AudioPreviewPlayInfoResponse()
+            self.audio_preview_play_info = temp_model.from_map(m['audio_preview_play_info'])
+        if m.get('category') is not None:
+            self.category = m.get('category')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('video_preview_play_info') is not None:
             temp_model = VideoPreviewPlayInfoResponse()
             self.video_preview_play_info = temp_model.from_map(m['video_preview_play_info'])
@@ -12174,81 +12954,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetUploadUrlResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CCPGetVideoPreviewPlayInfoResponse(TeaModel):
-    """
-    获取转码信息响应
-    """
-    def __init__(
-        self,
-        domain_id: str = None,
-        drive_id: str = None,
-        file_id: str = None,
-        share_id: str = None,
-        video_preview_play_info: VideoPreviewPlayInfoResponse = None,
-    ):
-        # domain_id
-        self.domain_id = domain_id
-        # drive_id
-        self.drive_id = drive_id
-        # file_id
-        self.file_id = file_id
-        # share_id
-        self.share_id = share_id
-        self.video_preview_play_info = video_preview_play_info
-
-    def validate(self):
-        if self.domain_id is not None:
-            self.validate_pattern(self.domain_id, 'domain_id', '[a-z0-9A-Z]+')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.file_id is not None:
-            self.validate_max_length(self.file_id, 'file_id', 50)
-            self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
-        if self.video_preview_play_info:
-            self.video_preview_play_info.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.domain_id is not None:
-            result['domain_id'] = self.domain_id
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.share_id is not None:
-            result['share_id'] = self.share_id
-        if self.video_preview_play_info is not None:
-            result['video_preview_play_info'] = self.video_preview_play_info.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('domain_id') is not None:
-            self.domain_id = m.get('domain_id')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('share_id') is not None:
-            self.share_id = m.get('share_id')
-        if m.get('video_preview_play_info') is not None:
-            temp_model = VideoPreviewPlayInfoResponse()
-            self.video_preview_play_info = temp_model.from_map(m['video_preview_play_info'])
-        return self
-
-
 class GetVideoPreviewPlayInfoModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         body: CCPGetVideoPreviewPlayInfoResponse = None,
     ):
         self.headers = headers
@@ -12277,81 +12990,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CCPGetVideoPreviewPlayInfoResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CCPGetVideoPreviewPlayMetaResponse(TeaModel):
-    """
-    获取播放元信息响应
-    """
-    def __init__(
-        self,
-        domain_id: str = None,
-        drive_id: str = None,
-        file_id: str = None,
-        share_id: str = None,
-        video_preview_play_meta: VideoPreviewPlayInfoResponse = None,
-    ):
-        # domain_id
-        self.domain_id = domain_id
-        # drive_id
-        self.drive_id = drive_id
-        # file_id
-        self.file_id = file_id
-        # share_id
-        self.share_id = share_id
-        self.video_preview_play_meta = video_preview_play_meta
-
-    def validate(self):
-        if self.domain_id is not None:
-            self.validate_pattern(self.domain_id, 'domain_id', '[a-z0-9A-Z]+')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.file_id is not None:
-            self.validate_max_length(self.file_id, 'file_id', 50)
-            self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
-        if self.video_preview_play_meta:
-            self.video_preview_play_meta.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.domain_id is not None:
-            result['domain_id'] = self.domain_id
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.share_id is not None:
-            result['share_id'] = self.share_id
-        if self.video_preview_play_meta is not None:
-            result['video_preview_play_meta'] = self.video_preview_play_meta.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('domain_id') is not None:
-            self.domain_id = m.get('domain_id')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('share_id') is not None:
-            self.share_id = m.get('share_id')
-        if m.get('video_preview_play_meta') is not None:
-            temp_model = VideoPreviewPlayInfoResponse()
-            self.video_preview_play_meta = temp_model.from_map(m['video_preview_play_meta'])
-        return self
-
-
 class GetVideoPreviewPlayMetaModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         body: CCPGetVideoPreviewPlayMetaResponse = None,
     ):
         self.headers = headers
@@ -12588,14 +13234,15 @@
         encrypt_mode: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         meta: str = None,
@@ -12675,14 +13322,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -12821,14 +13470,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -12946,14 +13597,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -13372,65 +14025,86 @@
 class CreateDetail(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         create_type: str = None,
+        is_over_write: bool = None,
         src_file_id: str = None,
     ):
         # CreateType
         self.create_type = create_type
+        self.is_over_write = is_over_write
         # SrcFileID
         self.src_file_id = src_file_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.create_type is not None:
             result['create_type'] = self.create_type
+        if self.is_over_write is not None:
+            result['is_over_write'] = self.is_over_write
         if self.src_file_id is not None:
             result['src_file_id'] = self.src_file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('create_type') is not None:
             self.create_type = m.get('create_type')
+        if m.get('is_over_write') is not None:
+            self.is_over_write = m.get('is_over_write')
         if m.get('src_file_id') is not None:
             self.src_file_id = m.get('src_file_id')
         return self
 
 
 class DeleteDetail(TeaModel):
     """
     *\
     """
-    def __init__(self):
-        pass
+    def __init__(
+        self,
+        src_parent_file_id: str = None,
+        tgt_parent_file_id: str = None,
+    ):
+        # SrcParentFileID
+        self.src_parent_file_id = src_parent_file_id
+        # TgtParentFileID
+        self.tgt_parent_file_id = tgt_parent_file_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.src_parent_file_id is not None:
+            result['src_parent_file_id'] = self.src_parent_file_id
+        if self.tgt_parent_file_id is not None:
+            result['tgt_parent_file_id'] = self.tgt_parent_file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('src_parent_file_id') is not None:
+            self.src_parent_file_id = m.get('src_parent_file_id')
+        if m.get('tgt_parent_file_id') is not None:
+            self.tgt_parent_file_id = m.get('tgt_parent_file_id')
         return self
 
 
 class EditDetail(TeaModel):
     """
     *\
     """
@@ -13529,61 +14203,83 @@
         return self
 
 
 class RestoreDetail(TeaModel):
     """
     *\
     """
-    def __init__(self):
-        pass
+    def __init__(
+        self,
+        src_parent_file_id: str = None,
+        tgt_parent_file_id: str = None,
+    ):
+        # SrcParentFileID
+        self.src_parent_file_id = src_parent_file_id
+        # TgtParentFileID
+        self.tgt_parent_file_id = tgt_parent_file_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.src_parent_file_id is not None:
+            result['src_parent_file_id'] = self.src_parent_file_id
+        if self.tgt_parent_file_id is not None:
+            result['tgt_parent_file_id'] = self.tgt_parent_file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('src_parent_file_id') is not None:
+            self.src_parent_file_id = m.get('src_parent_file_id')
+        if m.get('tgt_parent_file_id') is not None:
+            self.tgt_parent_file_id = m.get('tgt_parent_file_id')
         return self
 
 
 class TrashDetail(TeaModel):
     """
     *\
     """
     def __init__(
         self,
-        parent_file_id: str = None,
+        src_parent_file_id: str = None,
+        tgt_parent_file_id: str = None,
     ):
-        # ParentFileID
-        self.parent_file_id = parent_file_id
+        # SrcParentFileID
+        self.src_parent_file_id = src_parent_file_id
+        # TgtParentFileID
+        self.tgt_parent_file_id = tgt_parent_file_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.parent_file_id is not None:
-            result['parent_file_id'] = self.parent_file_id
+        if self.src_parent_file_id is not None:
+            result['src_parent_file_id'] = self.src_parent_file_id
+        if self.tgt_parent_file_id is not None:
+            result['tgt_parent_file_id'] = self.tgt_parent_file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('parent_file_id') is not None:
-            self.parent_file_id = m.get('parent_file_id')
+        if m.get('src_parent_file_id') is not None:
+            self.src_parent_file_id = m.get('src_parent_file_id')
+        if m.get('tgt_parent_file_id') is not None:
+            self.tgt_parent_file_id = m.get('tgt_parent_file_id')
         return self
 
 
 class ActionDetail(TeaModel):
     """
     *\
     """
@@ -14107,54 +14803,105 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ListFileResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeltaExtInfo(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        move_type: str = None,
+        src_name: str = None,
+        src_parent_file_id: str = None,
+    ):
+        self.move_type = move_type
+        self.src_name = src_name
+        self.src_parent_file_id = src_parent_file_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.move_type is not None:
+            result['move_type'] = self.move_type
+        if self.src_name is not None:
+            result['src_name'] = self.src_name
+        if self.src_parent_file_id is not None:
+            result['src_parent_file_id'] = self.src_parent_file_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('move_type') is not None:
+            self.move_type = m.get('move_type')
+        if m.get('src_name') is not None:
+            self.src_name = m.get('src_name')
+        if m.get('src_parent_file_id') is not None:
+            self.src_parent_file_id = m.get('src_parent_file_id')
+        return self
+
+
 class FileDeltaResponse(TeaModel):
     """
     the file op info
     """
     def __init__(
         self,
         current_category: str = None,
+        ext_info: DeltaExtInfo = None,
         file: BaseCCPFileResponse = None,
         file_id: str = None,
         op: str = None,
     ):
         self.current_category = current_category
+        self.ext_info = ext_info
         self.file = file
         self.file_id = file_id
         self.op = op
 
     def validate(self):
+        if self.ext_info:
+            self.ext_info.validate()
         if self.file:
             self.file.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.current_category is not None:
             result['current_category'] = self.current_category
+        if self.ext_info is not None:
+            result['ext_info'] = self.ext_info.to_map()
         if self.file is not None:
             result['file'] = self.file.to_map()
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.op is not None:
             result['op'] = self.op
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('current_category') is not None:
             self.current_category = m.get('current_category')
+        if m.get('ext_info') is not None:
+            temp_model = DeltaExtInfo()
+            self.ext_info = temp_model.from_map(m['ext_info'])
         if m.get('file') is not None:
             temp_model = BaseCCPFileResponse()
             self.file = temp_model.from_map(m['file'])
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('op') is not None:
             self.op = m.get('op')
@@ -16238,14 +16985,15 @@
         encrypt_mode: str = None,
         ex_fields_info: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         meta: str = None,
@@ -16325,14 +17073,16 @@
         self.file_id = file_id
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
         # last_modifier_type
@@ -16471,14 +17221,16 @@
             result['file_id'] = self.file_id
         if self.file_path_type is not None:
             result['file_path_type'] = self.file_path_type
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
             result['last_modifier_name'] = self.last_modifier_name
         if self.last_modifier_type is not None:
@@ -16596,14 +17348,16 @@
         if m.get('file_path_type') is not None:
             self.file_path_type = m.get('file_path_type')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
             self.last_modifier_name = m.get('last_modifier_name')
         if m.get('last_modifier_type') is not None:
@@ -18211,14 +18965,15 @@
         preview_count: int = None,
         preview_limit: int = None,
         report_count: int = None,
         require_login: bool = None,
         save_count: int = None,
         save_download_limit: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_icon: str = None,
         share_id: str = None,
         share_msg: str = None,
         share_name: str = None,
         share_policy: str = None,
         share_pwd: str = None,
         share_url: str = None,
@@ -18287,14 +19042,16 @@
         self.require_login = require_login
         # 转存次数
         self.save_count = save_count
         # 分享转存和下载的总次数限制
         self.save_download_limit = save_download_limit
         # 分享转存次数限制
         self.save_limit = save_limit
+        # 是否分享整个drive中的文件，仅文件分享才有效，true时file_id_list字段无效
+        self.share_all_files = share_all_files
         # share_icon
         self.share_icon = share_icon
         # share_id
         self.share_id = share_id
         # share_msg
         self.share_msg = share_msg
         # share_name
@@ -18388,14 +19145,16 @@
             result['require_login'] = self.require_login
         if self.save_count is not None:
             result['save_count'] = self.save_count
         if self.save_download_limit is not None:
             result['save_download_limit'] = self.save_download_limit
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_icon is not None:
             result['share_icon'] = self.share_icon
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.share_msg is not None:
             result['share_msg'] = self.share_msg
         if self.share_name is not None:
@@ -18481,14 +19240,16 @@
             self.require_login = m.get('require_login')
         if m.get('save_count') is not None:
             self.save_count = m.get('save_count')
         if m.get('save_download_limit') is not None:
             self.save_download_limit = m.get('save_download_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_icon') is not None:
             self.share_icon = m.get('share_icon')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('share_msg') is not None:
             self.share_msg = m.get('share_msg')
         if m.get('share_name') is not None:
@@ -18580,14 +19341,15 @@
         preview_count: int = None,
         preview_limit: int = None,
         report_count: int = None,
         require_login: bool = None,
         save_count: int = None,
         save_download_limit: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_icon: str = None,
         share_id: str = None,
         share_msg: str = None,
         share_name: str = None,
         share_policy: str = None,
         share_pwd: str = None,
         share_url: str = None,
@@ -18656,14 +19418,16 @@
         self.require_login = require_login
         # 转存次数
         self.save_count = save_count
         # 分享转存和下载的总次数限制
         self.save_download_limit = save_download_limit
         # 分享转存次数限制
         self.save_limit = save_limit
+        # 是否分享整个drive中的文件，仅文件分享才有效，true时file_id_list字段无效
+        self.share_all_files = share_all_files
         # share_icon
         self.share_icon = share_icon
         # share_id
         self.share_id = share_id
         # share_msg
         self.share_msg = share_msg
         # share_name
@@ -18757,14 +19521,16 @@
             result['require_login'] = self.require_login
         if self.save_count is not None:
             result['save_count'] = self.save_count
         if self.save_download_limit is not None:
             result['save_download_limit'] = self.save_download_limit
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_icon is not None:
             result['share_icon'] = self.share_icon
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.share_msg is not None:
             result['share_msg'] = self.share_msg
         if self.share_name is not None:
@@ -18850,14 +19616,16 @@
             self.require_login = m.get('require_login')
         if m.get('save_count') is not None:
             self.save_count = m.get('save_count')
         if m.get('save_download_limit') is not None:
             self.save_download_limit = m.get('save_download_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_icon') is not None:
             self.share_icon = m.get('share_icon')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('share_msg') is not None:
             self.share_msg = m.get('share_msg')
         if m.get('share_name') is not None:
@@ -19590,14 +20358,15 @@
         preview_count: int = None,
         preview_limit: int = None,
         report_count: int = None,
         require_login: bool = None,
         save_count: int = None,
         save_download_limit: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_icon: str = None,
         share_id: str = None,
         share_msg: str = None,
         share_name: str = None,
         share_policy: str = None,
         share_pwd: str = None,
         share_url: str = None,
@@ -19666,14 +20435,16 @@
         self.require_login = require_login
         # 转存次数
         self.save_count = save_count
         # 分享转存和下载的总次数限制
         self.save_download_limit = save_download_limit
         # 分享转存次数限制
         self.save_limit = save_limit
+        # 是否分享整个drive中的文件，仅文件分享才有效，true时file_id_list字段无效
+        self.share_all_files = share_all_files
         # share_icon
         self.share_icon = share_icon
         # share_id
         self.share_id = share_id
         # share_msg
         self.share_msg = share_msg
         # share_name
@@ -19767,14 +20538,16 @@
             result['require_login'] = self.require_login
         if self.save_count is not None:
             result['save_count'] = self.save_count
         if self.save_download_limit is not None:
             result['save_download_limit'] = self.save_download_limit
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_icon is not None:
             result['share_icon'] = self.share_icon
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.share_msg is not None:
             result['share_msg'] = self.share_msg
         if self.share_name is not None:
@@ -19860,14 +20633,16 @@
             self.require_login = m.get('require_login')
         if m.get('save_count') is not None:
             self.save_count = m.get('save_count')
         if m.get('save_download_limit') is not None:
             self.save_download_limit = m.get('save_download_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_icon') is not None:
             self.share_icon = m.get('share_icon')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('share_msg') is not None:
             self.share_msg = m.get('share_msg')
         if m.get('share_name') is not None:
@@ -22977,42 +23752,56 @@
 class CreateSyncMappingResponse(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         drive_id: str = None,
+        exist: bool = None,
         file_id: str = None,
+        name: str = None,
     ):
         # drive_id
         self.drive_id = drive_id
+        # exist
+        self.exist = exist
         # file_id
         self.file_id = file_id
+        # name string
+        self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.exist is not None:
+            result['exist'] = self.exist
         if self.file_id is not None:
             result['file_id'] = self.file_id
+        if self.name is not None:
+            result['name'] = self.name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('exist') is not None:
+            self.exist = m.get('exist')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         return self
 
 
 class CreateSyncMappingModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -24589,92 +25378,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = UpdateUserResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class UpdateDataProcessTemplateResponse(TeaModel):
-    """
-    template update response
-    """
-    def __init__(
-        self,
-        resource_id: str = None,
-        resource_type: str = None,
-        template: str = None,
-    ):
-        self.resource_id = resource_id
-        self.resource_type = resource_type
-        self.template = template
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.resource_id is not None:
-            result['resource_id'] = self.resource_id
-        if self.resource_type is not None:
-            result['resource_type'] = self.resource_type
-        if self.template is not None:
-            result['template'] = self.template
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('resource_id') is not None:
-            self.resource_id = m.get('resource_id')
-        if m.get('resource_type') is not None:
-            self.resource_type = m.get('resource_type')
-        if m.get('template') is not None:
-            self.template = m.get('template')
-        return self
-
-
-class UpdateDataProcessTemplateModel(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        body: UpdateDataProcessTemplateResponse = None,
-    ):
-        self.headers = headers
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = UpdateDataProcessTemplateResponse()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class SearchUserAndGroupResponse(TeaModel):
     """
     Search user and group response
     """
     def __init__(
         self,
         groups: List[BaseGroupResponse] = None,
@@ -24765,15 +25476,15 @@
             temp_model = SearchUserAndGroupResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class MergeFaceGroupResponse(TeaModel):
     """
-    Merge face group response
+    merge face group response
     """
     def __init__(
         self,
         status: str = None,
         task_id: str = None,
     ):
         self.status = status
@@ -24862,14 +25573,152 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         return self
 
 
+class GetDriveDataProcessTemplateResponse(TeaModel):
+    """
+    get drive data process template response
+    """
+    def __init__(
+        self,
+        template_id: str = None,
+    ):
+        self.template_id = template_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        return self
+
+
+class GetDataProcessTemplateModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetDriveDataProcessTemplateResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetDriveDataProcessTemplateResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateDriveDataProcessTemplateResponse(TeaModel):
+    """
+    update drive data process template response
+    """
+    def __init__(
+        self,
+        drive_id: str = None,
+        template_id: str = None,
+    ):
+        self.drive_id = drive_id
+        self.template_id = template_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        return self
+
+
+class UpdateDataProcessTemplateModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: UpdateDriveDataProcessTemplateResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = UpdateDriveDataProcessTemplateResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AddStoryFile(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         error_code: str = None,
@@ -25079,14 +25928,80 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CreateCustomizedStoryResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateSimilarImageClusterTaskResponse(TeaModel):
+    """
+    create similar image cluster task response
+    """
+    def __init__(
+        self,
+        task_id: str = None,
+    ):
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        return self
+
+
+class CreateSimilarImageClusterTaskModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: CreateSimilarImageClusterTaskResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = CreateSimilarImageClusterTaskResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateStoryResponse(TeaModel):
     """
     生成故事
     """
     def __init__(
         self,
         drive_id: str = None,
@@ -25146,14 +26061,86 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CreateStoryResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteLocationDateClusterResponse(TeaModel):
+    """
+    delete locationCluster response
+    """
+    def __init__(
+        self,
+        cluster_id: str = None,
+        drive_id: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['cluster_id'] = self.cluster_id
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cluster_id') is not None:
+            self.cluster_id = m.get('cluster_id')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
+class DeleteLocationDateClusterModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: DeleteLocationDateClusterResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = DeleteLocationDateClusterResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteStoryResponse(TeaModel):
     """
     删除故事
     """
     def __init__(
         self,
         drive_id: str = None,
@@ -25424,176 +26411,86 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = FindStoriesResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class FaceBoundary(TeaModel):
-    """
-    *\
-    """
+class GetFacegroupInfoModel(TeaModel):
     def __init__(
         self,
-        height: int = None,
-        left: int = None,
-        top: int = None,
-        width: int = None,
+        headers: Dict[str, str] = None,
+        body: ImageFaceGroupResponse = None,
     ):
-        self.height = height
-        self.left = left
-        self.top = top
-        self.width = width
+        self.headers = headers
+        self.body = body
 
     def validate(self):
-        pass
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.height is not None:
-            result['Height'] = self.height
-        if self.left is not None:
-            result['Left'] = self.left
-        if self.top is not None:
-            result['Top'] = self.top
-        if self.width is not None:
-            result['Width'] = self.width
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Height') is not None:
-            self.height = m.get('Height')
-        if m.get('Left') is not None:
-            self.left = m.get('Left')
-        if m.get('Top') is not None:
-            self.top = m.get('Top')
-        if m.get('Width') is not None:
-            self.width = m.get('Width')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = ImageFaceGroupResponse()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ImageFaceGroupResponse(TeaModel):
+class GetImageCountResponse(TeaModel):
     """
-    人脸分组信息
+    获取云照片个数结果
     """
     def __init__(
         self,
-        created_at: str = None,
-        group_cover_face_boundary: FaceBoundary = None,
-        group_cover_file_id: str = None,
-        group_cover_height: int = None,
-        group_cover_url: str = None,
-        group_cover_width: int = None,
-        group_id: str = None,
-        group_name: str = None,
         image_count: int = None,
-        remarks: str = None,
-        remarks_array: List[str] = None,
-        updated_at: str = None,
     ):
-        # 人脸分组生成时间
-        self.created_at = created_at
-        self.group_cover_face_boundary = group_cover_face_boundary
-        # group_cover_file_id
-        self.group_cover_file_id = group_cover_file_id
-        # group_cover_height
-        self.group_cover_height = group_cover_height
-        # 人脸分组封面头像地址
-        self.group_cover_url = group_cover_url
-        # group_cover_width
-        self.group_cover_width = group_cover_width
-        # 人脸分组 ID
-        self.group_id = group_id
-        # 人脸分组名称
-        self.group_name = group_name
-        # 照片个数
+        # image_count
         self.image_count = image_count
-        # remarks
-        self.remarks = remarks
-        # remarks_array
-        self.remarks_array = remarks_array
-        # 人脸分组修改时间
-        self.updated_at = updated_at
 
     def validate(self):
-        if self.group_cover_face_boundary:
-            self.group_cover_face_boundary.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.created_at is not None:
-            result['created_at'] = self.created_at
-        if self.group_cover_face_boundary is not None:
-            result['group_cover_face_boundary'] = self.group_cover_face_boundary.to_map()
-        if self.group_cover_file_id is not None:
-            result['group_cover_file_id'] = self.group_cover_file_id
-        if self.group_cover_height is not None:
-            result['group_cover_height'] = self.group_cover_height
-        if self.group_cover_url is not None:
-            result['group_cover_url'] = self.group_cover_url
-        if self.group_cover_width is not None:
-            result['group_cover_width'] = self.group_cover_width
-        if self.group_id is not None:
-            result['group_id'] = self.group_id
-        if self.group_name is not None:
-            result['group_name'] = self.group_name
         if self.image_count is not None:
             result['image_count'] = self.image_count
-        if self.remarks is not None:
-            result['remarks'] = self.remarks
-        if self.remarks_array is not None:
-            result['remarks_array'] = self.remarks_array
-        if self.updated_at is not None:
-            result['updated_at'] = self.updated_at
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('created_at') is not None:
-            self.created_at = m.get('created_at')
-        if m.get('group_cover_face_boundary') is not None:
-            temp_model = FaceBoundary()
-            self.group_cover_face_boundary = temp_model.from_map(m['group_cover_face_boundary'])
-        if m.get('group_cover_file_id') is not None:
-            self.group_cover_file_id = m.get('group_cover_file_id')
-        if m.get('group_cover_height') is not None:
-            self.group_cover_height = m.get('group_cover_height')
-        if m.get('group_cover_url') is not None:
-            self.group_cover_url = m.get('group_cover_url')
-        if m.get('group_cover_width') is not None:
-            self.group_cover_width = m.get('group_cover_width')
-        if m.get('group_id') is not None:
-            self.group_id = m.get('group_id')
-        if m.get('group_name') is not None:
-            self.group_name = m.get('group_name')
         if m.get('image_count') is not None:
             self.image_count = m.get('image_count')
-        if m.get('remarks') is not None:
-            self.remarks = m.get('remarks')
-        if m.get('remarks_array') is not None:
-            self.remarks_array = m.get('remarks_array')
-        if m.get('updated_at') is not None:
-            self.updated_at = m.get('updated_at')
         return self
 
 
-class GetFacegroupInfoModel(TeaModel):
+class GetPhotoCountModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: ImageFaceGroupResponse = None,
+        body: GetImageCountResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -25612,91 +26509,90 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = ImageFaceGroupResponse()
+            temp_model = GetImageCountResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetImageCountResponse(TeaModel):
-    """
-    获取云照片个数结果
-    """
+class GetStoryModel(TeaModel):
     def __init__(
         self,
-        image_count: int = None,
+        headers: Dict[str, str] = None,
+        body: GetStoryResponse = None,
     ):
-        # image_count
-        self.image_count = image_count
+        self.headers = headers
+        self.body = body
 
     def validate(self):
-        pass
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.image_count is not None:
-            result['image_count'] = self.image_count
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('image_count') is not None:
-            self.image_count = m.get('image_count')
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetStoryResponse()
+            self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetPhotoCountModel(TeaModel):
+class GetTaskStatusResponse(TeaModel):
+    """
+    get task status response
+    """
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        body: GetImageCountResponse = None,
+        status: str = None,
     ):
-        self.headers = headers
-        self.body = body
+        self.status = status
 
     def validate(self):
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.status is not None:
+            result['status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = GetImageCountResponse()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('status') is not None:
+            self.status = m.get('status')
         return self
 
 
-class GetStoryModel(TeaModel):
+class GetTaskStatusModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetStoryResponse = None,
+        body: GetTaskStatusResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -25715,15 +26611,15 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = GetStoryResponse()
+            temp_model = GetTaskStatusResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class Address(TeaModel):
     """
     *\
@@ -25861,17 +26757,19 @@
     """
     展示地点分组集合
     """
     def __init__(
         self,
         items: List[ImageAddressResponse] = None,
         next_marker: str = None,
+        total_count: int = None,
     ):
         self.items = items
         self.next_marker = next_marker
+        self.total_count = total_count
 
     def validate(self):
         if self.items:
             for k in self.items:
                 if k:
                     k.validate()
 
@@ -25883,25 +26781,29 @@
         result = dict()
         result['items'] = []
         if self.items is not None:
             for k in self.items:
                 result['items'].append(k.to_map() if k else None)
         if self.next_marker is not None:
             result['next_marker'] = self.next_marker
+        if self.total_count is not None:
+            result['total_count'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.items = []
         if m.get('items') is not None:
             for k in m.get('items'):
                 temp_model = ImageAddressResponse()
                 self.items.append(temp_model.from_map(k))
         if m.get('next_marker') is not None:
             self.next_marker = m.get('next_marker')
+        if m.get('total_count') is not None:
+            self.total_count = m.get('total_count')
         return self
 
 
 class ListAddressGroupsModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -25941,17 +26843,19 @@
     """
     展示人脸分组集合
     """
     def __init__(
         self,
         items: List[ImageFaceGroupResponse] = None,
         next_marker: str = None,
+        total_count: int = None,
     ):
         self.items = items
         self.next_marker = next_marker
+        self.total_count = total_count
 
     def validate(self):
         if self.items:
             for k in self.items:
                 if k:
                     k.validate()
 
@@ -25963,25 +26867,29 @@
         result = dict()
         result['items'] = []
         if self.items is not None:
             for k in self.items:
                 result['items'].append(k.to_map() if k else None)
         if self.next_marker is not None:
             result['next_marker'] = self.next_marker
+        if self.total_count is not None:
+            result['total_count'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.items = []
         if m.get('items') is not None:
             for k in m.get('items'):
                 temp_model = ImageFaceGroupResponse()
                 self.items.append(temp_model.from_map(k))
         if m.get('next_marker') is not None:
             self.next_marker = m.get('next_marker')
+        if m.get('total_count') is not None:
+            self.total_count = m.get('total_count')
         return self
 
 
 class ListFacegroupsModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -26198,15 +27106,15 @@
         if m.get('start') is not None:
             self.start = m.get('start')
         return self
 
 
 class ParseKeywordsResponse(TeaModel):
     """
-    Parse keywords response
+    parse keywords response
     """
     def __init__(
         self,
         address_line: str = None,
         tags: List[SystemTag] = None,
         time_range: ParseTimeRange = None,
     ):
@@ -26286,55 +27194,149 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ParseKeywordsResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DeleteLocationDateClusterResponse(TeaModel):
+class LocationDateCluster(TeaModel):
     """
-    delete locationCluster response
+    *\
     """
     def __init__(
         self,
+        address: Address = None,
         cluster_id: str = None,
+        created_at: str = None,
+        custom_labels: dict = None,
         drive_id: str = None,
+        end_time: str = None,
+        level: str = None,
+        start_time: str = None,
+        title: str = None,
+        updated_at: str = None,
     ):
+        self.address = address
         self.cluster_id = cluster_id
+        self.created_at = created_at
+        self.custom_labels = custom_labels
         self.drive_id = drive_id
+        self.end_time = end_time
+        self.level = level
+        self.start_time = start_time
+        self.title = title
+        self.updated_at = updated_at
 
     def validate(self):
-        pass
+        if self.address:
+            self.address.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.address is not None:
+            result['address'] = self.address.to_map()
         if self.cluster_id is not None:
             result['cluster_id'] = self.cluster_id
+        if self.created_at is not None:
+            result['created_at'] = self.created_at
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.end_time is not None:
+            result['end_time'] = self.end_time
+        if self.level is not None:
+            result['level'] = self.level
+        if self.start_time is not None:
+            result['start_time'] = self.start_time
+        if self.title is not None:
+            result['title'] = self.title
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('address') is not None:
+            temp_model = Address()
+            self.address = temp_model.from_map(m['address'])
         if m.get('cluster_id') is not None:
             self.cluster_id = m.get('cluster_id')
+        if m.get('created_at') is not None:
+            self.created_at = m.get('created_at')
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('end_time') is not None:
+            self.end_time = m.get('end_time')
+        if m.get('level') is not None:
+            self.level = m.get('level')
+        if m.get('start_time') is not None:
+            self.start_time = m.get('start_time')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
         return self
 
 
-class DeleteLocationDateClusterModel(TeaModel):
+class QueryLocationClustersResponse(TeaModel):
+    """
+    query locationCluster response
+    """
+    def __init__(
+        self,
+        location_date_clusters: List[LocationDateCluster] = None,
+        next_marker: str = None,
+    ):
+        self.location_date_clusters = location_date_clusters
+        self.next_marker = next_marker
+
+    def validate(self):
+        if self.location_date_clusters:
+            for k in self.location_date_clusters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['location_date_clusters'] = []
+        if self.location_date_clusters is not None:
+            for k in self.location_date_clusters:
+                result['location_date_clusters'].append(k.to_map() if k else None)
+        if self.next_marker is not None:
+            result['next_marker'] = self.next_marker
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.location_date_clusters = []
+        if m.get('location_date_clusters') is not None:
+            for k in m.get('location_date_clusters'):
+                temp_model = LocationDateCluster()
+                self.location_date_clusters.append(temp_model.from_map(k))
+        if m.get('next_marker') is not None:
+            self.next_marker = m.get('next_marker')
+        return self
+
+
+class QueryLocationDateClusterModel(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: DeleteLocationDateClusterResponse = None,
+        body: QueryLocationClustersResponse = None,
     ):
         self.headers = headers
         self.body = body
 
     def validate(self):
         self.validate_required(self.body, 'body')
         if self.body:
@@ -26353,15 +27355,133 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('body') is not None:
-            temp_model = DeleteLocationDateClusterResponse()
+            temp_model = QueryLocationClustersResponse()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SimilarImageCluster(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        files: List[BaseCCPFileResponse] = None,
+    ):
+        self.files = files
+
+    def validate(self):
+        if self.files:
+            for k in self.files:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['files'] = []
+        if self.files is not None:
+            for k in self.files:
+                result['files'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.files = []
+        if m.get('files') is not None:
+            for k in m.get('files'):
+                temp_model = BaseCCPFileResponse()
+                self.files.append(temp_model.from_map(k))
+        return self
+
+
+class QuerySimilarImageClusterResponse(TeaModel):
+    """
+    query similar image cluster response
+    """
+    def __init__(
+        self,
+        next_marker: str = None,
+        similar_image_clusters: List[SimilarImageCluster] = None,
+    ):
+        self.next_marker = next_marker
+        self.similar_image_clusters = similar_image_clusters
+
+    def validate(self):
+        if self.similar_image_clusters:
+            for k in self.similar_image_clusters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_marker is not None:
+            result['next_marker'] = self.next_marker
+        result['similar_image_clusters'] = []
+        if self.similar_image_clusters is not None:
+            for k in self.similar_image_clusters:
+                result['similar_image_clusters'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('next_marker') is not None:
+            self.next_marker = m.get('next_marker')
+        self.similar_image_clusters = []
+        if m.get('similar_image_clusters') is not None:
+            for k in m.get('similar_image_clusters'):
+                temp_model = SimilarImageCluster()
+                self.similar_image_clusters.append(temp_model.from_map(k))
+        return self
+
+
+class QuerySimilarImageClustersModel(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: QuerySimilarImageClusterResponse = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = QuerySimilarImageClusterResponse()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveStoryFilesResponse(TeaModel):
     """
     remove story files response
@@ -27318,14 +28438,15 @@
         fields: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         file_revision_id: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         joined_at: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
@@ -27409,14 +28530,16 @@
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         self.file_revision_id = file_revision_id
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         self.joined_at = joined_at
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
@@ -27561,14 +28684,16 @@
             result['file_path_type'] = self.file_path_type
         if self.file_revision_id is not None:
             result['file_revision_id'] = self.file_revision_id
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.joined_at is not None:
             result['joined_at'] = self.joined_at
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
@@ -27694,14 +28819,16 @@
         if m.get('file_revision_id') is not None:
             self.file_revision_id = m.get('file_revision_id')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('joined_at') is not None:
             self.joined_at = m.get('joined_at')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
@@ -27921,14 +29048,15 @@
         fields: dict = None,
         file_extension: str = None,
         file_id: str = None,
         file_path_type: str = None,
         file_revision_id: str = None,
         hidden: bool = None,
         image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
         joined_at: int = None,
         labels: List[str] = None,
         last_modifier_id: str = None,
         last_modifier_name: str = None,
         last_modifier_type: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
@@ -28012,14 +29140,16 @@
         # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
         self.file_path_type = file_path_type
         self.file_revision_id = file_revision_id
         # Hidden
         # type: boolean
         self.hidden = hidden
         self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
         self.joined_at = joined_at
         # labels
         self.labels = labels
         # last_modifier_id
         self.last_modifier_id = last_modifier_id
         # last_modifier_name
         self.last_modifier_name = last_modifier_name
@@ -28164,14 +29294,16 @@
             result['file_path_type'] = self.file_path_type
         if self.file_revision_id is not None:
             result['file_revision_id'] = self.file_revision_id
         if self.hidden is not None:
             result['hidden'] = self.hidden
         if self.image_media_metadata is not None:
             result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
         if self.joined_at is not None:
             result['joined_at'] = self.joined_at
         if self.labels is not None:
             result['labels'] = self.labels
         if self.last_modifier_id is not None:
             result['last_modifier_id'] = self.last_modifier_id
         if self.last_modifier_name is not None:
@@ -28297,14 +29429,16 @@
         if m.get('file_revision_id') is not None:
             self.file_revision_id = m.get('file_revision_id')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
         if m.get('image_media_metadata') is not None:
             temp_model = ImageMediaResponse()
             self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
         if m.get('joined_at') is not None:
             self.joined_at = m.get('joined_at')
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('last_modifier_id') is not None:
             self.last_modifier_id = m.get('last_modifier_id')
         if m.get('last_modifier_name') is not None:
@@ -29027,14 +30161,221 @@
         if m.get('role_arn') is not None:
             self.role_arn = m.get('role_arn')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class StoryFile(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        drive_id: str = None,
+        file_id: str = None,
+        revision_id: str = None,
+    ):
+        self.drive_id = drive_id
+        self.file_id = file_id
+        self.revision_id = revision_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.revision_id is not None:
+            result['revision_id'] = self.revision_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('revision_id') is not None:
+            self.revision_id = m.get('revision_id')
+        return self
+
+
+class AddStoryFilesRequest(TeaModel):
+    """
+    add story files request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        files: List[StoryFile] = None,
+        story_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        self.files = files
+        # story_id
+        self.story_id = story_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.files:
+            for k in self.files:
+                if k:
+                    k.validate()
+        self.validate_required(self.story_id, 'story_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        result['files'] = []
+        if self.files is not None:
+            for k in self.files:
+                result['files'].append(k.to_map() if k else None)
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        self.files = []
+        if m.get('files') is not None:
+            for k in m.get('files'):
+                temp_model = StoryFile()
+                self.files.append(temp_model.from_map(k))
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        return self
+
+
+class AddViewFileRequest(TeaModel):
+    """
+    add file to view
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        drive_id: str = None,
+        fields: dict = None,
+        file_id: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        self.drive_id = drive_id
+        self.fields = fields
+        self.file_id = file_id
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.fields is not None:
+            result['fields'] = self.fields
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
+class AlbumsBaseRequest(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        drive_id: str = None,
+    ):
+        # drive_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
 class AppAccessStrategy(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         effect: str = None,
@@ -29723,14 +31064,45 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('addition_data') is not None:
             self.addition_data = m.get('addition_data')
         return self
 
 
+class BaseAdditionDataV2Request(TeaModel):
+    """
+    从value只支持string升级为支持所有类型的附加数据，按需升级
+    """
+    def __init__(
+        self,
+        addition_data: dict = None,
+    ):
+        # addition_data
+        self.addition_data = addition_data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
+        return self
+
+
 class BaseAuthentication(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         email: str = None,
@@ -29930,14 +31302,484 @@
         if m.get('size') is not None:
             self.size = m.get('size')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class BaseFileDeltaInfo(TeaModel):
+    """
+    the delta file info
+    """
+    def __init__(
+        self,
+        action_list: List[str] = None,
+        auto_delete_left_sec: int = None,
+        category: str = None,
+        characteristic_hash: str = None,
+        content_hash: str = None,
+        content_hash_name: str = None,
+        content_type: str = None,
+        crc_64hash: str = None,
+        created_at: str = None,
+        creator_id: str = None,
+        creator_name: str = None,
+        creator_type: str = None,
+        custom_field_1: str = None,
+        custom_field_2: str = None,
+        custom_type: str = None,
+        description: str = None,
+        domain_id: str = None,
+        download_url: str = None,
+        drive_id: str = None,
+        encrypt_mode: str = None,
+        ex_fields_info: dict = None,
+        file_extension: str = None,
+        file_id: str = None,
+        file_path_type: str = None,
+        hidden: bool = None,
+        image_media_metadata: ImageMediaResponse = None,
+        investigation_status: int = None,
+        labels: List[str] = None,
+        last_modifier_id: str = None,
+        last_modifier_name: str = None,
+        last_modifier_type: str = None,
+        local_created_at: str = None,
+        local_modified_at: str = None,
+        meta: str = None,
+        mime_extension: str = None,
+        mime_type: str = None,
+        name: str = None,
+        parent_file_id: str = None,
+        punish_flag: int = None,
+        punish_reason: str = None,
+        revision_id: str = None,
+        revision_version: int = None,
+        share_id: str = None,
+        size: int = None,
+        starred: bool = None,
+        status: str = None,
+        streams_info: dict = None,
+        sync_device_flag: bool = None,
+        sync_flag: bool = None,
+        sync_meta: str = None,
+        thumbnail: str = None,
+        thumbnail_urls: dict = None,
+        trashed_at: str = None,
+        type: str = None,
+        updated_at: str = None,
+        upload_id: str = None,
+        url: str = None,
+        user_meta: str = None,
+        user_tags: dict = None,
+        video_media_metadata: VideoMediaResponse = None,
+        video_preview_metadata: VideoPreviewResponse = None,
+    ):
+        # action_list
+        self.action_list = action_list
+        # auto_delete_left_sec
+        self.auto_delete_left_sec = auto_delete_left_sec
+        # category
+        self.category = category
+        # CharacteristicHash
+        self.characteristic_hash = characteristic_hash
+        # Content Hash
+        self.content_hash = content_hash
+        # content_hash_name
+        self.content_hash_name = content_hash_name
+        # content_type
+        self.content_type = content_type
+        # crc64_hash
+        self.crc_64hash = crc_64hash
+        # created_at
+        self.created_at = created_at
+        # creator_id
+        self.creator_id = creator_id
+        # creator_name
+        self.creator_name = creator_name
+        # creator_type
+        self.creator_type = creator_type
+        # custom_field_1
+        self.custom_field_1 = custom_field_1
+        # custom_field_2
+        self.custom_field_2 = custom_field_2
+        # custom_type
+        self.custom_type = custom_type
+        # description
+        self.description = description
+        # DomainID
+        self.domain_id = domain_id
+        # download_url
+        self.download_url = download_url
+        # drive_id
+        self.drive_id = drive_id
+        # encrypt_mode
+        self.encrypt_mode = encrypt_mode
+        # ex_fields_info
+        self.ex_fields_info = ex_fields_info
+        # file_extension
+        self.file_extension = file_extension
+        # file_id
+        self.file_id = file_id
+        # TODO 先不在API上透出该字段，file_path_type目前在edm中返回；path type是否在PDS通用逻辑中展示，展示的含义是什么，需要再做分析
+        self.file_path_type = file_path_type
+        # Hidden
+        # type: boolean
+        self.hidden = hidden
+        self.image_media_metadata = image_media_metadata
+        # InvestigationStatus
+        self.investigation_status = investigation_status
+        # labels
+        self.labels = labels
+        # last_modifier_id
+        self.last_modifier_id = last_modifier_id
+        # last_modifier_name
+        self.last_modifier_name = last_modifier_name
+        # last_modifier_type
+        self.last_modifier_type = last_modifier_type
+        # local_created_at
+        self.local_created_at = local_created_at
+        self.local_modified_at = local_modified_at
+        self.meta = meta
+        # mime_extension
+        self.mime_extension = mime_extension
+        # mime_type
+        self.mime_type = mime_type
+        # name
+        self.name = name
+        # parent_file_id
+        self.parent_file_id = parent_file_id
+        # PunishFlag
+        self.punish_flag = punish_flag
+        # PunishReason
+        self.punish_reason = punish_reason
+        # revision_id
+        self.revision_id = revision_id
+        # revision_version
+        self.revision_version = revision_version
+        self.share_id = share_id
+        # Size
+        self.size = size
+        # starred
+        # type: boolean
+        self.starred = starred
+        # status
+        self.status = status
+        # @Deprecated streams url info
+        self.streams_info = streams_info
+        # sync_device_flag
+        self.sync_device_flag = sync_device_flag
+        # sync_flag
+        self.sync_flag = sync_flag
+        # sync_meta
+        self.sync_meta = sync_meta
+        # thumbnail
+        self.thumbnail = thumbnail
+        # thumbnail_urls
+        self.thumbnail_urls = thumbnail_urls
+        # trashed_at
+        self.trashed_at = trashed_at
+        # type
+        self.type = type
+        # updated_at
+        self.updated_at = updated_at
+        # upload_id
+        self.upload_id = upload_id
+        # url
+        self.url = url
+        # user_meta
+        self.user_meta = user_meta
+        # user_tags
+        self.user_tags = user_tags
+        self.video_media_metadata = video_media_metadata
+        self.video_preview_metadata = video_preview_metadata
+
+    def validate(self):
+        if self.domain_id is not None:
+            self.validate_pattern(self.domain_id, 'domain_id', '[a-z0-9A-Z]+')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.file_id is not None:
+            self.validate_max_length(self.file_id, 'file_id', 50)
+            self.validate_pattern(self.file_id, 'file_id', '[a-z0-9]{1,50}')
+        if self.image_media_metadata:
+            self.image_media_metadata.validate()
+        self.validate_required(self.name, 'name')
+        if self.name is not None:
+            self.validate_pattern(self.name, 'name', '[a-zA-Z0-9.-]{1,1000}')
+        if self.parent_file_id is not None:
+            self.validate_max_length(self.parent_file_id, 'parent_file_id', 50)
+            self.validate_pattern(self.parent_file_id, 'parent_file_id', '[a-z0-9]{1,50}')
+        if self.size is not None:
+            self.validate_minimum(self.size, 'size', 0)
+        if self.video_media_metadata:
+            self.video_media_metadata.validate()
+        if self.video_preview_metadata:
+            self.video_preview_metadata.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action_list is not None:
+            result['action_list'] = self.action_list
+        if self.auto_delete_left_sec is not None:
+            result['auto_delete_left_sec'] = self.auto_delete_left_sec
+        if self.category is not None:
+            result['category'] = self.category
+        if self.characteristic_hash is not None:
+            result['characteristic_hash'] = self.characteristic_hash
+        if self.content_hash is not None:
+            result['content_hash'] = self.content_hash
+        if self.content_hash_name is not None:
+            result['content_hash_name'] = self.content_hash_name
+        if self.content_type is not None:
+            result['content_type'] = self.content_type
+        if self.crc_64hash is not None:
+            result['crc64_hash'] = self.crc_64hash
+        if self.created_at is not None:
+            result['created_at'] = self.created_at
+        if self.creator_id is not None:
+            result['creator_id'] = self.creator_id
+        if self.creator_name is not None:
+            result['creator_name'] = self.creator_name
+        if self.creator_type is not None:
+            result['creator_type'] = self.creator_type
+        if self.custom_field_1 is not None:
+            result['custom_field_1'] = self.custom_field_1
+        if self.custom_field_2 is not None:
+            result['custom_field_2'] = self.custom_field_2
+        if self.custom_type is not None:
+            result['custom_type'] = self.custom_type
+        if self.description is not None:
+            result['description'] = self.description
+        if self.domain_id is not None:
+            result['domain_id'] = self.domain_id
+        if self.download_url is not None:
+            result['download_url'] = self.download_url
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.encrypt_mode is not None:
+            result['encrypt_mode'] = self.encrypt_mode
+        if self.ex_fields_info is not None:
+            result['ex_fields_info'] = self.ex_fields_info
+        if self.file_extension is not None:
+            result['file_extension'] = self.file_extension
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.file_path_type is not None:
+            result['file_path_type'] = self.file_path_type
+        if self.hidden is not None:
+            result['hidden'] = self.hidden
+        if self.image_media_metadata is not None:
+            result['image_media_metadata'] = self.image_media_metadata.to_map()
+        if self.investigation_status is not None:
+            result['investigation_status'] = self.investigation_status
+        if self.labels is not None:
+            result['labels'] = self.labels
+        if self.last_modifier_id is not None:
+            result['last_modifier_id'] = self.last_modifier_id
+        if self.last_modifier_name is not None:
+            result['last_modifier_name'] = self.last_modifier_name
+        if self.last_modifier_type is not None:
+            result['last_modifier_type'] = self.last_modifier_type
+        if self.local_created_at is not None:
+            result['local_created_at'] = self.local_created_at
+        if self.local_modified_at is not None:
+            result['local_modified_at'] = self.local_modified_at
+        if self.meta is not None:
+            result['meta'] = self.meta
+        if self.mime_extension is not None:
+            result['mime_extension'] = self.mime_extension
+        if self.mime_type is not None:
+            result['mime_type'] = self.mime_type
+        if self.name is not None:
+            result['name'] = self.name
+        if self.parent_file_id is not None:
+            result['parent_file_id'] = self.parent_file_id
+        if self.punish_flag is not None:
+            result['punish_flag'] = self.punish_flag
+        if self.punish_reason is not None:
+            result['punish_reason'] = self.punish_reason
+        if self.revision_id is not None:
+            result['revision_id'] = self.revision_id
+        if self.revision_version is not None:
+            result['revision_version'] = self.revision_version
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
+        if self.size is not None:
+            result['size'] = self.size
+        if self.starred is not None:
+            result['starred'] = self.starred
+        if self.status is not None:
+            result['status'] = self.status
+        if self.streams_info is not None:
+            result['streams_info'] = self.streams_info
+        if self.sync_device_flag is not None:
+            result['sync_device_flag'] = self.sync_device_flag
+        if self.sync_flag is not None:
+            result['sync_flag'] = self.sync_flag
+        if self.sync_meta is not None:
+            result['sync_meta'] = self.sync_meta
+        if self.thumbnail is not None:
+            result['thumbnail'] = self.thumbnail
+        if self.thumbnail_urls is not None:
+            result['thumbnail_urls'] = self.thumbnail_urls
+        if self.trashed_at is not None:
+            result['trashed_at'] = self.trashed_at
+        if self.type is not None:
+            result['type'] = self.type
+        if self.updated_at is not None:
+            result['updated_at'] = self.updated_at
+        if self.upload_id is not None:
+            result['upload_id'] = self.upload_id
+        if self.url is not None:
+            result['url'] = self.url
+        if self.user_meta is not None:
+            result['user_meta'] = self.user_meta
+        if self.user_tags is not None:
+            result['user_tags'] = self.user_tags
+        if self.video_media_metadata is not None:
+            result['video_media_metadata'] = self.video_media_metadata.to_map()
+        if self.video_preview_metadata is not None:
+            result['video_preview_metadata'] = self.video_preview_metadata.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action_list') is not None:
+            self.action_list = m.get('action_list')
+        if m.get('auto_delete_left_sec') is not None:
+            self.auto_delete_left_sec = m.get('auto_delete_left_sec')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('characteristic_hash') is not None:
+            self.characteristic_hash = m.get('characteristic_hash')
+        if m.get('content_hash') is not None:
+            self.content_hash = m.get('content_hash')
+        if m.get('content_hash_name') is not None:
+            self.content_hash_name = m.get('content_hash_name')
+        if m.get('content_type') is not None:
+            self.content_type = m.get('content_type')
+        if m.get('crc64_hash') is not None:
+            self.crc_64hash = m.get('crc64_hash')
+        if m.get('created_at') is not None:
+            self.created_at = m.get('created_at')
+        if m.get('creator_id') is not None:
+            self.creator_id = m.get('creator_id')
+        if m.get('creator_name') is not None:
+            self.creator_name = m.get('creator_name')
+        if m.get('creator_type') is not None:
+            self.creator_type = m.get('creator_type')
+        if m.get('custom_field_1') is not None:
+            self.custom_field_1 = m.get('custom_field_1')
+        if m.get('custom_field_2') is not None:
+            self.custom_field_2 = m.get('custom_field_2')
+        if m.get('custom_type') is not None:
+            self.custom_type = m.get('custom_type')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('domain_id') is not None:
+            self.domain_id = m.get('domain_id')
+        if m.get('download_url') is not None:
+            self.download_url = m.get('download_url')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('encrypt_mode') is not None:
+            self.encrypt_mode = m.get('encrypt_mode')
+        if m.get('ex_fields_info') is not None:
+            self.ex_fields_info = m.get('ex_fields_info')
+        if m.get('file_extension') is not None:
+            self.file_extension = m.get('file_extension')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('file_path_type') is not None:
+            self.file_path_type = m.get('file_path_type')
+        if m.get('hidden') is not None:
+            self.hidden = m.get('hidden')
+        if m.get('image_media_metadata') is not None:
+            temp_model = ImageMediaResponse()
+            self.image_media_metadata = temp_model.from_map(m['image_media_metadata'])
+        if m.get('investigation_status') is not None:
+            self.investigation_status = m.get('investigation_status')
+        if m.get('labels') is not None:
+            self.labels = m.get('labels')
+        if m.get('last_modifier_id') is not None:
+            self.last_modifier_id = m.get('last_modifier_id')
+        if m.get('last_modifier_name') is not None:
+            self.last_modifier_name = m.get('last_modifier_name')
+        if m.get('last_modifier_type') is not None:
+            self.last_modifier_type = m.get('last_modifier_type')
+        if m.get('local_created_at') is not None:
+            self.local_created_at = m.get('local_created_at')
+        if m.get('local_modified_at') is not None:
+            self.local_modified_at = m.get('local_modified_at')
+        if m.get('meta') is not None:
+            self.meta = m.get('meta')
+        if m.get('mime_extension') is not None:
+            self.mime_extension = m.get('mime_extension')
+        if m.get('mime_type') is not None:
+            self.mime_type = m.get('mime_type')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('parent_file_id') is not None:
+            self.parent_file_id = m.get('parent_file_id')
+        if m.get('punish_flag') is not None:
+            self.punish_flag = m.get('punish_flag')
+        if m.get('punish_reason') is not None:
+            self.punish_reason = m.get('punish_reason')
+        if m.get('revision_id') is not None:
+            self.revision_id = m.get('revision_id')
+        if m.get('revision_version') is not None:
+            self.revision_version = m.get('revision_version')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('starred') is not None:
+            self.starred = m.get('starred')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('streams_info') is not None:
+            self.streams_info = m.get('streams_info')
+        if m.get('sync_device_flag') is not None:
+            self.sync_device_flag = m.get('sync_device_flag')
+        if m.get('sync_flag') is not None:
+            self.sync_flag = m.get('sync_flag')
+        if m.get('sync_meta') is not None:
+            self.sync_meta = m.get('sync_meta')
+        if m.get('thumbnail') is not None:
+            self.thumbnail = m.get('thumbnail')
+        if m.get('thumbnail_urls') is not None:
+            self.thumbnail_urls = m.get('thumbnail_urls')
+        if m.get('trashed_at') is not None:
+            self.trashed_at = m.get('trashed_at')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('updated_at') is not None:
+            self.updated_at = m.get('updated_at')
+        if m.get('upload_id') is not None:
+            self.upload_id = m.get('upload_id')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        if m.get('user_meta') is not None:
+            self.user_meta = m.get('user_meta')
+        if m.get('user_tags') is not None:
+            self.user_tags = m.get('user_tags')
+        if m.get('video_media_metadata') is not None:
+            temp_model = VideoMediaResponse()
+            self.video_media_metadata = temp_model.from_map(m['video_media_metadata'])
+        if m.get('video_preview_metadata') is not None:
+            temp_model = VideoPreviewResponse()
+            self.video_preview_metadata = temp_model.from_map(m['video_preview_metadata'])
+        return self
+
+
 class BaseFileProcessRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         image_cropping_aspect_ratios: List[str] = None,
@@ -30577,14 +32419,60 @@
         if m.get('new_name') is not None:
             self.new_name = m.get('new_name')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         return self
 
 
+class BaseRequest(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        category: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        # category
+        self.category = category
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.category is not None:
+            result['category'] = self.category
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class BaseRevisionRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         drive_id: str = None,
@@ -30901,30 +32789,36 @@
     打包下载
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         drive_id: str = None,
+        file_ids: List[str] = None,
         files: List[FileInfo] = None,
         name: str = None,
+        recursive: bool = None,
         referer: str = None,
         share_id: str = None,
+        task_category: str = None,
     ):
         self.httpheaders = httpheaders
         # addition_data
         self.addition_data = addition_data
         # drive_id
         self.drive_id = drive_id
+        self.file_ids = file_ids
         self.files = files
         # file_name
         self.name = name
+        self.recursive = recursive
         self.referer = referer
         # share_id, either share_id or drive_id is required
         self.share_id = share_id
+        self.task_category = task_category
 
     def validate(self):
         if self.drive_id is not None:
             self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
         if self.files:
             for k in self.files:
                 if k:
@@ -30940,45 +32834,57 @@
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
         if self.addition_data is not None:
             result['addition_data'] = self.addition_data
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.file_ids is not None:
+            result['file_ids'] = self.file_ids
         result['files'] = []
         if self.files is not None:
             for k in self.files:
                 result['files'].append(k.to_map() if k else None)
         if self.name is not None:
             result['name'] = self.name
+        if self.recursive is not None:
+            result['recursive'] = self.recursive
         if self.referer is not None:
             result['referer'] = self.referer
         if self.share_id is not None:
             result['share_id'] = self.share_id
+        if self.task_category is not None:
+            result['task_category'] = self.task_category
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('addition_data') is not None:
             self.addition_data = m.get('addition_data')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('file_ids') is not None:
+            self.file_ids = m.get('file_ids')
         self.files = []
         if m.get('files') is not None:
             for k in m.get('files'):
                 temp_model = FileInfo()
                 self.files.append(temp_model.from_map(k))
         if m.get('name') is not None:
             self.name = m.get('name')
+        if m.get('recursive') is not None:
+            self.recursive = m.get('recursive')
         if m.get('referer') is not None:
             self.referer = m.get('referer')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
+        if m.get('task_category') is not None:
+            self.task_category = m.get('task_category')
         return self
 
 
 class CCPArchiveRequest(TeaModel):
     """
     *\
     """
@@ -31385,14 +33291,15 @@
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         category: str = None,
         drive_id: str = None,
         file_id: str = None,
         file_id_path: str = None,
+        get_master_url: bool = None,
         get_preview_url: bool = None,
         get_subtitle_info: bool = None,
         get_without_url: bool = None,
         location: str = None,
         referer: str = None,
         revision_id: str = None,
         share_id: str = None,
@@ -31407,14 +33314,16 @@
         # category
         self.category = category
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         self.file_id_path = file_id_path
+        # 获取master playlist播放地址，仅在quick_video中有效
+        self.get_master_url = get_master_url
         # get_preview_url
         self.get_preview_url = get_preview_url
         # get_subtitle_info
         self.get_subtitle_info = get_subtitle_info
         # get_without_url
         self.get_without_url = get_without_url
         # location
@@ -31456,14 +33365,16 @@
             result['category'] = self.category
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.file_id_path is not None:
             result['file_id_path'] = self.file_id_path
+        if self.get_master_url is not None:
+            result['get_master_url'] = self.get_master_url
         if self.get_preview_url is not None:
             result['get_preview_url'] = self.get_preview_url
         if self.get_subtitle_info is not None:
             result['get_subtitle_info'] = self.get_subtitle_info
         if self.get_without_url is not None:
             result['get_without_url'] = self.get_without_url
         if self.location is not None:
@@ -31494,14 +33405,16 @@
             self.category = m.get('category')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('file_id_path') is not None:
             self.file_id_path = m.get('file_id_path')
+        if m.get('get_master_url') is not None:
+            self.get_master_url = m.get('get_master_url')
         if m.get('get_preview_url') is not None:
             self.get_preview_url = m.get('get_preview_url')
         if m.get('get_subtitle_info') is not None:
             self.get_subtitle_info = m.get('get_subtitle_info')
         if m.get('get_without_url') is not None:
             self.get_without_url = m.get('get_without_url')
         if m.get('location') is not None:
@@ -32201,42 +34114,55 @@
 class ClearRecycleBinRequest(TeaModel):
     """
     清空回收站
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
         drive_id: str = None,
+        task_category: str = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         # drive_id
         self.drive_id = drive_id
+        self.task_category = task_category
 
     def validate(self):
         if self.drive_id is not None:
             self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.task_category is not None:
+            result['task_category'] = self.task_category
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('task_category') is not None:
+            self.task_category = m.get('task_category')
         return self
 
 
 class CompleteFileRequest(TeaModel):
     """
     合并文件上传任务
     """
@@ -32367,27 +34293,64 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('temporary_token') is not None:
             self.temporary_token = m.get('temporary_token')
         return self
 
 
+class KeepUserTags(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        all: bool = None,
+        keys: List[str] = None,
+    ):
+        self.all = all
+        self.keys = keys
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all is not None:
+            result['all'] = self.all
+        if self.keys is not None:
+            result['keys'] = self.keys
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('all') is not None:
+            self.all = m.get('all')
+        if m.get('keys') is not None:
+            self.keys = m.get('keys')
+        return self
+
+
 class CopyFileRequest(TeaModel):
     """
     文件拷贝
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         auto_rename: bool = None,
         batch_id: str = None,
         drive_id: str = None,
         file_id: str = None,
         file_id_path: str = None,
+        keep_user_tags: KeepUserTags = None,
         new_name: str = None,
         referer: str = None,
         share_id: str = None,
         to_drive_id: str = None,
         to_parent_file_id: str = None,
         to_share_id: str = None,
     ):
@@ -32399,14 +34362,15 @@
         self.auto_rename = auto_rename
         self.batch_id = batch_id
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         self.file_id_path = file_id_path
+        self.keep_user_tags = keep_user_tags
         # new_name
         self.new_name = new_name
         self.referer = referer
         # share_id, either share_id or drive_id is required
         self.share_id = share_id
         # to_drive_id
         self.to_drive_id = to_drive_id
@@ -32418,14 +34382,16 @@
     def validate(self):
         if self.drive_id is not None:
             self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
         self.validate_required(self.file_id, 'file_id')
         if self.file_id is not None:
             self.validate_max_length(self.file_id, 'file_id', 50)
             self.validate_pattern(self.file_id, 'file_id', '[a-z0-9.-_]{1,50}')
+        if self.keep_user_tags:
+            self.keep_user_tags.validate()
         if self.new_name is not None:
             self.validate_max_length(self.new_name, 'new_name', 1024)
         if self.to_drive_id is not None:
             self.validate_pattern(self.to_drive_id, 'to_drive_id', '[0-9]+')
         self.validate_required(self.to_parent_file_id, 'to_parent_file_id')
         if self.to_parent_file_id is not None:
             self.validate_max_length(self.to_parent_file_id, 'to_parent_file_id', 50)
@@ -32449,14 +34415,16 @@
             result['batch_id'] = self.batch_id
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.file_id_path is not None:
             result['file_id_path'] = self.file_id_path
+        if self.keep_user_tags is not None:
+            result['keep_user_tags'] = self.keep_user_tags.to_map()
         if self.new_name is not None:
             result['new_name'] = self.new_name
         if self.referer is not None:
             result['referer'] = self.referer
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.to_drive_id is not None:
@@ -32479,14 +34447,17 @@
             self.batch_id = m.get('batch_id')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('file_id_path') is not None:
             self.file_id_path = m.get('file_id_path')
+        if m.get('keep_user_tags') is not None:
+            temp_model = KeepUserTags()
+            self.keep_user_tags = temp_model.from_map(m['keep_user_tags'])
         if m.get('new_name') is not None:
             self.new_name = m.get('new_name')
         if m.get('referer') is not None:
             self.referer = m.get('referer')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('to_drive_id') is not None:
@@ -32494,14 +34465,137 @@
         if m.get('to_parent_file_id') is not None:
             self.to_parent_file_id = m.get('to_parent_file_id')
         if m.get('to_share_id') is not None:
             self.to_share_id = m.get('to_share_id')
         return self
 
 
+class CopyViewFilesRequest(TeaModel):
+    """
+    Copy view files
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
+        auto_rename: bool = None,
+        category: str = None,
+        drive_file_list: List[ShareFile] = None,
+        referer: str = None,
+        share_id: str = None,
+        to_drive_id: str = None,
+        to_parent_file_id: str = None,
+        to_view_id: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
+        # auto_rename
+        # type: boolean
+        self.auto_rename = auto_rename
+        # category
+        self.category = category
+        self.drive_file_list = drive_file_list
+        self.referer = referer
+        # share_id
+        self.share_id = share_id
+        # to_drive_id
+        self.to_drive_id = to_drive_id
+        # to_parent_file_id
+        self.to_parent_file_id = to_parent_file_id
+        # to_view_id
+        self.to_view_id = to_view_id
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        if self.drive_file_list:
+            for k in self.drive_file_list:
+                if k:
+                    k.validate()
+        if self.to_drive_id is not None:
+            self.validate_pattern(self.to_drive_id, 'to_drive_id', '[0-9]+')
+        self.validate_required(self.to_parent_file_id, 'to_parent_file_id')
+        if self.to_parent_file_id is not None:
+            self.validate_max_length(self.to_parent_file_id, 'to_parent_file_id', 50)
+            self.validate_pattern(self.to_parent_file_id, 'to_parent_file_id', '[a-z0-9.-_]{1,50}')
+        self.validate_required(self.to_view_id, 'to_view_id')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
+        if self.auto_rename is not None:
+            result['auto_rename'] = self.auto_rename
+        if self.category is not None:
+            result['category'] = self.category
+        result['drive_file_list'] = []
+        if self.drive_file_list is not None:
+            for k in self.drive_file_list:
+                result['drive_file_list'].append(k.to_map() if k else None)
+        if self.referer is not None:
+            result['referer'] = self.referer
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
+        if self.to_drive_id is not None:
+            result['to_drive_id'] = self.to_drive_id
+        if self.to_parent_file_id is not None:
+            result['to_parent_file_id'] = self.to_parent_file_id
+        if self.to_view_id is not None:
+            result['to_view_id'] = self.to_view_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
+        if m.get('auto_rename') is not None:
+            self.auto_rename = m.get('auto_rename')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        self.drive_file_list = []
+        if m.get('drive_file_list') is not None:
+            for k in m.get('drive_file_list'):
+                temp_model = ShareFile()
+                self.drive_file_list.append(temp_model.from_map(k))
+        if m.get('referer') is not None:
+            self.referer = m.get('referer')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
+        if m.get('to_drive_id') is not None:
+            self.to_drive_id = m.get('to_drive_id')
+        if m.get('to_parent_file_id') is not None:
+            self.to_parent_file_id = m.get('to_parent_file_id')
+        if m.get('to_view_id') is not None:
+            self.to_view_id = m.get('to_view_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class CorsRule(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         allowed_header: List[str] = None,
@@ -32641,14 +34735,107 @@
         if m.get('scope') is not None:
             self.scope = m.get('scope')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class CreateCustomizedStoryRequest(TeaModel):
+    """
+    # Create custom story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        custom_labels: dict = None,
+        drive_id: str = None,
+        story_cover: StoryFile = None,
+        story_files: List[StoryFile] = None,
+        story_name: str = None,
+        story_sub_type: str = None,
+        story_type: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # custom_labels
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        self.story_cover = story_cover
+        # story_file_ids
+        self.story_files = story_files
+        # story_name
+        self.story_name = story_name
+        # story_sub_type
+        self.story_sub_type = story_sub_type
+        # story_type
+        self.story_type = story_type
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.story_cover:
+            self.story_cover.validate()
+        if self.story_files:
+            for k in self.story_files:
+                if k:
+                    k.validate()
+        self.validate_required(self.story_type, 'story_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.story_cover is not None:
+            result['story_cover'] = self.story_cover.to_map()
+        result['story_files'] = []
+        if self.story_files is not None:
+            for k in self.story_files:
+                result['story_files'].append(k.to_map() if k else None)
+        if self.story_name is not None:
+            result['story_name'] = self.story_name
+        if self.story_sub_type is not None:
+            result['story_sub_type'] = self.story_sub_type
+        if self.story_type is not None:
+            result['story_type'] = self.story_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('story_cover') is not None:
+            temp_model = StoryFile()
+            self.story_cover = temp_model.from_map(m['story_cover'])
+        self.story_files = []
+        if m.get('story_files') is not None:
+            for k in m.get('story_files'):
+                temp_model = StoryFile()
+                self.story_files.append(temp_model.from_map(k))
+        if m.get('story_name') is not None:
+            self.story_name = m.get('story_name')
+        if m.get('story_sub_type') is not None:
+            self.story_sub_type = m.get('story_sub_type')
+        if m.get('story_type') is not None:
+            self.story_type = m.get('story_type')
+        return self
+
+
 class CreateDomainRequest(TeaModel):
     """
     create domain request
     """
     def __init__(
         self,
         auth_config: dict = None,
@@ -33101,14 +35288,15 @@
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         auto_rename: bool = None,
         category: str = None,
         check_name_mode: str = None,
+        check_parent_file_id_path: str = None,
         content_hash: str = None,
         content_hash_name: str = None,
         content_md_5: str = None,
         content_type: str = None,
         create_reason: str = None,
         custom_field_1: str = None,
         custom_field_2: str = None,
@@ -33150,14 +35338,15 @@
         # addition_data
         self.addition_data = addition_data
         self.auto_rename = auto_rename
         # category
         self.category = category
         # check_name_mode
         self.check_name_mode = check_name_mode
+        self.check_parent_file_id_path = check_parent_file_id_path
         # content_hash
         self.content_hash = content_hash
         # content_hash_name
         self.content_hash_name = content_hash_name
         # ContentMd5
         self.content_md_5 = content_md_5
         # ContentType
@@ -33262,14 +35451,16 @@
             result['addition_data'] = self.addition_data
         if self.auto_rename is not None:
             result['auto_rename'] = self.auto_rename
         if self.category is not None:
             result['category'] = self.category
         if self.check_name_mode is not None:
             result['check_name_mode'] = self.check_name_mode
+        if self.check_parent_file_id_path is not None:
+            result['check_parent_file_id_path'] = self.check_parent_file_id_path
         if self.content_hash is not None:
             result['content_hash'] = self.content_hash
         if self.content_hash_name is not None:
             result['content_hash_name'] = self.content_hash_name
         if self.content_md_5 is not None:
             result['content_md5'] = self.content_md_5
         if self.content_type is not None:
@@ -33360,14 +35551,16 @@
             self.addition_data = m.get('addition_data')
         if m.get('auto_rename') is not None:
             self.auto_rename = m.get('auto_rename')
         if m.get('category') is not None:
             self.category = m.get('category')
         if m.get('check_name_mode') is not None:
             self.check_name_mode = m.get('check_name_mode')
+        if m.get('check_parent_file_id_path') is not None:
+            self.check_parent_file_id_path = m.get('check_parent_file_id_path')
         if m.get('content_hash') is not None:
             self.content_hash = m.get('content_hash')
         if m.get('content_hash_name') is not None:
             self.content_hash_name = m.get('content_hash_name')
         if m.get('content_md5') is not None:
             self.content_md_5 = m.get('content_md5')
         if m.get('content_type') is not None:
@@ -33584,14 +35777,15 @@
         filter_group: str = None,
         office_editable: bool = None,
         preview_limit: int = None,
         referer: str = None,
         require_login: bool = None,
         save_download_limit: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_icon: str = None,
         share_name: str = None,
         share_pwd: str = None,
         user_id: str = None,
         view_id: str = None,
     ):
         self.httpheaders = httpheaders
@@ -33641,14 +35835,16 @@
         self.referer = referer
         # 企业内(domain)登录后才允许使用分享
         self.require_login = require_login
         # 分享转存和下载的总次数限制
         self.save_download_limit = save_download_limit
         # 分享转存次数限制
         self.save_limit = save_limit
+        # 是否分享整个drive中的文件，仅文件分享才有效，true时file_id_list字段无效
+        self.share_all_files = share_all_files
         # share_icon
         self.share_icon = share_icon
         # share_name
         self.share_name = share_name
         # share_pwd
         self.share_pwd = share_pwd
         # user_id, only admin or aksk can set
@@ -33720,14 +35916,16 @@
             result['referer'] = self.referer
         if self.require_login is not None:
             result['require_login'] = self.require_login
         if self.save_download_limit is not None:
             result['save_download_limit'] = self.save_download_limit
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_icon is not None:
             result['share_icon'] = self.share_icon
         if self.share_name is not None:
             result['share_name'] = self.share_name
         if self.share_pwd is not None:
             result['share_pwd'] = self.share_pwd
         if self.user_id is not None:
@@ -33789,14 +35987,16 @@
             self.referer = m.get('referer')
         if m.get('require_login') is not None:
             self.require_login = m.get('require_login')
         if m.get('save_download_limit') is not None:
             self.save_download_limit = m.get('save_download_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_icon') is not None:
             self.share_icon = m.get('share_icon')
         if m.get('share_name') is not None:
             self.share_name = m.get('share_name')
         if m.get('share_pwd') is not None:
             self.share_pwd = m.get('share_pwd')
         if m.get('user_id') is not None:
@@ -33923,14 +36123,239 @@
                 temp_model = SharePermissionPolicy()
                 self.share_policy.append(temp_model.from_map(k))
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
+class CreateSimilarImageClusterTaskRequest(TeaModel):
+    """
+    create similar image cluster task request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
+class CreateStoryRequest(TeaModel):
+    """
+    # Create story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        address: Address = None,
+        custom_id: str = None,
+        custom_labels: dict = None,
+        drive_id: str = None,
+        max_image_count: int = None,
+        min_image_count: int = None,
+        story_end_time: str = None,
+        story_id: str = None,
+        story_name: str = None,
+        story_start_time: str = None,
+        story_sub_type: str = None,
+        story_type: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.address = address
+        # custom_id
+        self.custom_id = custom_id
+        # custom_labels
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        # max_image_count
+        self.max_image_count = max_image_count
+        # min_image_count
+        self.min_image_count = min_image_count
+        # story_end_time
+        self.story_end_time = story_end_time
+        # story_id
+        self.story_id = story_id
+        # story_name
+        self.story_name = story_name
+        # story_start_time
+        self.story_start_time = story_start_time
+        # story_sub_type
+        self.story_sub_type = story_sub_type
+        # story_type
+        self.story_type = story_type
+
+    def validate(self):
+        if self.address:
+            self.address.validate()
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.story_type, 'story_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.address is not None:
+            result['address'] = self.address.to_map()
+        if self.custom_id is not None:
+            result['custom_id'] = self.custom_id
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.max_image_count is not None:
+            result['max_image_count'] = self.max_image_count
+        if self.min_image_count is not None:
+            result['min_image_count'] = self.min_image_count
+        if self.story_end_time is not None:
+            result['story_end_time'] = self.story_end_time
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        if self.story_name is not None:
+            result['story_name'] = self.story_name
+        if self.story_start_time is not None:
+            result['story_start_time'] = self.story_start_time
+        if self.story_sub_type is not None:
+            result['story_sub_type'] = self.story_sub_type
+        if self.story_type is not None:
+            result['story_type'] = self.story_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('address') is not None:
+            temp_model = Address()
+            self.address = temp_model.from_map(m['address'])
+        if m.get('custom_id') is not None:
+            self.custom_id = m.get('custom_id')
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('max_image_count') is not None:
+            self.max_image_count = m.get('max_image_count')
+        if m.get('min_image_count') is not None:
+            self.min_image_count = m.get('min_image_count')
+        if m.get('story_end_time') is not None:
+            self.story_end_time = m.get('story_end_time')
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        if m.get('story_name') is not None:
+            self.story_name = m.get('story_name')
+        if m.get('story_start_time') is not None:
+            self.story_start_time = m.get('story_start_time')
+        if m.get('story_sub_type') is not None:
+            self.story_sub_type = m.get('story_sub_type')
+        if m.get('story_type') is not None:
+            self.story_type = m.get('story_type')
+        return self
+
+
+class CreateViewRequest(TeaModel):
+    """
+    Create view request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        description: str = None,
+        name: str = None,
+        owner: str = None,
+        user_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # description
+        self.description = description
+        # name
+        self.name = name
+        # owner
+        self.owner = owner
+        # user_id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.owner, 'owner')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.description is not None:
+            result['description'] = self.description
+        if self.name is not None:
+            result['name'] = self.name
+        if self.owner is not None:
+            result['owner'] = self.owner
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
 class CustomBenefitMetaRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         enabled: bool = None,
@@ -34347,25 +36772,27 @@
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         return self
 
 
 class DeleteDriveRequest(TeaModel):
     """
-    Delete drive request
+    # Delete drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         drive_id: str = None,
+        force: bool = None,
         subdomain_id: str = None,
     ):
         self.httpheaders = httpheaders
         # Drive ID
         self.drive_id = drive_id
+        self.force = force
         # Subdomain ID
         self.subdomain_id = subdomain_id
 
     def validate(self):
         self.validate_required(self.drive_id, 'drive_id')
 
     def to_map(self):
@@ -34374,24 +36801,28 @@
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.force is not None:
+            result['force'] = self.force
         if self.subdomain_id is not None:
             result['subdomain_id'] = self.subdomain_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('force') is not None:
+            self.force = m.get('force')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
 class DeleteDriveResponse(TeaModel):
     """
@@ -34419,21 +36850,23 @@
 class DeleteFileRequest(TeaModel):
     """
     删除文件请求
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        check_folder_empty: bool = None,
         drive_id: str = None,
         file_id: str = None,
         file_id_path: str = None,
         permanently: bool = None,
         share_id: str = None,
     ):
         self.httpheaders = httpheaders
+        self.check_folder_empty = check_folder_empty
         # drive_id
         self.drive_id = drive_id
         self.file_id = file_id
         self.file_id_path = file_id_path
         # permanently
         # type: false
         self.permanently = permanently
@@ -34447,14 +36880,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.check_folder_empty is not None:
+            result['check_folder_empty'] = self.check_folder_empty
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.file_id_path is not None:
             result['file_id_path'] = self.file_id_path
         if self.permanently is not None:
@@ -34463,14 +36898,16 @@
             result['share_id'] = self.share_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('check_folder_empty') is not None:
+            self.check_folder_empty = m.get('check_folder_empty')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('file_id_path') is not None:
             self.file_id_path = m.get('file_id_path')
         if m.get('permanently') is not None:
@@ -34483,19 +36920,22 @@
 class DeleteFileUserTagsRequest(TeaModel):
     """
     删除文件 user_tags 字段
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
         drive_id: str = None,
         file_id: str = None,
         key_list: List[str] = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         # key_list
         self.key_list = key_list
 
@@ -34512,26 +36952,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.key_list is not None:
             result['key_list'] = self.key_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('key_list') is not None:
             self.key_list = m.get('key_list')
         return self
@@ -34651,14 +37095,59 @@
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         return self
 
 
+class DeleteLocationDateClusterRequest(TeaModel):
+    """
+    delete locationCluster request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        cluster_id: str = None,
+        drive_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.cluster_id = cluster_id
+        # drive_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.cluster_id is not None:
+            result['cluster_id'] = self.cluster_id
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('cluster_id') is not None:
+            self.cluster_id = m.get('cluster_id')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
 class DeleteRevisionRequest(TeaModel):
     """
     删除历史版本元数据
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -34749,14 +37238,113 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         return self
 
 
+class DeleteStoryRequest(TeaModel):
+    """
+    delete story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        story_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # story_id
+        self.story_id = story_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.story_id, 'story_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        return self
+
+
+class DeleteViewRequest(TeaModel):
+    """
+    Delete view request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class DeviceAuthorizeRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         client_id: str = None,
@@ -35337,14 +37925,209 @@
         if m.get('proof_version') is not None:
             self.proof_version = m.get('proof_version')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
+class QueryRequestTimeRange(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        end: str = None,
+        start: str = None,
+    ):
+        # end
+        self.end = end
+        # start
+        self.start = start
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end is not None:
+            result['end'] = self.end
+        if self.start is not None:
+            result['start'] = self.start
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('end') is not None:
+            self.end = m.get('end')
+        if m.get('start') is not None:
+            self.start = m.get('start')
+        return self
+
+
+class FindStoriesRequest(TeaModel):
+    """
+    find story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        cover_image_thumbnail_process: str = None,
+        cover_video_thumbnail_process: str = None,
+        create_time_range: QueryRequestTimeRange = None,
+        custom_labels: str = None,
+        drive_id: str = None,
+        face_group_ids: List[str] = None,
+        limit: int = None,
+        marker: str = None,
+        order: str = None,
+        sort: str = None,
+        story_end_time_range: QueryRequestTimeRange = None,
+        story_id: str = None,
+        story_name: str = None,
+        story_start_time_range: QueryRequestTimeRange = None,
+        story_type: str = None,
+        url_expire_sec: int = None,
+        with_empty_stories: bool = None,
+    ):
+        self.httpheaders = httpheaders
+        # cover_image_thumbnail_process
+        self.cover_image_thumbnail_process = cover_image_thumbnail_process
+        # cover_video_thumbnail_process
+        self.cover_video_thumbnail_process = cover_video_thumbnail_process
+        self.create_time_range = create_time_range
+        # custom_labels
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        # face_group_ids
+        self.face_group_ids = face_group_ids
+        # limit
+        self.limit = limit
+        # marker
+        self.marker = marker
+        # order
+        self.order = order
+        # sort
+        self.sort = sort
+        self.story_end_time_range = story_end_time_range
+        # story_id
+        self.story_id = story_id
+        # story_name
+        self.story_name = story_name
+        self.story_start_time_range = story_start_time_range
+        # story_type
+        self.story_type = story_type
+        # url_expire_sec
+        self.url_expire_sec = url_expire_sec
+        # with_empty_stories
+        self.with_empty_stories = with_empty_stories
+
+    def validate(self):
+        if self.create_time_range:
+            self.create_time_range.validate()
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.story_end_time_range:
+            self.story_end_time_range.validate()
+        if self.story_start_time_range:
+            self.story_start_time_range.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.cover_image_thumbnail_process is not None:
+            result['cover_image_thumbnail_process'] = self.cover_image_thumbnail_process
+        if self.cover_video_thumbnail_process is not None:
+            result['cover_video_thumbnail_process'] = self.cover_video_thumbnail_process
+        if self.create_time_range is not None:
+            result['create_time_range'] = self.create_time_range.to_map()
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.face_group_ids is not None:
+            result['face_group_ids'] = self.face_group_ids
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order is not None:
+            result['order'] = self.order
+        if self.sort is not None:
+            result['sort'] = self.sort
+        if self.story_end_time_range is not None:
+            result['story_end_time_range'] = self.story_end_time_range.to_map()
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        if self.story_name is not None:
+            result['story_name'] = self.story_name
+        if self.story_start_time_range is not None:
+            result['story_start_time_range'] = self.story_start_time_range.to_map()
+        if self.story_type is not None:
+            result['story_type'] = self.story_type
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        if self.with_empty_stories is not None:
+            result['with_empty_stories'] = self.with_empty_stories
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('cover_image_thumbnail_process') is not None:
+            self.cover_image_thumbnail_process = m.get('cover_image_thumbnail_process')
+        if m.get('cover_video_thumbnail_process') is not None:
+            self.cover_video_thumbnail_process = m.get('cover_video_thumbnail_process')
+        if m.get('create_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.create_time_range = temp_model.from_map(m['create_time_range'])
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('face_group_ids') is not None:
+            self.face_group_ids = m.get('face_group_ids')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order') is not None:
+            self.order = m.get('order')
+        if m.get('sort') is not None:
+            self.sort = m.get('sort')
+        if m.get('story_end_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.story_end_time_range = temp_model.from_map(m['story_end_time_range'])
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        if m.get('story_name') is not None:
+            self.story_name = m.get('story_name')
+        if m.get('story_start_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.story_start_time_range = temp_model.from_map(m['story_start_time_range'])
+        if m.get('story_type') is not None:
+            self.story_type = m.get('story_type')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        if m.get('with_empty_stories') is not None:
+            self.with_empty_stories = m.get('with_empty_stories')
+        return self
+
+
 class GetAccessTokenByLinkInfoRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -35688,15 +38471,15 @@
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         return self
 
 
 class GetDefaultDriveRequest(TeaModel):
     """
-    Get default drive request
+    # Get default drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         subdomain_id: str = None,
         user_id: str = None,
     ):
@@ -35784,22 +38567,25 @@
     get domain request
     """
     def __init__(
         self,
         domain_id: str = None,
         fields: str = None,
         get_benefit: bool = None,
+        get_quota_used: bool = None,
         get_share_detail: bool = None,
         merge_parent: bool = None,
     ):
         # Domain ID
         self.domain_id = domain_id
         # fields,需要获取的属性字段,英文逗号分隔,*表示获取所有fields支持的枚举属性字段,为空不获取任何枚举属性字段
         self.fields = fields
         self.get_benefit = get_benefit
+        # 是否获取 quota 使用情况
+        self.get_quota_used = get_quota_used
         # 是否获取share/share_link详情
         self.get_share_detail = get_share_detail
         # 是否 merge parent 配置
         self.merge_parent = merge_parent
 
     def validate(self):
         self.validate_required(self.domain_id, 'domain_id')
@@ -35812,28 +38598,32 @@
         result = dict()
         if self.domain_id is not None:
             result['domain_id'] = self.domain_id
         if self.fields is not None:
             result['fields'] = self.fields
         if self.get_benefit is not None:
             result['get_benefit'] = self.get_benefit
+        if self.get_quota_used is not None:
+            result['get_quota_used'] = self.get_quota_used
         if self.get_share_detail is not None:
             result['get_share_detail'] = self.get_share_detail
         if self.merge_parent is not None:
             result['merge_parent'] = self.merge_parent
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         if m.get('fields') is not None:
             self.fields = m.get('fields')
         if m.get('get_benefit') is not None:
             self.get_benefit = m.get('get_benefit')
+        if m.get('get_quota_used') is not None:
+            self.get_quota_used = m.get('get_quota_used')
         if m.get('get_share_detail') is not None:
             self.get_share_detail = m.get('get_share_detail')
         if m.get('merge_parent') is not None:
             self.merge_parent = m.get('merge_parent')
         return self
 
 
@@ -35953,17 +38743,56 @@
         if m.get('sign_token') is not None:
             self.sign_token = m.get('sign_token')
         if m.get('static_url') is not None:
             self.static_url = m.get('static_url')
         return self
 
 
+class GetDriveDataProcessTemplateRequest(TeaModel):
+    """
+    get drive data process template request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
 class GetDriveRequest(TeaModel):
     """
-    Get drive request
+    # Get drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         drive_id: str = None,
         subdomain_id: str = None,
     ):
@@ -35997,14 +38826,61 @@
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
+class GetFaceGroupInfoRequest(TeaModel):
+    """
+    # Get face group info request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        group_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # group_id 列举人脸分组接口中获取
+        self.group_id = group_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.group_id, 'group_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.group_id is not None:
+            result['group_id'] = self.group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('group_id') is not None:
+            self.group_id = m.get('group_id')
+        return self
+
+
 class GetFileByPathRequest(TeaModel):
     """
     根据路径获取 File 接口 body
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -36107,14 +38983,62 @@
         if m.get('url_expire_sec') is not None:
             self.url_expire_sec = m.get('url_expire_sec')
         if m.get('video_thumbnail_process') is not None:
             self.video_thumbnail_process = m.get('video_thumbnail_process')
         return self
 
 
+class GetFileFaceGroupsRequest(TeaModel):
+    """
+    获取文件人脸分组列表请求
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        file_id: str = None,
+        filter: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.drive_id = drive_id
+        self.file_id = file_id
+        self.filter = filter
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.filter is not None:
+            result['filter'] = self.filter
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('filter') is not None:
+            self.filter = m.get('filter')
+        return self
+
+
 class GetFileRequest(TeaModel):
     """
     获取文件元数据
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -36260,14 +39184,53 @@
         if m.get('url_expire_sec') is not None:
             self.url_expire_sec = m.get('url_expire_sec')
         if m.get('video_thumbnail_process') is not None:
             self.video_thumbnail_process = m.get('video_thumbnail_process')
         return self
 
 
+class GetImageCountRequest(TeaModel):
+    """
+    # Get photo count request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        return self
+
+
 class GetLastCursorRequest(TeaModel):
     """
     获取最新游标
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -36400,39 +39363,45 @@
 class GetOfficeEditUrlOption(TeaModel):
     """
     GetOfficeEditUrlOption 权限控制
     """
     def __init__(
         self,
         copy: bool = None,
+        print: bool = None,
         readonly: bool = None,
     ):
         # Copy
         self.copy = copy
+        self.print = print
         self.readonly = readonly
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.copy is not None:
             result['copy'] = self.copy
+        if self.print is not None:
+            result['print'] = self.print
         if self.readonly is not None:
             result['readonly'] = self.readonly
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('copy') is not None:
             self.copy = m.get('copy')
+        if m.get('print') is not None:
+            self.print = m.get('print')
         if m.get('readonly') is not None:
             self.readonly = m.get('readonly')
         return self
 
 
 class GetOfficeEditUrlWatermark(TeaModel):
     """
@@ -36593,26 +39562,63 @@
             self.share_id = m.get('share_id')
         if m.get('watermark') is not None:
             temp_model = GetOfficeEditUrlWatermark()
             self.watermark = temp_model.from_map(m['watermark'])
         return self
 
 
+class GetOfficePreviewUrlOption(TeaModel):
+    """
+    GetOfficePreviewUrlOption 权限控制
+    """
+    def __init__(
+        self,
+        copy: bool = None,
+        print: bool = None,
+    ):
+        self.copy = copy
+        self.print = print
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.copy is not None:
+            result['copy'] = self.copy
+        if self.print is not None:
+            result['print'] = self.print
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('copy') is not None:
+            self.copy = m.get('copy')
+        if m.get('print') is not None:
+            self.print = m.get('print')
+        return self
+
+
 class GetOfficePreviewUrlRequest(TeaModel):
     """
     获取office文档预览地址
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         allow_copy: bool = None,
         drive_id: str = None,
         file_id: str = None,
         language: str = None,
+        option: GetOfficePreviewUrlOption = None,
         referer: str = None,
         revision_id: str = None,
         share_id: str = None,
     ):
         self.httpheaders = httpheaders
         # addition_data
         self.addition_data = addition_data
@@ -36621,27 +39627,30 @@
         self.allow_copy = allow_copy
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         # language
         self.language = language
+        self.option = option
         self.referer = referer
         # revision_id
         self.revision_id = revision_id
         # share_id, either share_id or drive_id is required
         self.share_id = share_id
 
     def validate(self):
         if self.drive_id is not None:
             self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
         self.validate_required(self.file_id, 'file_id')
         if self.file_id is not None:
             self.validate_max_length(self.file_id, 'file_id', 50)
             self.validate_pattern(self.file_id, 'file_id', '[a-z0-9.-_]{1,50}')
+        if self.option:
+            self.option.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -36653,14 +39662,16 @@
             result['allow_copy'] = self.allow_copy
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.language is not None:
             result['language'] = self.language
+        if self.option is not None:
+            result['option'] = self.option.to_map()
         if self.referer is not None:
             result['referer'] = self.referer
         if self.revision_id is not None:
             result['revision_id'] = self.revision_id
         if self.share_id is not None:
             result['share_id'] = self.share_id
         return result
@@ -36675,14 +39686,17 @@
             self.allow_copy = m.get('allow_copy')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('language') is not None:
             self.language = m.get('language')
+        if m.get('option') is not None:
+            temp_model = GetOfficePreviewUrlOption()
+            self.option = temp_model.from_map(m['option'])
         if m.get('referer') is not None:
             self.referer = m.get('referer')
         if m.get('revision_id') is not None:
             self.revision_id = m.get('revision_id')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         return self
@@ -37342,14 +40356,117 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         return self
 
 
+class GetStoryRequest(TeaModel):
+    """
+    # Get story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        cover_image_thumbnail_process: str = None,
+        cover_video_thumbnail_process: str = None,
+        drive_id: str = None,
+        image_thumbnail_process: str = None,
+        image_url_process: str = None,
+        office_thumbnail_process: str = None,
+        story_id: str = None,
+        thumbnail_processes: dict = None,
+        url_expire_sec: int = None,
+        video_thumbnail_process: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # cover_image_thumbnail_process
+        self.cover_image_thumbnail_process = cover_image_thumbnail_process
+        # cover_video_thumbnail_process
+        self.cover_video_thumbnail_process = cover_video_thumbnail_process
+        # drive_id
+        self.drive_id = drive_id
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # image_url_process
+        self.image_url_process = image_url_process
+        # office_thumbnail_process
+        self.office_thumbnail_process = office_thumbnail_process
+        # story_id
+        self.story_id = story_id
+        self.thumbnail_processes = thumbnail_processes
+        # url_expire_sec
+        self.url_expire_sec = url_expire_sec
+        # video_thumbnail_process
+        # type:string
+        self.video_thumbnail_process = video_thumbnail_process
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.story_id, 'story_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.cover_image_thumbnail_process is not None:
+            result['cover_image_thumbnail_process'] = self.cover_image_thumbnail_process
+        if self.cover_video_thumbnail_process is not None:
+            result['cover_video_thumbnail_process'] = self.cover_video_thumbnail_process
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.image_url_process is not None:
+            result['image_url_process'] = self.image_url_process
+        if self.office_thumbnail_process is not None:
+            result['office_thumbnail_process'] = self.office_thumbnail_process
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        if self.thumbnail_processes is not None:
+            result['thumbnail_processes'] = self.thumbnail_processes
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('cover_image_thumbnail_process') is not None:
+            self.cover_image_thumbnail_process = m.get('cover_image_thumbnail_process')
+        if m.get('cover_video_thumbnail_process') is not None:
+            self.cover_video_thumbnail_process = m.get('cover_video_thumbnail_process')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('image_url_process') is not None:
+            self.image_url_process = m.get('image_url_process')
+        if m.get('office_thumbnail_process') is not None:
+            self.office_thumbnail_process = m.get('office_thumbnail_process')
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        if m.get('thumbnail_processes') is not None:
+            self.thumbnail_processes = m.get('thumbnail_processes')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        return self
+
+
 class GetSubdomainMgmtRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         domain_id: str = None,
@@ -37388,14 +40505,59 @@
         if m.get('get_share_detail') is not None:
             self.get_share_detail = m.get('get_share_detail')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
+class GetTaskStatusRequest(TeaModel):
+    """
+    get task status request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        task_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        self.task_id = task_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        return self
+
+
 class GetUploadUrlRequest(TeaModel):
     """
     获取文件上传URL
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -37674,14 +40836,130 @@
         if m.get('sign_token') is not None:
             self.sign_token = m.get('sign_token')
         if m.get('template_id') is not None:
             self.template_id = m.get('template_id')
         return self
 
 
+class GetViewFileRequest(TeaModel):
+    """
+    get file from view
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        drive_id: str = None,
+        file_id: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        self.drive_id = drive_id
+        self.file_id = file_id
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
+class GetViewRequest(TeaModel):
+    """
+    Get view request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class HostingCompleteFileRequest(TeaModel):
     """
     complete file request
     """
     def __init__(
         self,
         addition_data: dict = None,
@@ -40633,15 +43911,15 @@
         if m.get('parent_domain_id') is not None:
             self.parent_domain_id = m.get('parent_domain_id')
         return self
 
 
 class ListDriveRequest(TeaModel):
     """
-    List drive request
+    # List drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         limit: int = None,
         marker: str = None,
         owner: str = None,
@@ -41513,101 +44791,356 @@
         if m.get('url_expire_sec') is not None:
             self.url_expire_sec = m.get('url_expire_sec')
         if m.get('video_thumbnail_process') is not None:
             self.video_thumbnail_process = m.get('video_thumbnail_process')
         return self
 
 
-class ListMangeSharingFileRequest(TeaModel):
+class ListFileViewsRequest(TeaModel):
     """
-    列举用户管理的共享文件列表
+    list file view ids
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
-        creator_list: List[str] = None,
-        limit: int = None,
-        marker: str = None,
-        subdomain_id: str = None,
+        category: str = None,
+        drive_id: str = None,
+        file_id: str = None,
+        user_id: str = None,
     ):
         self.httpheaders = httpheaders
-        # 查询的用户列表，传入用户ID列表，不传默认查询所有有权限管理的共享
-        self.creator_list = creator_list
-        # 查询返回的记录数
-        self.limit = limit
-        # 上次查询返回的游标
-        self.marker = marker
-        self.subdomain_id = subdomain_id
+        self.category = category
+        self.drive_id = drive_id
+        self.file_id = file_id
+        # user_id
+        self.user_id = user_id
 
     def validate(self):
-        self.validate_required(self.limit, 'limit')
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
-        if self.creator_list is not None:
-            result['creator_list'] = self.creator_list
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.subdomain_id is not None:
-            result['subdomain_id'] = self.subdomain_id
+        if self.category is not None:
+            result['category'] = self.category
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
-        if m.get('creator_list') is not None:
-            self.creator_list = m.get('creator_list')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('subdomain_id') is not None:
-            self.subdomain_id = m.get('subdomain_id')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
         return self
 
 
-class ListMyDriveRequest(TeaModel):
+class ListImageAddressGroupsRequest(TeaModel):
     """
-    List my drive request
+    # List image address groups request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        image_thumbnail_process: str = None,
         limit: int = None,
         marker: str = None,
+        return_total_count: bool = None,
+        video_thumbnail_process: str = None,
     ):
         self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
         # 每页大小限制
         self.limit = limit
-        # 翻页标记, 接口返回的标记值
+        # 翻页标记
         self.marker = marker
+        # ReturnTotalCount 是否返回分组总数
+        self.return_total_count = return_total_count
+        # video_thumbnail_process
+        self.video_thumbnail_process = video_thumbnail_process
 
     def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
         if self.limit is not None:
             self.validate_maximum(self.limit, 'limit', 100)
             self.validate_minimum(self.limit, 'limit', 1)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
-        if self.limit is not None:
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.return_total_count is not None:
+            result['return_total_count'] = self.return_total_count
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('return_total_count') is not None:
+            self.return_total_count = m.get('return_total_count')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        return self
+
+
+class ListImageFaceGroupsRequest(TeaModel):
+    """
+    # List image face groups request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        limit: int = None,
+        marker: str = None,
+        remarks: str = None,
+        return_total_count: bool = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # 每页大小限制
+        self.limit = limit
+        # 翻页标记
+        self.marker = marker
+        self.remarks = remarks
+        # ReturnTotalCount 是否返回分组总数
+        self.return_total_count = return_total_count
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.limit is not None:
+            self.validate_maximum(self.limit, 'limit', 100)
+            self.validate_minimum(self.limit, 'limit', 1)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.remarks is not None:
+            result['remarks'] = self.remarks
+        if self.return_total_count is not None:
+            result['return_total_count'] = self.return_total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('remarks') is not None:
+            self.remarks = m.get('remarks')
+        if m.get('return_total_count') is not None:
+            self.return_total_count = m.get('return_total_count')
+        return self
+
+
+class ListImageTagsRequest(TeaModel):
+    """
+    # List image tags request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        image_thumbnail_process: str = None,
+        video_thumbnail_process: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # video_thumbnail_process
+        # type:string
+        self.video_thumbnail_process = video_thumbnail_process
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        return self
+
+
+class ListMangeSharingFileRequest(TeaModel):
+    """
+    列举用户管理的共享文件列表
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        creator_list: List[str] = None,
+        limit: int = None,
+        marker: str = None,
+        subdomain_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # 查询的用户列表，传入用户ID列表，不传默认查询所有有权限管理的共享
+        self.creator_list = creator_list
+        # 查询返回的记录数
+        self.limit = limit
+        # 上次查询返回的游标
+        self.marker = marker
+        self.subdomain_id = subdomain_id
+
+    def validate(self):
+        self.validate_required(self.limit, 'limit')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.creator_list is not None:
+            result['creator_list'] = self.creator_list
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.subdomain_id is not None:
+            result['subdomain_id'] = self.subdomain_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('creator_list') is not None:
+            self.creator_list = m.get('creator_list')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('subdomain_id') is not None:
+            self.subdomain_id = m.get('subdomain_id')
+        return self
+
+
+class ListMyDriveRequest(TeaModel):
+    """
+    # List my drive request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        limit: int = None,
+        marker: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # 每页大小限制
+        self.limit = limit
+        # 翻页标记, 接口返回的标记值
+        self.marker = marker
+
+    def validate(self):
+        if self.limit is not None:
+            self.validate_maximum(self.limit, 'limit', 100)
+            self.validate_minimum(self.limit, 'limit', 1)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.limit is not None:
             result['limit'] = self.limit
         if self.marker is not None:
             result['marker'] = self.marker
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
@@ -42571,14 +46104,226 @@
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('upload_id') is not None:
             self.upload_id = m.get('upload_id')
         return self
 
 
+class ListViewFilesRequest(TeaModel):
+    """
+    list view file
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        fields: str = None,
+        filter: str = None,
+        image_thumbnail_process: str = None,
+        image_url_process: str = None,
+        limit: int = None,
+        marker: str = None,
+        office_thumbnail_process: str = None,
+        order_by: str = None,
+        order_direction: str = None,
+        thumbnail_processes: dict = None,
+        url_expire_sec: int = None,
+        user_id: str = None,
+        video_thumbnail_process: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        self.fields = fields
+        self.filter = filter
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # image_url_process
+        self.image_url_process = image_url_process
+        self.limit = limit
+        self.marker = marker
+        # office_thumbnail_process
+        self.office_thumbnail_process = office_thumbnail_process
+        self.order_by = order_by
+        self.order_direction = order_direction
+        self.thumbnail_processes = thumbnail_processes
+        self.url_expire_sec = url_expire_sec
+        # user_id
+        self.user_id = user_id
+        # video_thumbnail_process
+        # type:string
+        self.video_thumbnail_process = video_thumbnail_process
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.fields is not None:
+            result['fields'] = self.fields
+        if self.filter is not None:
+            result['filter'] = self.filter
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.image_url_process is not None:
+            result['image_url_process'] = self.image_url_process
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.office_thumbnail_process is not None:
+            result['office_thumbnail_process'] = self.office_thumbnail_process
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.order_direction is not None:
+            result['order_direction'] = self.order_direction
+        if self.thumbnail_processes is not None:
+            result['thumbnail_processes'] = self.thumbnail_processes
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
+        if m.get('filter') is not None:
+            self.filter = m.get('filter')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('image_url_process') is not None:
+            self.image_url_process = m.get('image_url_process')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('office_thumbnail_process') is not None:
+            self.office_thumbnail_process = m.get('office_thumbnail_process')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('order_direction') is not None:
+            self.order_direction = m.get('order_direction')
+        if m.get('thumbnail_processes') is not None:
+            self.thumbnail_processes = m.get('thumbnail_processes')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
+class ListViewsRequest(TeaModel):
+    """
+    List views request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        limit: int = None,
+        marker: str = None,
+        order_by: str = None,
+        order_direction: str = None,
+        owner: str = None,
+        user_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # 每页大小限制
+        self.limit = limit
+        # marker
+        self.marker = marker
+        # order_by
+        self.order_by = order_by
+        # order_direction
+        self.order_direction = order_direction
+        # owner
+        self.owner = owner
+        # user_id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        if self.limit is not None:
+            self.validate_maximum(self.limit, 'limit', 100)
+            self.validate_minimum(self.limit, 'limit', 1)
+        self.validate_required(self.owner, 'owner')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.order_direction is not None:
+            result['order_direction'] = self.order_direction
+        if self.owner is not None:
+            result['owner'] = self.owner
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('order_direction') is not None:
+            self.order_direction = m.get('order_direction')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
 class LoginByCodeRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         access_token: str = None,
@@ -42784,14 +46529,76 @@
         if m.get('ClientID') is not None:
             self.client_id = m.get('ClientID')
         if m.get('LoginType') is not None:
             self.login_type = m.get('LoginType')
         return self
 
 
+class MergeFaceGroupRequest(TeaModel):
+    """
+    # Merge face group request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        from_group_id: str = None,
+        from_group_ids: List[str] = None,
+        to_group_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # from_group_id
+        self.from_group_id = from_group_id
+        # from_group_ids
+        self.from_group_ids = from_group_ids
+        # to_group_id
+        self.to_group_id = to_group_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.from_group_ids, 'from_group_ids')
+        self.validate_required(self.to_group_id, 'to_group_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.from_group_id is not None:
+            result['from_group_id'] = self.from_group_id
+        if self.from_group_ids is not None:
+            result['from_group_ids'] = self.from_group_ids
+        if self.to_group_id is not None:
+            result['to_group_id'] = self.to_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('from_group_id') is not None:
+            self.from_group_id = m.get('from_group_id')
+        if m.get('from_group_ids') is not None:
+            self.from_group_ids = m.get('from_group_ids')
+        if m.get('to_group_id') is not None:
+            self.to_group_id = m.get('to_group_id')
+        return self
+
+
 class MoveFileRequest(TeaModel):
     """
     文件移动请求
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -42937,14 +46744,50 @@
         if m.get('exist_file_id') is not None:
             self.exist_file_id = m.get('exist_file_id')
         if m.get('exist_file_type') is not None:
             self.exist_file_type = m.get('exist_file_type')
         return self
 
 
+class ParseKeywordsRequest(TeaModel):
+    """
+    # Parse keywords request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        keywords: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.keywords = keywords
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.keywords is not None:
+            result['keywords'] = self.keywords
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('keywords') is not None:
+            self.keywords = m.get('keywords')
+        return self
+
+
 class Permission(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         action_list: List[ActionItem] = None,
@@ -43224,19 +47067,22 @@
 class PutFileUserTagsRequest(TeaModel):
     """
     更新文件 user_tags 字段
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
         drive_id: str = None,
         file_id: str = None,
         user_tags: List[UserTag] = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         # user_tags
         self.user_tags = user_tags
 
@@ -43257,40 +47103,245 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         result['user_tags'] = []
         if self.user_tags is not None:
             for k in self.user_tags:
                 result['user_tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         self.user_tags = []
         if m.get('user_tags') is not None:
             for k in m.get('user_tags'):
                 temp_model = UserTag()
                 self.user_tags.append(temp_model.from_map(k))
         return self
 
 
+class QueryLocationDateClustersRequest(TeaModel):
+    """
+    query locationCluster request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        address: Address = None,
+        cluster_id: str = None,
+        create_time_range: QueryRequestTimeRange = None,
+        custom_labels: str = None,
+        drive_id: str = None,
+        end_time_range: QueryRequestTimeRange = None,
+        levels: List[str] = None,
+        limit: int = None,
+        marker: str = None,
+        order: str = None,
+        sort: str = None,
+        start_time_range: QueryRequestTimeRange = None,
+        title: str = None,
+        update_time_range: QueryRequestTimeRange = None,
+    ):
+        self.httpheaders = httpheaders
+        self.address = address
+        self.cluster_id = cluster_id
+        self.create_time_range = create_time_range
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        self.end_time_range = end_time_range
+        self.levels = levels
+        self.limit = limit
+        self.marker = marker
+        self.order = order
+        self.sort = sort
+        self.start_time_range = start_time_range
+        self.title = title
+        self.update_time_range = update_time_range
+
+    def validate(self):
+        if self.address:
+            self.address.validate()
+        if self.create_time_range:
+            self.create_time_range.validate()
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.end_time_range:
+            self.end_time_range.validate()
+        if self.start_time_range:
+            self.start_time_range.validate()
+        if self.update_time_range:
+            self.update_time_range.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.address is not None:
+            result['address'] = self.address.to_map()
+        if self.cluster_id is not None:
+            result['cluster_id'] = self.cluster_id
+        if self.create_time_range is not None:
+            result['create_time_range'] = self.create_time_range.to_map()
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.end_time_range is not None:
+            result['end_time_range'] = self.end_time_range.to_map()
+        if self.levels is not None:
+            result['levels'] = self.levels
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order is not None:
+            result['order'] = self.order
+        if self.sort is not None:
+            result['sort'] = self.sort
+        if self.start_time_range is not None:
+            result['start_time_range'] = self.start_time_range.to_map()
+        if self.title is not None:
+            result['title'] = self.title
+        if self.update_time_range is not None:
+            result['update_time_range'] = self.update_time_range.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('address') is not None:
+            temp_model = Address()
+            self.address = temp_model.from_map(m['address'])
+        if m.get('cluster_id') is not None:
+            self.cluster_id = m.get('cluster_id')
+        if m.get('create_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.create_time_range = temp_model.from_map(m['create_time_range'])
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('end_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.end_time_range = temp_model.from_map(m['end_time_range'])
+        if m.get('levels') is not None:
+            self.levels = m.get('levels')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order') is not None:
+            self.order = m.get('order')
+        if m.get('sort') is not None:
+            self.sort = m.get('sort')
+        if m.get('start_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.start_time_range = temp_model.from_map(m['start_time_range'])
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('update_time_range') is not None:
+            temp_model = QueryRequestTimeRange()
+            self.update_time_range = temp_model.from_map(m['update_time_range'])
+        return self
+
+
+class QuerySimilarImageClusterRequest(TeaModel):
+    """
+    query similar image clusters request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        image_thumbnail_process: str = None,
+        limit: int = None,
+        marker: str = None,
+        order: str = None,
+        thumbnail_processes: dict = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        self.image_thumbnail_process = image_thumbnail_process
+        self.limit = limit
+        self.marker = marker
+        self.order = order
+        self.thumbnail_processes = thumbnail_processes
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order is not None:
+            result['order'] = self.order
+        if self.thumbnail_processes is not None:
+            result['thumbnail_processes'] = self.thumbnail_processes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order') is not None:
+            self.order = m.get('order')
+        if m.get('thumbnail_processes') is not None:
+            self.thumbnail_processes = m.get('thumbnail_processes')
+        return self
+
+
 class RPVerifyBaseRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         user_id: str = None,
@@ -43626,14 +47677,140 @@
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         if m.get('store_id') is not None:
             self.store_id = m.get('store_id')
         return self
 
 
+class RemoveStoryFilesRequest(TeaModel):
+    """
+    remove story files request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        files: List[StoryFile] = None,
+        story_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        self.files = files
+        # story_id
+        self.story_id = story_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.files:
+            for k in self.files:
+                if k:
+                    k.validate()
+        self.validate_required(self.story_id, 'story_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        result['files'] = []
+        if self.files is not None:
+            for k in self.files:
+                result['files'].append(k.to_map() if k else None)
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        self.files = []
+        if m.get('files') is not None:
+            for k in m.get('files'):
+                temp_model = StoryFile()
+                self.files.append(temp_model.from_map(k))
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        return self
+
+
+class RemoveViewFileRequest(TeaModel):
+    """
+    remove file from view
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        drive_id: str = None,
+        file_id: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        self.drive_id = drive_id
+        self.file_id = file_id
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class ReportMediaPlayEventRequest(TeaModel):
     """
     report_media_play_event request
     """
     def __init__(
         self,
         duration: int = None,
@@ -43894,19 +48071,22 @@
 class RestoreRevisionRequest(TeaModel):
     """
     还原历史版本元数据
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
         drive_id: str = None,
         file_id: str = None,
         revision_id: str = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         # revision_id
         self.revision_id = revision_id
 
@@ -43927,26 +48107,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.revision_id is not None:
             result['revision_id'] = self.revision_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('revision_id') is not None:
             self.revision_id = m.get('revision_id')
         return self
@@ -44175,29 +48359,31 @@
         if m.get('service_code') is not None:
             self.service_code = m.get('service_code')
         return self
 
 
 class SearchDriveRequest(TeaModel):
     """
-    Search drive request
+    # Search drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        category: str = None,
         drive_name: str = None,
         limit: int = None,
         marker: str = None,
         order_by: str = None,
         order_direction: str = None,
         owner: str = None,
         owner_type: str = None,
         subdomain_id: str = None,
     ):
         self.httpheaders = httpheaders
+        self.category = category
         # Drive Fuzz Name
         self.drive_name = drive_name
         # 每页大小限制
         self.limit = limit
         # 翻页标记, 接口返回的标记值
         self.marker = marker
         self.order_by = order_by
@@ -44219,14 +48405,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
         if self.drive_name is not None:
             result['drive_name'] = self.drive_name
         if self.limit is not None:
             result['limit'] = self.limit
         if self.marker is not None:
             result['marker'] = self.marker
         if self.order_by is not None:
@@ -44241,14 +48429,16 @@
             result['subdomain_id'] = self.subdomain_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
         if m.get('drive_name') is not None:
             self.drive_name = m.get('drive_name')
         if m.get('limit') is not None:
             self.limit = m.get('limit')
         if m.get('marker') is not None:
             self.marker = m.get('marker')
         if m.get('order_by') is not None:
@@ -44339,17 +48529,19 @@
         image_url_process: str = None,
         limit: int = None,
         location: str = None,
         marker: str = None,
         office_thumbnail_process: str = None,
         order_by: str = None,
         query: str = None,
+        recursive: bool = None,
         referer: str = None,
         return_total_count: bool = None,
         sign_token: str = None,
+        system_folders: List[str] = None,
         thumbnail_processes: dict = None,
         url_expire_sec: int = None,
         video_thumbnail_process: str = None,
     ):
         self.httpheaders = httpheaders
         # addition_data
         self.addition_data = addition_data
@@ -44370,20 +48562,23 @@
         self.marker = marker
         # office_thumbnail_process
         self.office_thumbnail_process = office_thumbnail_process
         # order_by
         self.order_by = order_by
         # query
         self.query = query
+        self.recursive = recursive
         # referer
         self.referer = referer
         # return_total_count 是否返回查询总数
         self.return_total_count = return_total_count
         # sign_token
         self.sign_token = sign_token
+        # system_folders
+        self.system_folders = system_folders
         self.thumbnail_processes = thumbnail_processes
         # url_expire_sec
         self.url_expire_sec = url_expire_sec
         # video_thumbnail_process
         # type:string
         self.video_thumbnail_process = video_thumbnail_process
 
@@ -44427,20 +48622,24 @@
             result['marker'] = self.marker
         if self.office_thumbnail_process is not None:
             result['office_thumbnail_process'] = self.office_thumbnail_process
         if self.order_by is not None:
             result['order_by'] = self.order_by
         if self.query is not None:
             result['query'] = self.query
+        if self.recursive is not None:
+            result['recursive'] = self.recursive
         if self.referer is not None:
             result['referer'] = self.referer
         if self.return_total_count is not None:
             result['return_total_count'] = self.return_total_count
         if self.sign_token is not None:
             result['sign_token'] = self.sign_token
+        if self.system_folders is not None:
+            result['system_folders'] = self.system_folders
         if self.thumbnail_processes is not None:
             result['thumbnail_processes'] = self.thumbnail_processes
         if self.url_expire_sec is not None:
             result['url_expire_sec'] = self.url_expire_sec
         if self.video_thumbnail_process is not None:
             result['video_thumbnail_process'] = self.video_thumbnail_process
         return result
@@ -44469,29 +48668,114 @@
             self.marker = m.get('marker')
         if m.get('office_thumbnail_process') is not None:
             self.office_thumbnail_process = m.get('office_thumbnail_process')
         if m.get('order_by') is not None:
             self.order_by = m.get('order_by')
         if m.get('query') is not None:
             self.query = m.get('query')
+        if m.get('recursive') is not None:
+            self.recursive = m.get('recursive')
         if m.get('referer') is not None:
             self.referer = m.get('referer')
         if m.get('return_total_count') is not None:
             self.return_total_count = m.get('return_total_count')
         if m.get('sign_token') is not None:
             self.sign_token = m.get('sign_token')
+        if m.get('system_folders') is not None:
+            self.system_folders = m.get('system_folders')
         if m.get('thumbnail_processes') is not None:
             self.thumbnail_processes = m.get('thumbnail_processes')
         if m.get('url_expire_sec') is not None:
             self.url_expire_sec = m.get('url_expire_sec')
         if m.get('video_thumbnail_process') is not None:
             self.video_thumbnail_process = m.get('video_thumbnail_process')
         return self
 
 
+class SearchImageAddressGroupsRequest(TeaModel):
+    """
+    # Search image address groups request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        address_level: str = None,
+        address_names: List[str] = None,
+        br_geo_point: str = None,
+        drive_id: str = None,
+        image_thumbnail_process: str = None,
+        tl_geo_point: str = None,
+        video_thumbnail_process: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # 查询的地点级别
+        self.address_level = address_level
+        # 查询的地点数组
+        self.address_names = address_names
+        # br_geo_point
+        self.br_geo_point = br_geo_point
+        # drive_id
+        self.drive_id = drive_id
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # tl_geo_point
+        self.tl_geo_point = tl_geo_point
+        # video_thumbnail_process
+        self.video_thumbnail_process = video_thumbnail_process
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.address_level is not None:
+            result['address_level'] = self.address_level
+        if self.address_names is not None:
+            result['address_names'] = self.address_names
+        if self.br_geo_point is not None:
+            result['br_geo_point'] = self.br_geo_point
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.tl_geo_point is not None:
+            result['tl_geo_point'] = self.tl_geo_point
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('address_level') is not None:
+            self.address_level = m.get('address_level')
+        if m.get('address_names') is not None:
+            self.address_names = m.get('address_names')
+        if m.get('br_geo_point') is not None:
+            self.br_geo_point = m.get('br_geo_point')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('tl_geo_point') is not None:
+            self.tl_geo_point = m.get('tl_geo_point')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        return self
+
+
 class SearchShareLinkRequest(TeaModel):
     """
     search_share_link request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -44574,14 +48858,255 @@
         if m.get('query') is not None:
             self.query = m.get('query')
         if m.get('return_total_count') is not None:
             self.return_total_count = m.get('return_total_count')
         return self
 
 
+class SearchViewFilesRequest(TeaModel):
+    """
+    search view file
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        fields: str = None,
+        filter: str = None,
+        image_thumbnail_process: str = None,
+        image_url_process: str = None,
+        limit: int = None,
+        marker: str = None,
+        office_thumbnail_process: str = None,
+        order_by: str = None,
+        order_direction: str = None,
+        query: str = None,
+        return_total_count: bool = None,
+        thumbnail_processes: dict = None,
+        url_expire_sec: int = None,
+        user_id: str = None,
+        video_thumbnail_process: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        self.fields = fields
+        self.filter = filter
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # image_url_process
+        self.image_url_process = image_url_process
+        self.limit = limit
+        self.marker = marker
+        # office_thumbnail_process
+        self.office_thumbnail_process = office_thumbnail_process
+        self.order_by = order_by
+        self.order_direction = order_direction
+        # query
+        self.query = query
+        # return_total_count 是否返回查询总数
+        self.return_total_count = return_total_count
+        self.thumbnail_processes = thumbnail_processes
+        self.url_expire_sec = url_expire_sec
+        # user_id
+        self.user_id = user_id
+        # video_thumbnail_process
+        # type:string
+        self.video_thumbnail_process = video_thumbnail_process
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        if self.query is not None:
+            self.validate_max_length(self.query, 'query', 4096)
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.fields is not None:
+            result['fields'] = self.fields
+        if self.filter is not None:
+            result['filter'] = self.filter
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.image_url_process is not None:
+            result['image_url_process'] = self.image_url_process
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.office_thumbnail_process is not None:
+            result['office_thumbnail_process'] = self.office_thumbnail_process
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.order_direction is not None:
+            result['order_direction'] = self.order_direction
+        if self.query is not None:
+            result['query'] = self.query
+        if self.return_total_count is not None:
+            result['return_total_count'] = self.return_total_count
+        if self.thumbnail_processes is not None:
+            result['thumbnail_processes'] = self.thumbnail_processes
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
+        if m.get('filter') is not None:
+            self.filter = m.get('filter')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('image_url_process') is not None:
+            self.image_url_process = m.get('image_url_process')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('office_thumbnail_process') is not None:
+            self.office_thumbnail_process = m.get('office_thumbnail_process')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('order_direction') is not None:
+            self.order_direction = m.get('order_direction')
+        if m.get('query') is not None:
+            self.query = m.get('query')
+        if m.get('return_total_count') is not None:
+            self.return_total_count = m.get('return_total_count')
+        if m.get('thumbnail_processes') is not None:
+            self.thumbnail_processes = m.get('thumbnail_processes')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
+class SearchViewsRequest(TeaModel):
+    """
+    Search view request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        limit: int = None,
+        marker: str = None,
+        name: str = None,
+        order_by: str = None,
+        order_direction: str = None,
+        owner: str = None,
+        return_total_count: bool = None,
+        user_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # 每页大小限制
+        self.limit = limit
+        # marker
+        self.marker = marker
+        # name
+        self.name = name
+        # order_by
+        self.order_by = order_by
+        # order_direction
+        self.order_direction = order_direction
+        # owner
+        self.owner = owner
+        # return_total_count 是否返回查询总数
+        self.return_total_count = return_total_count
+        # user_id
+        self.user_id = user_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        if self.limit is not None:
+            self.validate_maximum(self.limit, 'limit', 100)
+            self.validate_minimum(self.limit, 'limit', 1)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.name is not None:
+            result['name'] = self.name
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.order_direction is not None:
+            result['order_direction'] = self.order_direction
+        if self.owner is not None:
+            result['owner'] = self.owner
+        if self.return_total_count is not None:
+            result['return_total_count'] = self.return_total_count
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('order_direction') is not None:
+            self.order_direction = m.get('order_direction')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        if m.get('return_total_count') is not None:
+            self.return_total_count = m.get('return_total_count')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        return self
+
+
 class SendSmsCodeRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -45192,14 +49717,157 @@
         if m.get('save_download_limit') is not None:
             self.save_download_limit = m.get('save_download_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
         return self
 
 
+class SimpleQuery(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        field: str = None,
+        operation: str = None,
+        sub_queries: List['SimpleQuery'] = None,
+        value: str = None,
+    ):
+        self.field = field
+        self.operation = operation
+        self.sub_queries = sub_queries
+        self.value = value
+
+    def validate(self):
+        if self.sub_queries:
+            for k in self.sub_queries:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.field is not None:
+            result['field'] = self.field
+        if self.operation is not None:
+            result['operation'] = self.operation
+        result['sub_queries'] = []
+        if self.sub_queries is not None:
+            for k in self.sub_queries:
+                result['sub_queries'].append(k.to_map() if k else None)
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('field') is not None:
+            self.field = m.get('field')
+        if m.get('operation') is not None:
+            self.operation = m.get('operation')
+        self.sub_queries = []
+        if m.get('sub_queries') is not None:
+            for k in m.get('sub_queries'):
+                temp_model = SimpleQuery()
+                self.sub_queries.append(temp_model.from_map(k))
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class SimpleQueryRequest(TeaModel):
+    """
+    simple query request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        aggregations: List[Aggregation] = None,
+        drive_id: str = None,
+        limit: int = None,
+        marker: str = None,
+        order: str = None,
+        query: SimpleQuery = None,
+        sort: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.aggregations = aggregations
+        # drive_id
+        self.drive_id = drive_id
+        self.limit = limit
+        self.marker = marker
+        self.order = order
+        self.query = query
+        self.sort = sort
+
+    def validate(self):
+        if self.aggregations:
+            for k in self.aggregations:
+                if k:
+                    k.validate()
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        if self.query:
+            self.query.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        result['aggregations'] = []
+        if self.aggregations is not None:
+            for k in self.aggregations:
+                result['aggregations'].append(k.to_map() if k else None)
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order is not None:
+            result['order'] = self.order
+        if self.query is not None:
+            result['query'] = self.query.to_map()
+        if self.sort is not None:
+            result['sort'] = self.sort
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        self.aggregations = []
+        if m.get('aggregations') is not None:
+            for k in m.get('aggregations'):
+                temp_model = Aggregation()
+                self.aggregations.append(temp_model.from_map(k))
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order') is not None:
+            self.order = m.get('order')
+        if m.get('query') is not None:
+            temp_model = SimpleQuery()
+            self.query = temp_model.from_map(m['query'])
+        if m.get('sort') is not None:
+            self.sort = m.get('sort')
+        return self
+
+
 class SimpleStreamInfo(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         content_hash: str = None,
@@ -45766,19 +50434,21 @@
 class TrashFileRequest(TeaModel):
     """
     删除文件请求，支持批量
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        check_folder_empty: bool = None,
         drive_id: str = None,
         file_id: str = None,
         share_id: str = None,
     ):
         self.httpheaders = httpheaders
+        self.check_folder_empty = check_folder_empty
         # drive_id
         self.drive_id = drive_id
         # file_id
         self.file_id = file_id
         # share_id, either share_id or drive_id is required
         self.share_id = share_id
 
@@ -45794,26 +50464,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.check_folder_empty is not None:
+            result['check_folder_empty'] = self.check_folder_empty
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.share_id is not None:
             result['share_id'] = self.share_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('check_folder_empty') is not None:
+            self.check_folder_empty = m.get('check_folder_empty')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         return self
@@ -45925,14 +50599,15 @@
         self,
         httpheaders: Dict[str, str] = None,
         addition_data: dict = None,
         auto_rename: bool = None,
         callback: CcpCallback = None,
         category: str = None,
         check_name_mode: str = None,
+        check_parent_file_id_path: str = None,
         content_hash: str = None,
         content_hash_mutable: bool = None,
         content_hash_name: str = None,
         content_md_5: str = None,
         content_type: str = None,
         create_reason: str = None,
         custom_field_1: str = None,
@@ -45980,14 +50655,15 @@
         self.addition_data = addition_data
         self.auto_rename = auto_rename
         self.callback = callback
         # category
         self.category = category
         # check_name_mode
         self.check_name_mode = check_name_mode
+        self.check_parent_file_id_path = check_parent_file_id_path
         # content_hash
         self.content_hash = content_hash
         # content_hash_mutable
         self.content_hash_mutable = content_hash_mutable
         # content_hash_name
         self.content_hash_name = content_hash_name
         # ContentMd5
@@ -46107,14 +50783,16 @@
             result['auto_rename'] = self.auto_rename
         if self.callback is not None:
             result['callback'] = self.callback.to_map()
         if self.category is not None:
             result['category'] = self.category
         if self.check_name_mode is not None:
             result['check_name_mode'] = self.check_name_mode
+        if self.check_parent_file_id_path is not None:
+            result['check_parent_file_id_path'] = self.check_parent_file_id_path
         if self.content_hash is not None:
             result['content_hash'] = self.content_hash
         if self.content_hash_mutable is not None:
             result['content_hash_mutable'] = self.content_hash_mutable
         if self.content_hash_name is not None:
             result['content_hash_name'] = self.content_hash_name
         if self.content_md_5 is not None:
@@ -46218,14 +50896,16 @@
         if m.get('callback') is not None:
             temp_model = CcpCallback()
             self.callback = temp_model.from_map(m['callback'])
         if m.get('category') is not None:
             self.category = m.get('category')
         if m.get('check_name_mode') is not None:
             self.check_name_mode = m.get('check_name_mode')
+        if m.get('check_parent_file_id_path') is not None:
+            self.check_parent_file_id_path = m.get('check_parent_file_id_path')
         if m.get('content_hash') is not None:
             self.content_hash = m.get('content_hash')
         if m.get('content_hash_mutable') is not None:
             self.content_hash_mutable = m.get('content_hash_mutable')
         if m.get('content_hash_name') is not None:
             self.content_hash_name = m.get('content_hash_name')
         if m.get('content_md5') is not None:
@@ -46565,14 +51245,75 @@
         if m.get('size') is not None:
             self.size = m.get('size')
         if m.get('upload_id') is not None:
             self.upload_id = m.get('upload_id')
         return self
 
 
+class UnAssignFaceGroupItemRequest(TeaModel):
+    """
+    # Unassign facegroup item request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        face_group_id: str = None,
+        file_id: str = None,
+        group_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # face_group_id
+        self.face_group_id = face_group_id
+        # file_id
+        self.file_id = file_id
+        # group_id 列举人脸分组接口中获取
+        self.group_id = group_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.file_id, 'file_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.face_group_id is not None:
+            result['face_group_id'] = self.face_group_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.group_id is not None:
+            result['group_id'] = self.group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('face_group_id') is not None:
+            self.face_group_id = m.get('face_group_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('group_id') is not None:
+            self.group_id = m.get('group_id')
+        return self
+
+
 class UnionAuthentication(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         authentication_type: str = None,
@@ -46988,17 +51729,62 @@
         if m.get('user_count_quota') is not None:
             self.user_count_quota = m.get('user_count_quota')
         if m.get('user_single_drive_enabled') is not None:
             self.user_single_drive_enabled = m.get('user_single_drive_enabled')
         return self
 
 
+class UpdateDriveDataProcessTemplateRequest(TeaModel):
+    """
+    update drive data process template request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        template_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        self.template_id = template_id
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        return self
+
+
 class UpdateDriveRequest(TeaModel):
     """
-    Update drive request
+    # Update drive request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         category: str = None,
         description: str = None,
         drive_id: str = None,
@@ -47084,21 +51870,90 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('total_size') is not None:
             self.total_size = m.get('total_size')
         return self
 
 
+class UpdateFaceGroupInfoRequest(TeaModel):
+    """
+    # Update face group info request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        drive_id: str = None,
+        group_cover_face_id: str = None,
+        group_id: str = None,
+        group_name: str = None,
+        remarks: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # drive_id
+        self.drive_id = drive_id
+        # group_cover_face_id
+        self.group_cover_face_id = group_cover_face_id
+        # group_id 列举人脸分组接口中获取
+        self.group_id = group_id
+        # group_name
+        self.group_name = group_name
+        # remarks
+        self.remarks = remarks
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.group_id, 'group_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.group_cover_face_id is not None:
+            result['group_cover_face_id'] = self.group_cover_face_id
+        if self.group_id is not None:
+            result['group_id'] = self.group_id
+        if self.group_name is not None:
+            result['group_name'] = self.group_name
+        if self.remarks is not None:
+            result['remarks'] = self.remarks
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('group_cover_face_id') is not None:
+            self.group_cover_face_id = m.get('group_cover_face_id')
+        if m.get('group_id') is not None:
+            self.group_id = m.get('group_id')
+        if m.get('group_name') is not None:
+            self.group_name = m.get('group_name')
+        if m.get('remarks') is not None:
+            self.remarks = m.get('remarks')
+        return self
+
+
 class UpdateFileMetaRequest(TeaModel):
     """
     更新文件元数据
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: dict = None,
         category: str = None,
         check_name_mode: str = None,
         custom_field_1: str = None,
         custom_field_2: str = None,
         custom_index_key: str = None,
         custom_type: str = None,
         description: str = None,
@@ -47118,14 +51973,16 @@
         share_id: str = None,
         sign_token: str = None,
         starred: bool = None,
         taken_at: str = None,
         user_meta: str = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         self.category = category
         # check_name_mode
         self.check_name_mode = check_name_mode
         self.custom_field_1 = custom_field_1
         self.custom_field_2 = custom_field_2
         self.custom_index_key = custom_index_key
         self.custom_type = custom_type
@@ -47178,14 +52035,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.category is not None:
             result['category'] = self.category
         if self.check_name_mode is not None:
             result['check_name_mode'] = self.check_name_mode
         if self.custom_field_1 is not None:
             result['custom_field_1'] = self.custom_field_1
         if self.custom_field_2 is not None:
@@ -47234,14 +52093,16 @@
             result['user_meta'] = self.user_meta
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('category') is not None:
             self.category = m.get('category')
         if m.get('check_name_mode') is not None:
             self.check_name_mode = m.get('check_name_mode')
         if m.get('custom_field_1') is not None:
             self.custom_field_1 = m.get('custom_field_1')
         if m.get('custom_field_2') is not None:
@@ -47287,14 +52148,71 @@
         if m.get('taken_at') is not None:
             self.taken_at = m.get('taken_at')
         if m.get('user_meta') is not None:
             self.user_meta = m.get('user_meta')
         return self
 
 
+class UpdateLocationDateClusterRequest(TeaModel):
+    """
+    update locationCluster request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        cluster_id: str = None,
+        custom_labels: dict = None,
+        drive_id: str = None,
+        title: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.cluster_id = cluster_id
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        self.title = title
+
+    def validate(self):
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.cluster_id is not None:
+            result['cluster_id'] = self.cluster_id
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('cluster_id') is not None:
+            self.cluster_id = m.get('cluster_id')
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
 class UpdateRevisionRequest(TeaModel):
     """
     更新版本元数据
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -47788,14 +52706,91 @@
                 temp_model = SharePermissionPolicy()
                 self.share_policy.append(temp_model.from_map(k))
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
+class UpdateStoryRequest(TeaModel):
+    """
+    # Update story request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        cover: StoryFile = None,
+        custom_id: str = None,
+        custom_labels: dict = None,
+        drive_id: str = None,
+        story_id: str = None,
+        story_name: str = None,
+    ):
+        self.httpheaders = httpheaders
+        self.cover = cover
+        # custom_id
+        self.custom_id = custom_id
+        # custom_labels
+        self.custom_labels = custom_labels
+        # drive_id
+        self.drive_id = drive_id
+        # story_id
+        self.story_id = story_id
+        # story_name
+        self.story_name = story_name
+
+    def validate(self):
+        if self.cover:
+            self.cover.validate()
+        self.validate_required(self.drive_id, 'drive_id')
+        if self.drive_id is not None:
+            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
+        self.validate_required(self.story_id, 'story_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.cover is not None:
+            result['cover'] = self.cover.to_map()
+        if self.custom_id is not None:
+            result['custom_id'] = self.custom_id
+        if self.custom_labels is not None:
+            result['custom_labels'] = self.custom_labels
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.story_id is not None:
+            result['story_id'] = self.story_id
+        if self.story_name is not None:
+            result['story_name'] = self.story_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('cover') is not None:
+            temp_model = StoryFile()
+            self.cover = temp_model.from_map(m['cover'])
+        if m.get('custom_id') is not None:
+            self.custom_id = m.get('custom_id')
+        if m.get('custom_labels') is not None:
+            self.custom_labels = m.get('custom_labels')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('story_id') is not None:
+            self.story_id = m.get('story_id')
+        if m.get('story_name') is not None:
+            self.story_name = m.get('story_name')
+        return self
+
+
 class UpdateSubdomainMgmtRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         description: str = None,
@@ -47883,14 +52878,94 @@
         if m.get('used_size_refresh_interval') is not None:
             self.used_size_refresh_interval = m.get('used_size_refresh_interval')
         if m.get('user_quota') is not None:
             self.user_quota = m.get('user_quota')
         return self
 
 
+class UpdateViewRequest(TeaModel):
+    """
+    Update view request
+    """
+    def __init__(
+        self,
+        httpheaders: Dict[str, str] = None,
+        category: str = None,
+        description: str = None,
+        ex_fields_info: dict = None,
+        file_count: int = None,
+        name: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        self.httpheaders = httpheaders
+        # category
+        self.category = category
+        # description
+        self.description = description
+        # ex_fields_info
+        self.ex_fields_info = ex_fields_info
+        # description
+        self.file_count = file_count
+        # name
+        self.name = name
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.httpheaders is not None:
+            result['httpheaders'] = self.httpheaders
+        if self.category is not None:
+            result['category'] = self.category
+        if self.description is not None:
+            result['description'] = self.description
+        if self.ex_fields_info is not None:
+            result['ex_fields_info'] = self.ex_fields_info
+        if self.file_count is not None:
+            result['file_count'] = self.file_count
+        if self.name is not None:
+            result['name'] = self.name
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('httpheaders') is not None:
+            self.httpheaders = m.get('httpheaders')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('ex_fields_info') is not None:
+            self.ex_fields_info = m.get('ex_fields_info')
+        if m.get('file_count') is not None:
+            self.file_count = m.get('file_count')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class UrlInfo(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         download_url: str = None,
@@ -48104,14 +53179,66 @@
         if m.get('sms_code_id') is not None:
             self.sms_code_id = m.get('sms_code_id')
         if m.get('verify_type') is not None:
             self.verify_type = m.get('verify_type')
         return self
 
 
+class ViewFileBaseRequest(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        category: str = None,
+        drive_id: str = None,
+        user_id: str = None,
+        view_id: str = None,
+    ):
+        # category
+        self.category = category
+        self.drive_id = drive_id
+        # user_id
+        self.user_id = user_id
+        # view_id
+        self.view_id = view_id
+
+    def validate(self):
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.view_id, 'view_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.category is not None:
+            result['category'] = self.category
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.view_id is not None:
+            result['view_id'] = self.view_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('view_id') is not None:
+            self.view_id = m.get('view_id')
+        return self
+
+
 class AddStoreResponse(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         accelerate_endpoint: str = None,
@@ -48320,14 +53447,151 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         return self
 
 
+class GrayscaleConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        enabled: bool = None,
+        percentage: int = None,
+    ):
+        self.enabled = enabled
+        self.percentage = percentage
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.percentage is not None:
+            result['percentage'] = self.percentage
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('percentage') is not None:
+            self.percentage = m.get('percentage')
+        return self
+
+
+class WhitelistConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        drive_whitelist: List[str] = None,
+        enabled: bool = None,
+        whitelist: List[str] = None,
+    ):
+        self.drive_whitelist = drive_whitelist
+        self.enabled = enabled
+        self.whitelist = whitelist
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.drive_whitelist is not None:
+            result['drive_whitelist'] = self.drive_whitelist
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.whitelist is not None:
+            result['whitelist'] = self.whitelist
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_whitelist') is not None:
+            self.drive_whitelist = m.get('drive_whitelist')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('whitelist') is not None:
+            self.whitelist = m.get('whitelist')
+        return self
+
+
+class ApiConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        blacklist: List[str] = None,
+        enabled: bool = None,
+        grayscale_config: GrayscaleConfig = None,
+        status: str = None,
+        whitelist_config: WhitelistConfig = None,
+    ):
+        self.blacklist = blacklist
+        self.enabled = enabled
+        self.grayscale_config = grayscale_config
+        self.status = status
+        self.whitelist_config = whitelist_config
+
+    def validate(self):
+        if self.grayscale_config:
+            self.grayscale_config.validate()
+        if self.whitelist_config:
+            self.whitelist_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.blacklist is not None:
+            result['blacklist'] = self.blacklist
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.grayscale_config is not None:
+            result['grayscale_config'] = self.grayscale_config.to_map()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.whitelist_config is not None:
+            result['whitelist_config'] = self.whitelist_config.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('blacklist') is not None:
+            self.blacklist = m.get('blacklist')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('grayscale_config') is not None:
+            temp_model = GrayscaleConfig()
+            self.grayscale_config = temp_model.from_map(m['grayscale_config'])
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('whitelist_config') is not None:
+            temp_model = WhitelistConfig()
+            self.whitelist_config = temp_model.from_map(m['whitelist_config'])
+        return self
+
+
 class AppConfig(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         allow_upload_custom_file_ext_list: List[str] = None,
@@ -49127,19 +54391,21 @@
 class OfficeEditConfig(TeaModel):
     """
     OfficeEditConfig 文档编辑配置
     """
     def __init__(
         self,
         cross_region_pds_endpoint: str = None,
+        disable_print: bool = None,
         enabled: bool = None,
         encode_user_id: bool = None,
         role: str = None,
     ):
         self.cross_region_pds_endpoint = cross_region_pds_endpoint
+        self.disable_print = disable_print
         self.enabled = enabled
         self.encode_user_id = encode_user_id
         self.role = role
 
     def validate(self):
         pass
 
@@ -49147,26 +54413,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cross_region_pds_endpoint is not None:
             result['cross_region_pds_endpoint'] = self.cross_region_pds_endpoint
+        if self.disable_print is not None:
+            result['disable_print'] = self.disable_print
         if self.enabled is not None:
             result['enabled'] = self.enabled
         if self.encode_user_id is not None:
             result['encode_user_id'] = self.encode_user_id
         if self.role is not None:
             result['role'] = self.role
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('cross_region_pds_endpoint') is not None:
             self.cross_region_pds_endpoint = m.get('cross_region_pds_endpoint')
+        if m.get('disable_print') is not None:
+            self.disable_print = m.get('disable_print')
         if m.get('enabled') is not None:
             self.enabled = m.get('enabled')
         if m.get('encode_user_id') is not None:
             self.encode_user_id = m.get('encode_user_id')
         if m.get('role') is not None:
             self.role = m.get('role')
         return self
@@ -49174,33 +54444,39 @@
 
 class OfficePreviewConfig(TeaModel):
     """
     OfficePreviewConfig 文档预览配置
     """
     def __init__(
         self,
+        disable_print: bool = None,
         enabled: bool = None,
     ):
+        self.disable_print = disable_print
         self.enabled = enabled
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.disable_print is not None:
+            result['disable_print'] = self.disable_print
         if self.enabled is not None:
             result['enabled'] = self.enabled
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('disable_print') is not None:
+            self.disable_print = m.get('disable_print')
         if m.get('enabled') is not None:
             self.enabled = m.get('enabled')
         return self
 
 
 class RecycleBinConfig(TeaModel):
     """
@@ -49246,20 +54522,22 @@
 
 class RoleConfig(TeaModel):
     """
     *\
     """
     def __init__(
         self,
+        default_group_drive_inherit_sub_group: bool = None,
         default_group_drive_role: str = None,
         disabled_admin_file_permission: bool = None,
         enabled: bool = None,
         enabled_admin_delete_personal_file_permission: bool = None,
         enabled_admin_personal_file_permission: bool = None,
     ):
+        self.default_group_drive_inherit_sub_group = default_group_drive_inherit_sub_group
         self.default_group_drive_role = default_group_drive_role
         self.disabled_admin_file_permission = disabled_admin_file_permission
         self.enabled = enabled
         self.enabled_admin_delete_personal_file_permission = enabled_admin_delete_personal_file_permission
         self.enabled_admin_personal_file_permission = enabled_admin_personal_file_permission
 
     def validate(self):
@@ -49267,28 +54545,32 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.default_group_drive_inherit_sub_group is not None:
+            result['default_group_drive_inherit_sub_group'] = self.default_group_drive_inherit_sub_group
         if self.default_group_drive_role is not None:
             result['default_group_drive_role'] = self.default_group_drive_role
         if self.disabled_admin_file_permission is not None:
             result['disabled_admin_file_permission'] = self.disabled_admin_file_permission
         if self.enabled is not None:
             result['enabled'] = self.enabled
         if self.enabled_admin_delete_personal_file_permission is not None:
             result['enabled_admin_delete_personal_file_permission'] = self.enabled_admin_delete_personal_file_permission
         if self.enabled_admin_personal_file_permission is not None:
             result['enabled_admin_personal_file_permission'] = self.enabled_admin_personal_file_permission
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('default_group_drive_inherit_sub_group') is not None:
+            self.default_group_drive_inherit_sub_group = m.get('default_group_drive_inherit_sub_group')
         if m.get('default_group_drive_role') is not None:
             self.default_group_drive_role = m.get('default_group_drive_role')
         if m.get('disabled_admin_file_permission') is not None:
             self.disabled_admin_file_permission = m.get('disabled_admin_file_permission')
         if m.get('enabled') is not None:
             self.enabled = m.get('enabled')
         if m.get('enabled_admin_delete_personal_file_permission') is not None:
@@ -49350,15 +54632,14 @@
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
 
 
 class VideoPreviewAppConfig(TeaModel):
     """
-    前端判断是否可以播放视频流程
     if OnlineVideoTranscodeEnable then do video_preview play  // 如果是离线转码, 那么用OfflineVideoTranscodeEnable代替, 音频类似
     else if appConfig.VideoPlayEnable then do source file play // 音频用AudioPlayEnable代替
     else notify user the function not support
     """
     def __init__(
         self,
         offline_audio_transcode_enable: bool = None,
@@ -49539,14 +54820,50 @@
         if m.get('skip_begin_percent') is not None:
             self.skip_begin_percent = m.get('skip_begin_percent')
         if m.get('skip_begin_sec') is not None:
             self.skip_begin_sec = m.get('skip_begin_sec')
         return self
 
 
+class VideoPreviewAutoCategoryConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        default_audio_category: str = None,
+        default_video_category: str = None,
+    ):
+        self.default_audio_category = default_audio_category
+        self.default_video_category = default_video_category
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default_audio_category is not None:
+            result['default_audio_category'] = self.default_audio_category
+        if self.default_video_category is not None:
+            result['default_video_category'] = self.default_video_category
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('default_audio_category') is not None:
+            self.default_audio_category = m.get('default_audio_category')
+        if m.get('default_video_category') is not None:
+            self.default_video_category = m.get('default_video_category')
+        return self
+
+
 class VideoPreviewBackupConfig(TeaModel):
     """
     转码备份配置（当前仅运维会用到）
     """
     def __init__(
         self,
         count_once: int = None,
@@ -49583,14 +54900,67 @@
             temp_model = Store()
             self.store = temp_model.from_map(m['store'])
         if m.get('store_id_map') is not None:
             self.store_id_map = m.get('store_id_map')
         return self
 
 
+class VideoPreviewCdnConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        cache_store: Store = None,
+        enable_m3u_8cache: bool = None,
+        enabled: bool = None,
+        gray_config: ApiConfig = None,
+    ):
+        self.cache_store = cache_store
+        self.enable_m3u_8cache = enable_m3u_8cache
+        self.enabled = enabled
+        self.gray_config = gray_config
+
+    def validate(self):
+        if self.cache_store:
+            self.cache_store.validate()
+        if self.gray_config:
+            self.gray_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cache_store is not None:
+            result['cache_store'] = self.cache_store.to_map()
+        if self.enable_m3u_8cache is not None:
+            result['enable_m3u8_cache'] = self.enable_m3u_8cache
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.gray_config is not None:
+            result['gray_config'] = self.gray_config.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cache_store') is not None:
+            temp_model = Store()
+            self.cache_store = temp_model.from_map(m['cache_store'])
+        if m.get('enable_m3u8_cache') is not None:
+            self.enable_m3u_8cache = m.get('enable_m3u8_cache')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('gray_config') is not None:
+            temp_model = ApiConfig()
+            self.gray_config = temp_model.from_map(m['gray_config'])
+        return self
+
+
 class VideoPreviewDrmConfig(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         region: str = None,
@@ -49668,14 +55038,58 @@
         if m.get('enable_transcode_when_play') is not None:
             self.enable_transcode_when_play = m.get('enable_transcode_when_play')
         if m.get('enable_transcode_when_uploaded') is not None:
             self.enable_transcode_when_uploaded = m.get('enable_transcode_when_uploaded')
         return self
 
 
+class VideoPreviewHlsSignParamsConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        disable_headers: bool = None,
+        enabled: bool = None,
+        gray_config: ApiConfig = None,
+    ):
+        self.disable_headers = disable_headers
+        self.enabled = enabled
+        self.gray_config = gray_config
+
+    def validate(self):
+        if self.gray_config:
+            self.gray_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.disable_headers is not None:
+            result['disable_headers'] = self.disable_headers
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.gray_config is not None:
+            result['gray_config'] = self.gray_config.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('disable_headers') is not None:
+            self.disable_headers = m.get('disable_headers')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('gray_config') is not None:
+            temp_model = ApiConfig()
+            self.gray_config = temp_model.from_map(m['gray_config'])
+        return self
+
+
 class VideoPreviewLiveTranscodingEnableConfig(TeaModel):
     """
     实时转码子开关配置
     """
     def __init__(
         self,
         disable_live_transcode: bool = None,
@@ -49936,14 +55350,154 @@
         if m.get('ts_count_when_ts_404') is not None:
             self.ts_count_when_ts_404 = m.get('ts_count_when_ts_404')
         if m.get('ts_file_prefix') is not None:
             self.ts_file_prefix = m.get('ts_file_prefix')
         return self
 
 
+class VideoPreviewQuickVideoInitialTsConfig(TeaModel):
+    """
+    快速起播配置
+    """
+    def __init__(
+        self,
+        initial_duration: float = None,
+        initial_ts_list: List[int] = None,
+    ):
+        self.initial_duration = initial_duration
+        self.initial_ts_list = initial_ts_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.initial_duration is not None:
+            result['initial_duration'] = self.initial_duration
+        if self.initial_ts_list is not None:
+            result['initial_ts_list'] = self.initial_ts_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('initial_duration') is not None:
+            self.initial_duration = m.get('initial_duration')
+        if m.get('initial_ts_list') is not None:
+            self.initial_ts_list = m.get('initial_ts_list')
+        return self
+
+
+class VideoPreviewQuickVideoConfig(TeaModel):
+    """
+    *\
+    """
+    def __init__(
+        self,
+        current_version: int = None,
+        deprecated_version: int = None,
+        enable_config: VideoPreviewLiveTranscodingEnableConfig = None,
+        enabled: bool = None,
+        initial_ts_config: VideoPreviewQuickVideoInitialTsConfig = None,
+        leading_prefix: str = None,
+        m_3u_8file_prefix: str = None,
+        segment: int = None,
+        subtitle_config: VideoPreviewLiveTranscodingSubtitleConfig = None,
+        template_list: List[str] = None,
+        template_name_map: dict = None,
+        ts_count_when_ts_404: int = None,
+    ):
+        self.current_version = current_version
+        self.deprecated_version = deprecated_version
+        self.enable_config = enable_config
+        self.enabled = enabled
+        self.initial_ts_config = initial_ts_config
+        self.leading_prefix = leading_prefix
+        self.m_3u_8file_prefix = m_3u_8file_prefix
+        self.segment = segment
+        self.subtitle_config = subtitle_config
+        self.template_list = template_list
+        self.template_name_map = template_name_map
+        self.ts_count_when_ts_404 = ts_count_when_ts_404
+
+    def validate(self):
+        if self.enable_config:
+            self.enable_config.validate()
+        if self.initial_ts_config:
+            self.initial_ts_config.validate()
+        if self.subtitle_config:
+            self.subtitle_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_version is not None:
+            result['current_version'] = self.current_version
+        if self.deprecated_version is not None:
+            result['deprecated_version'] = self.deprecated_version
+        if self.enable_config is not None:
+            result['enable_config'] = self.enable_config.to_map()
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.initial_ts_config is not None:
+            result['initial_ts_config'] = self.initial_ts_config.to_map()
+        if self.leading_prefix is not None:
+            result['leading_prefix'] = self.leading_prefix
+        if self.m_3u_8file_prefix is not None:
+            result['m3u8_file_prefix'] = self.m_3u_8file_prefix
+        if self.segment is not None:
+            result['segment'] = self.segment
+        if self.subtitle_config is not None:
+            result['subtitle_config'] = self.subtitle_config.to_map()
+        if self.template_list is not None:
+            result['template_list'] = self.template_list
+        if self.template_name_map is not None:
+            result['template_name_map'] = self.template_name_map
+        if self.ts_count_when_ts_404 is not None:
+            result['ts_count_when_ts_404'] = self.ts_count_when_ts_404
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('current_version') is not None:
+            self.current_version = m.get('current_version')
+        if m.get('deprecated_version') is not None:
+            self.deprecated_version = m.get('deprecated_version')
+        if m.get('enable_config') is not None:
+            temp_model = VideoPreviewLiveTranscodingEnableConfig()
+            self.enable_config = temp_model.from_map(m['enable_config'])
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('initial_ts_config') is not None:
+            temp_model = VideoPreviewQuickVideoInitialTsConfig()
+            self.initial_ts_config = temp_model.from_map(m['initial_ts_config'])
+        if m.get('leading_prefix') is not None:
+            self.leading_prefix = m.get('leading_prefix')
+        if m.get('m3u8_file_prefix') is not None:
+            self.m_3u_8file_prefix = m.get('m3u8_file_prefix')
+        if m.get('segment') is not None:
+            self.segment = m.get('segment')
+        if m.get('subtitle_config') is not None:
+            temp_model = VideoPreviewLiveTranscodingSubtitleConfig()
+            self.subtitle_config = temp_model.from_map(m['subtitle_config'])
+        if m.get('template_list') is not None:
+            self.template_list = m.get('template_list')
+        if m.get('template_name_map') is not None:
+            self.template_name_map = m.get('template_name_map')
+        if m.get('ts_count_when_ts_404') is not None:
+            self.ts_count_when_ts_404 = m.get('ts_count_when_ts_404')
+        return self
+
+
 class VideoPreviewRateLimitConfig(TeaModel):
     """
     转码文件下载限速配置
     """
     def __init__(
         self,
         rate_limit: int = None,
@@ -50496,60 +56050,78 @@
     转码配置
     """
     def __init__(
         self,
         audio_config: VideoPreviewAudioConfig = None,
         audio_template_list: List[str] = None,
         audio_thumbnail: VideoPreviewThumbnailConfig = None,
+        auto_category_config: VideoPreviewAutoCategoryConfig = None,
         backup_config: VideoPreviewBackupConfig = None,
+        cdn_config: VideoPreviewCdnConfig = None,
         drm_config: VideoPreviewDrmConfig = None,
         enable_config: VideoPreviewEnableConfig = None,
         enabled: bool = None,
+        hls_sign_params_config: VideoPreviewHlsSignParamsConfig = None,
         live_transcoding_config: VideoPreviewLiveTranscodingConfig = None,
+        quick_video_config: VideoPreviewQuickVideoConfig = None,
         rate_limit_config: VideoPreviewRateLimitConfig = None,
         sprite: VideoPreviewSpriteConfig = None,
         store: Store = None,
         store_id_map: dict = None,
         template_list: List[str] = None,
+        template_name_map: dict = None,
         template_policy_config: VideoPreviewTemplatePolicyConfig = None,
         thumbnail: VideoPreviewThumbnailConfig = None,
         video_config: VideoPreviewVideoConfig = None,
         video_filter_config: VideoPreviewVideoFilterConfig = None,
     ):
         self.audio_config = audio_config
         self.audio_template_list = audio_template_list
         self.audio_thumbnail = audio_thumbnail
+        self.auto_category_config = auto_category_config
         self.backup_config = backup_config
+        self.cdn_config = cdn_config
         self.drm_config = drm_config
         self.enable_config = enable_config
         self.enabled = enabled
+        self.hls_sign_params_config = hls_sign_params_config
         self.live_transcoding_config = live_transcoding_config
+        self.quick_video_config = quick_video_config
         self.rate_limit_config = rate_limit_config
         self.sprite = sprite
         self.store = store
         self.store_id_map = store_id_map
         self.template_list = template_list
+        self.template_name_map = template_name_map
         self.template_policy_config = template_policy_config
         self.thumbnail = thumbnail
         self.video_config = video_config
         self.video_filter_config = video_filter_config
 
     def validate(self):
         if self.audio_config:
             self.audio_config.validate()
         if self.audio_thumbnail:
             self.audio_thumbnail.validate()
+        if self.auto_category_config:
+            self.auto_category_config.validate()
         if self.backup_config:
             self.backup_config.validate()
+        if self.cdn_config:
+            self.cdn_config.validate()
         if self.drm_config:
             self.drm_config.validate()
         if self.enable_config:
             self.enable_config.validate()
+        if self.hls_sign_params_config:
+            self.hls_sign_params_config.validate()
         if self.live_transcoding_config:
             self.live_transcoding_config.validate()
+        if self.quick_video_config:
+            self.quick_video_config.validate()
         if self.rate_limit_config:
             self.rate_limit_config.validate()
         if self.sprite:
             self.sprite.validate()
         if self.store:
             self.store.validate()
         if self.template_policy_config:
@@ -50569,34 +56141,44 @@
         result = dict()
         if self.audio_config is not None:
             result['audio_config'] = self.audio_config.to_map()
         if self.audio_template_list is not None:
             result['audio_template_list'] = self.audio_template_list
         if self.audio_thumbnail is not None:
             result['audio_thumbnail'] = self.audio_thumbnail.to_map()
+        if self.auto_category_config is not None:
+            result['auto_category_config'] = self.auto_category_config.to_map()
         if self.backup_config is not None:
             result['backup_config'] = self.backup_config.to_map()
+        if self.cdn_config is not None:
+            result['cdn_config'] = self.cdn_config.to_map()
         if self.drm_config is not None:
             result['drm_config'] = self.drm_config.to_map()
         if self.enable_config is not None:
             result['enable_config'] = self.enable_config.to_map()
         if self.enabled is not None:
             result['enabled'] = self.enabled
+        if self.hls_sign_params_config is not None:
+            result['hls_sign_params_config'] = self.hls_sign_params_config.to_map()
         if self.live_transcoding_config is not None:
             result['live_transcoding_config'] = self.live_transcoding_config.to_map()
+        if self.quick_video_config is not None:
+            result['quick_video_config'] = self.quick_video_config.to_map()
         if self.rate_limit_config is not None:
             result['rate_limit_config'] = self.rate_limit_config.to_map()
         if self.sprite is not None:
             result['sprite'] = self.sprite.to_map()
         if self.store is not None:
             result['store'] = self.store.to_map()
         if self.store_id_map is not None:
             result['store_id_map'] = self.store_id_map
         if self.template_list is not None:
             result['template_list'] = self.template_list
+        if self.template_name_map is not None:
+            result['template_name_map'] = self.template_name_map
         if self.template_policy_config is not None:
             result['template_policy_config'] = self.template_policy_config.to_map()
         if self.thumbnail is not None:
             result['thumbnail'] = self.thumbnail.to_map()
         if self.video_config is not None:
             result['video_config'] = self.video_config.to_map()
         if self.video_filter_config is not None:
@@ -50609,41 +56191,55 @@
             temp_model = VideoPreviewAudioConfig()
             self.audio_config = temp_model.from_map(m['audio_config'])
         if m.get('audio_template_list') is not None:
             self.audio_template_list = m.get('audio_template_list')
         if m.get('audio_thumbnail') is not None:
             temp_model = VideoPreviewThumbnailConfig()
             self.audio_thumbnail = temp_model.from_map(m['audio_thumbnail'])
+        if m.get('auto_category_config') is not None:
+            temp_model = VideoPreviewAutoCategoryConfig()
+            self.auto_category_config = temp_model.from_map(m['auto_category_config'])
         if m.get('backup_config') is not None:
             temp_model = VideoPreviewBackupConfig()
             self.backup_config = temp_model.from_map(m['backup_config'])
+        if m.get('cdn_config') is not None:
+            temp_model = VideoPreviewCdnConfig()
+            self.cdn_config = temp_model.from_map(m['cdn_config'])
         if m.get('drm_config') is not None:
             temp_model = VideoPreviewDrmConfig()
             self.drm_config = temp_model.from_map(m['drm_config'])
         if m.get('enable_config') is not None:
             temp_model = VideoPreviewEnableConfig()
             self.enable_config = temp_model.from_map(m['enable_config'])
         if m.get('enabled') is not None:
             self.enabled = m.get('enabled')
+        if m.get('hls_sign_params_config') is not None:
+            temp_model = VideoPreviewHlsSignParamsConfig()
+            self.hls_sign_params_config = temp_model.from_map(m['hls_sign_params_config'])
         if m.get('live_transcoding_config') is not None:
             temp_model = VideoPreviewLiveTranscodingConfig()
             self.live_transcoding_config = temp_model.from_map(m['live_transcoding_config'])
+        if m.get('quick_video_config') is not None:
+            temp_model = VideoPreviewQuickVideoConfig()
+            self.quick_video_config = temp_model.from_map(m['quick_video_config'])
         if m.get('rate_limit_config') is not None:
             temp_model = VideoPreviewRateLimitConfig()
             self.rate_limit_config = temp_model.from_map(m['rate_limit_config'])
         if m.get('sprite') is not None:
             temp_model = VideoPreviewSpriteConfig()
             self.sprite = temp_model.from_map(m['sprite'])
         if m.get('store') is not None:
             temp_model = Store()
             self.store = temp_model.from_map(m['store'])
         if m.get('store_id_map') is not None:
             self.store_id_map = m.get('store_id_map')
         if m.get('template_list') is not None:
             self.template_list = m.get('template_list')
+        if m.get('template_name_map') is not None:
+            self.template_name_map = m.get('template_name_map')
         if m.get('template_policy_config') is not None:
             temp_model = VideoPreviewTemplatePolicyConfig()
             self.template_policy_config = temp_model.from_map(m['template_policy_config'])
         if m.get('thumbnail') is not None:
             temp_model = VideoPreviewThumbnailConfig()
             self.thumbnail = temp_model.from_map(m['thumbnail'])
         if m.get('video_config') is not None:
@@ -50805,14 +56401,15 @@
         role_config: RoleConfig = None,
         service_code: str = None,
         sharable: bool = None,
         share_detail: ShareDetailResponse = None,
         share_link_detail: ShareLinkDetailResponse = None,
         share_link_enabled: bool = None,
         size_quota: int = None,
+        size_quota_used: int = None,
         spi_instance_id: str = None,
         status: int = None,
         store_level: str = None,
         store_region_list: List[str] = None,
         subdomain_config: SubdomainConfig = None,
         updated_at: str = None,
         used_size: int = None,
@@ -50905,14 +56502,15 @@
         self.sharable = sharable
         self.share_detail = share_detail
         self.share_link_detail = share_link_detail
         # 是否开启了分享
         self.share_link_enabled = share_link_enabled
         # 容量配额
         self.size_quota = size_quota
+        self.size_quota_used = size_quota_used
         # SPI 实例 id
         self.spi_instance_id = spi_instance_id
         # domain状态：创建中，正常，已过期
         self.status = status
         # 存储级别
         self.store_level = store_level
         # 存储 Region 列表
@@ -51076,14 +56674,16 @@
             result['share_detail'] = self.share_detail.to_map()
         if self.share_link_detail is not None:
             result['share_link_detail'] = self.share_link_detail.to_map()
         if self.share_link_enabled is not None:
             result['share_link_enabled'] = self.share_link_enabled
         if self.size_quota is not None:
             result['size_quota'] = self.size_quota
+        if self.size_quota_used is not None:
+            result['size_quota_used'] = self.size_quota_used
         if self.spi_instance_id is not None:
             result['spi_instance_id'] = self.spi_instance_id
         if self.status is not None:
             result['status'] = self.status
         if self.store_level is not None:
             result['store_level'] = self.store_level
         if self.store_region_list is not None:
@@ -51224,14 +56824,16 @@
         if m.get('share_link_detail') is not None:
             temp_model = ShareLinkDetailResponse()
             self.share_link_detail = temp_model.from_map(m['share_link_detail'])
         if m.get('share_link_enabled') is not None:
             self.share_link_enabled = m.get('share_link_enabled')
         if m.get('size_quota') is not None:
             self.size_quota = m.get('size_quota')
+        if m.get('size_quota_used') is not None:
+            self.size_quota_used = m.get('size_quota_used')
         if m.get('spi_instance_id') is not None:
             self.spi_instance_id = m.get('spi_instance_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('store_level') is not None:
             self.store_level = m.get('store_level')
         if m.get('store_region_list') is not None:
@@ -51495,14 +57097,15 @@
         role_config: RoleConfig = None,
         service_code: str = None,
         sharable: bool = None,
         share_detail: ShareDetailResponse = None,
         share_link_detail: ShareLinkDetailResponse = None,
         share_link_enabled: bool = None,
         size_quota: int = None,
+        size_quota_used: int = None,
         spi_instance_id: str = None,
         status: int = None,
         store_level: str = None,
         store_region_list: List[str] = None,
         subdomain_config: SubdomainConfig = None,
         updated_at: str = None,
         used_size: int = None,
@@ -51595,14 +57198,15 @@
         self.sharable = sharable
         self.share_detail = share_detail
         self.share_link_detail = share_link_detail
         # 是否开启了分享
         self.share_link_enabled = share_link_enabled
         # 容量配额
         self.size_quota = size_quota
+        self.size_quota_used = size_quota_used
         # SPI 实例 id
         self.spi_instance_id = spi_instance_id
         # domain状态：创建中，正常，已过期
         self.status = status
         # 存储级别
         self.store_level = store_level
         # 存储 Region 列表
@@ -51766,14 +57370,16 @@
             result['share_detail'] = self.share_detail.to_map()
         if self.share_link_detail is not None:
             result['share_link_detail'] = self.share_link_detail.to_map()
         if self.share_link_enabled is not None:
             result['share_link_enabled'] = self.share_link_enabled
         if self.size_quota is not None:
             result['size_quota'] = self.size_quota
+        if self.size_quota_used is not None:
+            result['size_quota_used'] = self.size_quota_used
         if self.spi_instance_id is not None:
             result['spi_instance_id'] = self.spi_instance_id
         if self.status is not None:
             result['status'] = self.status
         if self.store_level is not None:
             result['store_level'] = self.store_level
         if self.store_region_list is not None:
@@ -51914,14 +57520,16 @@
         if m.get('share_link_detail') is not None:
             temp_model = ShareLinkDetailResponse()
             self.share_link_detail = temp_model.from_map(m['share_link_detail'])
         if m.get('share_link_enabled') is not None:
             self.share_link_enabled = m.get('share_link_enabled')
         if m.get('size_quota') is not None:
             self.size_quota = m.get('size_quota')
+        if m.get('size_quota_used') is not None:
+            self.size_quota_used = m.get('size_quota_used')
         if m.get('spi_instance_id') is not None:
             self.spi_instance_id = m.get('spi_instance_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('store_level') is not None:
             self.store_level = m.get('store_level')
         if m.get('store_region_list') is not None:
@@ -52649,33 +58257,37 @@
         biz_cname: str = None,
         cert_id: str = None,
         cert_name: str = None,
         cname_status: CNameStatus = None,
         cname_type: str = None,
         domain_id: str = None,
         is_vpc: bool = None,
+        subdomain_id: str = None,
     ):
         # biz cname
         self.biz_cname = biz_cname
         # cert name
         self.cert_id = cert_id
         # cert name
         self.cert_name = cert_name
         self.cname_status = cname_status
         # cname type
         self.cname_type = cname_type
         # domain ID
         self.domain_id = domain_id
         # is vpc
         self.is_vpc = is_vpc
+        # subdomain ID
+        self.subdomain_id = subdomain_id
 
     def validate(self):
         if self.cname_status:
             self.cname_status.validate()
         self.validate_required(self.domain_id, 'domain_id')
+        self.validate_required(self.subdomain_id, 'subdomain_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -52689,14 +58301,16 @@
             result['cname_status'] = self.cname_status.to_map()
         if self.cname_type is not None:
             result['cname_type'] = self.cname_type
         if self.domain_id is not None:
             result['domain_id'] = self.domain_id
         if self.is_vpc is not None:
             result['is_vpc'] = self.is_vpc
+        if self.subdomain_id is not None:
+            result['subdomain_id'] = self.subdomain_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('biz_cname') is not None:
             self.biz_cname = m.get('biz_cname')
         if m.get('cert_id') is not None:
@@ -52708,14 +58322,16 @@
             self.cname_status = temp_model.from_map(m['cname_status'])
         if m.get('cname_type') is not None:
             self.cname_type = m.get('cname_type')
         if m.get('domain_id') is not None:
             self.domain_id = m.get('domain_id')
         if m.get('is_vpc') is not None:
             self.is_vpc = m.get('is_vpc')
+        if m.get('subdomain_id') is not None:
+            self.subdomain_id = m.get('subdomain_id')
         return self
 
 
 class GetDomainResponse(TeaModel):
     """
     get domain response
     """
@@ -52769,14 +58385,15 @@
         role_config: RoleConfig = None,
         service_code: str = None,
         sharable: bool = None,
         share_detail: ShareDetailResponse = None,
         share_link_detail: ShareLinkDetailResponse = None,
         share_link_enabled: bool = None,
         size_quota: int = None,
+        size_quota_used: int = None,
         spi_instance_id: str = None,
         status: int = None,
         store_level: str = None,
         store_region_list: List[str] = None,
         subdomain_config: SubdomainConfig = None,
         updated_at: str = None,
         used_size: int = None,
@@ -52869,14 +58486,15 @@
         self.sharable = sharable
         self.share_detail = share_detail
         self.share_link_detail = share_link_detail
         # 是否开启了分享
         self.share_link_enabled = share_link_enabled
         # 容量配额
         self.size_quota = size_quota
+        self.size_quota_used = size_quota_used
         # SPI 实例 id
         self.spi_instance_id = spi_instance_id
         # domain状态：创建中，正常，已过期
         self.status = status
         # 存储级别
         self.store_level = store_level
         # 存储 Region 列表
@@ -53040,14 +58658,16 @@
             result['share_detail'] = self.share_detail.to_map()
         if self.share_link_detail is not None:
             result['share_link_detail'] = self.share_link_detail.to_map()
         if self.share_link_enabled is not None:
             result['share_link_enabled'] = self.share_link_enabled
         if self.size_quota is not None:
             result['size_quota'] = self.size_quota
+        if self.size_quota_used is not None:
+            result['size_quota_used'] = self.size_quota_used
         if self.spi_instance_id is not None:
             result['spi_instance_id'] = self.spi_instance_id
         if self.status is not None:
             result['status'] = self.status
         if self.store_level is not None:
             result['store_level'] = self.store_level
         if self.store_region_list is not None:
@@ -53188,14 +58808,16 @@
         if m.get('share_link_detail') is not None:
             temp_model = ShareLinkDetailResponse()
             self.share_link_detail = temp_model.from_map(m['share_link_detail'])
         if m.get('share_link_enabled') is not None:
             self.share_link_enabled = m.get('share_link_enabled')
         if m.get('size_quota') is not None:
             self.size_quota = m.get('size_quota')
+        if m.get('size_quota_used') is not None:
+            self.size_quota_used = m.get('size_quota_used')
         if m.get('spi_instance_id') is not None:
             self.spi_instance_id = m.get('spi_instance_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('store_level') is not None:
             self.store_level = m.get('store_level')
         if m.get('store_region_list') is not None:
@@ -54136,14 +59758,15 @@
         role_config: RoleConfig = None,
         service_code: str = None,
         sharable: bool = None,
         share_detail: ShareDetailResponse = None,
         share_link_detail: ShareLinkDetailResponse = None,
         share_link_enabled: bool = None,
         size_quota: int = None,
+        size_quota_used: int = None,
         spi_instance_id: str = None,
         status: int = None,
         store_level: str = None,
         store_region_list: List[str] = None,
         subdomain_config: SubdomainConfig = None,
         updated_at: str = None,
         used_size: int = None,
@@ -54236,14 +59859,15 @@
         self.sharable = sharable
         self.share_detail = share_detail
         self.share_link_detail = share_link_detail
         # 是否开启了分享
         self.share_link_enabled = share_link_enabled
         # 容量配额
         self.size_quota = size_quota
+        self.size_quota_used = size_quota_used
         # SPI 实例 id
         self.spi_instance_id = spi_instance_id
         # domain状态：创建中，正常，已过期
         self.status = status
         # 存储级别
         self.store_level = store_level
         # 存储 Region 列表
@@ -54407,14 +60031,16 @@
             result['share_detail'] = self.share_detail.to_map()
         if self.share_link_detail is not None:
             result['share_link_detail'] = self.share_link_detail.to_map()
         if self.share_link_enabled is not None:
             result['share_link_enabled'] = self.share_link_enabled
         if self.size_quota is not None:
             result['size_quota'] = self.size_quota
+        if self.size_quota_used is not None:
+            result['size_quota_used'] = self.size_quota_used
         if self.spi_instance_id is not None:
             result['spi_instance_id'] = self.spi_instance_id
         if self.status is not None:
             result['status'] = self.status
         if self.store_level is not None:
             result['store_level'] = self.store_level
         if self.store_region_list is not None:
@@ -54555,14 +60181,16 @@
         if m.get('share_link_detail') is not None:
             temp_model = ShareLinkDetailResponse()
             self.share_link_detail = temp_model.from_map(m['share_link_detail'])
         if m.get('share_link_enabled') is not None:
             self.share_link_enabled = m.get('share_link_enabled')
         if m.get('size_quota') is not None:
             self.size_quota = m.get('size_quota')
+        if m.get('size_quota_used') is not None:
+            self.size_quota_used = m.get('size_quota_used')
         if m.get('spi_instance_id') is not None:
             self.spi_instance_id = m.get('spi_instance_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('store_level') is not None:
             self.store_level = m.get('store_level')
         if m.get('store_region_list') is not None:
@@ -55004,121 +60632,67 @@
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('punish_reason') is not None:
             self.punish_reason = m.get('punish_reason')
         return self
 
 
-class StoryFile(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        drive_id: str = None,
-        file_id: str = None,
-        revision_id: str = None,
-    ):
-        self.drive_id = drive_id
-        self.file_id = file_id
-        self.revision_id = revision_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.revision_id is not None:
-            result['revision_id'] = self.revision_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('revision_id') is not None:
-            self.revision_id = m.get('revision_id')
-        return self
-
-
-class AddStoryFilesRequest(TeaModel):
+class SearchViewFilesResponse(TeaModel):
     """
-    add story files request
+    search view files response
     """
     def __init__(
         self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        files: List[StoryFile] = None,
-        story_id: str = None,
+        items: List[ViewFileItem] = None,
+        next_marker: str = None,
+        total_count: int = None,
     ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        self.files = files
-        # story_id
-        self.story_id = story_id
+        self.items = items
+        self.next_marker = next_marker
+        self.total_count = total_count
 
     def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.files:
-            for k in self.files:
+        if self.items:
+            for k in self.items:
                 if k:
                     k.validate()
-        self.validate_required(self.story_id, 'story_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        result['files'] = []
-        if self.files is not None:
-            for k in self.files:
-                result['files'].append(k.to_map() if k else None)
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
+        result['items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['items'].append(k.to_map() if k else None)
+        if self.next_marker is not None:
+            result['next_marker'] = self.next_marker
+        if self.total_count is not None:
+            result['total_count'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        self.files = []
-        if m.get('files') is not None:
-            for k in m.get('files'):
-                temp_model = StoryFile()
-                self.files.append(temp_model.from_map(k))
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
+        self.items = []
+        if m.get('items') is not None:
+            for k in m.get('items'):
+                temp_model = ViewFileItem()
+                self.items.append(temp_model.from_map(k))
+        if m.get('next_marker') is not None:
+            self.next_marker = m.get('next_marker')
+        if m.get('total_count') is not None:
+            self.total_count = m.get('total_count')
         return self
 
 
 class AddUserToSubdomainRequest(TeaModel):
     """
-    Add user to subdomain request
+    # Add user to subdomain request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         role: str = None,
         subdomain_id: str = None,
         user_id: str = None,
@@ -55158,117 +60732,14 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class AddViewFileRequest(TeaModel):
-    """
-    add file to view
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        drive_id: str = None,
-        fields: dict = None,
-        file_id: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        self.drive_id = drive_id
-        self.fields = fields
-        self.file_id = file_id
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.fields is not None:
-            result['fields'] = self.fields
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('fields') is not None:
-            self.fields = m.get('fields')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class AlbumsBaseRequest(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        drive_id: str = None,
-    ):
-        # drive_id
-        self.drive_id = drive_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        return self
-
-
 class AssignRequest(TeaModel):
     """
     分配角色请求
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -55451,60 +60922,14 @@
         if m.get('group_name') is not None:
             self.group_name = m.get('group_name')
         if m.get('is_root') is not None:
             self.is_root = m.get('is_root')
         return self
 
 
-class BaseRequest(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        category: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        # category
-        self.category = category
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.category is not None:
-            result['category'] = self.category
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
 class BindDeviceRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -55645,230 +61070,14 @@
         if m.get('role_id') is not None:
             self.role_id = m.get('role_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class CopyViewFilesRequest(TeaModel):
-    """
-    Copy view files
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        addition_data: dict = None,
-        auto_rename: bool = None,
-        category: str = None,
-        drive_file_list: List[ShareFile] = None,
-        referer: str = None,
-        share_id: str = None,
-        to_drive_id: str = None,
-        to_parent_file_id: str = None,
-        to_view_id: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # addition_data
-        self.addition_data = addition_data
-        # auto_rename
-        # type: boolean
-        self.auto_rename = auto_rename
-        # category
-        self.category = category
-        self.drive_file_list = drive_file_list
-        self.referer = referer
-        # share_id
-        self.share_id = share_id
-        # to_drive_id
-        self.to_drive_id = to_drive_id
-        # to_parent_file_id
-        self.to_parent_file_id = to_parent_file_id
-        # to_view_id
-        self.to_view_id = to_view_id
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        if self.drive_file_list:
-            for k in self.drive_file_list:
-                if k:
-                    k.validate()
-        if self.to_drive_id is not None:
-            self.validate_pattern(self.to_drive_id, 'to_drive_id', '[0-9]+')
-        self.validate_required(self.to_parent_file_id, 'to_parent_file_id')
-        if self.to_parent_file_id is not None:
-            self.validate_max_length(self.to_parent_file_id, 'to_parent_file_id', 50)
-            self.validate_pattern(self.to_parent_file_id, 'to_parent_file_id', '[a-z0-9.-_]{1,50}')
-        self.validate_required(self.to_view_id, 'to_view_id')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.addition_data is not None:
-            result['addition_data'] = self.addition_data
-        if self.auto_rename is not None:
-            result['auto_rename'] = self.auto_rename
-        if self.category is not None:
-            result['category'] = self.category
-        result['drive_file_list'] = []
-        if self.drive_file_list is not None:
-            for k in self.drive_file_list:
-                result['drive_file_list'].append(k.to_map() if k else None)
-        if self.referer is not None:
-            result['referer'] = self.referer
-        if self.share_id is not None:
-            result['share_id'] = self.share_id
-        if self.to_drive_id is not None:
-            result['to_drive_id'] = self.to_drive_id
-        if self.to_parent_file_id is not None:
-            result['to_parent_file_id'] = self.to_parent_file_id
-        if self.to_view_id is not None:
-            result['to_view_id'] = self.to_view_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('addition_data') is not None:
-            self.addition_data = m.get('addition_data')
-        if m.get('auto_rename') is not None:
-            self.auto_rename = m.get('auto_rename')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        self.drive_file_list = []
-        if m.get('drive_file_list') is not None:
-            for k in m.get('drive_file_list'):
-                temp_model = ShareFile()
-                self.drive_file_list.append(temp_model.from_map(k))
-        if m.get('referer') is not None:
-            self.referer = m.get('referer')
-        if m.get('share_id') is not None:
-            self.share_id = m.get('share_id')
-        if m.get('to_drive_id') is not None:
-            self.to_drive_id = m.get('to_drive_id')
-        if m.get('to_parent_file_id') is not None:
-            self.to_parent_file_id = m.get('to_parent_file_id')
-        if m.get('to_view_id') is not None:
-            self.to_view_id = m.get('to_view_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class CreateCustomizedStoryRequest(TeaModel):
-    """
-    Create custom story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        custom_labels: dict = None,
-        drive_id: str = None,
-        story_cover: StoryFile = None,
-        story_files: List[StoryFile] = None,
-        story_name: str = None,
-        story_sub_type: str = None,
-        story_type: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # custom_labels
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        self.story_cover = story_cover
-        # story_file_ids
-        self.story_files = story_files
-        # story_name
-        self.story_name = story_name
-        # story_sub_type
-        self.story_sub_type = story_sub_type
-        # story_type
-        self.story_type = story_type
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.story_cover:
-            self.story_cover.validate()
-        if self.story_files:
-            for k in self.story_files:
-                if k:
-                    k.validate()
-        self.validate_required(self.story_type, 'story_type')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.story_cover is not None:
-            result['story_cover'] = self.story_cover.to_map()
-        result['story_files'] = []
-        if self.story_files is not None:
-            for k in self.story_files:
-                result['story_files'].append(k.to_map() if k else None)
-        if self.story_name is not None:
-            result['story_name'] = self.story_name
-        if self.story_sub_type is not None:
-            result['story_sub_type'] = self.story_sub_type
-        if self.story_type is not None:
-            result['story_type'] = self.story_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('story_cover') is not None:
-            temp_model = StoryFile()
-            self.story_cover = temp_model.from_map(m['story_cover'])
-        self.story_files = []
-        if m.get('story_files') is not None:
-            for k in m.get('story_files'):
-                temp_model = StoryFile()
-                self.story_files.append(temp_model.from_map(k))
-        if m.get('story_name') is not None:
-            self.story_name = m.get('story_name')
-        if m.get('story_sub_type') is not None:
-            self.story_sub_type = m.get('story_sub_type')
-        if m.get('story_type') is not None:
-            self.story_type = m.get('story_type')
-        return self
-
-
 class CreateGroupRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -56096,200 +61305,109 @@
         if m.get('resource_type') is not None:
             self.resource_type = m.get('resource_type')
         if m.get('user_tags') is not None:
             self.user_tags = m.get('user_tags')
         return self
 
 
-class CreateStoryRequest(TeaModel):
-    """
-    Create story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        address: Address = None,
-        custom_id: str = None,
-        custom_labels: dict = None,
-        drive_id: str = None,
-        max_image_count: int = None,
-        min_image_count: int = None,
-        story_end_time: str = None,
-        story_id: str = None,
-        story_name: str = None,
-        story_start_time: str = None,
-        story_sub_type: str = None,
-        story_type: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.address = address
-        # custom_id
-        self.custom_id = custom_id
-        # custom_labels
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        # max_image_count
-        self.max_image_count = max_image_count
-        # min_image_count
-        self.min_image_count = min_image_count
-        # story_end_time
-        self.story_end_time = story_end_time
-        # story_id
-        self.story_id = story_id
-        # story_name
-        self.story_name = story_name
-        # story_start_time
-        self.story_start_time = story_start_time
-        # story_sub_type
-        self.story_sub_type = story_sub_type
-        # story_type
-        self.story_type = story_type
-
-    def validate(self):
-        if self.address:
-            self.address.validate()
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.story_type, 'story_type')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.address is not None:
-            result['address'] = self.address.to_map()
-        if self.custom_id is not None:
-            result['custom_id'] = self.custom_id
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.max_image_count is not None:
-            result['max_image_count'] = self.max_image_count
-        if self.min_image_count is not None:
-            result['min_image_count'] = self.min_image_count
-        if self.story_end_time is not None:
-            result['story_end_time'] = self.story_end_time
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        if self.story_name is not None:
-            result['story_name'] = self.story_name
-        if self.story_start_time is not None:
-            result['story_start_time'] = self.story_start_time
-        if self.story_sub_type is not None:
-            result['story_sub_type'] = self.story_sub_type
-        if self.story_type is not None:
-            result['story_type'] = self.story_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('address') is not None:
-            temp_model = Address()
-            self.address = temp_model.from_map(m['address'])
-        if m.get('custom_id') is not None:
-            self.custom_id = m.get('custom_id')
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('max_image_count') is not None:
-            self.max_image_count = m.get('max_image_count')
-        if m.get('min_image_count') is not None:
-            self.min_image_count = m.get('min_image_count')
-        if m.get('story_end_time') is not None:
-            self.story_end_time = m.get('story_end_time')
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        if m.get('story_name') is not None:
-            self.story_name = m.get('story_name')
-        if m.get('story_start_time') is not None:
-            self.story_start_time = m.get('story_start_time')
-        if m.get('story_sub_type') is not None:
-            self.story_sub_type = m.get('story_sub_type')
-        if m.get('story_type') is not None:
-            self.story_type = m.get('story_type')
-        return self
-
-
 class CreateSyncMappingRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        addition_data: str = None,
         custom_meta: str = None,
         device_name: str = None,
         drive_id: str = None,
+        file_id: str = None,
         fs_id: str = None,
+        hidden: bool = None,
         local_path: str = None,
+        name: str = None,
         sync_mode: str = None,
     ):
         self.httpheaders = httpheaders
+        # addition_data
+        self.addition_data = addition_data
         # custom_meta
         self.custom_meta = custom_meta
         # device_name
         self.device_name = device_name
         # drive_id
         self.drive_id = drive_id
+        # file_id
+        self.file_id = file_id
         # fs_id
         self.fs_id = fs_id
+        # hidden
+        self.hidden = hidden
         # local_path
         self.local_path = local_path
+        # name
+        self.name = name
         # sync_mode
         self.sync_mode = sync_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
         if self.custom_meta is not None:
             result['custom_meta'] = self.custom_meta
         if self.device_name is not None:
             result['device_name'] = self.device_name
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
         if self.fs_id is not None:
             result['fs_id'] = self.fs_id
+        if self.hidden is not None:
+            result['hidden'] = self.hidden
         if self.local_path is not None:
             result['local_path'] = self.local_path
+        if self.name is not None:
+            result['name'] = self.name
         if self.sync_mode is not None:
             result['sync_mode'] = self.sync_mode
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
         if m.get('custom_meta') is not None:
             self.custom_meta = m.get('custom_meta')
         if m.get('device_name') is not None:
             self.device_name = m.get('device_name')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
         if m.get('fs_id') is not None:
             self.fs_id = m.get('fs_id')
+        if m.get('hidden') is not None:
+            self.hidden = m.get('hidden')
         if m.get('local_path') is not None:
             self.local_path = m.get('local_path')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         if m.get('sync_mode') is not None:
             self.sync_mode = m.get('sync_mode')
         return self
 
 
 class GroupInfo(TeaModel):
     """
@@ -56326,15 +61444,15 @@
         if m.get('member_role') is not None:
             self.member_role = m.get('member_role')
         return self
 
 
 class CreateUserRequest(TeaModel):
     """
-    Create user request
+    # Create user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         avatar: str = None,
         default_location: str = None,
         deny_change_password_by_self: bool = None,
@@ -56490,81 +61608,14 @@
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         if m.get('user_name') is not None:
             self.user_name = m.get('user_name')
         return self
 
 
-class CreateViewRequest(TeaModel):
-    """
-    Create view request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        description: str = None,
-        name: str = None,
-        owner: str = None,
-        user_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # description
-        self.description = description
-        # name
-        self.name = name
-        # owner
-        self.owner = owner
-        # user_id
-        self.user_id = user_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.name, 'name')
-        self.validate_required(self.owner, 'owner')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.description is not None:
-            result['description'] = self.description
-        if self.name is not None:
-            result['name'] = self.name
-        if self.owner is not None:
-            result['owner'] = self.owner
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('description') is not None:
-            self.description = m.get('description')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('owner') is not None:
-            self.owner = m.get('owner')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
 class DeleteGroupRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -56601,59 +61652,14 @@
         if m.get('group_id') is not None:
             self.group_id = m.get('group_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class DeleteLocationDateClusterRequest(TeaModel):
-    """
-    delete locationCluster request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        cluster_id: str = None,
-        drive_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.cluster_id = cluster_id
-        # drive_id
-        self.drive_id = drive_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.cluster_id is not None:
-            result['cluster_id'] = self.cluster_id
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('cluster_id') is not None:
-            self.cluster_id = m.get('cluster_id')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        return self
-
-
 class DeleteMembershipRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -56768,82 +61774,41 @@
         if m.get('resource') is not None:
             self.resource = m.get('resource')
         if m.get('resource_type') is not None:
             self.resource_type = m.get('resource_type')
         return self
 
 
-class DeleteStoryRequest(TeaModel):
-    """
-    delete story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        story_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # story_id
-        self.story_id = story_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.story_id, 'story_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        return self
-
-
 class DeleteSyncMappingRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         device_name: str = None,
         drive_id: str = None,
         fs_id: str = None,
         local_path: str = None,
+        sync_mode: str = None,
+        sync_root_id: str = None,
     ):
         self.httpheaders = httpheaders
         # device_name
         self.device_name = device_name
         # drive_id
         self.drive_id = drive_id
         # fs_id
         self.fs_id = fs_id
         # local_path
         self.local_path = local_path
+        # sync_mode
+        self.sync_mode = sync_mode
+        # sync_root_id
+        self.sync_root_id = sync_root_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -56856,34 +61821,42 @@
             result['device_name'] = self.device_name
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.fs_id is not None:
             result['fs_id'] = self.fs_id
         if self.local_path is not None:
             result['local_path'] = self.local_path
+        if self.sync_mode is not None:
+            result['sync_mode'] = self.sync_mode
+        if self.sync_root_id is not None:
+            result['sync_root_id'] = self.sync_root_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('device_name') is not None:
             self.device_name = m.get('device_name')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('fs_id') is not None:
             self.fs_id = m.get('fs_id')
         if m.get('local_path') is not None:
             self.local_path = m.get('local_path')
+        if m.get('sync_mode') is not None:
+            self.sync_mode = m.get('sync_mode')
+        if m.get('sync_root_id') is not None:
+            self.sync_root_id = m.get('sync_root_id')
         return self
 
 
 class DeleteUserRequest(TeaModel):
     """
-    Delete user request
+    # Delete user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         user_id: str = None,
     ):
         self.httpheaders = httpheaders
@@ -56933,261 +61906,14 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         return self
 
 
-class DeleteViewRequest(TeaModel):
-    """
-    Delete view request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class QueryRequestTimeRange(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        end: str = None,
-        start: str = None,
-    ):
-        # end
-        self.end = end
-        # start
-        self.start = start
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.end is not None:
-            result['end'] = self.end
-        if self.start is not None:
-            result['start'] = self.start
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('end') is not None:
-            self.end = m.get('end')
-        if m.get('start') is not None:
-            self.start = m.get('start')
-        return self
-
-
-class FindStoriesRequest(TeaModel):
-    """
-    find story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        cover_image_thumbnail_process: str = None,
-        cover_video_thumbnail_process: str = None,
-        create_time_range: QueryRequestTimeRange = None,
-        custom_labels: str = None,
-        drive_id: str = None,
-        face_group_ids: List[str] = None,
-        limit: int = None,
-        marker: str = None,
-        order: str = None,
-        sort: str = None,
-        story_end_time_range: QueryRequestTimeRange = None,
-        story_id: str = None,
-        story_name: str = None,
-        story_start_time_range: QueryRequestTimeRange = None,
-        story_type: str = None,
-        url_expire_sec: int = None,
-        with_empty_stories: bool = None,
-    ):
-        self.httpheaders = httpheaders
-        # cover_image_thumbnail_process
-        self.cover_image_thumbnail_process = cover_image_thumbnail_process
-        # cover_video_thumbnail_process
-        self.cover_video_thumbnail_process = cover_video_thumbnail_process
-        self.create_time_range = create_time_range
-        # custom_labels
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        # face_group_ids
-        self.face_group_ids = face_group_ids
-        # limit
-        self.limit = limit
-        # marker
-        self.marker = marker
-        # order
-        self.order = order
-        # sort
-        self.sort = sort
-        self.story_end_time_range = story_end_time_range
-        # story_id
-        self.story_id = story_id
-        # story_name
-        self.story_name = story_name
-        self.story_start_time_range = story_start_time_range
-        # story_type
-        self.story_type = story_type
-        # url_expire_sec
-        self.url_expire_sec = url_expire_sec
-        # with_empty_stories
-        self.with_empty_stories = with_empty_stories
-
-    def validate(self):
-        if self.create_time_range:
-            self.create_time_range.validate()
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.story_end_time_range:
-            self.story_end_time_range.validate()
-        if self.story_start_time_range:
-            self.story_start_time_range.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.cover_image_thumbnail_process is not None:
-            result['cover_image_thumbnail_process'] = self.cover_image_thumbnail_process
-        if self.cover_video_thumbnail_process is not None:
-            result['cover_video_thumbnail_process'] = self.cover_video_thumbnail_process
-        if self.create_time_range is not None:
-            result['create_time_range'] = self.create_time_range.to_map()
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.face_group_ids is not None:
-            result['face_group_ids'] = self.face_group_ids
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.order is not None:
-            result['order'] = self.order
-        if self.sort is not None:
-            result['sort'] = self.sort
-        if self.story_end_time_range is not None:
-            result['story_end_time_range'] = self.story_end_time_range.to_map()
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        if self.story_name is not None:
-            result['story_name'] = self.story_name
-        if self.story_start_time_range is not None:
-            result['story_start_time_range'] = self.story_start_time_range.to_map()
-        if self.story_type is not None:
-            result['story_type'] = self.story_type
-        if self.url_expire_sec is not None:
-            result['url_expire_sec'] = self.url_expire_sec
-        if self.with_empty_stories is not None:
-            result['with_empty_stories'] = self.with_empty_stories
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('cover_image_thumbnail_process') is not None:
-            self.cover_image_thumbnail_process = m.get('cover_image_thumbnail_process')
-        if m.get('cover_video_thumbnail_process') is not None:
-            self.cover_video_thumbnail_process = m.get('cover_video_thumbnail_process')
-        if m.get('create_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.create_time_range = temp_model.from_map(m['create_time_range'])
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('face_group_ids') is not None:
-            self.face_group_ids = m.get('face_group_ids')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('order') is not None:
-            self.order = m.get('order')
-        if m.get('sort') is not None:
-            self.sort = m.get('sort')
-        if m.get('story_end_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.story_end_time_range = temp_model.from_map(m['story_end_time_range'])
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        if m.get('story_name') is not None:
-            self.story_name = m.get('story_name')
-        if m.get('story_start_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.story_start_time_range = temp_model.from_map(m['story_start_time_range'])
-        if m.get('story_type') is not None:
-            self.story_type = m.get('story_type')
-        if m.get('url_expire_sec') is not None:
-            self.url_expire_sec = m.get('url_expire_sec')
-        if m.get('with_empty_stories') is not None:
-            self.with_empty_stories = m.get('with_empty_stories')
-        return self
-
-
 class GetAppDebugCmdRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -57217,61 +61943,14 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('app_id') is not None:
             self.app_id = m.get('app_id')
         return self
 
 
-class GetFaceGroupInfoRequest(TeaModel):
-    """
-    Get face group info request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        group_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # group_id 列举人脸分组接口中获取
-        self.group_id = group_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.group_id, 'group_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.group_id is not None:
-            result['group_id'] = self.group_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('group_id') is not None:
-            self.group_id = m.get('group_id')
-        return self
-
-
 class GetGroupRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -57308,53 +61987,14 @@
         if m.get('group_id') is not None:
             self.group_id = m.get('group_id')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class GetImageCountRequest(TeaModel):
-    """
-    Get photo count request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        return self
-
-
 class GetMembershipRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -57469,120 +62109,17 @@
         if m.get('resource') is not None:
             self.resource = m.get('resource')
         if m.get('resource_type') is not None:
             self.resource_type = m.get('resource_type')
         return self
 
 
-class GetStoryRequest(TeaModel):
-    """
-    Get story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        cover_image_thumbnail_process: str = None,
-        cover_video_thumbnail_process: str = None,
-        drive_id: str = None,
-        image_thumbnail_process: str = None,
-        image_url_process: str = None,
-        office_thumbnail_process: str = None,
-        story_id: str = None,
-        thumbnail_processes: dict = None,
-        url_expire_sec: int = None,
-        video_thumbnail_process: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # cover_image_thumbnail_process
-        self.cover_image_thumbnail_process = cover_image_thumbnail_process
-        # cover_video_thumbnail_process
-        self.cover_video_thumbnail_process = cover_video_thumbnail_process
-        # drive_id
-        self.drive_id = drive_id
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # image_url_process
-        self.image_url_process = image_url_process
-        # office_thumbnail_process
-        self.office_thumbnail_process = office_thumbnail_process
-        # story_id
-        self.story_id = story_id
-        self.thumbnail_processes = thumbnail_processes
-        # url_expire_sec
-        self.url_expire_sec = url_expire_sec
-        # video_thumbnail_process
-        # type:string
-        self.video_thumbnail_process = video_thumbnail_process
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.story_id, 'story_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.cover_image_thumbnail_process is not None:
-            result['cover_image_thumbnail_process'] = self.cover_image_thumbnail_process
-        if self.cover_video_thumbnail_process is not None:
-            result['cover_video_thumbnail_process'] = self.cover_video_thumbnail_process
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.image_url_process is not None:
-            result['image_url_process'] = self.image_url_process
-        if self.office_thumbnail_process is not None:
-            result['office_thumbnail_process'] = self.office_thumbnail_process
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        if self.thumbnail_processes is not None:
-            result['thumbnail_processes'] = self.thumbnail_processes
-        if self.url_expire_sec is not None:
-            result['url_expire_sec'] = self.url_expire_sec
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('cover_image_thumbnail_process') is not None:
-            self.cover_image_thumbnail_process = m.get('cover_image_thumbnail_process')
-        if m.get('cover_video_thumbnail_process') is not None:
-            self.cover_video_thumbnail_process = m.get('cover_video_thumbnail_process')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('image_url_process') is not None:
-            self.image_url_process = m.get('image_url_process')
-        if m.get('office_thumbnail_process') is not None:
-            self.office_thumbnail_process = m.get('office_thumbnail_process')
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        if m.get('thumbnail_processes') is not None:
-            self.thumbnail_processes = m.get('thumbnail_processes')
-        if m.get('url_expire_sec') is not None:
-            self.url_expire_sec = m.get('url_expire_sec')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        return self
-
-
 class GetUserRequest(TeaModel):
     """
-    Get user request
+    # Get user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         user_id: str = None,
     ):
         self.httpheaders = httpheaders
@@ -57610,130 +62147,14 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class GetViewFileRequest(TeaModel):
-    """
-    get file from view
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        drive_id: str = None,
-        file_id: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        self.drive_id = drive_id
-        self.file_id = file_id
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class GetViewRequest(TeaModel):
-    """
-    Get view request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
 class GroupExtraItem(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         created_at: int = None,
@@ -57889,15 +62310,15 @@
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
 class ImportUserRequest(TeaModel):
     """
-    Import user request
+    # Import user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         authentication_display_name: str = None,
         authentication_type: str = None,
         auto_create_drive: bool = None,
@@ -58223,69 +62644,14 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class ListFileViewsRequest(TeaModel):
-    """
-    list file view ids
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        drive_id: str = None,
-        file_id: str = None,
-        user_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.category = category
-        self.drive_id = drive_id
-        self.file_id = file_id
-        # user_id
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
 class ListGroupRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -58388,200 +62754,14 @@
         if m.get('include_group_role') is not None:
             self.include_group_role = m.get('include_group_role')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class ListImageAddressGroupsRequest(TeaModel):
-    """
-    List image address groups request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        image_thumbnail_process: str = None,
-        limit: int = None,
-        marker: str = None,
-        video_thumbnail_process: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # 每页大小限制
-        self.limit = limit
-        # 翻页标记
-        self.marker = marker
-        # video_thumbnail_process
-        self.video_thumbnail_process = video_thumbnail_process
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.limit is not None:
-            self.validate_maximum(self.limit, 'limit', 100)
-            self.validate_minimum(self.limit, 'limit', 1)
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        return self
-
-
-class ListImageFaceGroupsRequest(TeaModel):
-    """
-    List image face groups request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        limit: int = None,
-        marker: str = None,
-        remarks: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # 每页大小限制
-        self.limit = limit
-        # 翻页标记
-        self.marker = marker
-        self.remarks = remarks
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.limit is not None:
-            self.validate_maximum(self.limit, 'limit', 100)
-            self.validate_minimum(self.limit, 'limit', 1)
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.remarks is not None:
-            result['remarks'] = self.remarks
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('remarks') is not None:
-            self.remarks = m.get('remarks')
-        return self
-
-
-class ListImageTagsRequest(TeaModel):
-    """
-    List image tags request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        image_thumbnail_process: str = None,
-        video_thumbnail_process: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # video_thumbnail_process
-        # type:string
-        self.video_thumbnail_process = video_thumbnail_process
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        return self
-
-
 class ListPermissionRequest(TeaModel):
     """
     request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -58629,19 +62809,22 @@
 class ListSyncMappingRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
+        sync_mode: str = None,
         device_name: str = None,
         limit: int = None,
         marker: str = None,
     ):
         self.httpheaders = httpheaders
+        # SyncMode
+        self.sync_mode = sync_mode
         # device_name
         self.device_name = device_name
         # limit
         self.limit = limit
         # marker
         self.marker = marker
 
@@ -58652,38 +62835,42 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.httpheaders is not None:
             result['httpheaders'] = self.httpheaders
+        if self.sync_mode is not None:
+            result['SyncMode'] = self.sync_mode
         if self.device_name is not None:
             result['device_name'] = self.device_name
         if self.limit is not None:
             result['limit'] = self.limit
         if self.marker is not None:
             result['marker'] = self.marker
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
+        if m.get('SyncMode') is not None:
+            self.sync_mode = m.get('SyncMode')
         if m.get('device_name') is not None:
             self.device_name = m.get('device_name')
         if m.get('limit') is not None:
             self.limit = m.get('limit')
         if m.get('marker') is not None:
             self.marker = m.get('marker')
         return self
 
 
 class ListUserRequest(TeaModel):
     """
-    List user request
+    # List user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         limit: int = None,
         marker: str = None,
         status: str = None,
@@ -58734,306 +62921,14 @@
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class ListViewFilesRequest(TeaModel):
-    """
-    list view file
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        fields: str = None,
-        filter: str = None,
-        image_thumbnail_process: str = None,
-        image_url_process: str = None,
-        limit: int = None,
-        marker: str = None,
-        office_thumbnail_process: str = None,
-        order_by: str = None,
-        order_direction: str = None,
-        url_expire_sec: int = None,
-        user_id: str = None,
-        video_thumbnail_process: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        self.fields = fields
-        self.filter = filter
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # image_url_process
-        self.image_url_process = image_url_process
-        self.limit = limit
-        self.marker = marker
-        # office_thumbnail_process
-        self.office_thumbnail_process = office_thumbnail_process
-        self.order_by = order_by
-        self.order_direction = order_direction
-        self.url_expire_sec = url_expire_sec
-        # user_id
-        self.user_id = user_id
-        # video_thumbnail_process
-        # type:string
-        self.video_thumbnail_process = video_thumbnail_process
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.fields is not None:
-            result['fields'] = self.fields
-        if self.filter is not None:
-            result['filter'] = self.filter
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.image_url_process is not None:
-            result['image_url_process'] = self.image_url_process
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.office_thumbnail_process is not None:
-            result['office_thumbnail_process'] = self.office_thumbnail_process
-        if self.order_by is not None:
-            result['order_by'] = self.order_by
-        if self.order_direction is not None:
-            result['order_direction'] = self.order_direction
-        if self.url_expire_sec is not None:
-            result['url_expire_sec'] = self.url_expire_sec
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('fields') is not None:
-            self.fields = m.get('fields')
-        if m.get('filter') is not None:
-            self.filter = m.get('filter')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('image_url_process') is not None:
-            self.image_url_process = m.get('image_url_process')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('office_thumbnail_process') is not None:
-            self.office_thumbnail_process = m.get('office_thumbnail_process')
-        if m.get('order_by') is not None:
-            self.order_by = m.get('order_by')
-        if m.get('order_direction') is not None:
-            self.order_direction = m.get('order_direction')
-        if m.get('url_expire_sec') is not None:
-            self.url_expire_sec = m.get('url_expire_sec')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class ListViewsRequest(TeaModel):
-    """
-    List views request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        limit: int = None,
-        marker: str = None,
-        order_by: str = None,
-        order_direction: str = None,
-        owner: str = None,
-        user_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # 每页大小限制
-        self.limit = limit
-        # marker
-        self.marker = marker
-        # order_by
-        self.order_by = order_by
-        # order_direction
-        self.order_direction = order_direction
-        # owner
-        self.owner = owner
-        # user_id
-        self.user_id = user_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        if self.limit is not None:
-            self.validate_maximum(self.limit, 'limit', 100)
-            self.validate_minimum(self.limit, 'limit', 1)
-        self.validate_required(self.owner, 'owner')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.order_by is not None:
-            result['order_by'] = self.order_by
-        if self.order_direction is not None:
-            result['order_direction'] = self.order_direction
-        if self.owner is not None:
-            result['owner'] = self.owner
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('order_by') is not None:
-            self.order_by = m.get('order_by')
-        if m.get('order_direction') is not None:
-            self.order_direction = m.get('order_direction')
-        if m.get('owner') is not None:
-            self.owner = m.get('owner')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
-class LocationDateCluster(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        address: Address = None,
-        cluster_id: str = None,
-        created_at: str = None,
-        custom_labels: dict = None,
-        drive_id: str = None,
-        end_time: str = None,
-        level: str = None,
-        start_time: str = None,
-        title: str = None,
-        updated_at: str = None,
-    ):
-        self.address = address
-        self.cluster_id = cluster_id
-        self.created_at = created_at
-        self.custom_labels = custom_labels
-        self.drive_id = drive_id
-        self.end_time = end_time
-        self.level = level
-        self.start_time = start_time
-        self.title = title
-        self.updated_at = updated_at
-
-    def validate(self):
-        if self.address:
-            self.address.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.address is not None:
-            result['address'] = self.address.to_map()
-        if self.cluster_id is not None:
-            result['cluster_id'] = self.cluster_id
-        if self.created_at is not None:
-            result['created_at'] = self.created_at
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.end_time is not None:
-            result['end_time'] = self.end_time
-        if self.level is not None:
-            result['level'] = self.level
-        if self.start_time is not None:
-            result['start_time'] = self.start_time
-        if self.title is not None:
-            result['title'] = self.title
-        if self.updated_at is not None:
-            result['updated_at'] = self.updated_at
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('address') is not None:
-            temp_model = Address()
-            self.address = temp_model.from_map(m['address'])
-        if m.get('cluster_id') is not None:
-            self.cluster_id = m.get('cluster_id')
-        if m.get('created_at') is not None:
-            self.created_at = m.get('created_at')
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('end_time') is not None:
-            self.end_time = m.get('end_time')
-        if m.get('level') is not None:
-            self.level = m.get('level')
-        if m.get('start_time') is not None:
-            self.start_time = m.get('start_time')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        if m.get('updated_at') is not None:
-            self.updated_at = m.get('updated_at')
-        return self
-
-
 class MemberIDInfo(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         member_type: str = None,
@@ -59068,69 +62963,14 @@
         if m.get('sub_group_id') is not None:
             self.sub_group_id = m.get('sub_group_id')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class MergeFaceGroupRequest(TeaModel):
-    """
-    Merge face group request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        from_group_id: str = None,
-        to_group_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # from_group_id
-        self.from_group_id = from_group_id
-        # to_group_id
-        self.to_group_id = to_group_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.from_group_id, 'from_group_id')
-        self.validate_required(self.to_group_id, 'to_group_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.from_group_id is not None:
-            result['from_group_id'] = self.from_group_id
-        if self.to_group_id is not None:
-            result['to_group_id'] = self.to_group_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('from_group_id') is not None:
-            self.from_group_id = m.get('from_group_id')
-        if m.get('to_group_id') is not None:
-            self.to_group_id = m.get('to_group_id')
-        return self
-
-
 class MigrateUserToSubdomainRequest(TeaModel):
     """
     MigrateUserToSubdomainRequest uc migrate user
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -59167,285 +63007,17 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class ParseKeywordsRequest(TeaModel):
-    """
-    Parse keywords request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        keywords: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.keywords = keywords
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.keywords is not None:
-            result['keywords'] = self.keywords
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('keywords') is not None:
-            self.keywords = m.get('keywords')
-        return self
-
-
-class QueryLocationClustersResponse(TeaModel):
-    """
-    query locationCluster response
-    """
-    def __init__(
-        self,
-        location_date_clusters: List[LocationDateCluster] = None,
-        next_marker: str = None,
-    ):
-        self.location_date_clusters = location_date_clusters
-        self.next_marker = next_marker
-
-    def validate(self):
-        if self.location_date_clusters:
-            for k in self.location_date_clusters:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['location_date_clusters'] = []
-        if self.location_date_clusters is not None:
-            for k in self.location_date_clusters:
-                result['location_date_clusters'].append(k.to_map() if k else None)
-        if self.next_marker is not None:
-            result['next_marker'] = self.next_marker
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.location_date_clusters = []
-        if m.get('location_date_clusters') is not None:
-            for k in m.get('location_date_clusters'):
-                temp_model = LocationDateCluster()
-                self.location_date_clusters.append(temp_model.from_map(k))
-        if m.get('next_marker') is not None:
-            self.next_marker = m.get('next_marker')
-        return self
-
-
-class QueryLocationDateClustersRequest(TeaModel):
-    """
-    query locationCluster request
-    """
-    def __init__(
-        self,
-        address: Address = None,
-        cluster_id: str = None,
-        create_time_range: QueryRequestTimeRange = None,
-        custom_labels: str = None,
-        drive_id: str = None,
-        end_time_range: QueryRequestTimeRange = None,
-        levels: List[str] = None,
-        limit: int = None,
-        marker: str = None,
-        order: str = None,
-        sort: str = None,
-        start_time_range: QueryRequestTimeRange = None,
-        title: str = None,
-        update_time_range: QueryRequestTimeRange = None,
-    ):
-        self.address = address
-        self.cluster_id = cluster_id
-        self.create_time_range = create_time_range
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        self.end_time_range = end_time_range
-        self.levels = levels
-        self.limit = limit
-        self.marker = marker
-        self.order = order
-        self.sort = sort
-        self.start_time_range = start_time_range
-        self.title = title
-        self.update_time_range = update_time_range
-
-    def validate(self):
-        if self.address:
-            self.address.validate()
-        if self.create_time_range:
-            self.create_time_range.validate()
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.end_time_range:
-            self.end_time_range.validate()
-        if self.start_time_range:
-            self.start_time_range.validate()
-        if self.update_time_range:
-            self.update_time_range.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.address is not None:
-            result['address'] = self.address.to_map()
-        if self.cluster_id is not None:
-            result['cluster_id'] = self.cluster_id
-        if self.create_time_range is not None:
-            result['create_time_range'] = self.create_time_range.to_map()
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.end_time_range is not None:
-            result['end_time_range'] = self.end_time_range.to_map()
-        if self.levels is not None:
-            result['levels'] = self.levels
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.order is not None:
-            result['order'] = self.order
-        if self.sort is not None:
-            result['sort'] = self.sort
-        if self.start_time_range is not None:
-            result['start_time_range'] = self.start_time_range.to_map()
-        if self.title is not None:
-            result['title'] = self.title
-        if self.update_time_range is not None:
-            result['update_time_range'] = self.update_time_range.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('address') is not None:
-            temp_model = Address()
-            self.address = temp_model.from_map(m['address'])
-        if m.get('cluster_id') is not None:
-            self.cluster_id = m.get('cluster_id')
-        if m.get('create_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.create_time_range = temp_model.from_map(m['create_time_range'])
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('end_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.end_time_range = temp_model.from_map(m['end_time_range'])
-        if m.get('levels') is not None:
-            self.levels = m.get('levels')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('order') is not None:
-            self.order = m.get('order')
-        if m.get('sort') is not None:
-            self.sort = m.get('sort')
-        if m.get('start_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.start_time_range = temp_model.from_map(m['start_time_range'])
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        if m.get('update_time_range') is not None:
-            temp_model = QueryRequestTimeRange()
-            self.update_time_range = temp_model.from_map(m['update_time_range'])
-        return self
-
-
-class RemoveStoryFilesRequest(TeaModel):
-    """
-    remove story files request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        files: List[StoryFile] = None,
-        story_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        self.files = files
-        # story_id
-        self.story_id = story_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.files:
-            for k in self.files:
-                if k:
-                    k.validate()
-        self.validate_required(self.story_id, 'story_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        result['files'] = []
-        if self.files is not None:
-            for k in self.files:
-                result['files'].append(k.to_map() if k else None)
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        self.files = []
-        if m.get('files') is not None:
-            for k in m.get('files'):
-                temp_model = StoryFile()
-                self.files.append(temp_model.from_map(k))
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        return self
-
-
 class RemoveUserFromSubdomainRequest(TeaModel):
     """
-    Remove user to subdomain request
+    # Remove user to subdomain request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         subdomain_id: str = None,
         user_id: str = None,
     ):
@@ -59479,78 +63051,14 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class RemoveViewFileRequest(TeaModel):
-    """
-    remove file from view
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        drive_id: str = None,
-        file_id: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        self.drive_id = drive_id
-        self.file_id = file_id
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
 class RollbackUserFromSubdomainRequest(TeaModel):
     """
     RollbackUserFromSubdomainRequest uc migrate user
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -59658,95 +63166,14 @@
         if m.get('marker') is not None:
             self.marker = m.get('marker')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class SearchImageAddressGroupsRequest(TeaModel):
-    """
-    Search image address groups request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        address_level: str = None,
-        address_names: List[str] = None,
-        br_geo_point: str = None,
-        drive_id: str = None,
-        image_thumbnail_process: str = None,
-        tl_geo_point: str = None,
-        video_thumbnail_process: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # 查询的地点级别
-        self.address_level = address_level
-        # 查询的地点数组
-        self.address_names = address_names
-        # br_geo_point
-        self.br_geo_point = br_geo_point
-        # drive_id
-        self.drive_id = drive_id
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # tl_geo_point
-        self.tl_geo_point = tl_geo_point
-        # video_thumbnail_process
-        self.video_thumbnail_process = video_thumbnail_process
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.address_level is not None:
-            result['address_level'] = self.address_level
-        if self.address_names is not None:
-            result['address_names'] = self.address_names
-        if self.br_geo_point is not None:
-            result['br_geo_point'] = self.br_geo_point
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.tl_geo_point is not None:
-            result['tl_geo_point'] = self.tl_geo_point
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('address_level') is not None:
-            self.address_level = m.get('address_level')
-        if m.get('address_names') is not None:
-            self.address_names = m.get('address_names')
-        if m.get('br_geo_point') is not None:
-            self.br_geo_point = m.get('br_geo_point')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('tl_geo_point') is not None:
-            self.tl_geo_point = m.get('tl_geo_point')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        return self
-
-
 class SearchPermissionRequest(TeaModel):
     """
     request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -59801,15 +63228,15 @@
         if m.get('query') is not None:
             self.query = m.get('query')
         return self
 
 
 class SearchUserAndGroupRequest(TeaModel):
     """
-    Search user and group request
+    # Search user and group request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         identity_type_list: List[str] = None,
         limit: int = None,
         marker: str = None,
@@ -59883,15 +63310,15 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
 class SearchUserRequest(TeaModel):
     """
-    Search user request
+    # Search user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         drive_status: str = None,
         email: str = None,
         expired_at_range: Int64Range = None,
@@ -60010,625 +63437,14 @@
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         if m.get('user_name') is not None:
             self.user_name = m.get('user_name')
         return self
 
 
-class SearchViewFilesRequest(TeaModel):
-    """
-    search view file
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        fields: str = None,
-        filter: str = None,
-        image_thumbnail_process: str = None,
-        image_url_process: str = None,
-        limit: int = None,
-        marker: str = None,
-        office_thumbnail_process: str = None,
-        order_by: str = None,
-        order_direction: str = None,
-        query: str = None,
-        return_total_count: bool = None,
-        url_expire_sec: int = None,
-        user_id: str = None,
-        video_thumbnail_process: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        self.fields = fields
-        self.filter = filter
-        # image_thumbnail_process
-        self.image_thumbnail_process = image_thumbnail_process
-        # image_url_process
-        self.image_url_process = image_url_process
-        self.limit = limit
-        self.marker = marker
-        # office_thumbnail_process
-        self.office_thumbnail_process = office_thumbnail_process
-        self.order_by = order_by
-        self.order_direction = order_direction
-        # query
-        self.query = query
-        # return_total_count 是否返回查询总数
-        self.return_total_count = return_total_count
-        self.url_expire_sec = url_expire_sec
-        # user_id
-        self.user_id = user_id
-        # video_thumbnail_process
-        # type:string
-        self.video_thumbnail_process = video_thumbnail_process
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        if self.query is not None:
-            self.validate_max_length(self.query, 'query', 4096)
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.fields is not None:
-            result['fields'] = self.fields
-        if self.filter is not None:
-            result['filter'] = self.filter
-        if self.image_thumbnail_process is not None:
-            result['image_thumbnail_process'] = self.image_thumbnail_process
-        if self.image_url_process is not None:
-            result['image_url_process'] = self.image_url_process
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.office_thumbnail_process is not None:
-            result['office_thumbnail_process'] = self.office_thumbnail_process
-        if self.order_by is not None:
-            result['order_by'] = self.order_by
-        if self.order_direction is not None:
-            result['order_direction'] = self.order_direction
-        if self.query is not None:
-            result['query'] = self.query
-        if self.return_total_count is not None:
-            result['return_total_count'] = self.return_total_count
-        if self.url_expire_sec is not None:
-            result['url_expire_sec'] = self.url_expire_sec
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.video_thumbnail_process is not None:
-            result['video_thumbnail_process'] = self.video_thumbnail_process
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('fields') is not None:
-            self.fields = m.get('fields')
-        if m.get('filter') is not None:
-            self.filter = m.get('filter')
-        if m.get('image_thumbnail_process') is not None:
-            self.image_thumbnail_process = m.get('image_thumbnail_process')
-        if m.get('image_url_process') is not None:
-            self.image_url_process = m.get('image_url_process')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('office_thumbnail_process') is not None:
-            self.office_thumbnail_process = m.get('office_thumbnail_process')
-        if m.get('order_by') is not None:
-            self.order_by = m.get('order_by')
-        if m.get('order_direction') is not None:
-            self.order_direction = m.get('order_direction')
-        if m.get('query') is not None:
-            self.query = m.get('query')
-        if m.get('return_total_count') is not None:
-            self.return_total_count = m.get('return_total_count')
-        if m.get('url_expire_sec') is not None:
-            self.url_expire_sec = m.get('url_expire_sec')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('video_thumbnail_process') is not None:
-            self.video_thumbnail_process = m.get('video_thumbnail_process')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
-class SearchViewFilesResponse(TeaModel):
-    """
-    search view files response
-    """
-    def __init__(
-        self,
-        items: List[ViewFileItem] = None,
-        next_marker: str = None,
-        total_count: int = None,
-    ):
-        self.items = items
-        self.next_marker = next_marker
-        self.total_count = total_count
-
-    def validate(self):
-        if self.items:
-            for k in self.items:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['items'] = []
-        if self.items is not None:
-            for k in self.items:
-                result['items'].append(k.to_map() if k else None)
-        if self.next_marker is not None:
-            result['next_marker'] = self.next_marker
-        if self.total_count is not None:
-            result['total_count'] = self.total_count
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.items = []
-        if m.get('items') is not None:
-            for k in m.get('items'):
-                temp_model = ViewFileItem()
-                self.items.append(temp_model.from_map(k))
-        if m.get('next_marker') is not None:
-            self.next_marker = m.get('next_marker')
-        if m.get('total_count') is not None:
-            self.total_count = m.get('total_count')
-        return self
-
-
-class SearchViewsRequest(TeaModel):
-    """
-    Search view request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        limit: int = None,
-        marker: str = None,
-        name: str = None,
-        order_by: str = None,
-        order_direction: str = None,
-        owner: str = None,
-        return_total_count: bool = None,
-        user_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # 每页大小限制
-        self.limit = limit
-        # marker
-        self.marker = marker
-        # name
-        self.name = name
-        # order_by
-        self.order_by = order_by
-        # order_direction
-        self.order_direction = order_direction
-        # owner
-        self.owner = owner
-        # return_total_count 是否返回查询总数
-        self.return_total_count = return_total_count
-        # user_id
-        self.user_id = user_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        if self.limit is not None:
-            self.validate_maximum(self.limit, 'limit', 100)
-            self.validate_minimum(self.limit, 'limit', 1)
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.name is not None:
-            result['name'] = self.name
-        if self.order_by is not None:
-            result['order_by'] = self.order_by
-        if self.order_direction is not None:
-            result['order_direction'] = self.order_direction
-        if self.owner is not None:
-            result['owner'] = self.owner
-        if self.return_total_count is not None:
-            result['return_total_count'] = self.return_total_count
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('order_by') is not None:
-            self.order_by = m.get('order_by')
-        if m.get('order_direction') is not None:
-            self.order_direction = m.get('order_direction')
-        if m.get('owner') is not None:
-            self.owner = m.get('owner')
-        if m.get('return_total_count') is not None:
-            self.return_total_count = m.get('return_total_count')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
-class SimpleQuery(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        field: str = None,
-        operation: str = None,
-        sub_queries: List['SimpleQuery'] = None,
-        value: str = None,
-    ):
-        self.field = field
-        self.operation = operation
-        self.sub_queries = sub_queries
-        self.value = value
-
-    def validate(self):
-        if self.sub_queries:
-            for k in self.sub_queries:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.field is not None:
-            result['field'] = self.field
-        if self.operation is not None:
-            result['operation'] = self.operation
-        result['sub_queries'] = []
-        if self.sub_queries is not None:
-            for k in self.sub_queries:
-                result['sub_queries'].append(k.to_map() if k else None)
-        if self.value is not None:
-            result['value'] = self.value
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('field') is not None:
-            self.field = m.get('field')
-        if m.get('operation') is not None:
-            self.operation = m.get('operation')
-        self.sub_queries = []
-        if m.get('sub_queries') is not None:
-            for k in m.get('sub_queries'):
-                temp_model = SimpleQuery()
-                self.sub_queries.append(temp_model.from_map(k))
-        if m.get('value') is not None:
-            self.value = m.get('value')
-        return self
-
-
-class SimpleQueryRequest(TeaModel):
-    """
-    simple query request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        aggregations: List[Aggregation] = None,
-        drive_id: str = None,
-        limit: int = None,
-        marker: str = None,
-        order: str = None,
-        query: SimpleQuery = None,
-        sort: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.aggregations = aggregations
-        # drive_id
-        self.drive_id = drive_id
-        self.limit = limit
-        self.marker = marker
-        self.order = order
-        self.query = query
-        self.sort = sort
-
-    def validate(self):
-        if self.aggregations:
-            for k in self.aggregations:
-                if k:
-                    k.validate()
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        if self.query:
-            self.query.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        result['aggregations'] = []
-        if self.aggregations is not None:
-            for k in self.aggregations:
-                result['aggregations'].append(k.to_map() if k else None)
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.limit is not None:
-            result['limit'] = self.limit
-        if self.marker is not None:
-            result['marker'] = self.marker
-        if self.order is not None:
-            result['order'] = self.order
-        if self.query is not None:
-            result['query'] = self.query.to_map()
-        if self.sort is not None:
-            result['sort'] = self.sort
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        self.aggregations = []
-        if m.get('aggregations') is not None:
-            for k in m.get('aggregations'):
-                temp_model = Aggregation()
-                self.aggregations.append(temp_model.from_map(k))
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('limit') is not None:
-            self.limit = m.get('limit')
-        if m.get('marker') is not None:
-            self.marker = m.get('marker')
-        if m.get('order') is not None:
-            self.order = m.get('order')
-        if m.get('query') is not None:
-            temp_model = SimpleQuery()
-            self.query = temp_model.from_map(m['query'])
-        if m.get('sort') is not None:
-            self.sort = m.get('sort')
-        return self
-
-
-class UnAssignFaceGroupItemRequest(TeaModel):
-    """
-    Unassign facegroup item request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        face_group_id: str = None,
-        file_id: str = None,
-        group_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # face_group_id
-        self.face_group_id = face_group_id
-        # file_id
-        self.file_id = file_id
-        # group_id 列举人脸分组接口中获取
-        self.group_id = group_id
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.file_id, 'file_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.face_group_id is not None:
-            result['face_group_id'] = self.face_group_id
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.group_id is not None:
-            result['group_id'] = self.group_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('face_group_id') is not None:
-            self.face_group_id = m.get('face_group_id')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('group_id') is not None:
-            self.group_id = m.get('group_id')
-        return self
-
-
-class UpdateDataProcessTemplateRequest(TeaModel):
-    """
-    update data process template request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        resource_id: str = None,
-        resource_type: str = None,
-        template: str = None,
-        user_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.resource_id = resource_id
-        self.resource_type = resource_type
-        self.template = template
-        self.user_id = user_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.resource_id is not None:
-            result['resource_id'] = self.resource_id
-        if self.resource_type is not None:
-            result['resource_type'] = self.resource_type
-        if self.template is not None:
-            result['template'] = self.template
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('resource_id') is not None:
-            self.resource_id = m.get('resource_id')
-        if m.get('resource_type') is not None:
-            self.resource_type = m.get('resource_type')
-        if m.get('template') is not None:
-            self.template = m.get('template')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        return self
-
-
-class UpdateFaceGroupInfoRequest(TeaModel):
-    """
-    Update face group info request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        drive_id: str = None,
-        group_cover_face_id: str = None,
-        group_id: str = None,
-        group_name: str = None,
-        remarks: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # drive_id
-        self.drive_id = drive_id
-        # group_cover_face_id
-        self.group_cover_face_id = group_cover_face_id
-        # group_id 列举人脸分组接口中获取
-        self.group_id = group_id
-        # group_name
-        self.group_name = group_name
-        # remarks
-        self.remarks = remarks
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.group_id, 'group_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.group_cover_face_id is not None:
-            result['group_cover_face_id'] = self.group_cover_face_id
-        if self.group_id is not None:
-            result['group_id'] = self.group_id
-        if self.group_name is not None:
-            result['group_name'] = self.group_name
-        if self.remarks is not None:
-            result['remarks'] = self.remarks
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('group_cover_face_id') is not None:
-            self.group_cover_face_id = m.get('group_cover_face_id')
-        if m.get('group_id') is not None:
-            self.group_id = m.get('group_id')
-        if m.get('group_name') is not None:
-            self.group_name = m.get('group_name')
-        if m.get('remarks') is not None:
-            self.remarks = m.get('remarks')
-        return self
-
-
 class UpdateGroupRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -60686,71 +63502,14 @@
         if m.get('is_root') is not None:
             self.is_root = m.get('is_root')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
-class UpdateLocationDateClusterRequest(TeaModel):
-    """
-    update locationCluster request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        cluster_id: str = None,
-        custom_labels: dict = None,
-        drive_id: str = None,
-        title: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.cluster_id = cluster_id
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        self.title = title
-
-    def validate(self):
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.cluster_id is not None:
-            result['cluster_id'] = self.cluster_id
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.title is not None:
-            result['title'] = self.title
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('cluster_id') is not None:
-            self.cluster_id = m.get('cluster_id')
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        return self
-
-
 class UpdateMembershipRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -60914,94 +63673,17 @@
         if m.get('resource_type') is not None:
             self.resource_type = m.get('resource_type')
         if m.get('user_tags') is not None:
             self.user_tags = m.get('user_tags')
         return self
 
 
-class UpdateStoryRequest(TeaModel):
-    """
-    Update story request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        cover: StoryFile = None,
-        custom_id: str = None,
-        custom_labels: dict = None,
-        drive_id: str = None,
-        story_id: str = None,
-        story_name: str = None,
-    ):
-        self.httpheaders = httpheaders
-        self.cover = cover
-        # custom_id
-        self.custom_id = custom_id
-        # custom_labels
-        self.custom_labels = custom_labels
-        # drive_id
-        self.drive_id = drive_id
-        # story_id
-        self.story_id = story_id
-        # story_name
-        self.story_name = story_name
-
-    def validate(self):
-        if self.cover:
-            self.cover.validate()
-        self.validate_required(self.drive_id, 'drive_id')
-        if self.drive_id is not None:
-            self.validate_pattern(self.drive_id, 'drive_id', '[0-9]+')
-        self.validate_required(self.story_id, 'story_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.cover is not None:
-            result['cover'] = self.cover.to_map()
-        if self.custom_id is not None:
-            result['custom_id'] = self.custom_id
-        if self.custom_labels is not None:
-            result['custom_labels'] = self.custom_labels
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.story_id is not None:
-            result['story_id'] = self.story_id
-        if self.story_name is not None:
-            result['story_name'] = self.story_name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('cover') is not None:
-            temp_model = StoryFile()
-            self.cover = temp_model.from_map(m['cover'])
-        if m.get('custom_id') is not None:
-            self.custom_id = m.get('custom_id')
-        if m.get('custom_labels') is not None:
-            self.custom_labels = m.get('custom_labels')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('story_id') is not None:
-            self.story_id = m.get('story_id')
-        if m.get('story_name') is not None:
-            self.story_name = m.get('story_name')
-        return self
-
-
 class UpdateUserRequest(TeaModel):
     """
-    Update user request
+    # Update user request
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
         avatar: str = None,
         deny_change_password_by_self: bool = None,
         description: str = None,
@@ -61136,94 +63818,14 @@
         if m.get('user_data') is not None:
             self.user_data = m.get('user_data')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
 
 
-class UpdateViewRequest(TeaModel):
-    """
-    Update view request
-    """
-    def __init__(
-        self,
-        httpheaders: Dict[str, str] = None,
-        category: str = None,
-        description: str = None,
-        ex_fields_info: dict = None,
-        file_count: int = None,
-        name: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        self.httpheaders = httpheaders
-        # category
-        self.category = category
-        # description
-        self.description = description
-        # ex_fields_info
-        self.ex_fields_info = ex_fields_info
-        # description
-        self.file_count = file_count
-        # name
-        self.name = name
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.httpheaders is not None:
-            result['httpheaders'] = self.httpheaders
-        if self.category is not None:
-            result['category'] = self.category
-        if self.description is not None:
-            result['description'] = self.description
-        if self.ex_fields_info is not None:
-            result['ex_fields_info'] = self.ex_fields_info
-        if self.file_count is not None:
-            result['file_count'] = self.file_count
-        if self.name is not None:
-            result['name'] = self.name
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('httpheaders') is not None:
-            self.httpheaders = m.get('httpheaders')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('description') is not None:
-            self.description = m.get('description')
-        if m.get('ex_fields_info') is not None:
-            self.ex_fields_info = m.get('ex_fields_info')
-        if m.get('file_count') is not None:
-            self.file_count = m.get('file_count')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
 class UpgradeCheckAppRequest(TeaModel):
     """
     *\
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -61267,66 +63869,14 @@
         if m.get('arch') is not None:
             self.arch = m.get('arch')
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
 
 
-class ViewFileBaseRequest(TeaModel):
-    """
-    *\
-    """
-    def __init__(
-        self,
-        category: str = None,
-        drive_id: str = None,
-        user_id: str = None,
-        view_id: str = None,
-    ):
-        # category
-        self.category = category
-        self.drive_id = drive_id
-        # user_id
-        self.user_id = user_id
-        # view_id
-        self.view_id = view_id
-
-    def validate(self):
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.view_id, 'view_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.category is not None:
-            result['category'] = self.category
-        if self.drive_id is not None:
-            result['drive_id'] = self.drive_id
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.view_id is not None:
-            result['view_id'] = self.view_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('drive_id') is not None:
-            self.drive_id = m.get('drive_id')
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('view_id') is not None:
-            self.view_id = m.get('view_id')
-        return self
-
-
 class GetDomainSummaryRequest(TeaModel):
     """
     查询 domain 概况
     """
     def __init__(
         self,
         httpheaders: Dict[str, str] = None,
@@ -61484,7 +64034,324 @@
         if m.get('httpheaders') is not None:
             self.httpheaders = m.get('httpheaders')
         if m.get('subdomain_id') is not None:
             self.subdomain_id = m.get('subdomain_id')
         return self
 
 
+class ClearAllRecycleBinRequest(TeaModel):
+    """
+    清理所有回收站文件元数据请求
+    """
+    def __init__(
+        self,
+        addition_data: dict = None,
+        file_path_type: str = None,
+    ):
+        # addition_data
+        self.addition_data = addition_data
+        self.file_path_type = file_path_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
+        if self.file_path_type is not None:
+            result['file_path_type'] = self.file_path_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
+        if m.get('file_path_type') is not None:
+            self.file_path_type = m.get('file_path_type')
+        return self
+
+
+class ClearAllRecycleBinResponse(TeaModel):
+    """
+    clear all recycle bin response
+    """
+    def __init__(
+        self,
+        items: List[ClearRecycleBinResponse] = None,
+    ):
+        self.items = items
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['items'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.items = []
+        if m.get('items') is not None:
+            for k in m.get('items'):
+                temp_model = ClearRecycleBinResponse()
+                self.items.append(temp_model.from_map(k))
+        return self
+
+
+class SearchAllRecycleBinRequest(TeaModel):
+    """
+    搜索所有回收站文件元数据请求
+    """
+    def __init__(
+        self,
+        addition_data: dict = None,
+        fields: str = None,
+        file_path_type: str = None,
+        image_cropping_aspect_ratios: List[str] = None,
+        image_thumbnail_process: str = None,
+        image_url_process: str = None,
+        limit: int = None,
+        location: str = None,
+        marker: str = None,
+        office_thumbnail_process: str = None,
+        order_by: str = None,
+        query: str = None,
+        recursive: bool = None,
+        referer: str = None,
+        sign_token: str = None,
+        url_expire_sec: int = None,
+        video_thumbnail_process: str = None,
+    ):
+        # addition_data
+        self.addition_data = addition_data
+        # fields
+        self.fields = fields
+        self.file_path_type = file_path_type
+        self.image_cropping_aspect_ratios = image_cropping_aspect_ratios
+        # image_thumbnail_process
+        self.image_thumbnail_process = image_thumbnail_process
+        # image_url_process
+        self.image_url_process = image_url_process
+        # limit
+        self.limit = limit
+        # location
+        self.location = location
+        # Marker
+        self.marker = marker
+        # office_thumbnail_process
+        self.office_thumbnail_process = office_thumbnail_process
+        # order_by
+        self.order_by = order_by
+        # query
+        self.query = query
+        self.recursive = recursive
+        # referer
+        self.referer = referer
+        # sign_token
+        self.sign_token = sign_token
+        # url_expire_sec
+        self.url_expire_sec = url_expire_sec
+        # video_thumbnail_process
+        # type:string
+        self.video_thumbnail_process = video_thumbnail_process
+
+    def validate(self):
+        if self.limit is not None:
+            self.validate_maximum(self.limit, 'limit', 200)
+            self.validate_minimum(self.limit, 'limit', 1)
+        if self.query is not None:
+            self.validate_max_length(self.query, 'query', 4096)
+        if self.url_expire_sec is not None:
+            self.validate_maximum(self.url_expire_sec, 'url_expire_sec', 14400)
+            self.validate_minimum(self.url_expire_sec, 'url_expire_sec', 10)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.addition_data is not None:
+            result['addition_data'] = self.addition_data
+        if self.fields is not None:
+            result['fields'] = self.fields
+        if self.file_path_type is not None:
+            result['file_path_type'] = self.file_path_type
+        if self.image_cropping_aspect_ratios is not None:
+            result['image_cropping_aspect_ratios'] = self.image_cropping_aspect_ratios
+        if self.image_thumbnail_process is not None:
+            result['image_thumbnail_process'] = self.image_thumbnail_process
+        if self.image_url_process is not None:
+            result['image_url_process'] = self.image_url_process
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.location is not None:
+            result['location'] = self.location
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.office_thumbnail_process is not None:
+            result['office_thumbnail_process'] = self.office_thumbnail_process
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.query is not None:
+            result['query'] = self.query
+        if self.recursive is not None:
+            result['recursive'] = self.recursive
+        if self.referer is not None:
+            result['referer'] = self.referer
+        if self.sign_token is not None:
+            result['sign_token'] = self.sign_token
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        if self.video_thumbnail_process is not None:
+            result['video_thumbnail_process'] = self.video_thumbnail_process
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('addition_data') is not None:
+            self.addition_data = m.get('addition_data')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
+        if m.get('file_path_type') is not None:
+            self.file_path_type = m.get('file_path_type')
+        if m.get('image_cropping_aspect_ratios') is not None:
+            self.image_cropping_aspect_ratios = m.get('image_cropping_aspect_ratios')
+        if m.get('image_thumbnail_process') is not None:
+            self.image_thumbnail_process = m.get('image_thumbnail_process')
+        if m.get('image_url_process') is not None:
+            self.image_url_process = m.get('image_url_process')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('location') is not None:
+            self.location = m.get('location')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('office_thumbnail_process') is not None:
+            self.office_thumbnail_process = m.get('office_thumbnail_process')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('query') is not None:
+            self.query = m.get('query')
+        if m.get('recursive') is not None:
+            self.recursive = m.get('recursive')
+        if m.get('referer') is not None:
+            self.referer = m.get('referer')
+        if m.get('sign_token') is not None:
+            self.sign_token = m.get('sign_token')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        if m.get('video_thumbnail_process') is not None:
+            self.video_thumbnail_process = m.get('video_thumbnail_process')
+        return self
+
+
+class SearchAllRecycleBinResponse(TeaModel):
+    """
+    search all recycle bin response
+    """
+    def __init__(
+        self,
+        items: List[BaseCCPFileResponse] = None,
+        next_marker: str = None,
+    ):
+        # items
+        self.items = items
+        # next_marker
+        self.next_marker = next_marker
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['items'].append(k.to_map() if k else None)
+        if self.next_marker is not None:
+            result['next_marker'] = self.next_marker
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.items = []
+        if m.get('items') is not None:
+            for k in m.get('items'):
+                temp_model = BaseCCPFileResponse()
+                self.items.append(temp_model.from_map(k))
+        if m.get('next_marker') is not None:
+            self.next_marker = m.get('next_marker')
+        return self
+
+
+class ShareListReceivedRequest(TeaModel):
+    """
+    list received share request
+    """
+    def __init__(
+        self,
+        limit: int = None,
+        marker: str = None,
+        order_by: str = None,
+        order_direction: str = None,
+    ):
+        self.limit = limit
+        self.marker = marker
+        self.order_by = order_by
+        self.order_direction = order_direction
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.marker is not None:
+            result['marker'] = self.marker
+        if self.order_by is not None:
+            result['order_by'] = self.order_by
+        if self.order_direction is not None:
+            result['order_direction'] = self.order_direction
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('marker') is not None:
+            self.marker = m.get('marker')
+        if m.get('order_by') is not None:
+            self.order_by = m.get('order_by')
+        if m.get('order_direction') is not None:
+            self.order_direction = m.get('order_direction')
+        return self
+
+
```

### Comparing `alibabacloud_pds_sdk-1.1.6/alibabacloud_pds_sdk.egg-info/PKG-INFO` & `alibabacloud_pds_sdk-1.1.7/alibabacloud_pds_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pds-sdk
-Version: 1.1.6
+Version: 1.1.7
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-pds-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pds_sdk-1.1.6/setup.py` & `alibabacloud_pds_sdk-1.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pds_sdk.
 
-Created on 02/12/2022
+Created on 21/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pds_sdk"
 NAME = "alibabacloud_pds_sdk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PDS SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-pds-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
     "alibabacloud_roa_util>=0.1.2, <1.0.0",
     "alibabacloud_credentials>=0.2.0, <1.0.0",
     "alibabacloud_pds_credentials>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

