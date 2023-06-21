# Comparing `tmp/acore_server_metadata-0.4.4.tar.gz` & `tmp/acore_server_metadata-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.4.4.tar", last modified: Tue Jun 20 04:28:33 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.4.5.tar", last modified: Wed Jun 21 18:22:41 2023, max compression
```

## Comparing `acore_server_metadata-0.4.4.tar` & `acore_server_metadata-0.4.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.098382 acore_server_metadata-0.4.4/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 04:28:33.098248 acore_server_metadata-0.4.4/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.4/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.095475 acore_server_metadata-0.4.4/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.4/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-20 04:26:54.000000 acore_server_metadata-0.4.4/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.4/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096289 acore_server_metadata-0.4.4/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.4/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    27068 2023-06-20 02:44:53.000000 acore_server_metadata-0.4.4/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.4/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096899 acore_server_metadata-0.4.4/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.4/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.097609 acore_server_metadata-0.4.4/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096175 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     3374 2023-06-20 04:26:30.000000 acore_server_metadata-0.4.4/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.4/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-20 04:28:33.098427 acore_server_metadata-0.4.4/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.097942 acore_server_metadata-0.4.4/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.4/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.4/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464861 acore_server_metadata-0.4.5/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-21 18:22:41.464722 acore_server_metadata-0.4.5/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.5/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.461737 acore_server_metadata-0.4.5/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.5/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-21 18:22:06.000000 acore_server_metadata-0.4.5/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.5/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.462674 acore_server_metadata-0.4.5/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.5/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27110 2023-06-21 18:19:29.000000 acore_server_metadata-0.4.5/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.5/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.463312 acore_server_metadata-0.4.5/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.5/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464056 acore_server_metadata-0.4.5/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.462553 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3589 2023-06-21 18:22:00.000000 acore_server_metadata-0.4.5/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.5/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.5/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-21 18:22:41.464907 acore_server_metadata-0.4.5/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464409 acore_server_metadata-0.4.5/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.5/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.5/tests/test_server.py
```

### Comparing `acore_server_metadata-0.4.4/AUTHORS.rst` & `acore_server_metadata-0.4.5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/LICENSE.txt` & `acore_server_metadata-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/PKG-INFO` & `acore_server_metadata-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.4.4
+Version: 0.4.5
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.4#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.4/README.rst` & `acore_server_metadata-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata/paths.py` & `acore_server_metadata-0.4.5/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata/server.py` & `acore_server_metadata-0.4.5/acore_server_metadata/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,27 +564,28 @@
         """
         if check_exists:
             ec2_inst = self.get_ec2(ec2_client, id=self.id)
             if ec2_inst is None:
                 raise ServerAlreadyExistsError(
                     f"EC2 instance {self.id!r} does not exist"
                 )
+        else:
+            ec2_inst = self.ec2_inst
 
         # check if this allocation id is already associated with an instance
         res = ec2_client.describe_addresses(AllocationIds=[allocation_id])
         address_data = res["Addresses"][0]
-        public_id = address_data["PublicIp"]
         instance_id = address_data.get("InstanceId", "invalid-instance-id")
-        if instance_id == self.ec2_inst.id:  # already associated
+        if instance_id == ec2_inst.id:  # already associated
             return None
 
         # associate eip address
         return ec2_client.associate_address(
             AllocationId=allocation_id,
-            InstanceId=self.ec2_inst.id,
+            InstanceId=ec2_inst.id,
         )
 
     def update_db_master_password(
         self,
         rds_client,
         master_password: str,
         check_exists: bool = True,
@@ -616,15 +617,15 @@
             rds_inst.tags.get("tech:master_password_digest", "invalid")
             == master_password_digest
         ):
             # do nothing
             return None
 
         response = rds_client.modify_db_instance(
-            DBInstanceIdentifier=self.rds_inst.id,
+            DBInstanceIdentifier=rds_inst.id,
             MasterUserPassword=master_password,
             ApplyImmediately=True,
         )
 
         rds_client.add_tags_to_resource(
             ResourceName=rds_inst.db_instance_arn,
             Tags=[
@@ -646,20 +647,23 @@
         在数据库运维过程中, 我们需要定期备份生产服务器的数据库. 该方法能为我们创建 DB snapshot
         并合理明明, 打上对应的 Tag.
         """
         if check_exists:
             rds_inst = self.get_rds(rds_client, id=self.id)
             if rds_inst is None:
                 raise ServerNotFoundError(f"RDS DB instance {self.id!r} does not exist")
+        else:
+            rds_inst = self.rds_inst
+
         snapshot_id = self._get_db_snapshot_id()
         rds_client.create_db_snapshot(
             DBSnapshotIdentifier=snapshot_id,
-            DBInstanceIdentifier=self.rds_inst.id,
+            DBInstanceIdentifier=rds_inst.id,
             Tags=[
-                dict(Key=settings.ID_TAG_KEY, Value=self.id),
+                dict(Key=settings.ID_TAG_KEY, Value=rds_inst.id),
                 dict(Key="tech:machine_creator", Value="acore_server_metadata"),
             ],
         )
 
     def cleanup_db_snapshot(
         self,
         rds_client,
```

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.4.5/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.4.5/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.4.5/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.4.5/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.4.4
+Version: 0.4.5
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.4#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.4/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.4.5/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/release-history.rst` & `acore_server_metadata-0.4.5/release-history.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.5 (2023-06-21)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug when "check=True", we didn't use the object representing the latest ec2 or rds metadata.
+
+
 0.4.4 (2023-06-20)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - ``acore_server_metadata.api.Server.run_rds`` now also copy ``tech:master_password_digest`` tag from snapshot to RDS instance.
```

### Comparing `acore_server_metadata-0.4.4/requirements-doc.txt` & `acore_server_metadata-0.4.5/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/setup.py` & `acore_server_metadata-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/tests/test_api.py` & `acore_server_metadata-0.4.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.4/tests/test_server.py` & `acore_server_metadata-0.4.5/tests/test_server.py`

 * *Files identical despite different names*

