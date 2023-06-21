# Comparing `tmp/pulumi_artifactory-3.6.0a1687054110.tar.gz` & `tmp/pulumi_artifactory-4.0.0a1687363033.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_artifactory-3.6.0a1687054110.tar", last modified: Sun Jun 18 02:15:01 2023, max compression
+gzip compressed data, was "pulumi_artifactory-4.0.0a1687363033.tar", last modified: Wed Jun 21 16:08:02 2023, max compression
```

## Comparing `pulumi_artifactory-3.6.0a1687054110.tar` & `pulumi_artifactory-4.0.0a1687363033.tar`

### file list

```diff
@@ -1,309 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/
--rw-r--r--   0 runner    (1001) docker     (123)    45822 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367032 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33734 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/anonymous_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifact_property_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifact_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifactory_release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/build_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/distribution_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/distribution_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/general_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_docker_v1_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_docker_v2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraformbackend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/ldap_group_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/ldap_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gitltfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_repository_multi_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_repository_single_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_backend_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_module_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_provider_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_vagrant_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/managed_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/oauth_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   320747 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/permission_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/permission_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/property_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/pull_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/push_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/release_bundle_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cargo_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cocoapods_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_go_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_maven_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_opkg_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_repository_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_terraform_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_vcs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/repository_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/saml_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    45108 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/scoped_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/single_replication_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/unmanaged_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_alpine_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_bower_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_chef_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_composer_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_conan_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_conda_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_cran_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_debian_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_docker_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gems_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_generic_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gitlfs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gradle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_helm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_ivy_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_npm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_nuget_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_p2_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_pub_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_puppet_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_pypi_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_sbt_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_swift_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_terraform_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 02:15:01.000000 pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:15:01.332838 pulumi_artifactory-3.6.0a1687054110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-18 02:15:00.000000 pulumi_artifactory-3.6.0a1687054110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/
+-rw-r--r--   0 runner    (1001) docker     (123)    45591 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   345890 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33734 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55059 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/anonymous_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifact_property_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifact_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifactory_release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37201 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/build_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/distribution_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/distribution_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52691 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59110 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64052 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67404 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58869 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58891 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68241 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69522 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58509 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82094 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82034 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58569 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58749 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58629 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74462 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81914 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58689 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59285 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59401 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58809 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/general_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17169 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17295 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_docker_v1_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_docker_v2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraformbackend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37605 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40841 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33399 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39044 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45435 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39966 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33181 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32963 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33072 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44332 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35325 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45831 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30892 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/ldap_group_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51241 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/ldap_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57650 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49759 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48928 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gitltfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48750 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71368 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55830 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48902 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_repository_multi_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54950 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_repository_single_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69786 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72133 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49174 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_backend_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49148 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_module_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_provider_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48940 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_vagrant_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26725 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/managed_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/oauth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   303865 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19731 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/permission_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/pull_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/push_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/release_bundle_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124638 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133172 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134454 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cargo_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124526 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133779 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cocoapods_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133433 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127509 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124508 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124620 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142128 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124504 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127348 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124662 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127340 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_go_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148774 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138407 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148612 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_maven_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124674 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139764 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124556 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_opkg_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124452 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124494 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124618 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41782 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_repository_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124468 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   148498 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124540 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131794 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_terraform_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134992 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_vcs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/repository_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43485 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/saml_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/scoped_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/single_replication_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27537 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/unmanaged_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44687 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_alpine_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48898 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_bower_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42194 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_chef_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38889 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_composer_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_conan_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_conda_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_cran_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_debian_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42611 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_docker_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gems_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38837 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_generic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38787 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gitlfs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50146 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gradle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46520 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_helm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50032 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_ivy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52303 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_npm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42573 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_nuget_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_p2_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38673 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_pub_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38791 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_puppet_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38699 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_pypi_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50054 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_sbt_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_swift_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38517 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_terraform_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:08:02.034588 pulumi_artifactory-4.0.0a1687363033/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-21 16:08:01.000000 pulumi_artifactory-4.0.0a1687363033/setup.py
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/PKG-INFO` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_artifactory
-Version: 3.6.0a1687054110
+Name: pulumi-artifactory
+Version: 4.0.0a1687363033
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -42,15 +42,15 @@
 
     $ pip install pulumi_artifactory
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-artifactory/sdk/v7
+    $ go get github.com/pulumi/pulumi-artifactory/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Artifactory
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/README.md` & `pulumi_artifactory-4.0.0a1687363033/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     $ pip install pulumi_artifactory
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-artifactory/sdk/v7
+    $ go get github.com/pulumi/pulumi-artifactory/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Artifactory
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/__init__.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,14 @@
 from .local_terraform_module_repository import *
 from .local_terraform_provider_repository import *
 from .local_vagrant_repository import *
 from .managed_user import *
 from .maven_repository import *
 from .oauth_settings import *
 from .permission_target import *
-from .permission_targets import *
 from .property_set import *
 from .provider import *
 from .proxy import *
 from .pull_replication import *
 from .push_replication import *
 from .release_bundle_webhook import *
 from .remote_alpine_repository import *
@@ -1015,22 +1014,14 @@
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/permissionTarget:PermissionTarget": "PermissionTarget"
   }
  },
  {
   "pkg": "artifactory",
-  "mod": "index/permissionTargets",
-  "fqn": "pulumi_artifactory",
-  "classes": {
-   "artifactory:index/permissionTargets:PermissionTargets": "PermissionTargets"
-  }
- },
- {
-  "pkg": "artifactory",
   "mod": "index/propertySet",
   "fqn": "pulumi_artifactory",
   "classes": {
    "artifactory:index/propertySet:PropertySet": "PropertySet"
   }
  },
  {
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/_inputs.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,37 +54,25 @@
     'FederatedSwiftRepositoryMemberArgs',
     'FederatedTerraformModuleRepositoryMemberArgs',
     'FederatedTerraformProviderRepositoryMemberArgs',
     'FederatedVagrantRepositoryMemberArgs',
     'LocalRepositoryMultiReplicationReplicationArgs',
     'OauthSettingsOauthProviderArgs',
     'PermissionTargetBuildArgs',
-    'PermissionTargetBuildActionsArgs',
-    'PermissionTargetBuildActionsGroupArgs',
-    'PermissionTargetBuildActionsUserArgs',
+    'PermissionTargetBuildActionArgs',
+    'PermissionTargetBuildActionGroupArgs',
+    'PermissionTargetBuildActionUserArgs',
     'PermissionTargetReleaseBundleArgs',
-    'PermissionTargetReleaseBundleActionsArgs',
-    'PermissionTargetReleaseBundleActionsGroupArgs',
-    'PermissionTargetReleaseBundleActionsUserArgs',
+    'PermissionTargetReleaseBundleActionArgs',
+    'PermissionTargetReleaseBundleActionGroupArgs',
+    'PermissionTargetReleaseBundleActionUserArgs',
     'PermissionTargetRepoArgs',
-    'PermissionTargetRepoActionsArgs',
-    'PermissionTargetRepoActionsGroupArgs',
-    'PermissionTargetRepoActionsUserArgs',
-    'PermissionTargetsBuildArgs',
-    'PermissionTargetsBuildActionsArgs',
-    'PermissionTargetsBuildActionsGroupArgs',
-    'PermissionTargetsBuildActionsUserArgs',
-    'PermissionTargetsReleaseBundleArgs',
-    'PermissionTargetsReleaseBundleActionsArgs',
-    'PermissionTargetsReleaseBundleActionsGroupArgs',
-    'PermissionTargetsReleaseBundleActionsUserArgs',
-    'PermissionTargetsRepoArgs',
-    'PermissionTargetsRepoActionsArgs',
-    'PermissionTargetsRepoActionsGroupArgs',
-    'PermissionTargetsRepoActionsUserArgs',
+    'PermissionTargetRepoActionArgs',
+    'PermissionTargetRepoActionGroupArgs',
+    'PermissionTargetRepoActionUserArgs',
     'PropertySetPropertyArgs',
     'PropertySetPropertyPredefinedValueArgs',
     'PushReplicationReplicationArgs',
     'ReleaseBundleWebhookCriteriaArgs',
     'ReleaseBundleWebhookHandlerArgs',
     'RemoteAlpineRepositoryContentSynchronisationArgs',
     'RemoteBowerRepositoryContentSynchronisationArgs',
@@ -2679,15 +2667,15 @@
         pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
 class PermissionTargetBuildArgs:
     def __init__(__self__, *,
                  repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetBuildActionsArgs']] = None,
+                 actions: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionArgs']]]] = None,
                  excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
         """
@@ -2709,19 +2697,19 @@
 
     @repositories.setter
     def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "repositories", value)
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetBuildActionsArgs']]:
+    def actions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionArgs']]]]:
         return pulumi.get(self, "actions")
 
     @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetBuildActionsArgs']]):
+    def actions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionArgs']]]]):
         pulumi.set(self, "actions", value)
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Pattern of artifacts to exclude.
@@ -2742,54 +2730,54 @@
 
     @includes_patterns.setter
     def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "includes_patterns", value)
 
 
 @pulumi.input_type
-class PermissionTargetBuildActionsArgs:
+class PermissionTargetBuildActionArgs:
     def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsUserArgs']]]] = None):
+                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionGroupArgs']]]] = None,
+                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionUserArgs']]]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsUserArgs']]] users: Users this permission target applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionGroupArgs']]] groups: Groups this permission applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionUserArgs']]] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsGroupArgs']]]]:
+    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionGroupArgs']]]]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsGroupArgs']]]]):
+    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionGroupArgs']]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsUserArgs']]]]:
+    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionUserArgs']]]]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
     @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionsUserArgs']]]]):
+    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildActionUserArgs']]]]):
         pulumi.set(self, "users", value)
 
 
 @pulumi.input_type
-class PermissionTargetBuildActionsGroupArgs:
+class PermissionTargetBuildActionGroupArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2814,15 +2802,15 @@
 
     @permissions.setter
     def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
-class PermissionTargetBuildActionsUserArgs:
+class PermissionTargetBuildActionUserArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2850,15 +2838,15 @@
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class PermissionTargetReleaseBundleArgs:
     def __init__(__self__, *,
                  repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetReleaseBundleActionsArgs']] = None,
+                 actions: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionArgs']]]] = None,
                  excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
         """
@@ -2880,19 +2868,19 @@
 
     @repositories.setter
     def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "repositories", value)
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetReleaseBundleActionsArgs']]:
+    def actions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionArgs']]]]:
         return pulumi.get(self, "actions")
 
     @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetReleaseBundleActionsArgs']]):
+    def actions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionArgs']]]]):
         pulumi.set(self, "actions", value)
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Pattern of artifacts to exclude.
@@ -2913,54 +2901,54 @@
 
     @includes_patterns.setter
     def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "includes_patterns", value)
 
 
 @pulumi.input_type
-class PermissionTargetReleaseBundleActionsArgs:
+class PermissionTargetReleaseBundleActionArgs:
     def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsUserArgs']]]] = None):
+                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionGroupArgs']]]] = None,
+                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionUserArgs']]]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsUserArgs']]] users: Users this permission target applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionGroupArgs']]] groups: Groups this permission applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionUserArgs']]] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsGroupArgs']]]]:
+    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionGroupArgs']]]]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsGroupArgs']]]]):
+    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionGroupArgs']]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsUserArgs']]]]:
+    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionUserArgs']]]]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
     @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionsUserArgs']]]]):
+    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleActionUserArgs']]]]):
         pulumi.set(self, "users", value)
 
 
 @pulumi.input_type
-class PermissionTargetReleaseBundleActionsGroupArgs:
+class PermissionTargetReleaseBundleActionGroupArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2985,15 +2973,15 @@
 
     @permissions.setter
     def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
-class PermissionTargetReleaseBundleActionsUserArgs:
+class PermissionTargetReleaseBundleActionUserArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -3021,15 +3009,15 @@
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
 class PermissionTargetRepoArgs:
     def __init__(__self__, *,
                  repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetRepoActionsArgs']] = None,
+                 actions: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionArgs']]]] = None,
                  excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
         """
@@ -3051,19 +3039,19 @@
 
     @repositories.setter
     def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "repositories", value)
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetRepoActionsArgs']]:
+    def actions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionArgs']]]]:
         return pulumi.get(self, "actions")
 
     @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetRepoActionsArgs']]):
+    def actions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionArgs']]]]):
         pulumi.set(self, "actions", value)
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Pattern of artifacts to exclude.
@@ -3084,54 +3072,54 @@
 
     @includes_patterns.setter
     def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "includes_patterns", value)
 
 
 @pulumi.input_type
-class PermissionTargetRepoActionsArgs:
+class PermissionTargetRepoActionArgs:
     def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsUserArgs']]]] = None):
+                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionGroupArgs']]]] = None,
+                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionUserArgs']]]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsUserArgs']]] users: Users this permission target applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionGroupArgs']]] groups: Groups this permission applies for.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionUserArgs']]] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsGroupArgs']]]]:
+    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionGroupArgs']]]]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsGroupArgs']]]]):
+    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionGroupArgs']]]]):
         pulumi.set(self, "groups", value)
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsUserArgs']]]]:
+    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionUserArgs']]]]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
     @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionsUserArgs']]]]):
+    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoActionUserArgs']]]]):
         pulumi.set(self, "users", value)
 
 
 @pulumi.input_type
-class PermissionTargetRepoActionsGroupArgs:
+class PermissionTargetRepoActionGroupArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -3156,528 +3144,15 @@
 
     @permissions.setter
     def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "permissions", value)
 
 
 @pulumi.input_type
-class PermissionTargetRepoActionsUserArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsBuildArgs:
-    def __init__(__self__, *,
-                 repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetsBuildActionsArgs']] = None,
-                 excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @repositories.setter
-    def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "repositories", value)
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetsBuildActionsArgs']]:
-        return pulumi.get(self, "actions")
-
-    @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetsBuildActionsArgs']]):
-        pulumi.set(self, "actions", value)
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @excludes_patterns.setter
-    def excludes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "excludes_patterns", value)
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-    @includes_patterns.setter
-    def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "includes_patterns", value)
-
-
-@pulumi.input_type
-class PermissionTargetsBuildActionsArgs:
-    def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsUserArgs']]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsUserArgs']]] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsGroupArgs']]]]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsGroupArgs']]]]):
-        pulumi.set(self, "groups", value)
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsUserArgs']]]]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-    @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsBuildActionsUserArgs']]]]):
-        pulumi.set(self, "users", value)
-
-
-@pulumi.input_type
-class PermissionTargetsBuildActionsGroupArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsBuildActionsUserArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsReleaseBundleArgs:
-    def __init__(__self__, *,
-                 repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetsReleaseBundleActionsArgs']] = None,
-                 excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @repositories.setter
-    def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "repositories", value)
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetsReleaseBundleActionsArgs']]:
-        return pulumi.get(self, "actions")
-
-    @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetsReleaseBundleActionsArgs']]):
-        pulumi.set(self, "actions", value)
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @excludes_patterns.setter
-    def excludes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "excludes_patterns", value)
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-    @includes_patterns.setter
-    def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "includes_patterns", value)
-
-
-@pulumi.input_type
-class PermissionTargetsReleaseBundleActionsArgs:
-    def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsUserArgs']]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsUserArgs']]] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsGroupArgs']]]]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsGroupArgs']]]]):
-        pulumi.set(self, "groups", value)
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsUserArgs']]]]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-    @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsReleaseBundleActionsUserArgs']]]]):
-        pulumi.set(self, "users", value)
-
-
-@pulumi.input_type
-class PermissionTargetsReleaseBundleActionsGroupArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsReleaseBundleActionsUserArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsRepoArgs:
-    def __init__(__self__, *,
-                 repositories: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 actions: Optional[pulumi.Input['PermissionTargetsRepoActionsArgs']] = None,
-                 excludes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 includes_patterns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes_patterns: Pattern of artifacts to exclude.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @repositories.setter
-    def repositories(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "repositories", value)
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional[pulumi.Input['PermissionTargetsRepoActionsArgs']]:
-        return pulumi.get(self, "actions")
-
-    @actions.setter
-    def actions(self, value: Optional[pulumi.Input['PermissionTargetsRepoActionsArgs']]):
-        pulumi.set(self, "actions", value)
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @excludes_patterns.setter
-    def excludes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "excludes_patterns", value)
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-    @includes_patterns.setter
-    def includes_patterns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "includes_patterns", value)
-
-
-@pulumi.input_type
-class PermissionTargetsRepoActionsArgs:
-    def __init__(__self__, *,
-                 groups: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsGroupArgs']]]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsUserArgs']]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsGroupArgs']]] groups: Groups this permission applies for.
-        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsUserArgs']]] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsGroupArgs']]]]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @groups.setter
-    def groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsGroupArgs']]]]):
-        pulumi.set(self, "groups", value)
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsUserArgs']]]]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-    @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetsRepoActionsUserArgs']]]]):
-        pulumi.set(self, "users", value)
-
-
-@pulumi.input_type
-class PermissionTargetsRepoActionsGroupArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "permissions")
-
-    @permissions.setter
-    def permissions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "permissions", value)
-
-
-@pulumi.input_type
-class PermissionTargetsRepoActionsUserArgs:
+class PermissionTargetRepoActionUserArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  permissions: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/_utilities.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/access_token.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/anonymous_user.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/api_key.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifact_property_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifact_property_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifact_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifact_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/artifactory_release_bundle_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/artifactory_release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/backup.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/build_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/build_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/certificate.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/config/vars.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/distribution_public_key.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/distribution_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/distribution_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/distribution_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_v1_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_v2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/docker_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/docker_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_v1_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_docker_v2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gitltfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_terraform_module_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_terraform_provider_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/federated_vagrant_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/general_security.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/general_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_v1_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_docker_v2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_terraform_module_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_terraform_provider_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_federated_vagrant_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_federated_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_file.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_fileinfo.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_fileinfo.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_group.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_docker_v1_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_docker_v1_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_docker_v2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_docker_v2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraform_module_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraform_provider_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_terraformbackend_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_terraformbackend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_local_vagrant_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_permission_target.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_permission_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_p2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_terraform_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_remote_vcs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_user.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_p2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/get_virtual_terraform_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/get_virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/group.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,31 +590,31 @@
         """
         When this parameter is set, any new users defined in the system are automatically assigned to this group.
         """
         return pulumi.get(self, "auto_join")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def description(self) -> pulumi.Output[str]:
         """
         A description for the group.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="detachAllUsers")
-    def detach_all_users(self) -> pulumi.Output[bool]:
+    def detach_all_users(self) -> pulumi.Output[Optional[bool]]:
         """
         When this is set to `true`, an empty or missing usernames array will detach all users from the group.
         """
         return pulumi.get(self, "detach_all_users")
 
     @property
     @pulumi.getter(name="externalId")
-    def external_id(self) -> pulumi.Output[Optional[str]]:
+    def external_id(self) -> pulumi.Output[str]:
         """
         New external group ID used to configure the corresponding group in Azure AD.
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter
@@ -638,15 +638,15 @@
         """
         The realm for the group.
         """
         return pulumi.get(self, "realm")
 
     @property
     @pulumi.getter(name="realmAttributes")
-    def realm_attributes(self) -> pulumi.Output[Optional[str]]:
+    def realm_attributes(self) -> pulumi.Output[str]:
         """
         The realm attributes for the group.
         """
         return pulumi.get(self, "realm_attributes")
 
     @property
     @pulumi.getter(name="reportsManager")
@@ -654,15 +654,15 @@
         """
         When this override is set, User in the group can manage Xray Reports on any resource type. Default value is `false`.
         """
         return pulumi.get(self, "reports_manager")
 
     @property
     @pulumi.getter(name="usersNames")
-    def users_names(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def users_names(self) -> pulumi.Output[Sequence[str]]:
         """
         List of users assigned to the group. If not set or empty, Terraform will not manage group membership.
         """
         return pulumi.get(self, "users_names")
 
     @property
     @pulumi.getter(name="watchManager")
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/keypair.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/ldap_group_setting.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/ldap_group_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/ldap_setting.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/ldap_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gitltfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gitltfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_repository_multi_replication.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_repository_multi_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_repository_single_replication.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_repository_single_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_backend_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_backend_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_module_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_module_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_terraform_provider_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_terraform_provider_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/local_vagrant_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/local_vagrant_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/managed_user.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/managed_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/oauth_settings.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/outputs.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,37 +55,25 @@
     'FederatedSwiftRepositoryMember',
     'FederatedTerraformModuleRepositoryMember',
     'FederatedTerraformProviderRepositoryMember',
     'FederatedVagrantRepositoryMember',
     'LocalRepositoryMultiReplicationReplication',
     'OauthSettingsOauthProvider',
     'PermissionTargetBuild',
-    'PermissionTargetBuildActions',
-    'PermissionTargetBuildActionsGroup',
-    'PermissionTargetBuildActionsUser',
+    'PermissionTargetBuildAction',
+    'PermissionTargetBuildActionGroup',
+    'PermissionTargetBuildActionUser',
     'PermissionTargetReleaseBundle',
-    'PermissionTargetReleaseBundleActions',
-    'PermissionTargetReleaseBundleActionsGroup',
-    'PermissionTargetReleaseBundleActionsUser',
+    'PermissionTargetReleaseBundleAction',
+    'PermissionTargetReleaseBundleActionGroup',
+    'PermissionTargetReleaseBundleActionUser',
     'PermissionTargetRepo',
-    'PermissionTargetRepoActions',
-    'PermissionTargetRepoActionsGroup',
-    'PermissionTargetRepoActionsUser',
-    'PermissionTargetsBuild',
-    'PermissionTargetsBuildActions',
-    'PermissionTargetsBuildActionsGroup',
-    'PermissionTargetsBuildActionsUser',
-    'PermissionTargetsReleaseBundle',
-    'PermissionTargetsReleaseBundleActions',
-    'PermissionTargetsReleaseBundleActionsGroup',
-    'PermissionTargetsReleaseBundleActionsUser',
-    'PermissionTargetsRepo',
-    'PermissionTargetsRepoActions',
-    'PermissionTargetsRepoActionsGroup',
-    'PermissionTargetsRepoActionsUser',
+    'PermissionTargetRepoAction',
+    'PermissionTargetRepoActionGroup',
+    'PermissionTargetRepoActionUser',
     'PropertySetProperty',
     'PropertySetPropertyPredefinedValue',
     'PushReplicationReplication',
     'ReleaseBundleWebhookCriteria',
     'ReleaseBundleWebhookHandler',
     'RemoteAlpineRepositoryContentSynchronisation',
     'RemoteBowerRepositoryContentSynchronisation',
@@ -2470,15 +2458,15 @@
 
     def get(self, key: str, default = None) -> Any:
         PermissionTargetBuild.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetBuildActions'] = None,
+                 actions: Optional[Sequence['outputs.PermissionTargetBuildAction']] = None,
                  excludes_patterns: Optional[Sequence[str]] = None,
                  includes_patterns: Optional[Sequence[str]] = None):
         """
         :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
         :param Sequence[str] includes_patterns: Pattern of artifacts to include.
         """
@@ -2496,15 +2484,15 @@
         """
         List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         """
         return pulumi.get(self, "repositories")
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetBuildActions']:
+    def actions(self) -> Optional[Sequence['outputs.PermissionTargetBuildAction']]:
         return pulumi.get(self, "actions")
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[Sequence[str]]:
         """
         Pattern of artifacts to exclude.
@@ -2517,46 +2505,46 @@
         """
         Pattern of artifacts to include.
         """
         return pulumi.get(self, "includes_patterns")
 
 
 @pulumi.output_type
-class PermissionTargetBuildActions(dict):
+class PermissionTargetBuildAction(dict):
     def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetBuildActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetBuildActionsUser']] = None):
+                 groups: Optional[Sequence['outputs.PermissionTargetBuildActionGroup']] = None,
+                 users: Optional[Sequence['outputs.PermissionTargetBuildActionUser']] = None):
         """
-        :param Sequence['PermissionTargetBuildActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetBuildActionsUserArgs'] users: Users this permission target applies for.
+        :param Sequence['PermissionTargetBuildActionGroupArgs'] groups: Groups this permission applies for.
+        :param Sequence['PermissionTargetBuildActionUserArgs'] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetBuildActionsGroup']]:
+    def groups(self) -> Optional[Sequence['outputs.PermissionTargetBuildActionGroup']]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetBuildActionsUser']]:
+    def users(self) -> Optional[Sequence['outputs.PermissionTargetBuildActionUser']]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
-class PermissionTargetBuildActionsGroup(dict):
+class PermissionTargetBuildActionGroup(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2573,15 +2561,15 @@
     @property
     @pulumi.getter
     def permissions(self) -> Sequence[str]:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
-class PermissionTargetBuildActionsUser(dict):
+class PermissionTargetBuildActionUser(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2620,15 +2608,15 @@
 
     def get(self, key: str, default = None) -> Any:
         PermissionTargetReleaseBundle.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetReleaseBundleActions'] = None,
+                 actions: Optional[Sequence['outputs.PermissionTargetReleaseBundleAction']] = None,
                  excludes_patterns: Optional[Sequence[str]] = None,
                  includes_patterns: Optional[Sequence[str]] = None):
         """
         :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
         :param Sequence[str] includes_patterns: Pattern of artifacts to include.
         """
@@ -2646,15 +2634,15 @@
         """
         List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         """
         return pulumi.get(self, "repositories")
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetReleaseBundleActions']:
+    def actions(self) -> Optional[Sequence['outputs.PermissionTargetReleaseBundleAction']]:
         return pulumi.get(self, "actions")
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[Sequence[str]]:
         """
         Pattern of artifacts to exclude.
@@ -2667,46 +2655,46 @@
         """
         Pattern of artifacts to include.
         """
         return pulumi.get(self, "includes_patterns")
 
 
 @pulumi.output_type
-class PermissionTargetReleaseBundleActions(dict):
+class PermissionTargetReleaseBundleAction(dict):
     def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetReleaseBundleActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetReleaseBundleActionsUser']] = None):
+                 groups: Optional[Sequence['outputs.PermissionTargetReleaseBundleActionGroup']] = None,
+                 users: Optional[Sequence['outputs.PermissionTargetReleaseBundleActionUser']] = None):
         """
-        :param Sequence['PermissionTargetReleaseBundleActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetReleaseBundleActionsUserArgs'] users: Users this permission target applies for.
+        :param Sequence['PermissionTargetReleaseBundleActionGroupArgs'] groups: Groups this permission applies for.
+        :param Sequence['PermissionTargetReleaseBundleActionUserArgs'] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetReleaseBundleActionsGroup']]:
+    def groups(self) -> Optional[Sequence['outputs.PermissionTargetReleaseBundleActionGroup']]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetReleaseBundleActionsUser']]:
+    def users(self) -> Optional[Sequence['outputs.PermissionTargetReleaseBundleActionUser']]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
-class PermissionTargetReleaseBundleActionsGroup(dict):
+class PermissionTargetReleaseBundleActionGroup(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2723,15 +2711,15 @@
     @property
     @pulumi.getter
     def permissions(self) -> Sequence[str]:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
-class PermissionTargetReleaseBundleActionsUser(dict):
+class PermissionTargetReleaseBundleActionUser(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2770,15 +2758,15 @@
 
     def get(self, key: str, default = None) -> Any:
         PermissionTargetRepo.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetRepoActions'] = None,
+                 actions: Optional[Sequence['outputs.PermissionTargetRepoAction']] = None,
                  excludes_patterns: Optional[Sequence[str]] = None,
                  includes_patterns: Optional[Sequence[str]] = None):
         """
         :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
         :param Sequence[str] includes_patterns: Pattern of artifacts to include.
         """
@@ -2796,15 +2784,15 @@
         """
         List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
         """
         return pulumi.get(self, "repositories")
 
     @property
     @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetRepoActions']:
+    def actions(self) -> Optional[Sequence['outputs.PermissionTargetRepoAction']]:
         return pulumi.get(self, "actions")
 
     @property
     @pulumi.getter(name="excludesPatterns")
     def excludes_patterns(self) -> Optional[Sequence[str]]:
         """
         Pattern of artifacts to exclude.
@@ -2817,46 +2805,46 @@
         """
         Pattern of artifacts to include.
         """
         return pulumi.get(self, "includes_patterns")
 
 
 @pulumi.output_type
-class PermissionTargetRepoActions(dict):
+class PermissionTargetRepoAction(dict):
     def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetRepoActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetRepoActionsUser']] = None):
+                 groups: Optional[Sequence['outputs.PermissionTargetRepoActionGroup']] = None,
+                 users: Optional[Sequence['outputs.PermissionTargetRepoActionUser']] = None):
         """
-        :param Sequence['PermissionTargetRepoActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetRepoActionsUserArgs'] users: Users this permission target applies for.
+        :param Sequence['PermissionTargetRepoActionGroupArgs'] groups: Groups this permission applies for.
+        :param Sequence['PermissionTargetRepoActionUserArgs'] users: Users this permission target applies for.
         """
         if groups is not None:
             pulumi.set(__self__, "groups", groups)
         if users is not None:
             pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetRepoActionsGroup']]:
+    def groups(self) -> Optional[Sequence['outputs.PermissionTargetRepoActionGroup']]:
         """
         Groups this permission applies for.
         """
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetRepoActionsUser']]:
+    def users(self) -> Optional[Sequence['outputs.PermissionTargetRepoActionUser']]:
         """
         Users this permission target applies for.
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
-class PermissionTargetRepoActionsGroup(dict):
+class PermissionTargetRepoActionGroup(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
@@ -2873,465 +2861,15 @@
     @property
     @pulumi.getter
     def permissions(self) -> Sequence[str]:
         return pulumi.get(self, "permissions")
 
 
 @pulumi.output_type
-class PermissionTargetRepoActionsUser(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsBuild(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "excludesPatterns":
-            suggest = "excludes_patterns"
-        elif key == "includesPatterns":
-            suggest = "includes_patterns"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PermissionTargetsBuild. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PermissionTargetsBuild.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PermissionTargetsBuild.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetsBuildActions'] = None,
-                 excludes_patterns: Optional[Sequence[str]] = None,
-                 includes_patterns: Optional[Sequence[str]] = None):
-        """
-        :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
-        :param Sequence[str] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> Sequence[str]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetsBuildActions']:
-        return pulumi.get(self, "actions")
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-
-@pulumi.output_type
-class PermissionTargetsBuildActions(dict):
-    def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetsBuildActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetsBuildActionsUser']] = None):
-        """
-        :param Sequence['PermissionTargetsBuildActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetsBuildActionsUserArgs'] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetsBuildActionsGroup']]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetsBuildActionsUser']]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-
-@pulumi.output_type
-class PermissionTargetsBuildActionsGroup(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsBuildActionsUser(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsReleaseBundle(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "excludesPatterns":
-            suggest = "excludes_patterns"
-        elif key == "includesPatterns":
-            suggest = "includes_patterns"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PermissionTargetsReleaseBundle. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PermissionTargetsReleaseBundle.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PermissionTargetsReleaseBundle.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetsReleaseBundleActions'] = None,
-                 excludes_patterns: Optional[Sequence[str]] = None,
-                 includes_patterns: Optional[Sequence[str]] = None):
-        """
-        :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
-        :param Sequence[str] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> Sequence[str]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetsReleaseBundleActions']:
-        return pulumi.get(self, "actions")
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-
-@pulumi.output_type
-class PermissionTargetsReleaseBundleActions(dict):
-    def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetsReleaseBundleActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetsReleaseBundleActionsUser']] = None):
-        """
-        :param Sequence['PermissionTargetsReleaseBundleActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetsReleaseBundleActionsUserArgs'] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetsReleaseBundleActionsGroup']]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetsReleaseBundleActionsUser']]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-
-@pulumi.output_type
-class PermissionTargetsReleaseBundleActionsGroup(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsReleaseBundleActionsUser(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsRepo(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "excludesPatterns":
-            suggest = "excludes_patterns"
-        elif key == "includesPatterns":
-            suggest = "includes_patterns"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PermissionTargetsRepo. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PermissionTargetsRepo.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PermissionTargetsRepo.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 repositories: Sequence[str],
-                 actions: Optional['outputs.PermissionTargetsRepoActions'] = None,
-                 excludes_patterns: Optional[Sequence[str]] = None,
-                 includes_patterns: Optional[Sequence[str]] = None):
-        """
-        :param Sequence[str] repositories: List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        :param Sequence[str] excludes_patterns: Pattern of artifacts to exclude.
-        :param Sequence[str] includes_patterns: Pattern of artifacts to include.
-        """
-        pulumi.set(__self__, "repositories", repositories)
-        if actions is not None:
-            pulumi.set(__self__, "actions", actions)
-        if excludes_patterns is not None:
-            pulumi.set(__self__, "excludes_patterns", excludes_patterns)
-        if includes_patterns is not None:
-            pulumi.set(__self__, "includes_patterns", includes_patterns)
-
-    @property
-    @pulumi.getter
-    def repositories(self) -> Sequence[str]:
-        """
-        List of repositories this permission target is applicable for. You can specify the name `ANY` in the repositories section in order to apply to all repositories, `ANY REMOTE` for all remote repositories and `ANY LOCAL` for all local repositories. The default value will be `[]` if nothing is specified.
-        """
-        return pulumi.get(self, "repositories")
-
-    @property
-    @pulumi.getter
-    def actions(self) -> Optional['outputs.PermissionTargetsRepoActions']:
-        return pulumi.get(self, "actions")
-
-    @property
-    @pulumi.getter(name="excludesPatterns")
-    def excludes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to exclude.
-        """
-        return pulumi.get(self, "excludes_patterns")
-
-    @property
-    @pulumi.getter(name="includesPatterns")
-    def includes_patterns(self) -> Optional[Sequence[str]]:
-        """
-        Pattern of artifacts to include.
-        """
-        return pulumi.get(self, "includes_patterns")
-
-
-@pulumi.output_type
-class PermissionTargetsRepoActions(dict):
-    def __init__(__self__, *,
-                 groups: Optional[Sequence['outputs.PermissionTargetsRepoActionsGroup']] = None,
-                 users: Optional[Sequence['outputs.PermissionTargetsRepoActionsUser']] = None):
-        """
-        :param Sequence['PermissionTargetsRepoActionsGroupArgs'] groups: Groups this permission applies for.
-        :param Sequence['PermissionTargetsRepoActionsUserArgs'] users: Users this permission target applies for.
-        """
-        if groups is not None:
-            pulumi.set(__self__, "groups", groups)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
-
-    @property
-    @pulumi.getter
-    def groups(self) -> Optional[Sequence['outputs.PermissionTargetsRepoActionsGroup']]:
-        """
-        Groups this permission applies for.
-        """
-        return pulumi.get(self, "groups")
-
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[Sequence['outputs.PermissionTargetsRepoActionsUser']]:
-        """
-        Users this permission target applies for.
-        """
-        return pulumi.get(self, "users")
-
-
-@pulumi.output_type
-class PermissionTargetsRepoActionsGroup(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 permissions: Sequence[str]):
-        """
-        :param str name: Name of permission.
-        """
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "permissions", permissions)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Name of permission.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def permissions(self) -> Sequence[str]:
-        return pulumi.get(self, "permissions")
-
-
-@pulumi.output_type
-class PermissionTargetsRepoActionsUser(dict):
+class PermissionTargetRepoActionUser(dict):
     def __init__(__self__, *,
                  name: str,
                  permissions: Sequence[str]):
         """
         :param str name: Name of permission.
         """
         pulumi.set(__self__, "name", name)
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/permission_target.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/permission_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,217 +12,217 @@
 from ._inputs import *
 
 __all__ = ['PermissionTargetArgs', 'PermissionTarget']
 
 @pulumi.input_type
 class PermissionTargetArgs:
     def __init__(__self__, *,
-                 build: Optional[pulumi.Input['PermissionTargetBuildArgs']] = None,
+                 builds: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 release_bundle: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']] = None,
-                 repo: Optional[pulumi.Input['PermissionTargetRepoArgs']] = None):
+                 release_bundles: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]] = None,
+                 repos: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]] = None):
         """
         The set of arguments for constructing a PermissionTarget resource.
-        :param pulumi.Input['PermissionTargetBuildArgs'] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]] builds: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
-        :param pulumi.Input['PermissionTargetReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
-        :param pulumi.Input['PermissionTargetRepoArgs'] repo: Repository permission configuration.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]] release_bundles: As for repo for for release-bundles permissions.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]] repos: Repository permission configuration.
         """
-        if build is not None:
-            pulumi.set(__self__, "build", build)
+        if builds is not None:
+            pulumi.set(__self__, "builds", builds)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if release_bundle is not None:
-            pulumi.set(__self__, "release_bundle", release_bundle)
-        if repo is not None:
-            pulumi.set(__self__, "repo", repo)
+        if release_bundles is not None:
+            pulumi.set(__self__, "release_bundles", release_bundles)
+        if repos is not None:
+            pulumi.set(__self__, "repos", repos)
 
     @property
     @pulumi.getter
-    def build(self) -> Optional[pulumi.Input['PermissionTargetBuildArgs']]:
+    def builds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]]:
         """
         As for repo but for artifactory-build-info permissions.
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "builds")
 
-    @build.setter
-    def build(self, value: Optional[pulumi.Input['PermissionTargetBuildArgs']]):
-        pulumi.set(self, "build", value)
+    @builds.setter
+    def builds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]]):
+        pulumi.set(self, "builds", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Name of permission.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="releaseBundle")
-    def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]:
+    @pulumi.getter(name="releaseBundles")
+    def release_bundles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]]:
         """
         As for repo for for release-bundles permissions.
         """
-        return pulumi.get(self, "release_bundle")
+        return pulumi.get(self, "release_bundles")
 
-    @release_bundle.setter
-    def release_bundle(self, value: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]):
-        pulumi.set(self, "release_bundle", value)
+    @release_bundles.setter
+    def release_bundles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]]):
+        pulumi.set(self, "release_bundles", value)
 
     @property
     @pulumi.getter
-    def repo(self) -> Optional[pulumi.Input['PermissionTargetRepoArgs']]:
+    def repos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]]:
         """
         Repository permission configuration.
         """
-        return pulumi.get(self, "repo")
+        return pulumi.get(self, "repos")
 
-    @repo.setter
-    def repo(self, value: Optional[pulumi.Input['PermissionTargetRepoArgs']]):
-        pulumi.set(self, "repo", value)
+    @repos.setter
+    def repos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]]):
+        pulumi.set(self, "repos", value)
 
 
 @pulumi.input_type
 class _PermissionTargetState:
     def __init__(__self__, *,
-                 build: Optional[pulumi.Input['PermissionTargetBuildArgs']] = None,
+                 builds: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 release_bundle: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']] = None,
-                 repo: Optional[pulumi.Input['PermissionTargetRepoArgs']] = None):
+                 release_bundles: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]] = None,
+                 repos: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]] = None):
         """
         Input properties used for looking up and filtering PermissionTarget resources.
-        :param pulumi.Input['PermissionTargetBuildArgs'] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]] builds: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
-        :param pulumi.Input['PermissionTargetReleaseBundleArgs'] release_bundle: As for repo for for release-bundles permissions.
-        :param pulumi.Input['PermissionTargetRepoArgs'] repo: Repository permission configuration.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]] release_bundles: As for repo for for release-bundles permissions.
+        :param pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]] repos: Repository permission configuration.
         """
-        if build is not None:
-            pulumi.set(__self__, "build", build)
+        if builds is not None:
+            pulumi.set(__self__, "builds", builds)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if release_bundle is not None:
-            pulumi.set(__self__, "release_bundle", release_bundle)
-        if repo is not None:
-            pulumi.set(__self__, "repo", repo)
+        if release_bundles is not None:
+            pulumi.set(__self__, "release_bundles", release_bundles)
+        if repos is not None:
+            pulumi.set(__self__, "repos", repos)
 
     @property
     @pulumi.getter
-    def build(self) -> Optional[pulumi.Input['PermissionTargetBuildArgs']]:
+    def builds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]]:
         """
         As for repo but for artifactory-build-info permissions.
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "builds")
 
-    @build.setter
-    def build(self, value: Optional[pulumi.Input['PermissionTargetBuildArgs']]):
-        pulumi.set(self, "build", value)
+    @builds.setter
+    def builds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetBuildArgs']]]]):
+        pulumi.set(self, "builds", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Name of permission.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="releaseBundle")
-    def release_bundle(self) -> Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]:
+    @pulumi.getter(name="releaseBundles")
+    def release_bundles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]]:
         """
         As for repo for for release-bundles permissions.
         """
-        return pulumi.get(self, "release_bundle")
+        return pulumi.get(self, "release_bundles")
 
-    @release_bundle.setter
-    def release_bundle(self, value: Optional[pulumi.Input['PermissionTargetReleaseBundleArgs']]):
-        pulumi.set(self, "release_bundle", value)
+    @release_bundles.setter
+    def release_bundles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetReleaseBundleArgs']]]]):
+        pulumi.set(self, "release_bundles", value)
 
     @property
     @pulumi.getter
-    def repo(self) -> Optional[pulumi.Input['PermissionTargetRepoArgs']]:
+    def repos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]]:
         """
         Repository permission configuration.
         """
-        return pulumi.get(self, "repo")
+        return pulumi.get(self, "repos")
 
-    @repo.setter
-    def repo(self, value: Optional[pulumi.Input['PermissionTargetRepoArgs']]):
-        pulumi.set(self, "repo", value)
+    @repos.setter
+    def repos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PermissionTargetRepoArgs']]]]):
+        pulumi.set(self, "repos", value)
 
 
 class PermissionTarget(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 build: Optional[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]] = None,
+                 builds: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 release_bundle: Optional[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]] = None,
-                 repo: Optional[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]] = None,
+                 release_bundles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]]]] = None,
+                 repos: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]]]] = None,
                  __props__=None):
         """
         Provides an Artifactory permission target resource. This can be used to create and manage Artifactory permission targets.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory permission target called testpermission
         test_perm = artifactory.PermissionTarget("test-perm",
-            build=artifactory.PermissionTargetBuildArgs(
-                actions=artifactory.PermissionTargetBuildActionsArgs(
-                    users=[artifactory.PermissionTargetBuildActionsUserArgs(
+            builds=[artifactory.PermissionTargetBuildArgs(
+                actions=[artifactory.PermissionTargetBuildActionArgs(
+                    users=[artifactory.PermissionTargetBuildActionUserArgs(
                         name="anonymous",
                         permissions=[
                             "read",
                             "write",
                         ],
                     )],
-                ),
+                )],
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
-            ),
-            release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
-                actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
-                    users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
+            )],
+            release_bundles=[artifactory.PermissionTargetReleaseBundleArgs(
+                actions=[artifactory.PermissionTargetReleaseBundleActionArgs(
+                    users=[artifactory.PermissionTargetReleaseBundleActionUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
-                ),
+                )],
                 includes_patterns=["**"],
                 repositories=["release-bundles"],
-            ),
-            repo=artifactory.PermissionTargetRepoArgs(
-                actions=artifactory.PermissionTargetRepoActionsArgs(
-                    groups=[artifactory.PermissionTargetRepoActionsGroupArgs(
+            )],
+            repos=[artifactory.PermissionTargetRepoArgs(
+                actions=[artifactory.PermissionTargetRepoActionArgs(
+                    groups=[artifactory.PermissionTargetRepoActionGroupArgs(
                         name="readers",
                         permissions=["read"],
                     )],
-                    users=[artifactory.PermissionTargetRepoActionsUserArgs(
+                    users=[artifactory.PermissionTargetRepoActionUserArgs(
                         name="anonymous",
                         permissions=[
                             "read",
                             "write",
                         ],
                     )],
-                ),
+                )],
                 excludes_patterns=["bar/**"],
                 includes_patterns=["foo/**"],
                 repositories=["example-repo-local"],
-            ))
+            )])
         ```
         ## Permissions
 
         The provider supports the following `permission` enums:
 
         * `read`
         * `write`
@@ -248,18 +248,18 @@
 
         ```sh
          $ pulumi import artifactory:index/permissionTarget:PermissionTarget terraform-test-permission mypermission
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]]] builds: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']] repo: Repository permission configuration.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]]] release_bundles: As for repo for for release-bundles permissions.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]]] repos: Repository permission configuration.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[PermissionTargetArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -270,55 +270,55 @@
 
         ```python
         import pulumi
         import pulumi_artifactory as artifactory
 
         # Create a new Artifactory permission target called testpermission
         test_perm = artifactory.PermissionTarget("test-perm",
-            build=artifactory.PermissionTargetBuildArgs(
-                actions=artifactory.PermissionTargetBuildActionsArgs(
-                    users=[artifactory.PermissionTargetBuildActionsUserArgs(
+            builds=[artifactory.PermissionTargetBuildArgs(
+                actions=[artifactory.PermissionTargetBuildActionArgs(
+                    users=[artifactory.PermissionTargetBuildActionUserArgs(
                         name="anonymous",
                         permissions=[
                             "read",
                             "write",
                         ],
                     )],
-                ),
+                )],
                 includes_patterns=["**"],
                 repositories=["artifactory-build-info"],
-            ),
-            release_bundle=artifactory.PermissionTargetReleaseBundleArgs(
-                actions=artifactory.PermissionTargetReleaseBundleActionsArgs(
-                    users=[artifactory.PermissionTargetReleaseBundleActionsUserArgs(
+            )],
+            release_bundles=[artifactory.PermissionTargetReleaseBundleArgs(
+                actions=[artifactory.PermissionTargetReleaseBundleActionArgs(
+                    users=[artifactory.PermissionTargetReleaseBundleActionUserArgs(
                         name="anonymous",
                         permissions=["read"],
                     )],
-                ),
+                )],
                 includes_patterns=["**"],
                 repositories=["release-bundles"],
-            ),
-            repo=artifactory.PermissionTargetRepoArgs(
-                actions=artifactory.PermissionTargetRepoActionsArgs(
-                    groups=[artifactory.PermissionTargetRepoActionsGroupArgs(
+            )],
+            repos=[artifactory.PermissionTargetRepoArgs(
+                actions=[artifactory.PermissionTargetRepoActionArgs(
+                    groups=[artifactory.PermissionTargetRepoActionGroupArgs(
                         name="readers",
                         permissions=["read"],
                     )],
-                    users=[artifactory.PermissionTargetRepoActionsUserArgs(
+                    users=[artifactory.PermissionTargetRepoActionUserArgs(
                         name="anonymous",
                         permissions=[
                             "read",
                             "write",
                         ],
                     )],
-                ),
+                )],
                 excludes_patterns=["bar/**"],
                 includes_patterns=["foo/**"],
                 repositories=["example-repo-local"],
-            ))
+            )])
         ```
         ## Permissions
 
         The provider supports the following `permission` enums:
 
         * `read`
         * `write`
@@ -357,92 +357,92 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 build: Optional[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]] = None,
+                 builds: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 release_bundle: Optional[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]] = None,
-                 repo: Optional[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]] = None,
+                 release_bundles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]]]] = None,
+                 repos: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PermissionTargetArgs.__new__(PermissionTargetArgs)
 
-            __props__.__dict__["build"] = build
+            __props__.__dict__["builds"] = builds
             __props__.__dict__["name"] = name
-            __props__.__dict__["release_bundle"] = release_bundle
-            __props__.__dict__["repo"] = repo
+            __props__.__dict__["release_bundles"] = release_bundles
+            __props__.__dict__["repos"] = repos
         super(PermissionTarget, __self__).__init__(
             'artifactory:index/permissionTarget:PermissionTarget',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            build: Optional[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]] = None,
+            builds: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            release_bundle: Optional[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]] = None,
-            repo: Optional[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]] = None) -> 'PermissionTarget':
+            release_bundles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]]]] = None,
+            repos: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]]]] = None) -> 'PermissionTarget':
         """
         Get an existing PermissionTarget resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']] build: As for repo but for artifactory-build-info permissions.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetBuildArgs']]]] builds: As for repo but for artifactory-build-info permissions.
         :param pulumi.Input[str] name: Name of permission.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']] release_bundle: As for repo for for release-bundles permissions.
-        :param pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']] repo: Repository permission configuration.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetReleaseBundleArgs']]]] release_bundles: As for repo for for release-bundles permissions.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PermissionTargetRepoArgs']]]] repos: Repository permission configuration.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PermissionTargetState.__new__(_PermissionTargetState)
 
-        __props__.__dict__["build"] = build
+        __props__.__dict__["builds"] = builds
         __props__.__dict__["name"] = name
-        __props__.__dict__["release_bundle"] = release_bundle
-        __props__.__dict__["repo"] = repo
+        __props__.__dict__["release_bundles"] = release_bundles
+        __props__.__dict__["repos"] = repos
         return PermissionTarget(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def build(self) -> pulumi.Output[Optional['outputs.PermissionTargetBuild']]:
+    def builds(self) -> pulumi.Output[Optional[Sequence['outputs.PermissionTargetBuild']]]:
         """
         As for repo but for artifactory-build-info permissions.
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "builds")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Name of permission.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="releaseBundle")
-    def release_bundle(self) -> pulumi.Output[Optional['outputs.PermissionTargetReleaseBundle']]:
+    @pulumi.getter(name="releaseBundles")
+    def release_bundles(self) -> pulumi.Output[Optional[Sequence['outputs.PermissionTargetReleaseBundle']]]:
         """
         As for repo for for release-bundles permissions.
         """
-        return pulumi.get(self, "release_bundle")
+        return pulumi.get(self, "release_bundles")
 
     @property
     @pulumi.getter
-    def repo(self) -> pulumi.Output[Optional['outputs.PermissionTargetRepo']]:
+    def repos(self) -> pulumi.Output[Optional[Sequence['outputs.PermissionTargetRepo']]]:
         """
         Repository permission configuration.
         """
-        return pulumi.get(self, "repo")
+        return pulumi.get(self, "repos")
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/property_set.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/property_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/provider.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/proxy.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/pull_replication.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/pull_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/push_replication.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/push_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/release_bundle_webhook.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/release_bundle_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cargo_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cargo_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cocoapods_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cocoapods_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_go_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_go_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_maven_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_maven_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_opkg_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_opkg_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_p2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_repository_replication.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_repository_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_terraform_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/remote_vcs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/remote_vcs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/replication_config.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/repository_layout.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/repository_layout.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/saml_settings.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/saml_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/scoped_token.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/scoped_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
         """
         A list of the other instances or services that should accept this token identified by their Service-IDs. Limited to total 255 characters. Default to '*@*' if not set. Service ID must begin with valid JFrog service type. Options: jfrt, jfxr, jfpip, jfds, jfmc, jfac, jfevt, jfmd, jfcon, or *. For instructions to retrieve the Artifactory Service ID see this [documentation](https://jfrog.com/help/r/jfrog-rest-apis/get-service-id)
         """
         return pulumi.get(self, "audiences")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def description(self) -> pulumi.Output[str]:
         """
         Free text token description. Useful for filtering and managing tokens. Limited to 1024 characters.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="expiresIn")
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/single_replication_config.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/single_replication_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/unmanaged_user.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/unmanaged_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/user.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_alpine_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_alpine_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_bower_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_bower_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_chef_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_chef_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_composer_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_composer_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_conan_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_conan_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_conda_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_conda_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_cran_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_cran_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_debian_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_debian_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_docker_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_docker_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gems_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gems_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_generic_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_generic_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gitlfs_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gitlfs_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_gradle_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_gradle_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_helm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_helm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_ivy_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_ivy_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_npm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_npm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_nuget_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_nuget_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_p2_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_p2_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_pub_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_pub_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_puppet_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_puppet_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_pypi_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_rpm_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_rpm_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_sbt_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_sbt_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_swift_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_swift_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory/virtual_terraform_repository.py` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory/virtual_terraform_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/PKG-INFO` & `pulumi_artifactory-4.0.0a1687363033/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-artifactory
-Version: 3.6.0a1687054110
+Name: pulumi_artifactory
+Version: 4.0.0a1687363033
 Summary: A Pulumi package for creating and managing artifactory cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-artifactory
 Keywords: pulumi artifactory
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -42,15 +42,15 @@
 
     $ pip install pulumi_artifactory
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-artifactory/sdk/v7
+    $ go get github.com/pulumi/pulumi-artifactory/sdk/v4
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Artifactory
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/pulumi_artifactory.egg-info/SOURCES.txt` & `pulumi_artifactory-4.0.0a1687363033/pulumi_artifactory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,14 @@
 pulumi_artifactory/local_terraform_provider_repository.py
 pulumi_artifactory/local_vagrant_repository.py
 pulumi_artifactory/managed_user.py
 pulumi_artifactory/maven_repository.py
 pulumi_artifactory/oauth_settings.py
 pulumi_artifactory/outputs.py
 pulumi_artifactory/permission_target.py
-pulumi_artifactory/permission_targets.py
 pulumi_artifactory/property_set.py
 pulumi_artifactory/provider.py
 pulumi_artifactory/proxy.py
 pulumi_artifactory/pull_replication.py
 pulumi_artifactory/pulumi-plugin.json
 pulumi_artifactory/push_replication.py
 pulumi_artifactory/py.typed
```

### Comparing `pulumi_artifactory-3.6.0a1687054110/setup.py` & `pulumi_artifactory-4.0.0a1687363033/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.6.0a1687054110"
-PLUGIN_VERSION = "3.6.0-alpha.1687054110+9dd909c2"
+VERSION = "4.0.0a1687363033"
+PLUGIN_VERSION = "4.0.0-alpha.1687363033+27a7606c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'artifactory', PLUGIN_VERSION])
         except OSError as error:
```

