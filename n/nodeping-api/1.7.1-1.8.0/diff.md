# Comparing `tmp/nodeping_api-1.7.1.tar.gz` & `tmp/nodeping_api-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeping_api-1.7.1.tar", last modified: Wed Nov 16 00:12:00 2022, max compression
+gzip compressed data, was "nodeping_api-1.8.0.tar", last modified: Wed Jun 21 21:51:46 2023, max compression
```

## Comparing `nodeping_api-1.7.1.tar` & `nodeping_api-1.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2022-11-16 00:12:00.475193 nodeping_api-1.7.1/
--rw-r-----   0 courtney  (1000) courtney  (1000)     1065 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/LICENSE
--rw-r-----   0 courtney  (1000) courtney  (1000)    28744 2022-11-16 00:12:00.475193 nodeping_api-1.7.1/PKG-INFO
--rw-r-----   0 courtney  (1000) courtney  (1000)    28264 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/README.md
-drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2022-11-16 00:12:00.465195 nodeping_api-1.7.1/nodeping_api/
--rw-r-----   0 courtney  (1000) courtney  (1000)       22 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/__init__.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     3592 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/_query_nodeping_api.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1528 2021-10-09 21:41:58.000000 nodeping_api-1.7.1/nodeping_api/_utils.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     4730 2021-08-28 19:44:14.000000 nodeping_api-1.7.1/nodeping_api/accounts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1305 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/check_token.py
--rw-r-----   0 courtney  (1000) courtney  (1000)       44 2020-09-15 20:47:37.000000 nodeping_api-1.7.1/nodeping_api/config.py
--rw-r-----   0 courtney  (1000) courtney  (1000)    10517 2021-10-09 23:10:24.000000 nodeping_api-1.7.1/nodeping_api/contacts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)    79407 2022-11-15 23:51:43.000000 nodeping_api-1.7.1/nodeping_api/create_check.py
--rw-r-----   0 courtney  (1000) courtney  (1000)      777 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/delete_checks.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1397 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/diagnostics.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     4177 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/disable_check.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     5334 2022-11-16 00:07:43.000000 nodeping_api-1.7.1/nodeping_api/get_checks.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     3182 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/group_contacts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1327 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/information.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     4494 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/maintenance.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     3340 2022-03-23 23:39:22.000000 nodeping_api-1.7.1/nodeping_api/notificationprofiles.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1452 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/notifications.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     5507 2020-09-12 21:30:35.000000 nodeping_api-1.7.1/nodeping_api/results.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     5080 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/nodeping_api/schedules.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     2689 2021-10-09 23:14:54.000000 nodeping_api-1.7.1/nodeping_api/update_checks.py
-drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2022-11-16 00:12:00.465195 nodeping_api-1.7.1/nodeping_api.egg-info/
--rw-r-----   0 courtney  (1000) courtney  (1000)    28744 2022-11-16 00:12:00.000000 nodeping_api-1.7.1/nodeping_api.egg-info/PKG-INFO
--rw-r-----   0 courtney  (1000) courtney  (1000)     1146 2022-11-16 00:12:00.000000 nodeping_api-1.7.1/nodeping_api.egg-info/SOURCES.txt
--rw-r-----   0 courtney  (1000) courtney  (1000)        1 2022-11-16 00:12:00.000000 nodeping_api-1.7.1/nodeping_api.egg-info/dependency_links.txt
--rw-r-----   0 courtney  (1000) courtney  (1000)       19 2022-11-16 00:12:00.000000 nodeping_api-1.7.1/nodeping_api.egg-info/top_level.txt
--rw-r-----   0 courtney  (1000) courtney  (1000)       38 2022-11-16 00:12:00.475193 nodeping_api-1.7.1/setup.cfg
--rw-r-----   0 courtney  (1000) courtney  (1000)      802 2022-11-16 00:07:22.000000 nodeping_api-1.7.1/setup.py
-drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2022-11-16 00:12:00.475193 nodeping_api-1.7.1/tests/
--rw-r-----   0 courtney  (1000) courtney  (1000)        0 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/__init__.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1498 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/checks_1_test_get.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     2618 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/checks_2_test_create.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1739 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/checks_3_test_update.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1315 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/checks_4_test_disable.py
--rw-r-----   0 courtney  (1000) courtney  (1000)      958 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/checks_5_test_delete.py
--rw-r-----   0 courtney  (1000) courtney  (1000)      504 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/parameters.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     2433 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_accounts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)      892 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_check_token.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     2776 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_contacts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1397 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_group_contacts.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1423 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_information.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     2380 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_maintenance.py
--rw-r-----   0 courtney  (1000) courtney  (1000)      850 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_notifications.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1030 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_results.py
--rw-r-----   0 courtney  (1000) courtney  (1000)     1744 2020-09-12 17:45:50.000000 nodeping_api-1.7.1/tests/test_schedules.py
+drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2023-06-21 21:51:46.177148 nodeping_api-1.8.0/
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1065 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/LICENSE
+-rw-r-----   0 courtney  (1000) courtney  (1000)    28744 2023-06-21 21:51:46.177148 nodeping_api-1.8.0/PKG-INFO
+-rw-r-----   0 courtney  (1000) courtney  (1000)    28264 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/README.md
+drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2023-06-21 21:51:46.167147 nodeping_api-1.8.0/nodeping_api/
+-rw-r-----   0 courtney  (1000) courtney  (1000)       22 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/__init__.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     3592 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/_query_nodeping_api.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1528 2021-10-09 21:41:58.000000 nodeping_api-1.8.0/nodeping_api/_utils.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     4730 2021-08-28 19:44:14.000000 nodeping_api-1.8.0/nodeping_api/accounts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1305 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/check_token.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)       44 2020-09-15 20:47:37.000000 nodeping_api-1.8.0/nodeping_api/config.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)    10517 2021-10-09 23:10:24.000000 nodeping_api-1.8.0/nodeping_api/contacts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)    82092 2023-06-21 21:42:04.000000 nodeping_api-1.8.0/nodeping_api/create_check.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)      777 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/delete_checks.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1397 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/diagnostics.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     4177 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/disable_check.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     5334 2022-11-16 00:07:43.000000 nodeping_api-1.8.0/nodeping_api/get_checks.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     3182 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/group_contacts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1327 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/information.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     4494 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/maintenance.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     3340 2022-03-23 23:39:22.000000 nodeping_api-1.8.0/nodeping_api/notificationprofiles.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1452 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/notifications.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     5507 2020-09-12 21:30:35.000000 nodeping_api-1.8.0/nodeping_api/results.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     5080 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/nodeping_api/schedules.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     2689 2021-10-09 23:14:54.000000 nodeping_api-1.8.0/nodeping_api/update_checks.py
+drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2023-06-21 21:51:46.167147 nodeping_api-1.8.0/nodeping_api.egg-info/
+-rw-r-----   0 courtney  (1000) courtney  (1000)    28744 2023-06-21 21:51:46.000000 nodeping_api-1.8.0/nodeping_api.egg-info/PKG-INFO
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1146 2023-06-21 21:51:46.000000 nodeping_api-1.8.0/nodeping_api.egg-info/SOURCES.txt
+-rw-r-----   0 courtney  (1000) courtney  (1000)        1 2023-06-21 21:51:46.000000 nodeping_api-1.8.0/nodeping_api.egg-info/dependency_links.txt
+-rw-r-----   0 courtney  (1000) courtney  (1000)       19 2023-06-21 21:51:46.000000 nodeping_api-1.8.0/nodeping_api.egg-info/top_level.txt
+-rw-r-----   0 courtney  (1000) courtney  (1000)       38 2023-06-21 21:51:46.177148 nodeping_api-1.8.0/setup.cfg
+-rw-r-----   0 courtney  (1000) courtney  (1000)      802 2023-06-21 21:44:57.000000 nodeping_api-1.8.0/setup.py
+drwxr-x---   0 courtney  (1000) courtney  (1000)        0 2023-06-21 21:51:46.167147 nodeping_api-1.8.0/tests/
+-rw-r-----   0 courtney  (1000) courtney  (1000)        0 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/__init__.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1498 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/checks_1_test_get.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     2618 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/checks_2_test_create.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1739 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/checks_3_test_update.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1315 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/checks_4_test_disable.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)      958 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/checks_5_test_delete.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)      504 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/parameters.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     2433 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_accounts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)      892 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_check_token.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     2776 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_contacts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1397 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_group_contacts.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1423 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_information.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     2380 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_maintenance.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)      850 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_notifications.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1030 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_results.py
+-rw-r-----   0 courtney  (1000) courtney  (1000)     1744 2020-09-12 17:45:50.000000 nodeping_api-1.8.0/tests/test_schedules.py
```

### Comparing `nodeping_api-1.7.1/LICENSE` & `nodeping_api-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/PKG-INFO` & `nodeping_api-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeping_api
-Version: 1.7.1
+Version: 1.8.0
 Summary: Python package for querying the NodePing API
 Home-page: https://github.com/NodePing/python-nodeping-api
 Author: NodePing
 Author-email: support@nodeping.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nodeping_api-1.7.1/README.md` & `nodeping_api-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/_query_nodeping_api.py` & `nodeping_api-1.8.0/nodeping_api/_query_nodeping_api.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/_utils.py` & `nodeping_api-1.8.0/nodeping_api/_utils.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/accounts.py` & `nodeping_api-1.8.0/nodeping_api/accounts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/check_token.py` & `nodeping_api-1.8.0/nodeping_api/check_token.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/contacts.py` & `nodeping_api-1.8.0/nodeping_api/contacts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/create_check.py` & `nodeping_api-1.8.0/nodeping_api/create_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,14 +568,15 @@
         target,
         customerid="",
         label="",
         autodiag=False,
         invert=False,
         contentstring="",
         data="",
+        clientcert="",
         method="",
         postdata="",
         receiveheaders="",
         sendheaders="",
         statuscode=200,
         ipv6=False,
         follow=False,
@@ -611,14 +612,16 @@
     :param label: Name of the check that will be created
     :type autodiag: bool
     :param autodiag: Enable/disable auto diagnostics for this check
     :type invert: bool
     :param invert: Used for "Does not contain" functionality
     :type data: dict
     :param data: key/value pair for POST fields
+    :type clientcert: string
+    :param clientcert: Specify the ID of a client certificate/key to be used
     :type method: string
     :param method: HTTP method
     :type postdata: dict
     :param postdata: alternative to the data object
     :type receiveheaders: dict
     :param receiveheaders: Headers that should be received
     :type sendheaders: dict
@@ -902,14 +905,90 @@
     check_variables = _package_variables(locals(), 'IMAP4')
 
     url = _utils.create_url(token, API_URL, customerid)
 
     return _query_nodeping_api.post(url, check_variables)
 
 
+def mongodb_check(
+        token,
+        target,
+        customerid=None,
+        label="",
+        query="",
+        fields=None,
+        database="",
+        namespace="",
+        autodiag=False,
+        interval=DEFAULTS['interval'],
+        enabled=DEFAULTS['enabled'],
+        public=DEFAULTS['public'],
+        runlocations=DEFAULTS['runlocations'],
+        homeloc=DEFAULTS['homeloc'],
+        threshold=DEFAULTS['threshold'],
+        sens=DEFAULTS['sens'],
+        mute=DEFAULTS['mute'],
+        dep="",
+        notifications="",
+        **kwargs
+):
+    """ Creates a NodePing MongoDB check
+
+    Expects a token and target variable. The rest are optional
+    and are configured to match the NodePing defaults as described
+    in the documentation.
+
+    :type token: string
+    :param token: NodePing account API token
+    :type target: string
+    :param target: URL to target host
+    :type customerid: string
+    :param customerid: Optional NodePing subaccount ID
+    :type label: string
+    :param label: Name of the check that will be created
+    :type query: string
+    :param query: query to send to the database server
+    :type fields: dict
+    :param fields: name, min, max key/values for matching
+    :type database: string
+    :param database: Name of the database to query
+    :type namespace: string
+    :param namespace: MongoDB collection
+    :type autodiag: bool
+    :param autodiag: Enable/disable auto diagnostics for this check
+    :type interval: int
+    :param interval: Interval in minutes to monitor target
+    :type enabled: bool
+    :param enabled: If created check will be enabled or disabled
+    :type public: bool
+    :param public: If the results for the created check will be public or not
+    :type runlocations: str or list
+    :param runlocations: Which region to be originated from
+    :type homeloc: str
+    :param homeloc: Which probe in the region to originate the check from
+    :type threshold: int
+    :param threshold: The max acceptable packet loss
+    :type sens: int
+    :param sens: Rechecks to help avoid unecessary notifications
+    :type dep: string
+    :param dep: ID of the check used for the notification dependency
+    :type notifications: list
+    :param notifications: list of objects containing contact ID, delay, and
+    scheduling for notifications
+    :return: Response from NodePing
+    :rtype: dict
+    """
+
+    check_variables = _package_variables(locals(), 'MONGODB')
+
+    url = _utils.create_url(token, API_URL, customerid)
+
+    return _query_nodeping_api.post(url, check_variables)
+
+
 def mtr_check(
         token,
         target,
         customerid=None,
         label="",
         autodiag=False,
         ipv6=DEFAULTS['ipv6'],
```

### Comparing `nodeping_api-1.7.1/nodeping_api/delete_checks.py` & `nodeping_api-1.8.0/nodeping_api/delete_checks.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/diagnostics.py` & `nodeping_api-1.8.0/nodeping_api/diagnostics.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/disable_check.py` & `nodeping_api-1.8.0/nodeping_api/disable_check.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/get_checks.py` & `nodeping_api-1.8.0/nodeping_api/get_checks.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/group_contacts.py` & `nodeping_api-1.8.0/nodeping_api/group_contacts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/information.py` & `nodeping_api-1.8.0/nodeping_api/information.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/maintenance.py` & `nodeping_api-1.8.0/nodeping_api/maintenance.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/notificationprofiles.py` & `nodeping_api-1.8.0/nodeping_api/notificationprofiles.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/notifications.py` & `nodeping_api-1.8.0/nodeping_api/notifications.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/results.py` & `nodeping_api-1.8.0/nodeping_api/results.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/schedules.py` & `nodeping_api-1.8.0/nodeping_api/schedules.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api/update_checks.py` & `nodeping_api-1.8.0/nodeping_api/update_checks.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/nodeping_api.egg-info/PKG-INFO` & `nodeping_api-1.8.0/nodeping_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeping-api
-Version: 1.7.1
+Version: 1.8.0
 Summary: Python package for querying the NodePing API
 Home-page: https://github.com/NodePing/python-nodeping-api
 Author: NodePing
 Author-email: support@nodeping.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nodeping_api-1.7.1/nodeping_api.egg-info/SOURCES.txt` & `nodeping_api-1.8.0/nodeping_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/setup.py` & `nodeping_api-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 NAME = "nodeping_api"
 DESCRIPTION = "Python package for querying the NodePing API"
 URL = "https://github.com/NodePing/python-nodeping-api"
 EMAIL = "support@nodeping.com"
 AUTHOR = "NodePing"
-VERSION = "1.7.1"
+VERSION = "1.8.0"
 LICENSE = "MIT"
 
 setuptools.setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `nodeping_api-1.7.1/tests/checks_1_test_get.py` & `nodeping_api-1.8.0/tests/checks_1_test_get.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/checks_2_test_create.py` & `nodeping_api-1.8.0/tests/checks_2_test_create.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/checks_3_test_update.py` & `nodeping_api-1.8.0/tests/checks_3_test_update.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/checks_4_test_disable.py` & `nodeping_api-1.8.0/tests/checks_4_test_disable.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/checks_5_test_delete.py` & `nodeping_api-1.8.0/tests/checks_5_test_delete.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_accounts.py` & `nodeping_api-1.8.0/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_check_token.py` & `nodeping_api-1.8.0/tests/test_check_token.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_contacts.py` & `nodeping_api-1.8.0/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_group_contacts.py` & `nodeping_api-1.8.0/tests/test_group_contacts.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_information.py` & `nodeping_api-1.8.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_maintenance.py` & `nodeping_api-1.8.0/tests/test_maintenance.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_notifications.py` & `nodeping_api-1.8.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_results.py` & `nodeping_api-1.8.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `nodeping_api-1.7.1/tests/test_schedules.py` & `nodeping_api-1.8.0/tests/test_schedules.py`

 * *Files identical despite different names*

