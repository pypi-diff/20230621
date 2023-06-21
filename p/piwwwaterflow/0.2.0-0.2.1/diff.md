# Comparing `tmp/piwwwaterflow-0.2.0.tar.gz` & `tmp/piwwwaterflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.2.0.tar", last modified: Tue Jun 20 07:30:24 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.2.1.tar", last modified: Wed Jun 21 17:03:32 2023, max compression
```

## Comparing `piwwwaterflow-0.2.0.tar` & `piwwwaterflow-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.682527 piwwwaterflow-0.2.0/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.795098 piwwwaterflow-0.2.1/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.795098 piwwwaterflow-0.2.1/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/tests/__init__.py
```

### Comparing `piwwwaterflow-0.2.0/PKG-INFO` & `piwwwaterflow-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.2.1/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.2.1/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.2.1/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.2.1/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.2.1/piwwwaterflow/static/js/code.js`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.2.1/piwwwaterflow/templates/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -94,13 +94,13 @@
 			</table>
 		</form>	
 	</div>
 	<div>
 		<textarea id="log" rows="12"  style = "width:100%; height:20vh; font-size: 0.27em;" readonly>Retrieving log...</textarea>
 	</div>
 	<div>
-		<iframe id="grafana_iframe" src="http://pi02:3000/d-solo/m_AskAmgk/jardin?orgId=2&showCategory=Override+2&from=now-24h&to=now&theme=dark&panelId=2" width="100%" height="50%" frameborder="0"></iframe>
+		<iframe id="grafana_iframe" src="https://grafana.phornee.synology.me/d-solo/m_AskAmgk/jardin?orgId=2&showCategory=Override+2&from=now-24h&to=now&theme=dark&panelId=2" width="100%" height="50%" frameborder="0"></iframe>
 	</div>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.0.1/socket.io.js" integrity="sha512-q/dWJ3kcmjBLU4Qc47E4A9kTB4m3wuTY7vkFJDTZKjTs8jhyGQnaUrxa0Ytd0ssMZhbNua9hE+E7Qv1j+DyZwA==" crossorigin="anonymous"></script>
 	<script type="text/javascript" src="static/js/code.js"></script>
 	</body>
 </html>
```

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/webservice.py` & `piwwwaterflow-0.2.1/piwwwaterflow/webservice.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 class PiWWWaterflowService:
     """Class for the web service... its an interface to the real functionality in piwaterflow package.
     """
     def __init__(self,  template_folder, static_folder):
 
         self.logger = Logger(self.class_name(), log_file_name='piwwwaterflow', mode=LoggerMode.BOTH, dry_run=False)
         self.logger.info("Launching piwwwaterflow...")
-        self.waterflow = Waterflow()
 
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
 
         self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
 
         self.app.add_url_rule('/', 'waterflow', self.waterflow_endpoint, methods=['GET', 'POST'])
 
         self.app.add_url_rule('/service', 'service', self.on_service_request, methods=['GET'])
         self.app.add_url_rule('/force', 'force', self.on_force, methods=['GET', 'POST'])
         self.app.add_url_rule('/stop', 'stop', self.on_stop, methods=['GET', 'POST'])
         self.app.add_url_rule('/save', 'save', self.on_save, methods=['POST'])
 
         Compress(self.app)
-        self.waterflow = Waterflow()
 
     @classmethod
     def class_name(cls):
         """ class name """
         return "piwwwaterflow"
 
     def get_app(self):
@@ -60,29 +58,32 @@
         """ Gets all the information from the waterflow service
         Args:
             data (dict):'first_time': This value is only bypassed to the caller
         Returns:
             dict:Dictionary with all the information about the status of the waterflow system
         """
         self.logger.info('Service requested...')
+
+        waterflow = Waterflow()
+
         try:
             ver_backend = version('piwaterflow')
             ver_frontend = version('piwwwwaterflow')
         except PackageNotFoundError:
             ver_backend = '?.?.?'
             ver_frontend = '?.?.?'
 
         responsedict = None
 
         try:
-            responsedict = {'log': self.waterflow.get_log(),
-                            'forced': self.waterflow.get_forced_info(),
-                            'stop': self.waterflow.stop_requested(),
-                            'config': self._get_public_config(),
-                            'lastlooptime': self.waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
+            responsedict = {'log': waterflow.get_log(),
+                            'forced': waterflow.get_forced_info(),
+                            'stop': waterflow.stop_requested(),
+                            'config': self._filter_public_config(waterflow.config.get_dict_copy()),
+                            'lastlooptime': waterflow.last_loop_time().strftime('%Y-%m-%dT%H:%M:%S'),
                             'version_backend': ver_backend,
                             'version_frontend': ver_frontend
                             }
             # Change to string so that javascript can manage with it
             for program in responsedict['config']['programs']:
                 program['start_time'] = program['start_time'].strftime('%H:%M')
         except Exception as ex:
@@ -93,50 +94,56 @@
 
     def on_force(self, data: dict):
         """ On force action request
         Args:
             data (dict): 'type': Must be 'valve' or 'program'
                          'value': Must be the index of the program or value to be forced
         """
+        waterflow = Waterflow()
+
         if request.method == 'POST':
-            print(f'Force requested... {data}')
+            self.logger.info('Force requested...%s', data)
             type_force = request.form.get['type']
             value_force = request.form.get['value']
-            self.waterflow.force(type_force, value_force)
+            waterflow.force(type_force, value_force)
         else:
-            forced_data = self.waterflow.get_forced_info()
+            forced_data = waterflow.get_forced_info()
             return forced_data
             # return json.dumps(forced_data)
 
     def on_stop(self):
         """ Event to stop current operation """
+        waterflow = Waterflow()
+
         if request.method == 'POST':
-            print('Stop requested...')
-            self.waterflow.stop()
+            self.logger.info('Stop requested...')
+            waterflow.stop()
         else:
-            stop_requested = self.waterflow.stop_requested()
+            stop_requested = waterflow.stop_requested()
             return "true" if stop_requested else "false"
 
     def on_save(self):
         """ Event to save the changes in the watering system schedulling
         Args:
             data (dict): Information about the required schedulling
         Returns:
             bool: If everything went ok
         """
+        waterflow = Waterflow()
+
+        self.logger.info("Saving programs...")
         data = request.form.get['save']
-        parsed_config = self.waterflow.config.get_dict_copy()
+        parsed_config = waterflow.config.get_dict_copy()
         for program, update in zip(parsed_config['programs'], data):
             self._change_program(program, update)
 
-        self.waterflow.update_config(programs=parsed_config['programs'])
+        waterflow.update_config(programs=parsed_config['programs'])
         return True
 
-    def _get_public_config(self):
-        config = self.waterflow.config.get_dict_copy()
+    def _filter_public_config(self, config):
         del config['influxdbconn']
         return config
 
     def _change_program(self, program, new_program):
         inputbox_text = new_program['time']
         time1 = datetime.strptime(inputbox_text, '%H:%M')
         new_datetime = program['start_time'].replace(hour=time1.hour, minute=time1.minute)
```

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.2.1/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.2.1/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.2.0/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.2.1/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.0/setup.py` & `piwwwaterflow-0.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.2.0",
+    version="0.2.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -21,15 +21,12 @@
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
-        'python-socketio>=5.8.0',
-        'flask-socketio>=5.3.3',
-        'eventlet==0.30.2', # Exact version required 0.30.2
         'piwaterflow>=0.6.0',
         'revproxy_auth>=0.1.7'
     ],
     python_requires='>=3.6',
 )
```

