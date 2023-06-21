# Comparing `tmp/resoto-plugin-aws-3.5.2.tar.gz` & `tmp/resoto-plugin-aws-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.5.2.tar", last modified: Tue Jun 13 13:07:29 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.5.3.tar", last modified: Wed Jun 21 14:22:50 2023, max compression
```

## Comparing `resoto-plugin-aws-3.5.2.tar` & `resoto-plugin-aws-3.5.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.305663 resoto-plugin-aws-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-13 13:07:29.305663 resoto-plugin-aws-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.293663 resoto-plugin-aws-3.5.2/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    31601 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.293663 resoto-plugin-aws-3.5.2/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.297663 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24038 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   115330 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.293663 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:03:40.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 13:07:29.000000 resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 13:07:29.305663 resoto-plugin-aws-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.301663 resoto-plugin-aws-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:29.305663 resoto-plugin-aws-3.5.2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 13:03:06.000000 resoto-plugin-aws-3.5.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    32234 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.277735 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24038 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115330 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.273735 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:06.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:22:50.000000 resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.281735 resoto-plugin-aws-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:22:50.285735 resoto-plugin-aws-3.5.3/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 14:18:35.000000 resoto-plugin-aws-3.5.3/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.5.2/PKG-INFO` & `resoto-plugin-aws-3.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.2
+Version: 3.5.3
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.5.2/README.md` & `resoto-plugin-aws-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/pyproject.toml` & `resoto-plugin-aws-3.5.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.2",
+    "resotolib==3.5.3",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
 aws = "resoto_plugin_aws:AWSCollectorPlugin"
```

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 import multiprocessing
+import os
 from concurrent import futures
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Sequence
 
 import boto3
 import botocore.exceptions
 from botocore.model import ListShape, OperationModel, Shape, StringShape, StructureShape
 from jsons import pascalcase
 from prometheus_client import Counter, Summary
-from resoto_plugin_aws.aws_client import AwsClient
 
 import resotolib.logger
 import resotolib.proc
+from resoto_plugin_aws.aws_client import AwsClient
 from resotolib.args import ArgumentParser, Namespace
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import (
     BaseAccount,
     BaseRegion,
     BaseResource,
     Cloud,
@@ -26,19 +28,18 @@
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.custom_command import execute_command_on_resource
 from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.logger import log, setup_logger
 from resotolib.types import JsonElement
 from resotolib.utils import NoExitArgumentParser, log_runtime
-
 from .collector import AwsAccountCollector
 from .configuration import AwsConfig
 from .resource.base import AwsAccount, AwsResource, get_client
-from .utils import arn_partition_by_region, aws_session, global_region_by_partition
+from .utils import arn_partition_by_region, aws_session, global_region_by_partition, get_aws_profiles_from_file
 
 logging.getLogger("boto").setLevel(logging.CRITICAL)
 
 metrics_collect = Summary("resoto_plugin_aws_collect_seconds", "Time it took the collect() method")
 metrics_unhandled_account_exceptions = Counter(
     "resoto_plugin_aws_unhandled_account_exceptions_total",
     "Unhandled AWS Plugin Account Exceptions",
@@ -533,64 +534,74 @@
     max_workers = len(accounts) if len(accounts) < Config.aws.account_pool_size else Config.aws.account_pool_size
     with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         executor.map(set_account_name, accounts)
 
 
 def get_accounts(core_feedback: CoreFeedback) -> List[AwsAccount]:
     accounts = []
-    profiles = [None]
+    profiles: Sequence[Optional[str]] = [None]
+    config: AwsConfig = Config.aws
 
-    if Config.aws.assume_current and not Config.aws.do_not_scrape_current:
+    if config.assume_current and not config.do_not_scrape_current:
         msg = (
             "You specified assume_current but not do_not_scrape_current! "
             "This will result in the same account being collected twice and is likely not what you want."
         )
-        core_feedback.error(msg)
+        core_feedback.error(msg, log)
         raise ValueError(msg)
 
-    if isinstance(Config.aws.profiles, list) and len(Config.aws.profiles) > 0:
+    credentials = Path(os.environ.get("AWS_SHARED_CREDENTIALS_FILE", os.path.expanduser("~/.aws/credentials")))
+    if isinstance(config.profiles, list) and len(config.profiles) > 0:
         log.debug("Using specified AWS profiles")
-        profiles = Config.aws.profiles
-        if Config.aws.account and len(Config.aws.profiles) > 1:
+        profiles = config.profiles
+        if config.account and len(config.profiles) > 1:
             msg = (
                 "You specified both a list of accounts and more than one profile! "
                 "This will result in the attempt to collect the same accounts for "
                 "every profile and is likely not what you want."
             )
-            core_feedback.error(msg)
+            core_feedback.error(msg, log)
             raise ValueError(msg)
+    elif not config.account and not config.access_key_id and credentials.is_file():
+        log.debug("Extracting AWS profiles from shared credentials file")
+        try:
+            profiles = get_aws_profiles_from_file(credentials)
+            log.debug("Discovered the following profiles: %s", profiles)
+        except Exception:
+            msg = "AWS Credentials file found but could not be parsed."
+            core_feedback.error(msg, log)
 
     for profile in profiles:
         if profile is not None:
             log.debug(f"Finding accounts for profile {profile}")
 
         try:
-            if Config.aws.role and Config.aws.scrape_org:
+            if config.role and config.scrape_org:
                 log.debug("Role and scrape_org are both set")
                 account_id, partition = current_account_id_and_partition(profile=profile)
                 accounts.extend(
                     [
-                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile, partition=partition)
+                        AwsAccount(id=aws_account_id, role=config.role, profile=profile, partition=partition)
                         for aws_account_id in get_org_accounts(
-                            filter_current_account=not Config.aws.assume_current,
+                            filter_current_account=not config.assume_current,
                             profile=profile,
                             core_feedback=core_feedback,
                             partition=partition,
                         )
-                        if aws_account_id not in Config.aws.scrape_exclude_account
+                        if aws_account_id not in config.scrape_exclude_account
                     ]
                 )
-                if not Config.aws.do_not_scrape_current:
+                if not config.do_not_scrape_current:
                     accounts.append(AwsAccount(id=account_id, partition=partition))
-            elif Config.aws.role and Config.aws.account:
+            elif config.role and config.account:
                 log.debug("Both, role and list of accounts specified")
-                for aws_account_id in Config.aws.account:
+                for aws_account_id in config.account:
                     partition = probe_partition(aws_account_id, profile=profile)
                     accounts.append(
-                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile, partition=partition)
+                        AwsAccount(id=aws_account_id, role=config.role, profile=profile, partition=partition)
                     )
             else:
                 account_id, partition = current_account_id_and_partition(profile=profile)
                 accounts.extend([AwsAccount(id=account_id, profile=profile, partition=partition)])
         except botocore.exceptions.NoCredentialsError:
             core_feedback.error(f"No AWS credentials found for {profile}", log)
         except botocore.exceptions.ClientError as e:
```

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/configuration.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import uuid
+from configparser import ConfigParser
+from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional
 
 from boto3.session import Session as BotoSession
 from botocore.exceptions import ConnectionClosedError, CredentialRetrievalError
 from prometheus_client import Counter
 from retrying import retry
 
@@ -14,14 +16,21 @@
 
 metrics_session_exceptions = Counter(
     "resoto_plugin_aws_session_exceptions_total",
     "Unhandled AWS Plugin Session Exceptions",
 )
 
 
+def get_aws_profiles_from_file(path: Path) -> List[str]:
+    parser = ConfigParser()
+    parser.read(path)
+    # Use all sections that have an access key id defined
+    return [s for s in parser.sections() if parser.get(s, "aws_access_key_id", fallback=None) is not None]
+
+
 def retry_on_session_error(e: Exception) -> bool:
     if isinstance(e, (ConnectionClosedError, CredentialRetrievalError)):
         metrics_session_exceptions.inc()
         return True
     return False
```

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.2
+Version: 3.5.3
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.5.2/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.5.3/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/__init__.py` & `resoto-plugin-aws-3.5.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/aws_client_test.py` & `resoto-plugin-aws-3.5.3/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/collector_test.py` & `resoto-plugin-aws-3.5.3/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/configuration_test.py` & `resoto-plugin-aws-3.5.3/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/graphbuilder_test.py` & `resoto-plugin-aws-3.5.3/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/__init__.py` & `resoto-plugin-aws-3.5.3/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.5.3/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/athena_test.py` & `resoto-plugin-aws-3.5.3/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.5.3/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/base_test.py` & `resoto-plugin-aws-3.5.3/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.5.3/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.5.3/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.5.3/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.5.3/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/cognito_test.py` & `resoto-plugin-aws-3.5.3/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.5.3/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/ec2_test.py` & `resoto-plugin-aws-3.5.3/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/ecs_test.py` & `resoto-plugin-aws-3.5.3/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/eks_test.py` & `resoto-plugin-aws-3.5.3/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.5.3/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.5.3/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/elb_test.py` & `resoto-plugin-aws-3.5.3/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.5.3/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/glacier_test.py` & `resoto-plugin-aws-3.5.3/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/iam_test.py` & `resoto-plugin-aws-3.5.3/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.5.3/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/kms_test.py` & `resoto-plugin-aws-3.5.3/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/lambda_test.py` & `resoto-plugin-aws-3.5.3/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/pricing_test.py` & `resoto-plugin-aws-3.5.3/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/rds_test.py` & `resoto-plugin-aws-3.5.3/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/redshift_test.py` & `resoto-plugin-aws-3.5.3/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/route53_test.py` & `resoto-plugin-aws-3.5.3/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/s3_test.py` & `resoto-plugin-aws-3.5.3/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.5.3/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.5.3/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/sns_test.py` & `resoto-plugin-aws-3.5.3/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.2/test/resources/sqs_test.py` & `resoto-plugin-aws-3.5.3/test/resources/sqs_test.py`

 * *Files identical despite different names*

