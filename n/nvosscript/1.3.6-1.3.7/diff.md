# Comparing `tmp/nvosscript-1.3.6.tar.gz` & `tmp/nvosscript-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.6.tar", last modified: Tue Jun 20 08:45:16 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.tar", last modified: Wed Jun 21 02:50:00 2023, max compression
```

## Comparing `nvosscript-1.3.6.tar` & `nvosscript-1.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.191358 nvosscript-1.3.6/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.6/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-20 08:45:16.191199 nvosscript-1.3.6/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.6/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.187465 nvosscript-1.3.6/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.6/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    13886 2023-06-20 08:38:00.000000 nvosscript-1.3.6/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8796 2023-06-20 08:44:42.000000 nvosscript-1.3.6/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.6/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.188342 nvosscript-1.3.6/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-06-20 08:45:16.191405 nvosscript-1.3.6/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-06-20 07:21:24.000000 nvosscript-1.3.6/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.189437 nvosscript-1.3.6/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.6/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.6/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.6/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     2531 2023-06-14 01:42:31.000000 nvosscript-1.3.6/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.190605 nvosscript-1.3.6/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.6/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1663 2023-05-29 07:39:37.000000 nvosscript-1.3.6/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-06-20 07:21:24.000000 nvosscript-1.3.6/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.6/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.190854 nvosscript-1.3.6/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.6/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.291493 nvosscript-1.3.7/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-21 02:50:00.291348 nvosscript-1.3.7/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.287919 nvosscript-1.3.7/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    13886 2023-06-20 08:38:00.000000 nvosscript-1.3.7/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.288755 nvosscript-1.3.7/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-06-21 02:50:00.291557 nvosscript-1.3.7/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-06-21 02:49:53.000000 nvosscript-1.3.7/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.289775 nvosscript-1.3.7/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.7/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     2531 2023-06-14 01:42:31.000000 nvosscript-1.3.7/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.290808 nvosscript-1.3.7/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-06-21 02:49:49.000000 nvosscript-1.3.7/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.291036 nvosscript-1.3.7/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.6/LICENSE` & `nvosscript-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/nvos/file.py` & `nvosscript-1.3.7/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/nvos/remote.py` & `nvosscript-1.3.7/nvos/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     bucket = s3.Bucket(bucket_name)
     bucket.upload_file(file_path, file_name)
 
 
 def file_upload_notify(workspace_path, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/analyse")
-    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
+    post_param = {"userId": login.get_user_id(workspace_path), "fileDirectory": workspace_path, "projectSpaceList": project_list}
     data = post_data(url, post_param)
     return data
 
 def upload_file(workspace_path, file_path_list, project_space_list):
     upload_list = []
     filter_upload_re = filter_upload_dir()
     for project_space in project_space_list:
@@ -93,51 +93,51 @@
                 logger.info(f"file :{f} ")
                 continue
 
             if project_space["project_space"] in file_path["file_path"]:
                 local_file_path = file_path["file_path"]
                 temp_file = {"local_file_path": local_file_path, "project_space": project_space["project_space"], "project_space_git_branch": project_space["git_branch"]}
                 upload_list.append(temp_file)
-    upload_process(upload_list)
+    upload_process(workspace_path,upload_list)
 
     file_upload_notify(workspace_path, project_space_list)
 
-def upload_process(upload_list):
+def upload_process(workspace_path,upload_list):
     global global_var
     multiprocessing.set_start_method('spawn', True)
     cores = multiprocessing.cpu_count()
     with concurrent.futures.ThreadPoolExecutor(max_workers=cores) as executor, tqdm(desc="uploading", total=len(upload_list)) as progress:
         for index, file in enumerate(upload_list):
-            executor.submit(uploading_file, file)
+            executor.submit(uploading_file, workspace_path, file)
         time_count = 0
         addition = 0
         while True:
             time.sleep(1)
             time_count += 1
             progress.update(global_var - addition)
             addition = global_var
             if (global_var == len(upload_list) or global_var >= len(upload_list) - 20):
                 break
             if time_count == 60:
                 break
 
 
-def uploading_file(file):
+def uploading_file(workspace_path, file):
 
     global global_var
 
     get_current_env()
     url = "%s%s" % (daemon_network, "/file/upload")
 
     local_file_path = file["local_file_path"]
 
     try:
         with open(local_file_path, 'r', encoding=utils.file_encoding) as f:
             contents = f.read()
-        post_param = {"projectSpaceGitBranch": file["project_space_git_branch"], "projectSpaceFileDirectory": file["project_space"], "userId": login.get_user_id(), "filePath": local_file_path, "fileContent": contents}
+        post_param = {"projectSpaceGitBranch": file["project_space_git_branch"], "projectSpaceFileDirectory": file["project_space"], "userId": login.get_user_id(workspace_path), "filePath": local_file_path, "fileContent": contents}
         post_data(url, post_param)
         logger.info(f"upload file local full path:{local_file_path}")
         global_var += 1
     except Exception:
         traceback.print_exc()
         logger.exception('uploading_file error: %s', local_file_path)
 
@@ -159,22 +159,22 @@
             logger.exception(f"this file sync fail  id:{file_id} ")
         else:
             logger.info(f"this file sync success  id:{file_id} ")
 
 def save_workspace(workspace_path, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/add")
-    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
+    post_param = {"userId": login.get_user_id(workspace_path), "fileDirectory": workspace_path, "projectSpaceList": project_list}
     return post_data(url, post_param)
 
 
 def pull_workspace(workspace, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/getChangedFiles")
-    post_param = {"userId": login.get_user_id(), "fileDirectory": workspace, "projectSpaceList": project_list}
+    post_param = {"userId": login.get_user_id(workspace), "fileDirectory": workspace, "projectSpaceList": project_list}
     return post_data(url, post_param)
 
 
 def post_data(url, params):
     headers = {"content-type": "application/json"}
     logger.info(f'request url:{url} params:{params}')
     response = requests.post(url, headers=headers, data=json.dumps(params))
```

### Comparing `nvosscript-1.3.6/nvos/run.py` & `nvosscript-1.3.7/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/setup.py` & `nvosscript-1.3.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.6',
+    version='1.3.7',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.6/skyeye/loghandler.py` & `nvosscript-1.3.7/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/skyeye/remote.py` & `nvosscript-1.3.7/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/start/login.py` & `nvosscript-1.3.7/start/login.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,18 +34,21 @@
     with open(path, 'r') as file:
         content = file.readline()
         login_data = json.loads(content)
         login_success = login_data["login"] == "success"
     return login_success
 
 
-def get_user_id():
-    workspace_path, success = utils.check_workspace_exist(os.getcwd())
-    if not success:
-        return False
-
+def get_user_id(workspace_value = None):
+    workspace_path = ""
+    if workspace_value is None:
+        workspace_path, success = utils.check_workspace_exist(os.getcwd())
+        if not success:
+            return False
+    else:
+        workspace_path = workspace_value
     path = os.path.join(workspace_path, '.ndtc', "login")
     with open(path, 'r') as file:
         content = file.readline()
         login_data = json.loads(content)
         user_id = login_data["user_name"]
     return user_id
```

### Comparing `nvosscript-1.3.6/start/main.py` & `nvosscript-1.3.7/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.6")
+        print("1.3.7")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.6/start/utils.py` & `nvosscript-1.3.7/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.6/win/win_auto_script.py` & `nvosscript-1.3.7/win/win_auto_script.py`

 * *Files identical despite different names*

