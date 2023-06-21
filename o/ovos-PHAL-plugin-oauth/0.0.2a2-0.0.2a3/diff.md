# Comparing `tmp/ovos-PHAL-plugin-oauth-0.0.2a2.tar.gz` & `tmp/ovos-PHAL-plugin-oauth-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a2.tar", last modified: Wed Jun 14 01:44:06 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a3.tar", last modified: Wed Jun 21 16:13:23 2023, max compression
```

## Comparing `ovos-PHAL-plugin-oauth-0.0.2a2.tar` & `ovos-PHAL-plugin-oauth-0.0.2a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:43:58.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:44:06.000000 ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:44:06.725565 ovos-PHAL-plugin-oauth-0.0.2a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-14 01:43:55.000000 ovos-PHAL-plugin-oauth-0.0.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.122564 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:13:15.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.122564 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-21 16:13:23.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/setup.py
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a2/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a2/README.md` & `ovos-PHAL-plugin-oauth-0.0.2a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth/__init__.py` & `ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 from ovos_bus_client.message import Message
 from oauthlib.oauth2 import WebApplicationClient
 from ovos_backend_client.database import (OAuthApplicationDatabase,
                                           OAuthTokenDatabase)
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.log import LOG
 from ovos_utils.network_utils import get_ip
+from ovos_utils import classproperty
+from ovos_utils.process_utils import RuntimeRequirements
 
 os.environ['OAUTHLIB_INSECURE_TRANSPORT'] = '1'
 
 app = Flask(__name__)
 
+
 @app.route("/auth/callback/<munged_id>", methods=['GET'])
 def oauth_callback(munged_id):
     """ user completed oauth, save token to db """
     params = dict(request.args)
     code = params["code"]
 
     data = OAuthApplicationDatabase()[munged_id]
@@ -78,31 +81,42 @@
     validator = OAuthPluginValidator
 
     def __init__(self, bus=None, config=None):
         self.config = config
         self.port = self.config.get("port", 36536)
         self.local_flask_host = None
         self.oauth_skills = {}
-        
+
         super().__init__(bus=bus, name="ovos-PHAL-plugin-oauth", config=config)
-        
+
         # self.bus can only be used after call to super()
         self.bus.on("oauth.register", self.handle_oauth_register)
         self.bus.on("oauth.start", self.handle_start_oauth)
         self.bus.on("oauth.get", self.handle_get_auth_url)
         self.bus.on("ovos.shell.oauth.register.credentials",
                     self.handle_client_secret)
 
         # QR Code Remote OAuth Process Support
         self.bus.on("oauth.get.app.host.info", self.handle_get_app_host_info)
         self.bus.on("oauth.generate.qr.request", self.handle_generate_qr)
 
         # trigger register events from oauth skills
         self.bus.emit(Message("oauth.ping"))
 
+    @classproperty
+    def runtime_requirements(self):
+        return RuntimeRequirements(internet_before_load=True,
+                                   network_before_load=True,
+                                   gui_before_load=False,
+                                   requires_internet=True,
+                                   requires_network=True,
+                                   requires_gui=True,
+                                   no_internet_fallback=False,
+                                   no_network_fallback=False,
+                                   no_gui_fallback=True)
 
     def handle_client_secret(self, message):
         skill_id = message.data.get("skill_id")
         app_id = message.data.get("app_id")
         munged_id = f"{skill_id}_{app_id}"  # key for oauth db
 
         client_id = message.data.get("client_id")
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a2/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO` & `ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-oauth
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a2/setup.py` & `ovos-PHAL-plugin-oauth-0.0.2a3/setup.py`

 * *Files identical despite different names*

