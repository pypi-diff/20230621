# Comparing `tmp/kpops-1.1.5.tar.gz` & `tmp/kpops-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.1.5.tar", max compression
+gzip compressed data, was "kpops-1.2.0.tar", max compression
```

## Comparing `kpops-1.1.5.tar` & `kpops-1.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     1064 2023-06-07 12:01:07.240769 kpops-1.1.5/LICENSE
--rw-r--r--   0        0        0     2370 2023-06-07 12:01:07.240769 kpops-1.1.5/README.md
--rw-r--r--   0        0        0       22 2023-06-07 12:01:31.725022 kpops-1.1.5/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/exception.py
--rw-r--r--   0        0        0    11727 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/main.py
--rw-r--r--   0        0        0     4206 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9357 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     4373 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8142 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      235 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5823 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1851 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      999 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      231 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9454 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6917 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     8338 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     7457 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    16472 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     6778 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3272 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0    11401 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2859 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9097 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     4080 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    10738 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     2589 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1032 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/environment.py
--rw-r--r--   0        0        0     5808 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      594 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1221 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1867 2023-06-07 12:01:31.709022 kpops-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 kpops-1.1.5/setup.py
--rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 kpops-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-21 11:16:42.240658 kpops-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2350 2023-06-21 11:16:42.240658 kpops-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11727 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/main.py
+-rw-r--r--   0        0        0     4206 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1969 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       52 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0    10517 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4341 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8142 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      235 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5832 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1825 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      999 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6272 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9358 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6917 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     7127 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     6658 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    15917 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     7306 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0       66 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2471 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3340 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     8915 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1110 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2831 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9067 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     3463 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    13226 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     3878 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2597 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1032 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5620 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      552 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     2563 2023-06-21 11:16:42.248658 kpops-1.2.0/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1900 2023-06-21 11:16:42.248658 kpops-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 kpops-1.2.0/PKG-INFO
```

### Comparing `kpops-1.1.5/LICENSE` & `kpops-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/README.md` & `kpops-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.
 - **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).
 - **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.
 
 ## Documentation
 
 For detailed usage and installation instructions, check out
-the [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).
+the [documentation](https://bakdata.github.io/kpops/latest).
 
 ## Install KPOps
 
 KPOps comes as a [PyPI package](https://pypi.org/project/kpops/). 
 You can install it with [pip](https://github.com/pypa/pip):
 
 ```shell
```

### Comparing `kpops-1.1.5/kpops/cli/custom_formatter.py` & `kpops-1.2.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/cli/main.py` & `kpops-1.2.0/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/cli/pipeline_config.py` & `kpops-1.2.0/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/cli/registry.py` & `kpops-1.2.0/kpops/cli/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import inspect
 import os
 import sys
 from collections.abc import Iterator
 from dataclasses import dataclass, field
 from typing import TypeVar
 
+from kpops import __name__
 from kpops.cli.exception import ClassNotFoundError
 from kpops.components.base_components.pipeline_component import PipelineComponent
 
+KPOPS_MODULE = __name__ + "."
+
 T = TypeVar("T")
 ClassDict = dict[str, type[T]]  # type -> class
 
 sys.path.append(os.getcwd())
 
 
 @dataclass
@@ -46,9 +49,14 @@
     except StopIteration:
         raise ClassNotFoundError
 
 
 def _find_classes(module_name: str, baseclass: type[T]) -> Iterator[type[T]]:
     module = importlib.import_module(module_name)
     for _, _class in inspect.getmembers(module, inspect.isclass):
-        if issubclass(_class, baseclass) and module_name in _class.__module__:
+        if issubclass(_class, baseclass):
+            # filter out internal kpops classes unless specifically requested
+            if _class.__module__.startswith(
+                KPOPS_MODULE
+            ) and not module_name.startswith(KPOPS_MODULE):
+                continue
             yield _class
```

### Comparing `kpops-1.1.5/kpops/component_handlers/__init__.py` & `kpops-1.2.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.2.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 from kpops.component_handlers.helm_wrapper.exception import ReleaseNotFoundException
 from kpops.component_handlers.helm_wrapper.model import (
     HelmConfig,
     HelmTemplate,
     HelmTemplateFlags,
     HelmUpgradeInstallFlags,
     RepoAuthFlags,
+    Version,
     YamlReader,
 )
 
 log = logging.getLogger("Helm")
 
 
 class Helm:
     def __init__(self, helm_config: HelmConfig) -> None:
         self._context = helm_config.context
         self._debug = helm_config.debug
+        self._version = self.get_version()
+        if self._version.major != 3:
+            raise RuntimeError(
+                f"The supported Helm version is 3.x.x. The current Helm version is {self._version.major}.{self._version.minor}.{self._version.patch}"
+            )
 
     def add_repo(
         self,
         repository_name: str,
         repository_url: str,
         repo_auth_flags: RepoAuthFlags = RepoAuthFlags(),
     ) -> None:
@@ -64,15 +70,18 @@
                 )
                 is not None
             ):
                 log.error(f"Could not add repository {repository_name}. {e}")
             else:
                 raise e
 
-        self.__execute(["helm", "repo", "update"])
+        if self._version.minor > 7:
+            self.__execute(["helm", "repo", "update", repository_name])
+        else:
+            self.__execute(["helm", "repo", "update"])
 
     def upgrade_install(
         self,
         release_name: str,
         chart: str,
         dry_run: bool,
         namespace: str,
@@ -104,17 +113,15 @@
 
     def uninstall(
         self,
         namespace: str,
         release_name: str,
         dry_run: bool,
     ) -> str | None:
-        """
-        Prepares and executes the helm uninstall command
-        """
+        """Prepares and executes the helm uninstall command"""
         command = [
             "helm",
             "uninstall",
             release_name,
             "--namespace",
             namespace,
         ]
@@ -127,39 +134,46 @@
                 f"Release with name {release_name} not found. Could not uninstall app."
             )
 
     def template(
         self,
         release_name: str,
         chart: str,
+        namespace: str,
         values: dict,
         flags: HelmTemplateFlags = HelmTemplateFlags(),
     ) -> str:
-        """
-        From HELM: Render chart templates locally and display the output.
+        """From HELM: Render chart templates locally and display the output.
 
         Any values that would normally be looked up or retrieved in-cluster will
         be faked locally. Additionally, none of the server-side testing of chart
         validity (e.g. whether an API is supported) is done.
 
         :param str release_name: the release name for which the command is ran
-        :param str chart: Helm chart to be templated
-        :param dict[str, str] values: `values.yaml` to be used
-        :param flags: the flags to be set for `helm template`
-        :type flags: HelmTemplateFlags
+        :type release_name: str
+        :param chart: Helm chart to be templated
+        :type chart: str
+        :param namespace: The Kubernetes namespace the command should execute in
+        :type namespace: str
+        :param values: `values.yaml` to be used
+        :type values: dict
+        :param flags: the flags to be set for `helm template`, defaults to HelmTemplateFlags()
+        :type flags: HelmTemplateFlags, optional
         :return: the output of `helm template`
         :rtype: str
         """
         with tempfile.NamedTemporaryFile("w") as values_file:
             yaml.safe_dump(values, values_file)
             command = [
                 "helm",
                 "template",
                 release_name,
                 chart,
+                "--namespace",
+                namespace,
                 "--values",
                 values_file.name,
             ]
             command = Helm.__enrich_template_command(command, flags)
             return self.__execute(command)
 
     def get_manifest(self, release_name: str, namespace: str) -> Iterable[HelmTemplate]:
@@ -174,14 +188,25 @@
 
         try:
             stdout = self.__execute(command=command)
             return Helm.load_manifest(stdout)
         except ReleaseNotFoundException:
             return ()
 
+    def get_version(self) -> Version:
+        command = ["helm", "version", "--short"]
+        short_version = self.__execute(command)
+        version_match = re.search(r"^v(\d+(?:\.\d+){0,2})", short_version)
+        if version_match is None:
+            raise RuntimeError(
+                f"Could not parse the Helm version.\n\nHelm output:\n{short_version}"
+            )
+        version = map(int, version_match.group(1).split("."))
+        return Version(*version)
+
     @staticmethod
     def load_manifest(yaml_contents: str) -> Iterator[HelmTemplate]:
         is_beginning: bool = False
         template_name = None
         current_yaml_doc: list[str] = []
         for line in YamlReader(yaml_contents):
             if line.startswith("---"):
```

### Comparing `kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.2.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.2.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,30 @@
 from pydantic import BaseModel, Field
 
 from kpops.utils.docstring import describe_attr
 from kpops.utils.pydantic import CamelCaseConfig, DescConfig
 
 
 class HelmDiffConfig(BaseModel):
-    enable: bool = Field(
-        default=True,
-        description="Enable Helm Diff.",
-    )
     ignore: set[str] = Field(
         default_factory=set,
         description="Set of keys that should not be checked.",
         example="- name\n- imageTag",
     )
 
 
 class RepoAuthFlags(BaseModel):
     """Authorisation-related flags for `helm repo`
 
     :param username: Username, defaults to None
-    :type username: str, None, optional
+    :type username: str, optional
     :param password: Password, defaults to None
-    :type password: str, None, optional
+    :type password: str, optional
     :param ca_file: Certificate file, defaults to None
-    :type ca_file: Path, None, optional
+    :type ca_file: Path, optional
     :param insecure_skip_tls_verify: If true, Kubernetes API server's certificate will not be checked for validity
         , defaults to False
     :type insecure_skip_tls_verify: bool, optional
     """
 
     username: str | None = Field(
         default=None, description=describe_attr("username", __doc__)
@@ -147,7 +143,14 @@
         if HELM_NOTES in self.content:
             end = self.content.index(HELM_NOTES)
         else:
             end = -1
         self.content = self.content[start:end]
         yield from self.content.splitlines()
         yield "---"  # add final divider to make parsing easier
+
+
+@dataclass
+class Version:
+    major: int
+    minor: int = 0
+    patch: int = 0
```

### Comparing `kpops-1.1.5/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.2.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.2.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.2.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     ConnectorStateException,
 )
 from kpops.component_handlers.kafka_connect.model import KafkaConnectConfig
 from kpops.component_handlers.kafka_connect.timeout import timeout
 from kpops.utils.colorify import magentaify
 from kpops.utils.dict_differ import render_diff
 
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
 if TYPE_CHECKING:
     from kpops.cli.pipeline_config import PipelineConfig
 
 log = logging.getLogger("KafkaConnectHandler")
 
 
 class KafkaConnectHandler:
@@ -139,14 +144,12 @@
             log.debug(f"HOST: {self._connect_wrapper.host}")
         except ConnectorNotFoundException:
             log.warning(
                 f"Connector Destruction: connector {connector_name} does not exist and cannot be deleted. Skipping."
             )
 
     @classmethod
-    def from_pipeline_config(
-        cls, pipeline_config: PipelineConfig
-    ) -> KafkaConnectHandler:  # TODO: annotate as typing.Self once mypy supports it
+    def from_pipeline_config(cls, pipeline_config: PipelineConfig) -> Self:
         return cls(
             connect_wrapper=ConnectWrapper(host=pipeline_config.kafka_connect_host),
             timeout=pipeline_config.timeout,
         )
```

### Comparing `kpops-1.1.5/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.2.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Settings specific to Kafka Connectors"""
 
     class Config(DescConfig):
         extra = Extra.allow
 
         @override
         @staticmethod
-        def schema_extra(schema: dict[str, Any], model: type[BaseModel]) -> None:  # type: ignore[override]
+        def schema_extra(schema: dict[str, Any], model: type[BaseModel]) -> None:
             schema["description"] = describe_object(model.__doc__)
             schema["additionalProperties"] = {"type": "string"}
 
 
 class ConnectorTask(BaseModel):
     connector: str
     task: int
```

### Comparing `kpops-1.1.5/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.2.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.2.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import logging
 from functools import cached_property
 
 from schema_registry.client import SchemaRegistryClient
+from schema_registry.client.schema import AvroSchema
 
 from kpops.cli.exception import ClassNotFoundError
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.cli.registry import find_class
 from kpops.component_handlers.schema_handler.schema_provider import (
     Schema,
     SchemaProvider,
@@ -27,16 +28,16 @@
     @cached_property
     def schema_provider(self) -> SchemaProvider:
         try:
             if not self.components_module:
                 raise ValueError(
                     f"The Schema Registry URL is set but you haven't specified the component module path. Please provide a valid component module path where your {SchemaProvider.__name__} implementation exists."
                 )
-            schema_provider_class = find_class(self.components_module, SchemaProvider)  # type: ignore[type-abstract]
-            return schema_provider_class()
+            schema_provider_class = find_class(self.components_module, SchemaProvider)
+            return schema_provider_class()  # pyright: ignore[reportGeneralTypeIssues]
         except ClassNotFoundError:
             raise ValueError(
                 f"No schema provider found in components module {self.components_module}. "
                 f"Please implement the abstract method in {SchemaProvider.__module__}.{SchemaProvider.__name__}."
             )
 
     @classmethod
@@ -134,16 +135,21 @@
         self, schema: Schema, schema_class: str, subject: str
     ) -> None:
         registered_version = self.schema_registry_client.check_version(subject, schema)
         if registered_version is None:
             if not self.schema_registry_client.test_compatibility(
                 subject=subject, schema=schema
             ):
+                schema_str = (
+                    schema.flat_schema
+                    if isinstance(schema, AvroSchema)
+                    else str(schema)
+                )
                 raise Exception(
-                    f"Schema is not compatible for {subject} and model {schema_class}. \n {json.dumps(schema.flat_schema, indent=4)}"
+                    f"Schema is not compatible for {subject} and model {schema_class}. \n {json.dumps(schema_str, indent=4)}"
                 )
         else:
             log.debug(
                 f"Schema Submission: schema was already submitted for the subject {subject} as version {registered_version.schema}. Therefore, the specified schema must be compatible."
             )
 
         log.info(
```

### Comparing `kpops-1.1.5/kpops/component_handlers/topic/handler.py` & `kpops-1.2.0/kpops/component_handlers/topic/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 
 
 class TopicHandler:
     def __init__(self, proxy_wrapper: ProxyWrapper):
         self.proxy_wrapper = proxy_wrapper
 
     def create_topics(self, to_section: ToSection, dry_run: bool) -> None:
-        topics: dict[str, TopicConfig] = to_section.topics
-        for topic_name, topic_config in topics.items():
+        for topic_name, topic_config in to_section.topics.items():
             topic_spec = self.__prepare_body(topic_name, topic_config)
             if dry_run:
                 self.__dry_run_topic_creation(topic_name, topic_spec, topic_config)
             else:
                 try:
                     self.proxy_wrapper.get_topic(topic_name=topic_name)
                     topic_config_in_cluster = self.proxy_wrapper.get_topic_config(
@@ -62,16 +61,15 @@
                         log.info(
                             f"Topic Creation: config of topic {topic_name} didn't change. Skipping update."
                         )
                 except TopicNotFoundException:
                     self.proxy_wrapper.create_topic(topic_spec=topic_spec)
 
     def delete_topics(self, to_section: ToSection, dry_run: bool) -> None:
-        topics: dict[str, TopicConfig] = to_section.topics
-        for topic_name in topics.keys():
+        for topic_name in to_section.topics.keys():
             if dry_run:
                 self.__dry_run_topic_deletion(topic_name=topic_name)
             else:
                 try:
                     self.proxy_wrapper.get_topic(topic_name=topic_name)
                     self.proxy_wrapper.delete_topic(topic_name=topic_name)
                 except TopicNotFoundException:
```

### Comparing `kpops-1.1.5/kpops/component_handlers/topic/model.py` & `kpops-1.2.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.2.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/topic/utils.py` & `kpops-1.2.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/component_handlers/utils/exception.py` & `kpops-1.2.0/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/components/base_components/base_defaults_component.py` & `kpops-1.2.0/kpops/components/base_components/base_defaults_component.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import inspect
 import logging
 from collections import deque
-from collections.abc import Mapping, Sequence
+from collections.abc import Sequence
 from pathlib import Path
 from typing import TypeVar
 
 import typer
 from pydantic import BaseModel, Field
 
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.component_handlers import ComponentHandlers
+from kpops.utils.dict_ops import update_nested
 from kpops.utils.docstring import describe_attr
 from kpops.utils.environment import ENV
 from kpops.utils.pydantic import DescConfig
 from kpops.utils.yaml_loading import load_yaml_file
 
 log = logging.getLogger("PipelineComponentEnricher")
 
@@ -204,47 +205,7 @@
 
     :param seq: Sequence to be 'cleaned'
     :type seq: Sequence[T]
     :returns: Cleaned sequence in the form of a list
     :rtype: list[T]
     """
     return list(dict.fromkeys(seq))
-
-
-def update_nested_pair(original_dict: dict, other_dict: Mapping) -> dict:
-    """Nested update for 2 dictionaries
-
-    :param original_dict: Dictionary to be updated
-    :type original_dict: dict
-    :param other_dict: Mapping that contains new or updated key-value pairs
-    :type other_dict: Mapping
-    :return: Updated dictionary
-    :rtype: dict
-    """
-    for key, value in other_dict.items():
-        if isinstance(value, Mapping):
-            nested_val = original_dict.get(key, {})
-            if nested_val is not None:
-                original_dict[key] = update_nested_pair(nested_val, value)
-        else:
-            if key not in original_dict:
-                original_dict[key] = value
-    return original_dict
-
-
-def update_nested(*argv: dict) -> dict:
-    """Merge multiple configuration dicts.
-
-    The dicts have multiple layers. These layers will be merged recursively.
-
-    :param argv: n dictionaries
-    :type argv: dict
-    :returns: Merged configuration dict
-    :rtype: dict
-    """
-    if len(argv) == 0:
-        return {}
-    if len(argv) == 1:
-        return argv[0]
-    if len(argv) == 2:
-        return update_nested_pair(argv[0], argv[1])
-    return update_nested(update_nested_pair(argv[0], argv[1]), *argv[2:])
```

### Comparing `kpops-1.1.5/kpops/components/base_components/kafka_app.py` & `kpops-1.2.0/kpops/components/base_components/kafka_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 
 import logging
 from typing import Literal
 
 from pydantic import BaseModel, Extra, Field
 from typing_extensions import override
 
-from kpops.component_handlers.helm_wrapper.helm import Helm
 from kpops.component_handlers.helm_wrapper.model import (
     HelmRepoConfig,
     HelmUpgradeInstallFlags,
 )
 from kpops.component_handlers.helm_wrapper.utils import trim_release_name
 from kpops.components.base_components.kubernetes_app import (
     KubernetesApp,
     KubernetesAppConfig,
 )
 from kpops.utils.docstring import describe_attr, describe_object
 from kpops.utils.pydantic import CamelCaseConfig, DescConfig
-from kpops.utils.yaml_loading import substitute
 
 log = logging.getLogger("KafkaApp")
 
 
 class KafkaStreamsConfig(BaseModel):
     """Kafka Streams config
 
     :param brokers: Brokers
     :type brokers: str
     :param schema_registry_url: URL of the schema registry, defaults to None
-    :type schema_registry_url: str, None, optional
+    :type schema_registry_url: str, optional
     """
 
     brokers: str = Field(default=..., description=describe_attr("brokers", __doc__))
     schema_registry_url: str | None = Field(
         default=None, description=describe_attr("schema_registry_url", __doc__)
     )
 
@@ -43,15 +41,15 @@
 
 class KafkaAppConfig(KubernetesAppConfig):
     """Settings specific to Kafka Apps
 
     :param streams: Kafka streams config
     :type streams: KafkaStreamsConfig
     :param name_override: Override name with this value, defaults to None
-    :type name_override: str, None, optional
+    :type name_override: str, optional
     """
 
     streams: KafkaStreamsConfig = Field(
         default=..., description=describe_attr("streams", __doc__)
     )
     name_override: str | None = Field(
         default=None, description=describe_attr("name_override", __doc__)
@@ -69,21 +67,21 @@
         defaults to "kafka-app"
     :type schema_type: Literal["kafka-app"], optional
     :param app: Application-specific settings
     :type app: KafkaAppConfig
     :param repo_config: Configuration of the Helm chart repo to be used for
         deploying the component,
         defaults to HelmRepoConfig(repository_name="bakdata-streams-bootstrap", url="https://bakdata.github.io/streams-bootstrap/")
-    :type repo_config: HelmRepoConfig, None, optional
+    :type repo_config: HelmRepoConfig, optional
     :param version: Helm chart version, defaults to "2.9.0"
     :type version: str, optional
     """
 
     type: str = Field(default="kafka-app", description="Component type")
-    schema_type: Literal["kafka-app"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["kafka-app"] = Field(
         default="kafka-app",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     app: KafkaAppConfig = Field(
         default=...,
@@ -92,30 +90,19 @@
     repo_config: HelmRepoConfig = Field(
         default=HelmRepoConfig(
             repository_name="bakdata-streams-bootstrap",
             url="https://bakdata.github.io/streams-bootstrap/",
         ),
         description=describe_attr("repo_config", __doc__),
     )
-    version = Field(
+    version: str | None = Field(
         default="2.9.0",
         description=describe_attr("version", __doc__),
     )
 
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
-        self.app.streams.brokers = substitute(
-            self.app.streams.brokers, {"broker": self.config.broker}
-        )
-        if self.app.streams.schema_registry_url:
-            self.app.streams.schema_registry_url = substitute(
-                self.app.streams.schema_registry_url,
-                {"schema_registry_url": self.config.schema_registry_url},
-            )
-
     @property
     def clean_up_helm_chart(self) -> str:
         """Helm chart used to destroy and clean this component"""
         raise NotImplementedError()
 
     @override
     def deploy(self, dry_run: bool) -> None:
@@ -156,20 +143,16 @@
 
         log.info(f"Init cleanup job for {clean_up_release_name}")
 
         stdout = self.__install_clean_up_job(
             clean_up_release_name, suffix, values, dry_run
         )
 
-        if dry_run and self.helm_diff.config.enable:
-            current_release = self.helm.get_manifest(
-                clean_up_release_name, self.namespace
-            )
-            new_release = Helm.load_manifest(stdout)
-            self.helm_diff.log_helm_diff(log, current_release, new_release)
+        if dry_run:
+            self.dry_run_handler.print_helm_diff(stdout, clean_up_release_name, log)
 
         if not retain_clean_jobs:
             log.info(f"Uninstall cleanup job for {clean_up_release_name}")
             self.__uninstall_clean_up_job(clean_up_release_name, dry_run)
 
     def __uninstall_clean_up_job(self, release_name: str, dry_run: bool) -> None:
         """Uninstall clean up job
```

### Comparing `kpops-1.1.5/kpops/components/base_components/kafka_connector.py` & `kpops-1.2.0/kpops/components/base_components/kafka_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-import json
 import logging
 from abc import ABC
 from functools import cached_property
 from typing import Literal, NoReturn
 
 from pydantic import Field
 from typing_extensions import override
 
+from kpops.component_handlers.helm_wrapper.dry_run_handler import DryRunHandler
 from kpops.component_handlers.helm_wrapper.helm import Helm
 from kpops.component_handlers.helm_wrapper.helm_diff import HelmDiff
 from kpops.component_handlers.helm_wrapper.model import (
     HelmRepoConfig,
     HelmTemplateFlags,
     HelmUpgradeInstallFlags,
 )
@@ -44,26 +44,26 @@
         defaults to "kafka-connector"
     :type schema_type: Literal["kafka-connector"], optional
     :param app: Application-specific settings
     :type app: KafkaAppConfig
     :param repo_config: Configuration of the Helm chart repo to be used for
         deploying the component,
         defaults to HelmRepoConfig(repository_name="bakdata-kafka-connect-resetter", url="https://bakdata.github.io/kafka-connect-resetter/")
-    :type repo_config: HelmRepoConfig, None, optional
+    :type repo_config: HelmRepoConfig, optional
     :param namespace: Namespace in which the component shall be deployed
     :type namespace: str
     :param version: Helm chart version, defaults to "1.0.4"
     :type version: str, optional
     :param resetter_values: Overriding Kafka Connect Resetter Helm values. E.g. to override the Image Tag etc.,
         defaults to dict
     :type resetter_values: dict, optional
     """
 
     type: str = Field(default="kafka-connector", description="Component type")
-    schema_type: Literal["kafka-connector"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["kafka-connector"] = Field(
         default="kafka-connector",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     app: KafkaConnectConfig = Field(
         default=...,
@@ -76,27 +76,23 @@
         ),
         description=describe_attr("repo_config", __doc__),
     )
     namespace: str = Field(
         default=...,
         description=describe_attr("namespace", __doc__),
     )
-    version = Field(default="1.0.4", description="Helm chart version")
+    version: str | None = Field(default="1.0.4", description="Helm chart version")
     resetter_values: dict = Field(
         default_factory=dict,
         description=describe_attr("resetter_values", __doc__),
     )
 
     class Config(CamelCaseConfig):
         pass
 
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
-        self.prepare_connector_config()
-
     @cached_property
     def helm(self) -> Helm:
         """Helm object that contains component-specific config such as repo"""
         helm_repo_config = self.repo_config
         helm = Helm(self.config.helm_config)
         helm.add_repo(
             helm_repo_config.repository_name,
@@ -110,31 +106,23 @@
 
         :return: returns the component resetter's helm chart
         :rtype: str
         """
         return f"{self.repo_config.repository_name}/kafka-connect-resetter"
 
     @cached_property
-    def helm_diff(self) -> HelmDiff:
-        """Helm diff object of last and current release of this component"""
-        return HelmDiff(self.config.helm_diff_config)
+    def dry_run_handler(self) -> DryRunHandler:
+        helm_diff = HelmDiff(self.config.helm_diff_config)
+        return DryRunHandler(self.helm, helm_diff, self.namespace)
 
     @property
     def kafka_connect_resetter_chart(self) -> str:
         """Resetter chart for this component"""
         return f"{self.repo_config.repository_name}/kafka-connect-resetter"
 
-    def prepare_connector_config(self) -> None:
-        """Substitute component related variables in config"""
-        substituted_config = self.substitute_component_variables(
-            json.dumps(self.app.dict())
-        )
-        out: dict = json.loads(substituted_config)
-        self.app = KafkaConnectConfig(**out)
-
     @override
     def deploy(self, dry_run: bool) -> None:
         if self.to:
             self.handlers.topic_handler.create_topics(
                 to_section=self.to, dry_run=dry_run
             )
 
@@ -201,18 +189,16 @@
             )
         )
 
         stdout = self.__install_connect_resetter(
             trimmed_name, connector_name, connector_type, dry_run, **kwargs
         )
 
-        if dry_run and self.helm_diff.config.enable:
-            current_release = self.helm.get_manifest(trimmed_name, self.namespace)
-            new_release = Helm.load_manifest(stdout)
-            self.helm_diff.log_helm_diff(log, current_release, new_release)
+        if dry_run:
+            self.dry_run_handler.print_helm_diff(stdout, trimmed_name, log)
 
         if not retain_clean_jobs:
             log.info(magentaify("Connector Cleanup: uninstall Kafka Resetter."))
             self.__uninstall_connect_resetter(trimmed_name, dry_run)
 
     def _get_kafka_resetter_release_name(self, connector_name: str) -> str:
         """Get connector resetter's release name
@@ -316,22 +302,22 @@
     :type type: str, optional
     :param schema_type: Used for schema generation, same as :param:`type`,
         defaults to "kafka-source-connector"
     :type schema_type: Literal["kafka-source-connector"], optional
     :param offset_topic: offset.storage.topic,
         more info: https://kafka.apache.org/documentation/#connect_running,
         defaults to None
-    :type schema_type: str, None
+    :type schema_type: str, optional
     """
 
     type: str = Field(
         default="kafka-source-connector",
         description=describe_attr("type", __doc__),
     )
-    schema_type: Literal["kafka-source-connector"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["kafka-source-connector"] = Field(
         default="kafka-source-connector",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     offset_topic: str | None = Field(
         default=None,
@@ -351,14 +337,15 @@
             self.name,
             KafkaConnectorType.SOURCE,
             offset_topic=self.offset_topic,
         )
         stdout = self.helm.template(
             self._get_kafka_resetter_release_name(self.name),
             self._get_resetter_helm_chart(),
+            self.namespace,
             values,
             flags,
         )
         print(stdout)
 
     @override
     def reset(self, dry_run: bool) -> None:
@@ -394,15 +381,15 @@
     :type schema_type: Literal["kafka-sink-connector"], optional
     """
 
     type: str = Field(
         default="kafka-sink-connector",
         description=describe_attr("type", __doc__),
     )
-    schema_type: Literal["kafka-sink-connector"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["kafka-sink-connector"] = Field(
         default="kafka-sink-connector",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
 
     @override
@@ -419,14 +406,15 @@
         flags = HelmTemplateFlags(api_version, ca_file, cert_file, self.version)
         values = self._get_kafka_connect_resetter_values(
             self.name, KafkaConnectorType.SINK
         )
         stdout = self.helm.template(
             self._get_kafka_resetter_release_name(self.name),
             self._get_resetter_helm_chart(),
+            self.namespace,
             values,
             flags,
         )
         print(stdout)
 
     @override
     def set_input_pattern(self, name: str) -> None:
```

### Comparing `kpops-1.1.5/kpops/components/base_components/kubernetes_app.py` & `kpops-1.2.0/kpops/components/base_components/kubernetes_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 from functools import cached_property
 from typing import Any, Literal
 
 from pydantic import BaseModel, Extra, Field
 from typing_extensions import override
 
+from kpops.component_handlers.helm_wrapper.dry_run_handler import DryRunHandler
 from kpops.component_handlers.helm_wrapper.helm import Helm
 from kpops.component_handlers.helm_wrapper.helm_diff import HelmDiff
 from kpops.component_handlers.helm_wrapper.model import (
     HelmRepoConfig,
     HelmTemplateFlags,
     HelmUpgradeInstallFlags,
 )
@@ -30,46 +31,47 @@
 class KubernetesAppConfig(BaseModel):
     """Settings specific to Kubernetes Apps"""
 
     class Config(CamelCaseConfig, DescConfig):
         extra = Extra.allow
 
 
-# TODO: label and annotations
 class KubernetesApp(PipelineComponent):
     """Base class for all Kubernetes apps.
 
     All built-in components are Kubernetes apps, except for the Kafka connectors.
 
     :param type: Component type, defaults to "kubernetes-app"
-    :type type: str, optional
     :param schema_type: Used for schema generation, same as :param:`type`,
         defaults to "kubernetes-app"
-    :type schema_type: Literal["kubernetes-app"], optional
+    :param validate_name: Whether to check if the name of the component is
+        compatible with Kubernetes, defaults to True
     :param app: Application-specific settings
-    :type app: KubernetesAppConfig
     :param repo_config: Configuration of the Helm chart repo to be used for
         deploying the component, defaults to None
-    :type repo_config: HelmRepoConfig, None, optional
     :param namespace: Namespace in which the component shall be deployed
-    :type namespace: str
     :param version: Helm chart version, defaults to None
-    :type version: str, None, optional
     """
 
     type: str = Field(
         default="kubernetes-app",
         description=describe_attr("type", __doc__),
     )
-    schema_type: Literal["kubernetes-app"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["kubernetes-app"] = Field(
         default="kubernetes-app",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
+    validate_name: bool = Field(
+        default=True,
+        description=describe_attr("validate_name", __doc__),
+        exclude=True,
+        hidden_from_schema=True,
+    )
     app: KubernetesAppConfig = Field(
         default=...,
         description=describe_attr("app", __doc__),
     )
     repo_config: HelmRepoConfig | None = Field(
         default=None,
         description=describe_attr("repo_config", __doc__),
@@ -83,16 +85,17 @@
         description=describe_attr("version", __doc__),
     )
 
     class Config(CamelCaseConfig, DescConfig):
         pass
 
     def __init__(self, **kwargs):
+        if kwargs.get("validate_name", True):
+            self.validate_kubernetes_name(kwargs["name"])
         super().__init__(**kwargs)
-        self.__check_compatible_name()
 
     @cached_property
     def helm(self) -> Helm:
         """Helm object that contains component-specific config such as repo"""
         helm = Helm(self.config.helm_config)
         if self.repo_config is not None:
             helm.add_repo(
@@ -103,26 +106,35 @@
         return helm
 
     @cached_property
     def helm_diff(self) -> HelmDiff:
         """Helm diff object of last and current release of this component"""
         return HelmDiff(self.config.helm_diff_config)
 
+    @cached_property
+    def dry_run_handler(self) -> DryRunHandler:
+        helm_diff = HelmDiff(self.config.helm_diff_config)
+        return DryRunHandler(self.helm, helm_diff, self.namespace)
+
     @property
     def helm_release_name(self) -> str:
         """The name for the Helm release. Can be overridden."""
         return self.name
 
     @override
     def template(
         self, api_version: str | None, ca_file: str | None, cert_file: str | None
     ) -> None:
         flags = HelmTemplateFlags(api_version, ca_file, cert_file, self.version)
         stdout = self.helm.template(
-            self.helm_release_name, self.get_helm_chart(), self.to_helm_values(), flags
+            self.helm_release_name,
+            self.get_helm_chart(),
+            self.namespace,
+            self.to_helm_values(),
+            flags,
         )
         print(stdout)
 
     @override
     def deploy(self, dry_run: bool) -> None:
         stdout = self.helm.upgrade_install(
             self.helm_release_name,
@@ -130,16 +142,16 @@
             dry_run,
             self.namespace,
             self.to_helm_values(),
             HelmUpgradeInstallFlags(
                 create_namespace=self.config.create_namespace, version=self.version
             ),
         )
-        if dry_run and self.helm_diff.config.enable:
-            self.print_helm_diff(stdout)
+        if dry_run:
+            self.dry_run_handler.print_helm_diff(stdout, self.helm_release_name, log)
 
     @override
     def destroy(self, dry_run: bool) -> None:
         stdout = self.helm.uninstall(
             self.namespace,
             self.helm_release_name,
             dry_run,
@@ -178,20 +190,23 @@
         :return: Helm chart of this component
         :rtype: str
         """
         raise NotImplementedError(
             f"Please implement the get_helm_chart() method of the {self.__module__} module."
         )
 
-    def __check_compatible_name(self) -> None:
-        """Check if the component's name `self.name` is valid for Kubernetes"""
-        if not bool(KUBERNETES_NAME_CHECK_PATTERN.match(self.name)):  # TODO: SMARTER
-            raise ValueError(
-                f"The component name {self.name} is invalid for Kubernetes."
-            )
+    @staticmethod
+    def validate_kubernetes_name(name: str) -> None:
+        """Check if a name is valid for a Kubernetes resource
+
+        :param name: Name that is to be used for the resource
+        :raises ValueError: The component name {name} is invalid for Kubernetes.
+        """
+        if not bool(KUBERNETES_NAME_CHECK_PATTERN.match(name)):
+            raise ValueError(f"The component name {name} is invalid for Kubernetes.")
 
     @override
     def dict(self, *, exclude=None, **kwargs) -> dict[str, Any]:
         # HACK: workaround for Pydantic to exclude cached properties during model export
         if exclude is None:
             exclude = set()
         exclude.add("helm")
```

### Comparing `kpops-1.1.5/kpops/components/base_components/models/from_section.py` & `kpops-1.2.0/kpops/components/base_components/models/from_section.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import NewType
 
 from pydantic import BaseModel, Extra, Field, root_validator
 
+from kpops.components.base_components.models import TopicName
 from kpops.utils.docstring import describe_attr
 from kpops.utils.pydantic import DescConfig
 
 
 class InputTopicTypes(str, Enum):
     """Input topic types
 
@@ -50,15 +51,14 @@
         if not is_extra_topic and values.get("role"):
             raise ValueError(
                 "If you do not define an input component, input topic, or input pattern, the role is unnecessary."
             )
         return values
 
 
-TopicName = NewType("TopicName", str)
 ComponentName = NewType("ComponentName", str)
 
 
 class FromSection(BaseModel):
     """Holds multiple input topics
 
     :param topics: Input topics
```

### Comparing `kpops-1.1.5/kpops/components/base_components/models/to_section.py` & `kpops-1.2.0/kpops/components/base_components/models/to_section.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Any
 
 from pydantic import BaseModel, Extra, Field, root_validator
 
+from kpops.components.base_components.models import TopicName
 from kpops.utils.docstring import describe_attr
 from kpops.utils.pydantic import DescConfig
 
 
 class OutputTopicTypes(str, Enum):
     """Types of output topic
 
@@ -85,13 +86,13 @@
     """
 
     # TODO: really multiple models?
     # any because snapshot versions must be supported
     models: dict[str, Any] = Field(
         default={}, description=describe_attr("models", __doc__)
     )
-    topics: dict[str, TopicConfig] = Field(
+    topics: dict[TopicName, TopicConfig] = Field(
         ..., description=describe_attr("topics", __doc__)
     )
 
     class Config(DescConfig):
         extra = Extra.allow
```

### Comparing `kpops-1.1.5/kpops/components/base_components/pipeline_component.py` & `kpops-1.2.0/kpops/components/base_components/pipeline_component.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,44 +15,42 @@
 )
 from kpops.components.base_components.models.to_section import (
     OutputTopicTypes,
     TopicConfig,
     ToSection,
 )
 from kpops.utils.docstring import describe_attr, describe_object
-from kpops.utils.environment import ENV
 from kpops.utils.pydantic import CamelCaseConfig, DescConfig
-from kpops.utils.yaml_loading import substitute
 
 
 class PipelineComponent(BaseDefaultsComponent):
     """Base class for all components
 
     :param name: Component name
     :type name: str
     :param from_: Topic(s) and/or components from which the component will read
         input, defaults to None
-    :type from_: FromSection, None, optional
+    :type from_: FromSection, optional
     :param app: Application-specific settings, defaults to None
-    :type app: object, None, optional
+    :type app: object, optional
     :param to: Topic(s) into which the component will write output,
         defaults to None
-    :type to: ToSection, None, optional
+    :type to: ToSection, optional
     :param prefix: Pipeline prefix that will prefix every component name.
         If you wish to not have any prefix you can specify an empty string.,
         defaults to "${pipeline_name}-"
     :type prefix: str, optional
     """
 
     type: str = Field(
         default="pipeline-component",
         description=describe_attr("type", __doc__),
         const=True,
     )
-    schema_type: Literal["pipeline-component"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["pipeline-component"] = Field(
         default="pipeline-component",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     name: str = Field(default=..., description="Component name")
     from_: FromSection | None = Field(
@@ -74,69 +72,19 @@
         description=describe_attr("prefix", __doc__),
     )
 
     class Config(CamelCaseConfig, DescConfig):
         extra = Extra.allow
         keep_untouched = (cached_property,)
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
-        self.substitute_output_topic_names()
-        self.substitute_name()
-        self.substitute_prefix()
         self.set_input_topics()
         self.set_output_topics()
 
-    def substitute_output_topic_names(self) -> None:
-        """Substitute component and topic sepcific names in output topics"""
-        if self.to:
-            updated_to = {}
-            for name, topic in self.to.topics.items():
-                name = self.substitute_component_variables(name)
-                updated_to[name] = topic
-            self.to.topics = updated_to
-
-    @staticmethod
-    def substitute_component_names(key: str, _type: str, **kwargs) -> str:
-        """Substitute component field name, e.g., `error_topic_name`
-
-        :param key: The raw input containing $-placeholders
-        :type key: str
-        :param _type: The key-value mapping containing substitutions
-        :type _type: str
-        :param **kwargs: Additional key-value mappings that contain substitutions
-        :return: Substituted input string
-        :rtype: str
-        """
-        return substitute(key, {"component_type": _type, **kwargs})
-
-    def substitute_component_variables(self, topic_name: str) -> str:
-        """Substitute component, env and topic-specific variables in topic's name
-
-        :param topic_name: topic name
-        :return: final topic name
-        """
-        error_topic_name = self.substitute_component_names(
-            self.config.topic_name_config.default_error_topic_name,
-            self.type,
-            **ENV,
-        )
-        output_topic_name = self.substitute_component_names(
-            self.config.topic_name_config.default_output_topic_name,
-            self.type,
-            **ENV,
-        )
-        return self.substitute_component_names(
-            topic_name,
-            self.type,
-            component_name=self.name,
-            error_topic_name=error_topic_name,
-            output_topic_name=output_topic_name,
-        )
-
     def add_input_topics(self, topics: list[str]) -> None:
         """Add given topics to the list of input topics.
 
         :param topics: Input topics
         :type topics: list[str]
         """
 
@@ -255,23 +203,16 @@
             topic_name
             for topic_name, topic_config in to.topics.items()
             if topic_config.type == OutputTopicTypes.OUTPUT
         ]
         for input_topic in input_topics:
             self.apply_from_inputs(input_topic, from_topic)
 
-    def substitute_name(self) -> None:
-        """Substitute $ placeholders in `self.name` with `self.type`"""
-        if self.name:
-            self.name = self.substitute_component_names(self.name, self.type)
-        else:
-            raise ValueError("Every component must have a name in the end.")
-
     def inflate(self) -> list[PipelineComponent]:
-        """Inflate a component.
+        """Inflate a component
 
         This is helpful if one component should result in multiple components.
         To support this, override this method and return a list of components
         the component you result in. The order of the components is the order
         the components will be deployed in.
         """
         return [self]
@@ -285,21 +226,21 @@
         From HELM: Render chart templates locally and display the output.
         Any values that would normally be looked up or retrieved in-cluster will
         be faked locally. Additionally, none of the server-side testing of chart
         validity (e.g. whether an API is supported) is done.
 
         :param api_version: Kubernetes API version used for
             Capabilities.APIVersions, `--api_versions` in Helm
-        :type api_version: str, None
+        :type api_version: str, optional
         :param ca_file: verify certificates of HTTPS-enabled servers using this
             CA bundle, `--ca-file` in Helm
-        :type ca_file: str, None
+        :type ca_file: str, optional
         :param cert_file: identify HTTPS client using this SSL certificate file,
             `--cert-file` in Helm
-        :type cert_file: str, None
+        :type cert_file: str, optional
         """
 
     def deploy(self, dry_run: bool) -> None:
         """Deploy the component (self) to the k8s cluster
 
         :param dry_run: Whether to do a dry run of the command
         :type dry_run: bool
@@ -321,11 +262,7 @@
 
     def clean(self, dry_run: bool) -> None:
         """Remove component (self) and any trace of it
 
         :param dry_run: Whether to do a dry run of the command
         :type dry_run: bool
         """
-
-    def substitute_prefix(self) -> None:
-        """Substitute $-placeholders in self.prefix with environment variables"""
-        self.prefix = substitute(self.prefix, ENV)
```

### Comparing `kpops-1.1.5/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.2.0/kpops/components/streams_bootstrap/producer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class ProducerStreamsConfig(KafkaStreamsConfig):
     """Kafka Streams settings specific to Producer
 
     :param extra_output_topics: Extra output topics
     :type extra_output_topics: dict[str, str], optional
     :param output_topic: Output topic, defaults to None
-    :type output_topic: str, None, optional
+    :type output_topic: str, optional
     """
 
     extra_output_topics: dict[str, str] = Field(
         default={}, description=describe_attr("extra_output_topics", __doc__)
     )
     output_topic: str | None = Field(
         default=None, description=describe_attr("output_topic", __doc__)
```

### Comparing `kpops-1.1.5/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.2.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     :param app: Application-specific settings
     :type app: ProducerValues
     :param from_: Producer doesn't support FromSection, defaults to None
     :type from_: None, optional
     """
 
     type: str = Field(default="producer", description="Component type")
-    schema_type: Literal["producer"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["producer"] = Field(
         default="producer",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     app: ProducerValues = Field(
         default=...,
```

### Comparing `kpops-1.1.5/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.2.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 class StreamsConfig(KafkaStreamsConfig):
     """Streams Bootstrap streams section
 
     :param input_topics: Input topics, defaults to []
     :type input_topics: list[str], optional
     :param input_pattern: Input pattern, defaults to None
-    :type input_pattern: str, None, optional
+    :type input_pattern: str, optional
     :param extra_input_topics: Extra input topics, defaults to {}
     :type extra_input_topics: dict[str, list[str]], optional
     :param extra_input_patterns: Extra input patterns, defaults to {}
     :type extra_input_patterns: dict[str, str], optional
     :param extra_output_topics: Extra output topics, defaults to {}
     :type extra_output_topics: dict[str, str], optional
     :param output_topic: Output topic, defaults to None
-    :type output_topic: str, None, optional
+    :type output_topic: str, optional
     :param error_topic: Error topic, defaults to None
-    :type error_topic: str, None, optional
+    :type error_topic: str, optional
     :param config: Configuration, defaults to {}
     :type config: dict[str, str], optional
     """
 
     input_topics: list[str] = Field(
         default=[], description=describe_attr("input_topics", __doc__)
     )
@@ -153,15 +153,15 @@
         https://keda.sh/docs/2.9/concepts/scaling-deployments/#maxreplicacount,
         defaults to 1
     :type max_replicas: int, optional
     :param idle_replicas: If this property is set, KEDA will scale the resource
         down to this number of replicas.
         https://keda.sh/docs/2.9/concepts/scaling-deployments/#idlereplicacount,
         defaults to None
-    :type idle_replicas: int, None, optional
+    :type idle_replicas: int, optional
     :param topics: List of auto-generated Kafka Streams topics used by the streams app.,
         defaults to []
     :type topics: list[str]
     """
 
     enabled: bool = Field(
         default=False,
@@ -218,15 +218,15 @@
     """StreamsBoostrap app configurations.
 
     The attributes correspond to keys and values that are used as values for the streams bootstrap helm chart.
 
     :params streams: Streams Bootstrap streams section
     :type streams: StreamsConfig
     :params autoscaling:Kubernetes Event-driven Autoscaling config, defaults to None
-    :type autoscaling:StreamsAppAutoScaling, None, optional
+    :type autoscaling:StreamsAppAutoScaling, optional
     """
 
     streams: StreamsConfig = Field(
         default=...,
         description=describe_attr("streams", __doc__),
     )
     autoscaling: StreamsAppAutoScaling | None = Field(
```

### Comparing `kpops-1.1.5/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.2.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,32 +24,28 @@
     :type app: StreamsAppConfig
     """
 
     type: str = Field(
         default="streams-app",
         description=describe_attr("type", __doc__),
     )
-    schema_type: Literal["streams-app"] = Field(  # type: ignore[assignment]
+    schema_type: Literal["streams-app"] = Field(
         default="streams-app",
         title="Component type",
         description=describe_object(__doc__),
         exclude=True,
     )
     app: StreamsAppConfig = Field(
         default=...,
         description=describe_attr("app", __doc__),
     )
 
     class Config(DescConfig):
         extra = Extra.allow
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.__substitute_autoscaling_topic_names()
-
     @override
     def add_input_topics(self, topics: list[str]) -> None:
         self.app.streams.add_input_topics(topics)
 
     @override
     def add_extra_input_topic(self, role: str, topics: list[str]) -> None:
         self.app.streams.add_extra_input_topics(role, topics)
@@ -102,19 +98,7 @@
         values = self.to_helm_values()
         values["streams"]["deleteOutput"] = delete_output
         self._run_clean_up_job(
             values=values,
             dry_run=dry_run,
             retain_clean_jobs=self.config.retain_clean_jobs,
         )
-
-    def __substitute_autoscaling_topic_names(self) -> None:
-        """Substitute autoscaling topics' names"""
-        if not self.app.autoscaling:
-            return
-        self.app.autoscaling.topics = [
-            self.substitute_component_variables(topic)
-            for topic in self.app.autoscaling.topics
-        ]
-        self.app.autoscaling.consumer_group = self.substitute_component_variables(
-            self.app.autoscaling.consumer_group
-        )
```

### Comparing `kpops-1.1.5/kpops/pipeline_generator/pipeline.py` & `kpops-1.2.0/kpops/pipeline_generator/pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 from pydantic import BaseModel
 from rich.console import Console
 from rich.syntax import Syntax
 
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.cli.registry import Registry
 from kpops.component_handlers import ComponentHandlers
-from kpops.components.base_components.base_defaults_component import update_nested_pair
 from kpops.components.base_components.pipeline_component import PipelineComponent
+from kpops.utils.dict_ops import generate_substitution, update_nested_pair
 from kpops.utils.environment import ENV
-from kpops.utils.yaml_loading import load_yaml_file, substitute
+from kpops.utils.yaml_loading import load_yaml_file, substitute, substitute_nested
 
 log = logging.getLogger("PipelineGenerator")
 
 
 class ParsingException(Exception):
     pass
 
 
 class PipelineComponents(BaseModel):
+    """Stores the pipeline components"""
+
     components: list[PipelineComponent] = []
 
     @property
     def last(self) -> PipelineComponent:
         return self.components[-1]
 
     def find(self, component_name: str) -> PipelineComponent:
@@ -42,15 +44,15 @@
     def add(self, component: PipelineComponent) -> None:
         self._populate_component_name(component)
         self.components.append(component)
 
     def __bool__(self) -> bool:
         return bool(self.components)
 
-    def __iter__(self) -> Iterator[PipelineComponent]:  # type: ignore[override]
+    def __iter__(self) -> Iterator[PipelineComponent]:
         return iter(self.components)
 
     @staticmethod
     def _populate_component_name(component: PipelineComponent) -> None:
         component.name = component.prefix + component.name
         with suppress(
             AttributeError  # Some components like Kafka Connect do not have a name_override attribute
@@ -58,31 +60,28 @@
             if component.app and getattr(component.app, "name_override") is None:
                 setattr(component.app, "name_override", component.name)
 
 
 def create_env_components_index(
     environment_components: list[dict],
 ) -> dict[str, dict]:
-    """
-    Create an index for all registered components in the project
+    """Create an index for all registered components in the project
 
-    :param environment_components: list of components
+    :param environment_components: List of all components to be included
+    :type environment_components: list[dict]
     :return: component index
+    :rtype: dict[str, dict]
     """
-    index = {}
+    index: dict[str, dict] = {}
     for component in environment_components:
         if "type" not in component or "name" not in component:
             raise ValueError(
                 "To override components per environment, every component should at least have a type and a name."
             )
-        index[
-            PipelineComponent.substitute_component_names(
-                component["name"], component["type"], **ENV
-            )
-        ] = component
+        index[component["name"]] = component
     return index
 
 
 class Pipeline:
     def __init__(
         self,
         component_list: list[dict],
@@ -103,34 +102,60 @@
         cls,
         base_dir: Path,
         path: Path,
         registry: Registry,
         config: PipelineConfig,
         handlers: ComponentHandlers,
     ) -> Pipeline:
+        """Load pipeline definition from yaml
+
+        The file is often named ``pipeline.yaml``
+
+        :param base_dir: Base directory to the pipelines (default is current working directory)
+        :type base_dir: Path
+        :param path: Path to pipeline definition yaml file
+        :type path: Path
+        :param registry: Pipeline components registry
+        :type registry: Registry
+        :param config: Pipeline config
+        :type config: PipelineConfig
+        :param handlers: Component handlers
+        :type handlers: ComponentHandlers
+        :raises TypeError: The pipeline definition should contain a list of components
+        :raises TypeError: The env-specific pipeline definition should contain a list of components
+        :returns: Initialized pipeline object
+        :rtype: Pipeline
+        """
         Pipeline.set_pipeline_name_env_vars(base_dir, path)
 
         main_content = load_yaml_file(path, substitution=ENV)
         if not isinstance(main_content, list):
             raise TypeError(
                 f"The pipeline definition {path} should contain a list of components"
             )
-
         env_content = []
         if (env_file := Pipeline.pipeline_filename_environment(path, config)).exists():
             env_content = load_yaml_file(env_file, substitution=ENV)
             if not isinstance(env_content, list):
                 raise TypeError(
                     f"The pipeline definition {env_file} should contain a list of components"
                 )
 
         pipeline = cls(main_content, env_content, registry, config, handlers)
         return pipeline
 
     def parse_components(self, component_list: list[dict]) -> None:
+        """Instantiate, enrich and inflate a list of components
+
+        :param component_list: List of components
+        :type component_list: list[dict]
+        :raises ValueError: Every component must have a type defined
+        :raises ParsingException: Error enriching component
+        :raises ParsingException: All undefined exceptions
+        """
         for component_data in component_list:
             try:
                 try:
                     component_type: str = component_data["type"]
                 except KeyError:
                     raise ValueError(
                         "Every component must have a type defined, this component does not have one."
@@ -144,23 +169,27 @@
                     ) from ex
                 else:
                     raise ParsingException() from ex
 
     def apply_component(
         self, component_class: type[PipelineComponent], component_data: dict
     ) -> None:
-        """Instantiates, enriches and inflates pipeline component.
+        """Instantiate, enrich and inflate pipeline component.
+
         Applies input topics according to FromSection.
 
         :param component_class: Type of pipeline component
+        :type component_class: type[PipelineComponent]
         :param component_data: Arguments for instantiation of pipeline component
+        :type component_data: dict
         """
         component = component_class(
             config=self.config,
             handlers=self.handlers,
+            validate_name=False,
             **component_data,
         )
         component = self.enrich_component(component)
 
         # inflate & enrich components
         for inflated_component in component.inflate():  # TODO: recursively
             enriched_component = self.enrich_component(inflated_component)
@@ -190,34 +219,49 @@
                 enriched_component.weave_from_topics(prev_component.to)
             self.components.add(enriched_component)
 
     def enrich_component(
         self,
         component: PipelineComponent,
     ) -> PipelineComponent:
-        env_component_definition = self.env_components_index.get(component.name, {})
-        pair = update_nested_pair(
-            env_component_definition,
+        """Enrich a pipeline component with env-specific config and substitute variables
+
+        :param component: Component to be enriched
+        :type component: PipelineComponent
+        :returns: Enriched component
+        :rtype: PipelineComponent
+        """
+        env_component_as_dict = update_nested_pair(
+            self.env_components_index.get(component.name, {}),
             # HACK: Pydantic .dict() doesn't create jsonable dict
             json.loads(component.json(by_alias=True)),
         )
+        if "validate_name" in env_component_as_dict:
+            del env_component_as_dict["validate_name"]
 
-        component_data = self.substitute_component_specific_variables(component, pair)
+        component_data = self.substitute_in_component(env_component_as_dict)
 
         component_class = type(component)
         return component_class(
             enrich=False,
             config=self.config,
             handlers=self.handlers,
             **component_data,
         )
 
     def print_yaml(self, substitution: dict | None = None) -> None:
+        """Print the generated pipeline definition
+
+        :param substitution: Substitution dictionary, defaults to None
+        :type substitution: dict | None, optional
+        """
         syntax = Syntax(
-            substitute(str(self), substitution), "yaml", background_color="default"
+            substitute(str(self), substitution),
+            "yaml",
+            background_color="default",
         )
         Console(
             width=1000  # HACK: overwrite console width to avoid truncating output
         ).print(syntax)
 
     def __iter__(self) -> Iterator[PipelineComponent]:
         return iter(self.components)
@@ -225,53 +269,72 @@
     def __str__(self) -> str:
         return yaml.dump(
             json.loads(  # HACK: serialize types on Pydantic model export, which are not serialized by .dict(); e.g. pathlib.Path
                 self.components.json(exclude_none=True, by_alias=True)
             )
         )
 
-    @staticmethod
-    def substitute_component_specific_variables(
-        component: PipelineComponent, pair: dict  # TODO: better parameter name for pair
-    ) -> dict:
-        """Overrides component config with component config in pipeline environment definition."""
-        # HACK: why do we need an intermediate JSON object?
-        component_data: dict = json.loads(
-            substitute(
-                json.dumps(pair),
-                {
-                    "component_type": component.type,
-                    "component_name": component.name,
-                },
+    def substitute_in_component(self, component_as_dict: dict) -> dict:
+        """Substitute all $-placeholders in a component in dict representation
+
+        :param component_as_dict: Component represented as dict
+        :type component_as_dict: dict
+        :return: Updated component
+        :rtype: dict
+        """
+        config = self.config
+        # Leftover variables that were previously introduced in the component by the substitution
+        # functions, still hardcoded, because of their names.
+        # TODO: Get rid of them
+        substitution_hardcoded = {
+            "error_topic_name": config.topic_name_config.default_error_topic_name,
+            "output_topic_name": config.topic_name_config.default_output_topic_name,
+        }
+        component_substitution = generate_substitution(
+            component_as_dict,
+            "component",
+            substitution_hardcoded,
+        )
+        substitution = generate_substitution(
+            json.loads(config.json()), existing_substitution=component_substitution
+        )
+
+        return json.loads(
+            substitute_nested(
+                json.dumps(component_as_dict),
+                **update_nested_pair(substitution, ENV),
             )
         )
-        return component_data
 
     @staticmethod
     def pipeline_filename_environment(path: Path, config: PipelineConfig) -> Path:
-        """
-        Adds the environment name from the PipelineConfig to the pipeline.yaml path
+        """Add the environment name from the PipelineConfig to the pipeline.yaml path
+
         :param path: Path to pipeline.yaml file
         :param config: The PipelineConfig
-        :return: Absolute path to the pipeline_<environment>.yaml
+        :returns: An absolute path to the pipeline_<environment>.yaml
         """
         return path.with_stem(f"{path.stem}_{config.environment}")
 
     @staticmethod
     def set_pipeline_name_env_vars(base_dir: Path, path: Path) -> None:
-        """
-        Sets the environment variable pipeline_name relative to the given base_dir.
+        """Set the environment variable pipeline_name relative to the given base_dir.
+
         Moreover, for each sub-path an environment variable is set.
         For example, for a given path ./data/v1/dev/pipeline.yaml the pipeline_name would be
         set to data-v1-dev. Then the sub environment variables are set:
+
         pipeline_name_0 = data
         pipeline_name_1 = v1
         pipeline_name_2 = dev
+
         :param base_dir: Base directory to the pipeline files
+        :type base_dir: Path
         :param path: Path to pipeline.yaml file
+        :type path: Path
         """
         path_without_file = path.resolve().relative_to(base_dir.resolve()).parts[:-1]
         if not path_without_file:
             raise ValueError("The pipeline-base-dir should not equal the pipeline-path")
         pipeline_name = "-".join(path_without_file)
         ENV["pipeline_name"] = pipeline_name
         for level, parent in enumerate(path_without_file):
```

### Comparing `kpops-1.1.5/kpops/utils/dict_differ.py` & `kpops-1.2.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/utils/docstring.py` & `kpops-1.2.0/kpops/utils/docstring.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """Read attribute description from class docstring
 
     **Works only with reStructuredText docstrings.**
 
     :param name: Attribute name
     :type name: str
     :param docstr: Docstring from which to read. Note that the class' docstring is stored in attr ``__doc__``
-    :type docstr: str, None
+    :type docstr: str, optional
     :returns: Description of the class attribute read from the class docstring
     :rtype: str
     """
     if docstr is None:
         return ""
     docstr = docstr.partition(f":param {name}:")[2]
     return _trim_description_end(docstr)
@@ -25,15 +25,15 @@
     """Return description from an object's docstring
 
     Excludes parameters and return definitions
 
     **Works only with reStructuredText docstrings.**
 
     :param docstr: The docstring
-    :type docstr: str, None
+    :type docstr: str, optional
     :returns: Description taken from the docstring
     :rtype: str
     """
     if docstr is None:
         return ""
 
     # reST docstrings have a short description/title as their first line.
```

### Comparing `kpops-1.1.5/kpops/utils/environment.py` & `kpops-1.2.0/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.5/kpops/utils/gen_schema.py` & `kpops-1.2.0/kpops/utils/gen_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,29 +89,27 @@
     :type components_module: str
     :param components: Tuple of components to which to add, defaults to ()
     :type components: tuple, optional
     :return: Extended tuple
     :rtype: tuple
     """
     if components is None:
-        components = tuple()  # type: ignore[assignment]
-    # HACK: mypy doesn't narrow the tuple's type without this assertion
-    assert components is not None
+        components = tuple()
     # Set of existing types, against which to check the new ones
     defined_component_types: set[str] = {
         component.__fields__["schema_type"].default
         for component in components
         if component.__fields__.get("schema_type")
     }
     custom_components = [
         component
         for component in _find_classes(components_module, PipelineComponent)
         if _is_valid_component(defined_component_types, component)
     ]
-    components += tuple(custom_components)  # type: ignore[assignment]
+    components += tuple(custom_components)
     return components
 
 
 def gen_pipeline_schema(
     components_module: str | None = None, include_stock_components: bool = True
 ) -> None:
     """Generate a json schema from the models of pipeline components.
@@ -130,15 +128,15 @@
     # Add stock components if enabled
     if include_stock_components:
         components = tuple(_find_classes("kpops.components", PipelineComponent))
     else:
         components = tuple()
     # Add custom components if provided
     if components_module:
-        components = _add_components(components_module, components)  # type: ignore[arg-type]
+        components = _add_components(components_module, components)
     # Create a type union that will hold the union of all component types
     PipelineComponents = Union[components]  # type: ignore[valid-type]
 
     AnnotatedPipelineComponents = Annotated[
         PipelineComponents, Field(discriminator="schema_type")
     ]
```

### Comparing `kpops-1.1.5/kpops/utils/pydantic.py` & `kpops-1.2.0/kpops/utils/pydantic.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from kpops.utils.docstring import describe_object
 
 
 def to_camel(field: str) -> str:
     if field == "schema_type":
         return field
-    return humps.camelize(field)  # type: ignore
+    return humps.camelize(field)
 
 
 class CamelCaseConfig(BaseConfig):
     alias_generator = to_camel
     allow_population_by_field_name = True
 
 
 class DescConfig(BaseConfig):
     @staticmethod
-    def schema_extra(schema: dict[str, Any], model: type[BaseModel]) -> None:  # type: ignore[override]
+    def schema_extra(schema: dict[str, Any], model: type[BaseModel]) -> None:
         schema["description"] = describe_object(model.__doc__)
```

### Comparing `kpops-1.1.5/pyproject.toml` & `kpops-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.1.5"
+version = "1.2.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
@@ -24,35 +24,36 @@
 ]
 
 [tool.poetry.scripts]
 kpops = "kpops.cli.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = {extras = ["dotenv"], version = "^1.10.8"}
+pydantic = { extras = ["dotenv"], version = "^1.10.8" }
 rich = "^12.4.4"
 PyYAML = "^6.0"
 requests = "^2.28.0"
 typer = { extras = ["all"], version = "^0.6.1" }
 pyhumps = "^3.7.3"
 cachetools = "^5.2.0"
 dictdiffer = "^0.9.0"
 python-schema-registry-client = "^2.4.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
+pytest-timeout = "^2.1.0"
 snapshottest = "^0.6.0"
 responses = "^0.22.0"
 pre-commit = "^2.19.0"
-mypy = "^0.990"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 isort = "^5.12.0"
 typer-cli = "^0.0.13"
+pyright = "^1.1.314"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-material = "^9.0.0"
```

### Comparing `kpops-1.1.5/PKG-INFO` & `kpops-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.1.5
+Version: 1.2.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
@@ -12,17 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
@@ -51,15 +49,15 @@
 - **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.
 - **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).
 - **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.
 
 ## Documentation
 
 For detailed usage and installation instructions, check out
-the [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).
+the [documentation](https://bakdata.github.io/kpops/latest).
 
 ## Install KPOps
 
 KPOps comes as a [PyPI package](https://pypi.org/project/kpops/). 
 You can install it with [pip](https://github.com/pypa/pip):
 
 ```shell
```

