# Comparing `tmp/auterion-cli-1.0.9.tar.gz` & `tmp/auterion-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.9.tar", last modified: Tue May  2 10:11:33 2023, max compression
+gzip compressed data, was "auterion-cli-1.1.0.tar", last modified: Wed Jun 21 12:06:06 2023, max compression
```

## Comparing `auterion-cli-1.0.9.tar` & `auterion-cli-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:11:31.000000 auterion-cli-1.0.9/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-02 10:11:33.000000 auterion-cli-1.0.9/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-02 10:11:23.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-02 10:11:23.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 12:06:04.000000 auterion-cli-1.1.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-21 12:06:06.000000 auterion-cli-1.1.0/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/setup.py
```

### Comparing `auterion-cli-1.0.9/README.md` & `auterion-cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.1.0/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_command.py` & `auterion-cli-1.1.0/auterioncli/commands/app_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         start_parser.add_argument('app_name', help='The name of the app to start')
 
         stop_parser = command_subparsers.add_parser('stop', help='Stop an app')
         stop_parser.add_argument('app_name', help='The name of the app to stop')
 
         restart_parser = command_subparsers.add_parser('restart', help='Restart an app')
         restart_parser.add_argument('app_name', help='The name of the app to restart')
+        restart_parser.add_argument('-t', '--stop-timeout', type=int, help='Timeout in seconds to wait for app to stop')
 
         enable_parser = command_subparsers.add_parser('enable', help='Enable an app')
         enable_parser.add_argument('app_name', help='The name of the app to enable')
 
         disable_parser = command_subparsers.add_parser('disable', help='Disable an app')
         disable_parser.add_argument('app_name', help='The name of the app to disable')
 
@@ -141,15 +142,20 @@
         self._print_app_result(data, args.app_name, "started")
 
     def stop(self, args):
         data = requests.post(f'{self._apps_api_endpoint}/apps/{args.app_name}/stop')
         self._print_app_result(data, args.app_name, "stopped")
 
     def restart(self, args):
-        data = requests.post(f'{self._apps_api_endpoint}/apps/{args.app_name}/restart')
+        params = None
+        if args.stop_timeout is not None:
+            params = {
+                'stop_timeout': args.stop_timeout
+            }
+        data = requests.post(f'{self._apps_api_endpoint}/apps/{args.app_name}/restart', json=params)
         self._print_app_result(data, args.app_name, "restarted")
 
     def enable(self, args):
         data = requests.post(f'{self._apps_api_endpoint}/apps/{args.app_name}/enable')
         self._print_app_result(data, args.app_name, "enabled")
 
     def disable(self, args):
```

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,26 +179,33 @@
         if not os.path.exists(build_dir):
             os.mkdir(build_dir)
 
         target_file = os.path.join(build_dir, meta['app-author'] + '.' + meta['app-name'] + '.tar')
 
         # generate a minimal docker-compose file in temp dir for building using docker-compose
         # (don't use self._temp_dir, as podman-compose sets cwd to that directory)
-        compose_file = os.path.join(args.project_dir, 'docker-compose-tmp.yml')
+        compose_file = os.path.join(args.project_dir, 'build-compose.yml')
         compose = self._compose_for_building_from_meta(meta)
         with open(compose_file, 'w') as f:
             yaml.dump(compose, f)
 
         if not args.skip_docker_build:
             # Just export the required images from the local docker
             target_platform = self._extract_target_platform(meta)
-            ret = run_command(compose_cmd + ['-f', compose_file, 'build'], cwd=args.project_dir)
+
+            build_command = compose_cmd + ['-f', compose_file, 'build']
+            ret = run_command(build_command, cwd=args.project_dir)
 
             if ret != 0:
-                error("Docker compose build failed.")
+                error("------------------------------------------------------\n"
+                      "Docker build failed. \n"
+                      "Temporary `build-compose.yml` file left in tree. \n\n"
+                      "This is most likely not a problem with auterion-cli.\n"
+                      "To debug the build without auterion-cli, run \n"
+                      f"{' '.join(build_command)}")
             os.remove(compose_file)
 
             non_built_images = [v['image'] for k, v in compose['services'].items() if 'build' not in v]
             if len(non_built_images) > 0:
                 print(f'Need to pull {len(non_built_images)} images for this build..')
                 for image in non_built_images:
                     run_command(['docker', 'pull', '--platform', target_platform, image])
@@ -231,25 +238,25 @@
     def _compress_image(self, image):
         run_command(['gzip', image])
         p = pathlib.Path(image + '.gz')
         target_name = p.with_suffix('').with_suffix('.image')
         p.rename(target_name)
         return str(target_name)
 
-    def _generate_legacy_app_file(self, meta, app_file):
+    def _generate_legacy_app_file(self, meta, slug, app_file):
         # add default settings for compose
         compose = self._compose_for_building_from_meta(meta)
         app_dict = copy.deepcopy(compose)
         for name, service in app_dict['services'].items():
             if 'restart' not in service:
                 service['restart'] = 'unless-stopped'
             if 'network_mode' not in service:
                 service['network_mode'] = 'host'
             if 'volumes' not in service:
-                service['volumes'] = [f'/data/app/{meta["app-name"]}/data:/data']
+                service['volumes'] = [f'/data/app/{slug}/data:/data']
             if 'environment' not in service:
                 service['environment'] = ['PYTHONUNBUFFERED=1']
             if 'env_file' not in service:
                 service['env_file'] = ['settings.default.env', 'settings.user.env']
 
             # older docker-compose get confused about the platform and build tags
             if 'platform' in service:
@@ -299,15 +306,15 @@
             '-f', os.path.abspath(version_file),
             '-f', os.path.abspath(settings_file),
             '-f', os.path.abspath(user_settings_file)
         ]
 
         if meta['auterion-api-version'] < 2:
             app_file = os.path.join(self._temp_dir, 'app.yml')
-            self._generate_legacy_app_file(meta, app_file)
+            self._generate_legacy_app_file(meta, slug, app_file)
             file_args += ['-f', app_file]
 
         pathlib.Path(settings_file).touch()
 
         ret = run_command([
             'docker',
             'run',
```

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.1.0/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/container_command.py` & `auterion-cli-1.1.0/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/device_command.py` & `auterion-cli-1.1.0/auterioncli/commands/device_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import zeroconf
 import time
 import socket
 from .command_base import CliCommand
 from tabulate import tabulate
-from .utils import error
+from .utils import error, eprint
 
 
 def _find_devices_zeroconf(timeout):
     devices = {}
 
     class Listener(zeroconf.ServiceListener):
         def add_service(self, zc_inst, service_type, name):
@@ -28,20 +28,24 @@
                         }
 
         def remove_service(self, zc_inst, service_type, name):
             pass
 
         def update_service(self, zc_inst, service_type, name):
             pass
+    try:
+        zc = zeroconf.Zeroconf()
+        listener = Listener()
+        browser = zeroconf.ServiceBrowser(zc, '_https._tcp.local.', listener)
+        time.sleep(timeout)
+        zc.close()
+    except OSError as e:
+        eprint('Warn: Zeroconf initialization failed: %s' % e)
+        eprint('      Dynamic discovery will not be available.')
 
-    zc = zeroconf.Zeroconf()
-    listener = Listener()
-    browser = zeroconf.ServiceBrowser(zc, '_https._tcp.local.', listener)
-    time.sleep(timeout)
-    zc.close()
     return devices
 
 
 def _find_devices_address(addresses, timeout=0.5):
     devices = {}
     for address in addresses:
         url = f"http://{address}/api/sysinfo/v1.0/device"
```

### Comparing `auterion-cli-1.0.9/auterioncli/commands/info_command.py` & `auterion-cli-1.1.0/auterioncli/commands/info_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 print("{}:".format(name))
                 if data['status'] == "running":
                     status_str = "[\033[32mRUNNING\033[39m]"
                 elif data['status'] == "succeeded":
                     status_str = "[\033[32mSUCCEEDED\033[39m]"
                 else:
                     status_str = "[\033[31mERROR\033[39m]"
-                print("\thash: {}".format(data['hash']))
+                print("\tversion: {}".format(data.get('version', data.get('hash', 'no version information'))))
                 print("\tstatus: {}".format(status_str))
         else:
             print("No software information available")
 
         print("\n===== System services Information =====")
         services = self._get_information("services")
         if services:
```

### Comparing `auterion-cli-1.0.9/auterioncli/commands/report_command.py` & `auterion-cli-1.1.0/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/commands/utils.py` & `auterion-cli-1.1.0/auterioncli/commands/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from tqdm import tqdm
 import requests
+import sys
 
 
 class Device:
     def __init__(self, address, version):
         self._address = address
         self._version = version
 
@@ -26,10 +27,14 @@
             progress_bar.update(len(data))
             file.write(data)
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong while downloading..")
 
 
+def eprint(*args, **kwargs):
+    print(*args, file=sys.stderr, **kwargs)
+
+
 def error(msg, code=1):
-    print(msg)
+    eprint(msg)
     exit(code)
```

### Comparing `auterion-cli-1.0.9/auterioncli/main.py` & `auterion-cli-1.1.0/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/auterioncli/meta_util.py` & `auterion-cli-1.1.0/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.9/setup.py` & `auterion-cli-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     git_version = git_version.replace('-', '.dev', 1).replace('-', '+', 1)
     return git_version
 
 
 setup(name='auterion-cli',
       version=get_version(),
       description='CLI tool to interact with AuterionOS devices and apps',
-      url='https://github.com/Auterion/auterion-cli',
+      url='https://docs.auterion.com/developers',
       author='Auterion',
       author_email='support@auterion.com',
       license='proprietary',
       packages=find_packages(),
       install_requires=[
           'tabulate',
           'requests',
```

