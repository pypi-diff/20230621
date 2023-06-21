# Comparing `tmp/remotivelabs_cli-0.0.1a4.tar.gz` & `tmp/remotivelabs_cli-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a4.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a5.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a4.tar` & `remotivelabs_cli-0.0.1a5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a4/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a4/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a4/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-06-19 13:36:54.800059 remotivelabs_cli-0.0.1a4/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a4/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3875 2023-06-20 11:44:37.485261 remotivelabs_cli-0.0.1a4/cli/cloud/auth.py
--rw-r--r--   0        0        0     1392 2023-06-20 08:34:18.147931 remotivelabs_cli-0.0.1a4/cli/cloud/auth_keys.py
--rw-r--r--   0        0        0     2306 2023-06-20 11:51:25.452149 remotivelabs_cli-0.0.1a4/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1611 2023-06-20 11:54:09.099670 remotivelabs_cli-0.0.1a4/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a4/cli/cloud/configs.py
--rw-r--r--   0        0        0     1083 2023-06-20 12:47:24.741759 remotivelabs_cli-0.0.1a4/cli/cloud/projects.py
--rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a4/cli/cloud/recordings.py
--rw-r--r--   0        0        0     2979 2023-06-20 12:44:49.774042 remotivelabs_cli-0.0.1a4/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a4/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1176 2023-06-19 13:50:30.024795 remotivelabs_cli-0.0.1a4/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a4/cli/lib/__about__.py
--rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a4/cli/lib/broker.py
--rw-r--r--   0        0        0      315 2023-06-20 11:51:00.031101 remotivelabs_cli-0.0.1a4/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a4/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a4/cli/test/test_simple.py
--rw-r--r--   0        0        0      498 2023-06-20 13:26:20.274638 remotivelabs_cli-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a5/LICENSE
+-rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a5/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a5/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a5/cli/__init__.py
+-rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a5/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a5/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     4568 2023-06-21 14:05:59.199099 remotivelabs_cli-0.0.1a5/cli/cloud/auth.py
+-rw-r--r--   0        0        0     1391 2023-06-21 11:01:07.131368 remotivelabs_cli-0.0.1a5/cli/cloud/auth_keys.py
+-rw-r--r--   0        0        0     2321 2023-06-21 11:04:28.728967 remotivelabs_cli-0.0.1a5/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a5/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a5/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a5/cli/cloud/projects.py
+-rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a5/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     3486 2023-06-21 12:56:24.052615 remotivelabs_cli-0.0.1a5/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a5/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a5/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a5/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a5/cli/lib/broker.py
+-rw-r--r--   0        0        0      315 2023-06-20 11:51:00.031101 remotivelabs_cli-0.0.1a5/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a5/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a5/cli/test/test_simple.py
+-rw-r--r--   0        0        0      498 2023-06-21 14:07:53.672220 remotivelabs_cli-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a5/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a4/LICENSE` & `remotivelabs_cli-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a4/README.md` & `remotivelabs_cli-0.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import Path
 from threading import Thread
 import typer
 from . import rest_helper as rest
 from . import auth_keys
 
-app = typer.Typer()
+help="""
+Manage how you authenticate with our cloud platform
+"""
+
+app = typer.Typer(help=help)
+
 app.add_typer(auth_keys.app, name="keys", help="Manage users personal access keys")
 config_dir_name = str(Path.home()) + "/.config/.remotive/"
 token_file_name = str(Path.home()) + "/.config/.remotive/cloud.secret.token"
 
 
-
 class S(BaseHTTPRequestHandler):
     def _set_response(self):
         self.send_response(200)
         # self.send_response(301)
         # self.send_header('Location', 'https://cloud.remotivelabs.com')
         # self.end_headers()
         self.send_header('Content-type', 'text/html')
@@ -41,75 +45,103 @@
 
         if not os.path.exists(config_dir_name):
             os.makedirs(config_dir_name)
         write_token(path[1:])
         print("Successfully logged on, you are ready to go with cli")
 
 
-def start_local_webserver(server_class=HTTPServer, handler_class=S, port=8089):
+def start_local_webserver(server_class=HTTPServer, handler_class=S, port=0):
     server_address = ('', port)
     global httpd
     httpd = server_class(server_address, handler_class)
-    httpd.serve_forever()
 
 
-@app.command(help="Login to the cloud")
+#
+# CLI commands go here
+#
+
+@app.command(name="login")
 def login():
-    webbrowser.open(f'{rest.base_url}/login?redirectUrl=http://localhost:8089', new=1, autoraise=True)
+    """
+    Login to the cli using browser
+
+    This will be used as the current access token in all subsequent requests. This would
+    be the same as activating a personal access key or service-account access key.
+    """
     start_local_webserver()
+    webbrowser.open(f'{rest.base_url}/login?redirectUrl=http://localhost:{httpd.server_address[1]}', new=1, autoraise=True)
+    httpd.serve_forever()
 
-@app.command(help="Who am I?")
+@app.command()
 def whoami():
+    """
+    Validates authentication and fetches your user information
+    """
     rest.handle_get('/api/whoami')
 
-@app.command(help="Print access token")
+@app.command()
 def print_access_token():
+    """
+    Print current active access token
+    """
     print(read_token())
 
 
-@app.command(help="List available auth tokens")
+@app.command()
 def list():
+    """
+    List available key files in remotivelabs config directory
+    """
     for file in os.listdir(config_dir_name):
         print(file)
 
 
-@app.command(help="Show token file")
+@app.command()
 def describe(
         file: str = typer.Option(..., help="File name")):
+    """
+    Show contents of specified key file
+    """
     print(read_file(file))
 
 
-
-
-@app.command(help="Activate the account file")
+@app.command()
 def activate(
         file: str = typer.Option(..., help="File name")):
+    """
+    Activate a key file to be used for authentication.
+
+    --file
+
+    This will be used as the current access token in all subsequent requests. This would
+    be the same as login with a browser.
+    """
     # Best effort to read file
     if os.path.exists(file):
         token_file = json.loads(read_file_with_path(file))
         write_token(token_file['token'])
     elif os.path.exists(str(Path.home()) + f"/.config/.remotive/{file}"):
         token_file = json.loads(read_file(file))
         write_token(token_file['token'])
     else:
         sys.stderr.write("File could not be found \n")
 
 
-@app.command(help="Clear access token")
-def logout():
-    write_token("")
-    print("Access token removed")
+#@app.command(help="Clear access token")
+#def logout():
+#    write_token("")
+#    print("Access token removed")
 
 
-@app.command(help="Test authentication")
-def test():
-    if rest.has_access('/api/whoami'):
-        print("Access granted, good to go!")
-    else:
-        print("Access failed (401), please login again")
+#@app.command(help="Test authentication")
+#def test():
+#    if rest.has_access('/api/whoami'):
+#        print("Access granted, good to go!")
+#    else:
+#        print("Access failed (401), please login again")
 
 
 def read_token():
     f = open(token_file_name, "r")
     token = f.read()
     f.close()
     return token
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/auth_keys.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/auth_keys.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,9 +38,9 @@
 
 def write_personal_token(file, token):
     path = str(Path.home()) + f"/.config/.remotive/{file}"
     f = open(path, "w")
     f.write(token)
     f.close()
     print(f"Personal key written to {path}")
-    print("Use 'remotive cloud auth activate filename' to use this key from cli")
+    print(f"Use 'remotive cloud auth activate {file}' to use this key from cli")
     print('\033[93m This file contains secrets and must never be compromised')
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/brokers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         body = {"size": "S", 'tag': tag_to_use}
     else:
         body = {"size": "S", 'apiKey': api_key, 'tag': tag_to_use}
     return rest.handle_post(f"/api/project/{project}/brokers/{name}", body=json.dumps(body),
                             return_response=return_response)
 
 
-@app.command(help="Starts a broker in project")
+@app.command(name="create", help="Create a broker in project")
 def start(name: str,
           project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT'),
           tag: str = typer.Option("", help="Optional specific tag/version"),
           silent: bool = typer.Option(False, help="Optional specific tag/version"),
           api_key: str = typer.Option("", help="Start with your own api-key")):
 
     with Progress(
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/cloud_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 def licenses(
         organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
         filter: str = typer.Option("all", help="all, valid, expired")
 ):
     rest.handle_get(f"/api/bu/{organisation}/licenses", {'filter': filter})
 
 
-@app.command(help="Get your organisation and projects with permissions")
-def home(
-        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
-):
-    rest.handle_get(f"/api/bu/{organisation}/me")
+#@app.command(help="Get your organisation and projects with permissions")
+#def home(
+#        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
+#):
+#    rest.handle_get(f"/api/bu/{organisation}/me")
 
 
 # @app.command(help="Get your organisation and projects with permissions")
 # def home2():
 #    rest.handle_get(f"/api/home")
 
 
-@app.command(help="List users in an organisation")
-def users(
-        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
-):
-    rest.handle_get(f"/api/bu/{organisation}/users")
+#@app.command(help="List users in an organisation")
+#def users(
+#        organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
+#):
+#    rest.handle_get(f"/api/bu/{organisation}/users")
 
 
 app.add_typer(projects.app, name="projects", help="Manage projects")
-app.add_typer(auth.app, name="auth", help="Manage access to cloud resources")
+app.add_typer(auth.app, name="auth")
 app.add_typer(brokers.app, name="brokers", help="Manage cloud broker lifecycle")
 app.add_typer(recordings.app, name="recordings", help="Manage recordings")
 app.add_typer(configs.app, name="signal-databases", help="Manage signal databases")
 app.add_typer(service_accounts.app, name="service-accounts", help="Manage project service account keys")
 
 
 if __name__ == "__main__":
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/projects.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/projects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import json
-
 import typer
 from . import rest_helper as rest
+
 app = typer.Typer()
 
 
 @app.command(name="list", help="List your projects")
 def list_projects(organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION')):
     r = rest.handle_get(url=f'/api/bu/{organisation}/me',  return_response=True)
     if r.status_code == 200:
+        # extract the project uid parts
         projects = r.json()['projects']
         projects = map(lambda p: p['uid'], projects)
         print(json.dumps(list(projects)))
+    else:
+        print(r.status_code)
+        print(r.text)
 
 
 @app.command(name="create")
 def create_project(
     organisation: str = typer.Option(..., help="Organisation ID", envvar='REMOTIVE_CLOUD_ORGANISATION'),
     project_uid: str = typer.Option(..., help="Project UID"),
     project_display_name: str = typer.Option(default="", help="Project display name")
@@ -23,8 +27,13 @@
 
     create_project_req = {
         'uid': project_uid,
         'displayName': project_display_name if project_display_name != "" else project_uid,
         'description': ''
     }
 
-    rest.handle_post(url=f'/api/bu/{organisation}/project', body=json.dumps(create_project_req))
+    rest.handle_post(url=f'/api/bu/{organisation}/project', body=json.dumps(create_project_req))
+
+
+@app.command(name="delete")
+def delete(project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
+    rest.handle_delete(url=f'/api/project/{project}')
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a4/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a5/cli/cloud/service_accounts.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,24 @@
     data = {
         'name': name,
         'roles': role
     }
     rest.handle_post(url=f"/api/project/{project}/admin/accounts", body=json.dumps(data))
 
 
-@app.command(name="delete", help="Create service account")
+@app.command(name="update", help="Update service account")
+def update_service_account(
+        service_account: str = typer.Option(..., help="Service account name"),
+        role: List[str] = typer.Option(..., help="Roles to apply"),
+        project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
+
+    rest.handle_put(url=f"/api/project/{project}/admin/accounts/{service_account}", body=json.dumps(role))
+
+
+@app.command(name="delete", help="Delete service account")
 def delete_service_account(
         name: str,
         project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     rest.handle_delete(url=f"/api/project/{project}/admin/accounts/{name}")
 
 
 app.add_typer(service_account_keys.app, name="keys", help="Manage project service account keys")
```

### Comparing `remotivelabs_cli-0.0.1a4/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a5/cli/lib/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import signal
 import binascii
 import queue
 from threading import Thread
 import remotivelabs.broker.sync as br
 
 
 class Broker:
@@ -61,19 +63,20 @@
         for networkInfo in configuration.networkInfo:
             res = self.system_stub.ListSignals(networkInfo.namespace)
             for finfo in res.frame:
                 for sinfo in finfo.childInfo:
                     signal_names.append({'signal': sinfo.id.name, 'namespace' : networkInfo.namespace.name})
         return signal_names
 
-    def subscribe(self, signals: list, on_frame, changed_values_only: bool = True):
+
+    def subscribe(self, signals: list, namespace, on_frame, changed_values_only: bool = True):
         client_id = br.common_pb2.ClientId(id="cloud_demo")
 
         signals_to_subscribe_on = \
-            map(lambda signal: self.signal_creator.signal(signal, "custom_can"), signals)
+            map(lambda signal: self.signal_creator.signal(signal, namespace), signals)
 
         Thread(
             target=br.act_on_signal,
             args=(
                 client_id,
                 self.network_stub,
                 signals_to_subscribe_on,
```

### Comparing `remotivelabs_cli-0.0.1a4/PKG-INFO` & `remotivelabs_cli-0.0.1a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

