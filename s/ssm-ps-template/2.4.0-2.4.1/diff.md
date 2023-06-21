# Comparing `tmp/ssm-ps-template-2.4.0.tar.gz` & `tmp/ssm-ps-template-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.4.0.tar", last modified: Fri Jun 16 16:25:02 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.4.1.tar", last modified: Wed Jun 21 18:19:42 2023, max compression
```

## Comparing `ssm-ps-template-2.4.0.tar` & `ssm-ps-template-2.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    12692 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10056 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1875 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2814 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12692 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-16 16:25:02.000000 ssm-ps-template-2.4.0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 16:25:02.580162 ssm-ps-template-2.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3021 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-16 16:24:52.000000 ssm-ps-template-2.4.0/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12757 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10121 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 18:19:42.806566 ssm-ps-template-2.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12757 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-21 18:19:42.000000 ssm-ps-template-2.4.1/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 18:19:42.802565 ssm-ps-template-2.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-21 18:19:31.000000 ssm-ps-template-2.4.1/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.4.0/LICENSE.txt` & `ssm-ps-template-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/PKG-INFO` & `ssm-ps-template-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.4.0
+Version: 2.4.1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -76,33 +76,37 @@
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
-foo: {{ get_parameter('/my-application/foo'}}
-bar: {{ get_parameter('/my-application/bar'}}
+foo: {{ get_parameter('/my-application/foo') }}
+bar: {{ get_parameter('/my-application/bar') }}
 ```
+
 Will render as:
+
 ```yaml
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
+
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use Jinja filters to convert them to YAML:
+
 ```yaml
 {{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
@@ -197,22 +201,25 @@
 templates:
   - source: /etc/ssm-templates/nginx-example
     destination: /etc/nginx/sites-available/example
     prefix: /namespaced/application/nginx/
   - source: /etc/ssm-templates/postgres-example
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
+    user: postgres
+    group: postgres
+    mode: 0600
 profile: default
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
-```
+```sh
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
                        [--verbose] [--version]
                        config
 
 Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
@@ -228,9 +235,10 @@
                         Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
   --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
   --version             show program's version number and exit
 ```
+
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.4.0/README.md` & `ssm-ps-template-2.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,33 +27,37 @@
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
-foo: {{ get_parameter('/my-application/foo'}}
-bar: {{ get_parameter('/my-application/bar'}}
+foo: {{ get_parameter('/my-application/foo') }}
+bar: {{ get_parameter('/my-application/bar') }}
 ```
+
 Will render as:
+
 ```yaml
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
+
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use Jinja filters to convert them to YAML:
+
 ```yaml
 {{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
@@ -148,22 +152,25 @@
 templates:
   - source: /etc/ssm-templates/nginx-example
     destination: /etc/nginx/sites-available/example
     prefix: /namespaced/application/nginx/
   - source: /etc/ssm-templates/postgres-example
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
+    user: postgres
+    group: postgres
+    mode: 0600
 profile: default
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
-```
+```sh
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
                        [--verbose] [--version]
                        config
 
 Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
@@ -179,9 +186,10 @@
                         Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
   --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
   --version             show program's version number and exit
 ```
+
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.4.0/pyproject.toml` & `ssm-ps-template-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.4.0"
+version = "2.4.1"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
@@ -14,15 +14,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Natural Language :: English",
     "Topic :: Text Processing",
     "Topic :: Utilities"
 ]
 dependencies = [
-    "boto3>=1.26,<2",
+    "boto3>=1,<2",
     "flatdict>=4,<5",
     "jinja2>=3,<4",
     "pyyaml>=5.3.1,<7",
     "toml>=0.10,<1"
 ]
 keywords = ["aws", "ssm", "parameter store", "templating"]
 license = {file = "LICENSE.txt"}
```

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template/__main__.py` & `ssm-ps-template-2.4.1/ssm_ps_template/__main__.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template/config.py` & `ssm-ps-template-2.4.1/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template/discovery.py` & `ssm-ps-template-2.4.1/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template/render.py` & `ssm-ps-template-2.4.1/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template/ssm.py` & `ssm-ps-template-2.4.1/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.4.1/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.4.0
+Version: 2.4.1
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -76,33 +76,37 @@
 ### Getting Parameter Store Values
 
 The application exposes `get_parameter(name: str, default: typing.Optional[str] = None)` in templates to access the values in SSM Parameter Store.
 
 In the following example we assume there are Parameter Store values for the keys `/my-application/foo` and `/my-application/bar` and that the application is called with a prefix of `/my-appliction`:
 
 ```yaml
-foo: {{ get_parameter('/my-application/foo'}}
-bar: {{ get_parameter('/my-application/bar'}}
+foo: {{ get_parameter('/my-application/foo') }}
+bar: {{ get_parameter('/my-application/bar') }}
 ```
+
 Will render as:
+
 ```yaml
 foo: bar
 baz: qux
 ```
 
 Additionally, there is another function exposed `get_parameters_by_path(path: str, default: typing.Optional[dict] = None)` which will return a dictionary for the specified path.
 
 The following example will iterate over the results:
+
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
 Or you can use Jinja filters to convert them to YAML:
+
 ```yaml
 {{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
@@ -197,22 +201,25 @@
 templates:
   - source: /etc/ssm-templates/nginx-example
     destination: /etc/nginx/sites-available/example
     prefix: /namespaced/application/nginx/
   - source: /etc/ssm-templates/postgres-example
     destination: /etc/postgresql/14/main/postgresql.conf
     prefix: /namespaced/application/postgres/
+    user: postgres
+    group: postgres
+    mode: 0600
 profile: default
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
-```
+```sh
 usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
                        [--verbose] [--version]
                        config
 
 Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
@@ -228,9 +235,10 @@
                         Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
   --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
                         Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
   --version             show program's version number and exit
 ```
+
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.4.0/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.4.1/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/tests/test_config.py` & `ssm-ps-template-2.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/tests/test_discovery.py` & `ssm-ps-template-2.4.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/tests/test_main.py` & `ssm-ps-template-2.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/tests/test_render.py` & `ssm-ps-template-2.4.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.4.0/tests/test_ssm.py` & `ssm-ps-template-2.4.1/tests/test_ssm.py`

 * *Files identical despite different names*

