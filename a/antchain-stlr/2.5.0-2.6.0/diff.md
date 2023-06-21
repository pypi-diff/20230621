# Comparing `tmp/antchain_stlr-2.5.0.tar.gz` & `tmp/antchain_stlr-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.5.0.tar", last modified: Mon Jun 12 03:57:38 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.6.0.tar", last modified: Wed Jun 21 09:35:35 2023, max compression
```

## Comparing `antchain_stlr-2.5.0.tar` & `antchain_stlr-2.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111327 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   261187 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-12 03:57:38.000000 antchain_stlr-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   113763 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   266168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/setup.py
```

### Comparing `antchain_stlr-2.5.0/LICENSE` & `antchain_stlr-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.5.0/PKG-INFO` & `antchain_stlr-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.5.0
+Version: 2.6.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.5.0/README-CN.md` & `antchain_stlr-2.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.5.0/README.md` & `antchain_stlr-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.5.0/antchain_sdk_stlr/client.py` & `antchain_stlr-2.6.0/antchain_sdk_stlr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.5.0',
+                    'sdk_version': '2.6.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.5.0',
+                    'sdk_version': '2.6.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2545,14 +2545,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.DetailEcarOffsettranslateResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.offsettranslate.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def submit_ecar_lcaassement(
+        self,
+        request: stlr_models.SubmitEcarLcaassementRequest,
+    ) -> stlr_models.SubmitEcarLcaassementResponse:
+        """
+        Description: 平台方LCA评估结果提交接口，支持三方平台提交LCA评估结果数据
+        Summary: 平台方LCA评估结果提交
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_ecar_lcaassement_ex(request, headers, runtime)
+
+    async def submit_ecar_lcaassement_async(
+        self,
+        request: stlr_models.SubmitEcarLcaassementRequest,
+    ) -> stlr_models.SubmitEcarLcaassementResponse:
+        """
+        Description: 平台方LCA评估结果提交接口，支持三方平台提交LCA评估结果数据
+        Summary: 平台方LCA评估结果提交
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_ecar_lcaassement_ex_async(request, headers, runtime)
+
+    def submit_ecar_lcaassement_ex(
+        self,
+        request: stlr_models.SubmitEcarLcaassementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcaassementResponse:
+        """
+        Description: 平台方LCA评估结果提交接口，支持三方平台提交LCA评估结果数据
+        Summary: 平台方LCA评估结果提交
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcaassementResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.lcaassement.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_ecar_lcaassement_ex_async(
+        self,
+        request: stlr_models.SubmitEcarLcaassementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcaassementResponse:
+        """
+        Description: 平台方LCA评估结果提交接口，支持三方平台提交LCA评估结果数据
+        Summary: 平台方LCA评估结果提交
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcaassementResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.lcaassement.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.5.0/antchain_sdk_stlr/models.py` & `antchain_stlr-2.6.0/antchain_sdk_stlr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6670,14 +6670,140 @@
         if m.get('drawing_account_did') is not None:
             self.drawing_account_did = m.get('drawing_account_did')
         if m.get('receipt_account_did') is not None:
             self.receipt_account_did = m.get('receipt_account_did')
         return self
 
 
+class SubmitEcarLcaassementRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_no: str = None,
+        status: str = None,
+        project_summary: str = None,
+        process_datum: str = None,
+        assement_result: str = None,
+        assement_report: str = None,
+        extra_datum: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单编号，碳矩阵关联的订单编号，业务主键
+        self.order_no = order_no
+        # LCA产品评估状态，返回约定的状态编码
+        self.status = status
+        # 项目摘要信息，包括有关产品详情和报告时间等，JSON格式，按照约定的格式解析成碳矩阵对应的碳足迹项目和产品信息
+        self.project_summary = project_summary
+        # 产品工序数据，JSON格式，按照约定的格式解析成碳矩阵对应的工序信息
+        self.process_datum = process_datum
+        # 碳足迹评估结果数据，JSON格式，按照约定的格式解析成碳矩阵对应的评估结果
+        self.assement_result = assement_result
+        # 碳足迹评估报告，包括一些报告文件地址等，JSON格式，碳矩阵下载保存对应的报告文件
+        self.assement_report = assement_report
+        # 扩展信息，JSON格式，预留需提交的数据
+        self.extra_datum = extra_datum
+
+    def validate(self):
+        self.validate_required(self.order_no, 'order_no')
+        self.validate_required(self.status, 'status')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_no is not None:
+            result['order_no'] = self.order_no
+        if self.status is not None:
+            result['status'] = self.status
+        if self.project_summary is not None:
+            result['project_summary'] = self.project_summary
+        if self.process_datum is not None:
+            result['process_datum'] = self.process_datum
+        if self.assement_result is not None:
+            result['assement_result'] = self.assement_result
+        if self.assement_report is not None:
+            result['assement_report'] = self.assement_report
+        if self.extra_datum is not None:
+            result['extra_datum'] = self.extra_datum
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_no') is not None:
+            self.order_no = m.get('order_no')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('project_summary') is not None:
+            self.project_summary = m.get('project_summary')
+        if m.get('process_datum') is not None:
+            self.process_datum = m.get('process_datum')
+        if m.get('assement_result') is not None:
+            self.assement_result = m.get('assement_result')
+        if m.get('assement_report') is not None:
+            self.assement_report = m.get('assement_report')
+        if m.get('extra_datum') is not None:
+            self.extra_datum = m.get('extra_datum')
+        return self
+
+
+class SubmitEcarLcaassementResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.5.0/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.6.0/antchain_stlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.5.0
+Version: 2.6.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.5.0/setup.py` & `antchain_stlr-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 12/06/2023
+Created on 21/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
```

