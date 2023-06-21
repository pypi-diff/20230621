# Comparing `tmp/censys_cloud_connectors-3.1.2.tar.gz` & `tmp/censys_cloud_connectors-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys_cloud_connectors-3.1.2.tar", max compression
+gzip compressed data, was "censys_cloud_connectors-3.1.3.tar", max compression
```

## Comparing `censys_cloud_connectors-3.1.2.tar` & `censys_cloud_connectors-3.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11342 2023-05-10 15:51:44.059371 censys_cloud_connectors-3.1.2/LICENSE
--rw-r--r--   0        0        0     2143 2023-05-10 15:51:44.059371 censys_cloud_connectors-3.1.2/README.md
--rw-r--r--   0        0        0     4562 2023-05-10 15:51:44.072372 censys_cloud_connectors-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      920 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/__init__.py
--rw-r--r--   0        0        0      439 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/__init__.py
--rw-r--r--   0        0        0    28603 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/connector.py
--rw-r--r--   0        0        0     2766 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/enums.py
--rw-r--r--   0        0        0    18732 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/provider_setup.py
--rwxr-xr-x   0        0        0     1240 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/serverless.py
--rw-r--r--   0        0        0     8355 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/service.py
--rw-r--r--   0        0        0     4192 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/settings.py
--rw-r--r--   0        0        0      343 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/__init__.py
--rw-r--r--   0        0        0    10933 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/connector.py
--rw-r--r--   0        0        0      895 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/enums.py
--rw-r--r--   0        0        0     9199 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/provider_setup.py
--rw-r--r--   0        0        0     1665 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/settings.py
--rw-r--r--   0        0        0      713 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/__init__.py
--rw-r--r--   0        0        0      849 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/__init__.py
--rw-r--r--   0        0        0      888 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/args.py
--rw-r--r--   0        0        0     6405 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/base.py
--rw-r--r--   0        0        0       87 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/__init__.py
--rw-r--r--   0        0        0     2948 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/config.py
--rw-r--r--   0        0        0     3277 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/scan.py
--rw-r--r--   0        0        0     9860 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/provider_setup.py
--rw-r--r--   0        0        0     2609 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cloud_asset.py
--rw-r--r--   0        0        0     8372 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/connector.py
--rw-r--r--   0        0        0      659 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/context.py
--rw-r--r--   0        0        0     1598 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/enums.py
--rw-r--r--   0        0        0     6533 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/healthcheck.py
--rw-r--r--   0        0        0      957 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/ignore_list.py
--rw-r--r--   0        0        0      857 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/logger.py
--rw-r--r--   0        0        0      506 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/models.py
--rw-r--r--   0        0        0      296 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/__init__.py
--rw-r--r--   0        0        0      489 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/events.py
--rw-r--r--   0        0        0     1455 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/plugin.py
--rw-r--r--   0        0        0     5633 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/registry.py
--rw-r--r--   0        0        0     2858 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/seed.py
--rw-r--r--   0        0        0     8864 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/settings.py
--rw-r--r--   0        0        0      329 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/__init__.py
--rw-r--r--   0        0        0    12081 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/connector.py
--rw-r--r--   0        0        0     5883 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/enums.py
--rw-r--r--   0        0        0    27935 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/provider_setup.py
--rw-r--r--   0        0        0     1688 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/settings.py
--rw-r--r--   0        0        0       36 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/__init__.py
--rw-r--r--   0        0        0    14559 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/aws_tags.py
--rw-r--r--   0        0        0     1882 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/example.py
--rw-r--r--   0        0        0        0 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/py.typed
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-21 16:29:59.071797 censys_cloud_connectors-3.1.3/LICENSE
+-rw-r--r--   0        0        0     2143 2023-06-21 16:29:59.071797 censys_cloud_connectors-3.1.3/README.md
+-rw-r--r--   0        0        0     4491 2023-06-21 16:29:59.083792 censys_cloud_connectors-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0      920 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/__init__.py
+-rw-r--r--   0        0        0    27101 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/connector.py
+-rw-r--r--   0        0        0     2766 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/enums.py
+-rw-r--r--   0        0        0    18732 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/provider_setup.py
+-rwxr-xr-x   0        0        0     1240 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/serverless.py
+-rw-r--r--   0        0        0     8355 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/service.py
+-rw-r--r--   0        0        0     4192 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/settings.py
+-rw-r--r--   0        0        0      343 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/__init__.py
+-rw-r--r--   0        0        0    10933 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/connector.py
+-rw-r--r--   0        0        0      895 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/enums.py
+-rw-r--r--   0        0        0     9199 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/provider_setup.py
+-rw-r--r--   0        0        0     1665 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/settings.py
+-rw-r--r--   0        0        0      713 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/args.py
+-rw-r--r--   0        0        0     6405 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/base.py
+-rw-r--r--   0        0        0       87 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/config.py
+-rw-r--r--   0        0        0     3277 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/scan.py
+-rw-r--r--   0        0        0     9860 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/provider_setup.py
+-rw-r--r--   0        0        0     2609 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cloud_asset.py
+-rw-r--r--   0        0        0     8524 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/connector.py
+-rw-r--r--   0        0        0      659 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/context.py
+-rw-r--r--   0        0        0     1598 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/enums.py
+-rw-r--r--   0        0        0     6533 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/healthcheck.py
+-rw-r--r--   0        0        0      957 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/ignore_list.py
+-rw-r--r--   0        0        0      857 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/logger.py
+-rw-r--r--   0        0        0      506 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/models.py
+-rw-r--r--   0        0        0      296 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/events.py
+-rw-r--r--   0        0        0     1455 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/plugin.py
+-rw-r--r--   0        0        0     5633 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/registry.py
+-rw-r--r--   0        0        0     2858 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/seed.py
+-rw-r--r--   0        0        0     8864 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/settings.py
+-rw-r--r--   0        0        0      329 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/__init__.py
+-rw-r--r--   0        0        0    12081 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/connector.py
+-rw-r--r--   0        0        0     5883 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/enums.py
+-rw-r--r--   0        0        0    27935 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/provider_setup.py
+-rw-r--r--   0        0        0     1688 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/settings.py
+-rw-r--r--   0        0        0       36 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/__init__.py
+-rw-r--r--   0        0        0    14168 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/aws_tags.py
+-rw-r--r--   0        0        0     1882 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/example.py
+-rw-r--r--   0        0        0        0 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/py.typed
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.3/PKG-INFO
```

### Comparing `censys_cloud_connectors-3.1.2/LICENSE` & `censys_cloud_connectors-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/README.md` & `censys_cloud_connectors-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/pyproject.toml` & `censys_cloud_connectors-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys-cloud-connectors"
-version = "3.1.2"
+version = "3.1.3"
 description = "The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "censys/cloud_connectors", from = "src" }]
 keywords = ["censys", "cloud", "connector", "attack surface management"]
 classifiers = [
@@ -69,19 +69,15 @@
 pep8-naming = "^0.12.1"
 pre-commit = "^2.17.0"
 pyupgrade = "^2.31.1"
 # Typing
 mypy = "^0.942"
 types-PyYAML = "^6.0.5"
 types-requests = "^2.27.14"
-
-[tool.poetry.group.test]
-optional = true
-
-[tool.poetry.group.test.dependencies]
+# Testing
 parameterized = "^0.8.1"
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 pytest-datadir = "^1.3.1"
 pytest-mock = "^3.7.0"
 responses = "^0.21.0"
```

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/__init__.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/connector.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     TagTypeDef,
 )
 from mypy_boto3_ecs import ECSClient
 from mypy_boto3_elb import ElasticLoadBalancingClient
 from mypy_boto3_elbv2 import ElasticLoadBalancingv2Client
 from mypy_boto3_rds import RDSClient
 from mypy_boto3_route53 import Route53Client
-from mypy_boto3_route53domains import Route53DomainsClient
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_sts import STSClient
 from mypy_boto3_sts.type_defs import CredentialsTypeDef
 
 from censys.cloud_connectors.aws_connector.enums import (
     AwsDefaults,
     AwsResourceTypes,
@@ -79,15 +78,15 @@
         """
         super().__init__(settings)
         self.seed_scanners = {
             AwsResourceTypes.API_GATEWAY: self.get_api_gateway_domains,
             AwsResourceTypes.LOAD_BALANCER: self.get_load_balancers,
             AwsResourceTypes.NETWORK_INTERFACE: self.get_network_interfaces,
             AwsResourceTypes.RDS: self.get_rds_instances,
-            AwsResourceTypes.ROUTE53: self.get_route53_instances,
+            AwsResourceTypes.ROUTE53: self.get_route53_zones,
             AwsResourceTypes.ECS: self.get_ecs_instances,
         }
         self.cloud_asset_scanners = {
             AwsResourceTypes.STORAGE_BUCKET: self.get_s3_instances,
         }
 
         self.ignored_tags = []
@@ -525,55 +524,14 @@
                 if domain_name := instance.get("Endpoint", {}).get("Address"):
                     with SuppressValidationError():
                         domain_seed = DomainSeed(value=domain_name, label=label)
                         self.add_seed(domain_seed, rds_res=instance)
         except ClientError as e:
             self.logger.error(f"Could not connect to RDS Service. Error: {e}")
 
-    def _get_route53_domains(self, client: Route53DomainsClient):
-        """Retrieve Paginated Route 53 Domains.
-
-        Args:
-            client (Route53DomainsClient): Route 53 Client.
-
-        Yields:
-            Generator[dict]: A Page of Route 53 Domains
-        """
-        next_page_marker = None
-        while True:
-            try:
-                if next_page_marker:
-                    data = client.list_domains(Marker=next_page_marker)
-                else:
-                    data = client.list_domains()
-
-                yield data
-
-                if not (next_page_marker := data.get("NextPageMarker")):
-                    break
-            except ClientError as e:
-                self.logger.error(f"Could not connect to Route 53 Domains. Error: {e}")
-                break
-
-    def get_route53_domains(self):
-        """Retrieve Route 53 Domains and emit seeds."""
-        client: Route53DomainsClient = self.get_aws_client(
-            service=AwsServices.ROUTE53_DOMAINS
-        )
-        label = self.format_label(SeedLabel.ROUTE53_DOMAINS)
-
-        for data in self._get_route53_domains(client):
-            for domain in data.get("Domains", []):
-                if domain_name := domain.get("DomainName"):
-                    with SuppressValidationError():
-                        domain_seed = DomainSeed(value=domain_name, label=label)
-                        self.add_seed(
-                            domain_seed, route53_domain_res=domain, aws_client=client
-                        )
-
     def _get_route53_zone_hosts(self, client: botocore.client.BaseClient) -> dict:
         """Retrieve Route 53 Zone hosts.
 
         Args:
             client (botocore.client.BaseClient): Route53 Client
 
         Returns:
@@ -609,14 +567,20 @@
 
         try:
             zones = self._get_route53_zone_hosts(client)
             for zone in zones.get("HostedZones", []):
                 if zone.get("Config", {}).get("PrivateZone"):
                     continue
 
+                # Add the zone itself as a seed
+                domain_name = zone.get("Name").rstrip(".")
+                with SuppressValidationError():
+                    domain_seed = DomainSeed(value=domain_name, label=label)
+                    self.add_seed(domain_seed, route53_zone_res=zone, aws_client=client)
+
                 id = zone.get("Id")
                 resource_sets = self._get_route53_zone_resources(client, id)
                 for resource_set in resource_sets.get("ResourceRecordSets", []):
                     if resource_set.get("Type") not in VALID_RECORD_TYPES:
                         continue
 
                     domain_name = resource_set.get("Name").rstrip(".")
@@ -624,20 +588,14 @@
                         domain_seed = DomainSeed(value=domain_name, label=label)
                         self.add_seed(
                             domain_seed, route53_zone_res=zone, aws_client=client
                         )
         except ClientError as e:
             self.logger.error(f"Could not connect to Route 53 Zones. Error: {e}")
 
-    def get_route53_instances(self):
-        """Retrieve Route 53 data and emit seeds."""
-        # Route53 domains have been removed until a client need is identified.
-        # self.get_route53_domains()
-        self.get_route53_zones()
-
     def get_ecs_instances(self):
         """Retrieve Elastic Container Service data and emit seeds."""
         ecs: ECSClient = self.get_aws_client(AwsServices.ECS)
         ec2: EC2Client = self.get_aws_client(AwsServices.EC2)
         label = self.format_label(SeedLabel.ECS)
 
         try:
```

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/enums.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/provider_setup.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/serverless.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/serverless.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/service.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/service.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/settings.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/connector.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/enums.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/provider_setup.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/settings.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/__init__.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/__init__.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/args.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/base.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/base.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/config.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/scan.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/scan.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/provider_setup.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cloud_asset.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cloud_asset.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/connector.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,22 +209,28 @@
                 res.status_code,
                 error_message,
                 res.text,
                 error_code=json_data.get("errorCode"),
             )
         return json_data
 
+    def clear(self):
+        """Clear the seeds and cloud assets."""
+        self.seeds.clear()
+        self.cloud_assets.clear()
+
     def submit(self):  # pragma: no cover
         """Submit the seeds and cloud assets to the Censys ASM."""
         if self.settings.dry_run:
             self.logger.info("Dry run enabled. Skipping submission.")
         else:
             self.logger.info("Submitting seeds and assets...")
             self.submit_seeds()
             self.submit_cloud_assets()
+        self.clear()
 
     def scan(self):
         """Scan the seeds and cloud assets."""
         self.logger.info("Gathering seeds and assets...")
         self.dispatch_event(EventTypeEnum.SCAN_STARTED)
         self.get_seeds()
         self.get_cloud_assets()
```

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/context.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/context.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/enums.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/healthcheck.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/healthcheck.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/ignore_list.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/ignore_list.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/logger.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/logger.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/plugin.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/registry.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/seed.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/seed.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/settings.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/connector.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/enums.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/provider_setup.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/settings.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/aws_tags.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/aws_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import urllib.parse
 from typing import Callable, Optional
 
 from botocore.exceptions import ClientError
 from mypy_boto3_elb import ElasticLoadBalancingClient
 from mypy_boto3_elbv2 import ElasticLoadBalancingv2Client
 from mypy_boto3_route53 import Route53Client
-from mypy_boto3_route53domains import Route53DomainsClient
 from mypy_boto3_s3 import S3Client
 from requests import HTTPError
 
 from censys.asm import AsmClient
 from censys.common.exceptions import (
     CensysAsmException,
     CensysDomainNotFoundException,
@@ -370,33 +369,27 @@
         """Get Route53 tags.
 
         Args:
             context: Event context.
             seed: Seed.
             kwargs: Additional event data.
         """
-        route53_domain_res = kwargs.get("route53_domain_res")
         route53_zone_res = kwargs.get("route53_zone_res")
-        if not route53_domain_res and not route53_zone_res:
+        if not route53_zone_res:
             return
         pre_processed_tags = None
-        if route53_domain_res:
-            domains_client: Route53DomainsClient = kwargs.get("aws_client")  # type: ignore
-            if not domains_client:
-                return
-            pre_processed_tags = domains_client.list_tags_for_domain(
-                DomainName=route53_domain_res["DomainName"]
-            )["TagList"]
-        elif route53_zone_res:
-            client: Route53Client = kwargs.get("aws_client")  # type: ignore
-            if not client:
-                return
-            pre_processed_tags = client.list_tags_for_resource(
-                ResourceType="hostedzone", ResourceId=route53_zone_res["Id"]
-            )["ResourceTagSet"]["Tags"]
+        client: Route53Client = kwargs.get("aws_client")  # type: ignore
+        if not client:
+            return
+        resource_id = route53_zone_res["Id"]
+        if resource_id.startswith("/hostedzone/"):
+            resource_id = resource_id.split("/hostedzone/")[1]
+        pre_processed_tags = client.list_tags_for_resource(
+            ResourceType="hostedzone", ResourceId=resource_id
+        )["ResourceTagSet"]["Tags"]
 
         if not pre_processed_tags:
             return
 
         tags = {tag["Key"]: tag["Value"] for tag in pre_processed_tags}
 
         self.add_domain_tags(context, seed, tags)  # type: ignore
```

### Comparing `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/example.py` & `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/example.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.2/PKG-INFO` & `censys_cloud_connectors-3.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censys-cloud-connectors
-Version: 3.1.2
+Version: 3.1.3
 Summary: The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM.
 License: Apache-2.0
 Keywords: censys,cloud,connector,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
```

