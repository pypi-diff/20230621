# Comparing `tmp/eClinical-1.0.8.4.tar.gz` & `tmp/eClinical-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\github\PyPackage\eClinical\dist\tmp8o7mdlam\eClinical-1.0.8.4.tar", last modified: Mon Jun 20 10:09:34 2022, max compression
+gzip compressed data, was "D:\github\PyPackage\eClinical\dist\tmp09jg0bot\eClinical-1.0.9.tar", last modified: Fri Jul  1 03:36:00 2022, max compression
```

## Comparing `eClinical-1.0.8.4.tar` & `eClinical-1.0.9.tar`

### file list

```diff
@@ -1,221 +1,236 @@
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.257695 eClinical-1.0.8.4/
--rw-rw-rw-   0        0        0     1073 2022-02-04 16:23:58.000000 eClinical-1.0.8.4/LICENSE
--rw-rw-rw-   0        0        0      884 2022-06-20 10:09:34.258666 eClinical-1.0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0      416 2022-05-11 03:28:13.000000 eClinical-1.0.8.4/README.md
--rw-rw-rw-   0        0        0      103 2022-02-04 17:03:06.000000 eClinical-1.0.8.4/pyproject.toml
--rw-rw-rw-   0        0        0      988 2022-06-20 10:09:34.264663 eClinical-1.0.8.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.703693 eClinical-1.0.8.4/src/
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.832960 eClinical-1.0.8.4/src/eClinical.egg-info/
--rw-rw-rw-   0        0        0      884 2022-06-20 10:09:30.000000 eClinical-1.0.8.4/src/eClinical.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8743 2022-06-20 10:09:32.000000 eClinical-1.0.8.4/src/eClinical.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-20 10:09:30.000000 eClinical-1.0.8.4/src/eClinical.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2022-06-20 10:09:31.000000 eClinical-1.0.8.4/src/eClinical.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2022-06-20 10:09:31.000000 eClinical-1.0.8.4/src/eClinical.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-20 10:09:32.000000 eClinical-1.0.8.4/src/eClinical.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.850965 eClinical-1.0.8.4/src/eclinical/
--rw-rw-rw-   0        0        0     1080 2022-03-04 03:38:21.000000 eClinical-1.0.8.4/src/eclinical/__init__.py
--rw-rw-rw-   0        0        0    14481 2022-03-17 10:51:16.000000 eClinical-1.0.8.4/src/eclinical/eclinical_cmd.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.881024 eClinical-1.0.8.4/src/eclinical/environment/
--rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/environment/__init__.py
--rw-rw-rw-   0        0        0     2109 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/environment/environment.py
--rw-rw-rw-   0        0        0      238 2022-03-04 03:38:21.000000 eClinical-1.0.8.4/src/eclinical/environment/function_environment.py
--rw-rw-rw-   0        0        0      232 2022-03-04 03:38:21.000000 eClinical-1.0.8.4/src/eclinical/environment/smoke_environment.py
--rw-rw-rw-   0        0        0     1106 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/execption.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.896024 eClinical-1.0.8.4/src/eclinical/record/
--rw-rw-rw-   0        0        0        0 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.928213 eClinical-1.0.8.4/src/eclinical/record/api_spec/
--rw-rw-rw-   0        0        0        0 2022-04-30 10:39:01.000000 eClinical-1.0.8.4/src/eclinical/record/api_spec/__init__.py
--rw-rw-rw-   0        0        0     1641 2022-04-30 11:05:19.000000 eClinical-1.0.8.4/src/eclinical/record/api_spec/api_spec.py
--rw-rw-rw-   0        0        0      779 2022-05-05 03:31:59.000000 eClinical-1.0.8.4/src/eclinical/record/api_spec/swagger.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.968023 eClinical-1.0.8.4/src/eclinical/record/ext/
--rw-rw-rw-   0        0        0        0 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:32.991023 eClinical-1.0.8.4/src/eclinical/record/ext/api/
--rw-rw-rw-   0        0        0        0 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/ext/api/__init__.py
--rw-rw-rw-   0        0        0     1886 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/ext/api/api_spec.py
--rw-rw-rw-   0        0        0     1301 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/ext/api/swagger.py
--rw-rw-rw-   0        0        0      808 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/ext/common.py
--rw-rw-rw-   0        0        0     2157 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/record/ext/eclinical_service.py
--rw-rw-rw-   0        0        0      600 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/ext/memcached.py
--rw-rw-rw-   0        0        0     1116 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/ext/proxy.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.018529 eClinical-1.0.8.4/src/eclinical/record/mitm/
--rw-rw-rw-   0        0        0        0 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/mitm/__init__.py
--rw-rw-rw-   0        0        0       69 2022-04-30 11:23:47.000000 eClinical-1.0.8.4/src/eclinical/record/mitm/mitm_addons.py
--rw-rw-rw-   0        0        0     1482 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/record/mitm/mitm_process.py
--rw-rw-rw-   0        0        0     1691 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/player.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.044236 eClinical-1.0.8.4/src/eclinical/record/view/
--rw-rw-rw-   0        0        0        0 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/view/__init__.py
--rw-rw-rw-   0        0        0     1344 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/view/alert_dialog.py
--rw-rw-rw-   0        0        0     8786 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/record/view/record_ui.py
--rw-rw-rw-   0        0        0      221 2022-04-30 10:38:37.000000 eClinical-1.0.8.4/src/eclinical/record/view/status.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.049132 eClinical-1.0.8.4/src/eclinical/scaffold/
--rw-rw-rw-   0        0        0        0 2022-04-02 03:22:04.000000 eClinical-1.0.8.4/src/eclinical/scaffold/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.077816 eClinical-1.0.8.4/src/eclinical/scaffold/command/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/__init__.py
--rw-rw-rw-   0        0        0     2220 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/ecl.py
--rw-rw-rw-   0        0        0     4535 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/edk.py
--rw-rw-rw-   0        0        0     1343 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/mc.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.094057 eClinical-1.0.8.4/src/eclinical/scaffold/command/resource/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/resource/__init__.py
--rw-rw-rw-   0        0        0      638 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/resource/global_conftest.txt
--rw-rw-rw-   0        0        0      402 2022-04-18 14:29:20.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/resource/init_environment.yaml
--rw-rw-rw-   0        0        0     1006 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/command/sc.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.117061 eClinical-1.0.8.4/src/eclinical/scaffold/files/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/files/__init__.py
--rw-rw-rw-   0        0        0     1830 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/files/gen_meta.py
--rw-rw-rw-   0        0        0     1447 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/files/gen_service.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.135062 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/__init__.py
--rw-rw-rw-   0        0        0      508 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/application.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.165261 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/component/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/component/__init__.py
--rw-rw-rw-   0        0        0      474 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/component/radio.py
--rw-rw-rw-   0        0        0      785 2022-04-18 14:29:20.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/component/text.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.196257 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/ecl/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/ecl/__init__.py
--rw-rw-rw-   0        0        0      281 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/ecl/module_name.py
--rw-rw-rw-   0        0        0      344 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/ecl/module_service.py
--rw-rw-rw-   0        0        0      406 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/ecl/module_type.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.296255 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/__init__.py
--rw-rw-rw-   0        0        0      279 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/account.py
--rw-rw-rw-   0        0        0      369 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/company.py
--rw-rw-rw-   0        0        0      272 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/db_host.py
--rw-rw-rw-   0        0        0      587 2022-05-11 03:17:07.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/eclinical_uri.py
--rw-rw-rw-   0        0        0      518 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/environment_name.py
--rw-rw-rw-   0        0        0      401 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/life_cycle.py
--rw-rw-rw-   0        0        0      282 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/pass_word.py
--rw-rw-rw-   0        0        0      398 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/port.py
--rw-rw-rw-   0        0        0      290 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/schema.py
--rw-rw-rw-   0        0        0      279 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/sponsor.py
--rw-rw-rw-   0        0        0      363 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/study.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.330254 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/__init__.py
--rw-rw-rw-   0        0        0      559 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/meta_attrs.py
--rw-rw-rw-   0        0        0      285 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/meta_name.py
--rw-rw-rw-   0        0        0      417 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/meta_service.py
--rw-rw-rw-   0        0        0      382 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/meta_type.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.347672 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/sc/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/sc/__init__.py
--rw-rw-rw-   0        0        0      291 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/inputs/sc/service_name.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.381946 eClinical-1.0.8.4/src/eclinical/scaffold/template/
--rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/template/__init__.py
--rw-rw-rw-   0        0        0     1157 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/template/file_operate.py
--rw-rw-rw-   0        0        0     1393 2022-04-02 06:14:33.000000 eClinical-1.0.8.4/src/eclinical/scaffold/template/meta.py
--rw-rw-rw-   0        0        0     3618 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/scaffold/template/service.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.513669 eClinical-1.0.8.4/src/eclinical/service/
--rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/service/__init__.py
--rw-rw-rw-   0        0        0     1945 2022-03-17 06:15:25.000000 eClinical-1.0.8.4/src/eclinical/service/_login_service.py
--rw-rw-rw-   0        0        0     2042 2022-04-08 11:41:25.000000 eClinical-1.0.8.4/src/eclinical/service/_sponsor_login_service.py
--rw-rw-rw-   0        0        0     1994 2022-04-08 11:41:25.000000 eClinical-1.0.8.4/src/eclinical/service/_study_login_service.py
--rw-rw-rw-   0        0        0      896 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/ctms_login_service.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.540700 eClinical-1.0.8.4/src/eclinical/service/data/
--rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/service/data/__init__.py
--rw-rw-rw-   0        0        0      770 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/service/data/_sponsor_login_data.py
--rw-rw-rw-   0        0        0     1091 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/service/data/_study_login_data.py
--rw-rw-rw-   0        0        0      569 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/design_login_service.py
--rw-rw-rw-   0        0        0      565 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/edc_login_service.py
--rw-rw-rw-   0        0        0     1122 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/service/ediary_login_service.py
--rw-rw-rw-   0        0        0      896 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/etmf_login_service.py
--rw-rw-rw-   0        0        0      568 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/iwrs_login_service.py
--rw-rw-rw-   0        0        0      528 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/portal_administrator_login_service.py
--rw-rw-rw-   0        0        0      540 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/portal_login_service.py
--rw-rw-rw-   0        0        0      886 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/service/pv_login_service.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.548699 eClinical-1.0.8.4/src/eclinical/standard/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.573701 eClinical-1.0.8.4/src/eclinical/standard/base/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/base/__init__.py
--rw-rw-rw-   0        0        0       94 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/base/container.py
--rw-rw-rw-   0        0        0      198 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/base/ok_response.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.590702 eClinical-1.0.8.4/src/eclinical/standard/design/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/design/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.618796 eClinical-1.0.8.4/src/eclinical/standard/design/dto/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/design/dto/__init__.py
--rw-rw-rw-   0        0        0      329 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/design/dto/archive_file.py
--rw-rw-rw-   0        0        0      354 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/design/dto/version_info.py
--rw-rw-rw-   0        0        0     1642 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/design/versioning.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.676758 eClinical-1.0.8.4/src/eclinical/standard/portal/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.859624 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/__init__.py
--rw-rw-rw-   0        0        0      742 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/company_envs.py
--rw-rw-rw-   0        0        0      600 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/envs.py
--rw-rw-rw-   0        0        0      868 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/group_user.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.885625 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/__init__.py
--rw-rw-rw-   0        0        0      823 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/node.py
--rw-rw-rw-   0        0        0      879 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/site.py
--rw-rw-rw-   0        0        0     1211 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/sponsor.py
--rw-rw-rw-   0        0        0     1088 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/study.py
--rw-rw-rw-   0        0        0     1966 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchy.py
--rw-rw-rw-   0        0        0      317 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/permission_tree.py
--rw-rw-rw-   0        0        0      215 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/query_sponsors.py
--rw-rw-rw-   0        0        0      740 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/query_studies.py
--rw-rw-rw-   0        0        0      773 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/query_user_groups.py
--rw-rw-rw-   0        0        0      758 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/querysponsors.py
--rw-rw-rw-   0        0        0      885 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/role_list.py
--rw-rw-rw-   0        0        0     1138 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/role_rel_user.py
--rw-rw-rw-   0        0        0      631 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/systems.py
--rw-rw-rw-   0        0        0      702 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_access.py
--rw-rw-rw-   0        0        0     1134 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_group_info.py
--rw-rw-rw-   0        0        0     1139 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_group_role_rel.py
--rw-rw-rw-   0        0        0      750 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_roles.py
--rw-rw-rw-   0        0        0      963 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/dto/users.py
--rw-rw-rw-   0        0        0     4850 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/hierarchies.py
--rw-rw-rw-   0        0        0     1899 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/role.py
--rw-rw-rw-   0        0        0     3858 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/user.py
--rw-rw-rw-   0        0        0     4920 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/user_groups.py
--rw-rw-rw-   0        0        0     2368 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/portal/user_role.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.895626 eClinical-1.0.8.4/src/eclinical/standard/steps/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.900624 eClinical-1.0.8.4/src/eclinical/standard/steps/design/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/design/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.951664 eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/__init__.py
--rw-rw-rw-   0        0        0      972 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_download_publish_sql.py
--rw-rw-rw-   0        0        0      953 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_fileids.py
--rw-rw-rw-   0        0        0      846 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_get_last_version.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:33.968700 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.045666 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/__init__.py
--rw-rw-rw-   0        0        0      984 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_create_sponsor.py
--rw-rw-rw-   0        0        0     1296 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_create_study.py
--rw-rw-rw-   0        0        0     1328 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_find_sponsor.py
--rw-rw-rw-   0        0        0     1344 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_find_study.py
--rw-rw-rw-   0        0        0     1397 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_sponsor_no_start.py
--rw-rw-rw-   0        0        0     1428 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_startup_sponsor.py
--rw-rw-rw-   0        0        0     1363 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_startup_study.py
--rw-rw-rw-   0        0        0     1379 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_study_no_start.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.076668 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/__init__.py
--rw-rw-rw-   0        0        0     1108 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_create_role.py
--rw-rw-rw-   0        0        0      919 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_find_role.py
--rw-rw-rw-   0        0        0     1337 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_get_permission_tree.py
--rw-rw-rw-   0        0        0     1223 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_set_permissions.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.131665 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/__init__.py
--rw-rw-rw-   0        0        0     1128 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_associated_usergroup.py
--rw-rw-rw-   0        0        0     1312 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_create_user.py
--rw-rw-rw-   0        0        0      872 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_find_user.py
--rw-rw-rw-   0        0        0      801 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_find_user_role.py
--rw-rw-rw-   0        0        0     1093 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_study_title.py
--rw-rw-rw-   0        0        0     1140 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_user_access.py
--rw-rw-rw-   0        0        0     2254 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_user_append_usergroup.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.206705 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_add_group_user.py
--rw-rw-rw-   0        0        0     1284 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_create_usergroup.py
--rw-rw-rw-   0        0        0     1308 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_find_un_added_user.py
--rw-rw-rw-   0        0        0      965 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_find_usergroup.py
--rw-rw-rw-   0        0        0      993 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_get_company_envs.py
--rw-rw-rw-   0        0        0     1991 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_get_lifecycle_hierarchies.py
--rw-rw-rw-   0        0        0     1364 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_get_user_group_info.py
--rw-rw-rw-   0        0        0      868 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_life_cycle.py
--rw-rw-rw-   0        0        0     2657 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_set_lifecycle_hierarchies.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.231664 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/
--rw-rw-rw-   0        0        0        0 2022-06-20 10:07:08.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/__init__.py
--rw-rw-rw-   0        0        0      907 2022-06-20 10:07:09.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/portal_find_no_rel_user.py
--rw-rw-rw-   0        0        0     1017 2022-06-20 10:07:09.000000 eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/portal_get_user_role.py
-drwxrwxrwx   0        0        0        0 2022-06-20 10:09:34.246664 eClinical-1.0.8.4/src/eclinical/utils/
--rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.8.4/src/eclinical/utils/__init__.py
--rw-rw-rw-   0        0        0      697 2022-03-17 06:26:43.000000 eClinical-1.0.8.4/src/eclinical/utils/ecrypto.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.364421 eClinical-1.0.9/
+-rw-rw-rw-   0        0        0     1073 2022-02-04 16:23:58.000000 eClinical-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      945 2022-07-01 03:36:00.366418 eClinical-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2022-07-01 03:31:49.000000 eClinical-1.0.9/README.md
+-rw-rw-rw-   0        0        0      103 2022-02-04 17:03:06.000000 eClinical-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      986 2022-07-01 03:36:00.370948 eClinical-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.422279 eClinical-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.607283 eClinical-1.0.9/src/eClinical.egg-info/
+-rw-rw-rw-   0        0        0      945 2022-07-01 03:35:57.000000 eClinical-1.0.9/src/eClinical.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9377 2022-07-01 03:35:58.000000 eClinical-1.0.9/src/eClinical.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-01 03:35:57.000000 eClinical-1.0.9/src/eClinical.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      230 2022-07-01 03:35:57.000000 eClinical-1.0.9/src/eClinical.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2022-07-01 03:35:57.000000 eClinical-1.0.9/src/eClinical.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-07-01 03:35:57.000000 eClinical-1.0.9/src/eClinical.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.633290 eClinical-1.0.9/src/eclinical/
+-rw-rw-rw-   0        0        0     1080 2022-03-04 03:38:21.000000 eClinical-1.0.9/src/eclinical/__init__.py
+-rw-rw-rw-   0        0        0    14481 2022-03-17 10:51:16.000000 eClinical-1.0.9/src/eclinical/eclinical_cmd.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.666283 eClinical-1.0.9/src/eclinical/environment/
+-rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/environment/__init__.py
+-rw-rw-rw-   0        0        0     2109 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/environment/environment.py
+-rw-rw-rw-   0        0        0      238 2022-03-04 03:38:21.000000 eClinical-1.0.9/src/eclinical/environment/function_environment.py
+-rw-rw-rw-   0        0        0      232 2022-03-04 03:38:21.000000 eClinical-1.0.9/src/eclinical/environment/smoke_environment.py
+-rw-rw-rw-   0        0        0     1106 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/execption.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.682935 eClinical-1.0.9/src/eclinical/record/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.703463 eClinical-1.0.9/src/eclinical/record/api_spec/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/api_spec/__init__.py
+-rw-rw-rw-   0        0        0     1641 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/api_spec/api_spec.py
+-rw-rw-rw-   0        0        0      778 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/api_spec/swagger.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.737461 eClinical-1.0.9/src/eclinical/record/ext/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.760464 eClinical-1.0.9/src/eclinical/record/ext/api/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/api/__init__.py
+-rw-rw-rw-   0        0        0     1886 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/api/api_spec.py
+-rw-rw-rw-   0        0        0     1301 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/api/swagger.py
+-rw-rw-rw-   0        0        0      808 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/common.py
+-rw-rw-rw-   0        0        0     2157 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/eclinical_service.py
+-rw-rw-rw-   0        0        0      600 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/memcached.py
+-rw-rw-rw-   0        0        0     1116 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/ext/proxy.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.781462 eClinical-1.0.9/src/eclinical/record/mitm/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/mitm/__init__.py
+-rw-rw-rw-   0        0        0       69 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/mitm/mitm_addons.py
+-rw-rw-rw-   0        0        0     1482 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/mitm/mitm_process.py
+-rw-rw-rw-   0        0        0     1691 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/player.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.808463 eClinical-1.0.9/src/eclinical/record/view/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/view/__init__.py
+-rw-rw-rw-   0        0        0     1344 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/view/alert_dialog.py
+-rw-rw-rw-   0        0        0     8786 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/view/record_ui.py
+-rw-rw-rw-   0        0        0      221 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/record/view/status.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.816461 eClinical-1.0.9/src/eclinical/scaffold/
+-rw-rw-rw-   0        0        0        0 2022-04-02 03:22:04.000000 eClinical-1.0.9/src/eclinical/scaffold/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.890467 eClinical-1.0.9/src/eclinical/scaffold/command/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/__init__.py
+-rw-rw-rw-   0        0        0     2220 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/ecl.py
+-rw-rw-rw-   0        0        0     4535 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/scaffold/command/edk.py
+-rw-rw-rw-   0        0        0     1343 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/mc.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.915465 eClinical-1.0.9/src/eclinical/scaffold/command/resource/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/resource/__init__.py
+-rw-rw-rw-   0        0        0      638 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/resource/global_conftest.txt
+-rw-rw-rw-   0        0        0      402 2022-04-18 14:29:20.000000 eClinical-1.0.9/src/eclinical/scaffold/command/resource/init_environment.yaml
+-rw-rw-rw-   0        0        0     1006 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/command/sc.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.934462 eClinical-1.0.9/src/eclinical/scaffold/files/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/files/__init__.py
+-rw-rw-rw-   0        0        0     1830 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/files/gen_meta.py
+-rw-rw-rw-   0        0        0     1447 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/files/gen_service.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.947466 eClinical-1.0.9/src/eclinical/scaffold/inputs/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/__init__.py
+-rw-rw-rw-   0        0        0      508 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/application.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.967463 eClinical-1.0.9/src/eclinical/scaffold/inputs/component/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/component/__init__.py
+-rw-rw-rw-   0        0        0      474 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/component/radio.py
+-rw-rw-rw-   0        0        0      785 2022-04-18 14:29:20.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/component/text.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:58.999471 eClinical-1.0.9/src/eclinical/scaffold/inputs/ecl/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/ecl/__init__.py
+-rw-rw-rw-   0        0        0      281 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/ecl/module_name.py
+-rw-rw-rw-   0        0        0      344 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/ecl/module_service.py
+-rw-rw-rw-   0        0        0      406 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/ecl/module_type.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.083464 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/__init__.py
+-rw-rw-rw-   0        0        0      279 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/account.py
+-rw-rw-rw-   0        0        0      369 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/company.py
+-rw-rw-rw-   0        0        0      272 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/db_host.py
+-rw-rw-rw-   0        0        0      587 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/eclinical_uri.py
+-rw-rw-rw-   0        0        0      518 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/environment_name.py
+-rw-rw-rw-   0        0        0      401 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/life_cycle.py
+-rw-rw-rw-   0        0        0      282 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/pass_word.py
+-rw-rw-rw-   0        0        0      398 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/port.py
+-rw-rw-rw-   0        0        0      290 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/schema.py
+-rw-rw-rw-   0        0        0      279 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/sponsor.py
+-rw-rw-rw-   0        0        0      363 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/study.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.118462 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/__init__.py
+-rw-rw-rw-   0        0        0      559 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/meta_attrs.py
+-rw-rw-rw-   0        0        0      285 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/meta_name.py
+-rw-rw-rw-   0        0        0      417 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/meta_service.py
+-rw-rw-rw-   0        0        0      382 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/meta_type.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.130471 eClinical-1.0.9/src/eclinical/scaffold/inputs/sc/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/sc/__init__.py
+-rw-rw-rw-   0        0        0      291 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/inputs/sc/service_name.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.171467 eClinical-1.0.9/src/eclinical/scaffold/template/
+-rw-rw-rw-   0        0        0        0 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/template/__init__.py
+-rw-rw-rw-   0        0        0     1157 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/template/file_operate.py
+-rw-rw-rw-   0        0        0     1393 2022-04-02 06:14:33.000000 eClinical-1.0.9/src/eclinical/scaffold/template/meta.py
+-rw-rw-rw-   0        0        0     3618 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/scaffold/template/service.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.331994 eClinical-1.0.9/src/eclinical/service/
+-rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/service/__init__.py
+-rw-rw-rw-   0        0        0     1945 2022-03-17 06:15:25.000000 eClinical-1.0.9/src/eclinical/service/_login_service.py
+-rw-rw-rw-   0        0        0     2042 2022-04-08 11:41:25.000000 eClinical-1.0.9/src/eclinical/service/_sponsor_login_service.py
+-rw-rw-rw-   0        0        0     1994 2022-04-08 11:41:25.000000 eClinical-1.0.9/src/eclinical/service/_study_login_service.py
+-rw-rw-rw-   0        0        0      896 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/ctms_login_service.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.353995 eClinical-1.0.9/src/eclinical/service/data/
+-rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/service/data/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/service/data/_sponsor_login_data.py
+-rw-rw-rw-   0        0        0     1091 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/service/data/_study_login_data.py
+-rw-rw-rw-   0        0        0      569 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/design_login_service.py
+-rw-rw-rw-   0        0        0      565 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/edc_login_service.py
+-rw-rw-rw-   0        0        0     1122 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/service/ediary_login_service.py
+-rw-rw-rw-   0        0        0      896 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/etmf_login_service.py
+-rw-rw-rw-   0        0        0      568 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/iwrs_login_service.py
+-rw-rw-rw-   0        0        0      528 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/portal_administrator_login_service.py
+-rw-rw-rw-   0        0        0      540 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/portal_login_service.py
+-rw-rw-rw-   0        0        0      886 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/service/pv_login_service.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.360005 eClinical-1.0.9/src/eclinical/standard/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.385993 eClinical-1.0.9/src/eclinical/standard/base/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/base/__init__.py
+-rw-rw-rw-   0        0        0       94 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/base/container.py
+-rw-rw-rw-   0        0        0      198 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/base/ok_response.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.402990 eClinical-1.0.9/src/eclinical/standard/ctms/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/__init__.py
+-rw-rw-rw-   0        0        0     4722 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/ctms_api.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.448002 eClinical-1.0.9/src/eclinical/standard/ctms/dto/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/__init__.py
+-rw-rw-rw-   0        0        0      618 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/country.py
+-rw-rw-rw-   0        0        0      312 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/menus.py
+-rw-rw-rw-   0        0        0      768 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/site_entities.py
+-rw-rw-rw-   0        0        0      981 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/sites_of_study.py
+-rw-rw-rw-   0        0        0      738 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/ctms/dto/studies.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.462036 eClinical-1.0.9/src/eclinical/standard/design/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/design/__init__.py
+-rw-rw-rw-   0        0        0     1642 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/design/design_api.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.545628 eClinical-1.0.9/src/eclinical/standard/design/dto/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/design/dto/__init__.py
+-rw-rw-rw-   0        0        0      329 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/design/dto/archive_file.py
+-rw-rw-rw-   0        0        0      354 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/design/dto/version_info.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.557611 eClinical-1.0.9/src/eclinical/standard/portal/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.691608 eClinical-1.0.9/src/eclinical/standard/portal/dto/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/__init__.py
+-rw-rw-rw-   0        0        0      742 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/company_envs.py
+-rw-rw-rw-   0        0        0      600 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/envs.py
+-rw-rw-rw-   0        0        0      868 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/group_user.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.735133 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/__init__.py
+-rw-rw-rw-   0        0        0      823 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/node.py
+-rw-rw-rw-   0        0        0      879 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/site.py
+-rw-rw-rw-   0        0        0     1211 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/sponsor.py
+-rw-rw-rw-   0        0        0     1088 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/study.py
+-rw-rw-rw-   0        0        0     1966 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchy.py
+-rw-rw-rw-   0        0        0      317 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/permission_tree.py
+-rw-rw-rw-   0        0        0      740 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/query_studies.py
+-rw-rw-rw-   0        0        0      773 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/query_user_groups.py
+-rw-rw-rw-   0        0        0      758 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/querysponsors.py
+-rw-rw-rw-   0        0        0      885 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/role_list.py
+-rw-rw-rw-   0        0        0     1138 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/role_rel_user.py
+-rw-rw-rw-   0        0        0      631 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/systems.py
+-rw-rw-rw-   0        0        0      702 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/user_access.py
+-rw-rw-rw-   0        0        0     1134 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/user_group_info.py
+-rw-rw-rw-   0        0        0     1139 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/user_group_role_rel.py
+-rw-rw-rw-   0        0        0      750 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/user_roles.py
+-rw-rw-rw-   0        0        0      963 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/dto/users.py
+-rw-rw-rw-   0        0        0    14362 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/portal/portal_api.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.741132 eClinical-1.0.9/src/eclinical/standard/steps/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.818132 eClinical-1.0.9/src/eclinical/standard/steps/ctms/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/__init__.py
+-rw-rw-rw-   0        0        0      715 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_all_menu.py
+-rw-rw-rw-   0        0        0     1040 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_common_country.py
+-rw-rw-rw-   0        0        0     2547 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_create_site_entity.py
+-rw-rw-rw-   0        0        0     1453 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_find_site.py
+-rw-rw-rw-   0        0        0      716 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_find_study.py
+-rw-rw-rw-   0        0        0     1057 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_find_study_site.py
+-rw-rw-rw-   0        0        0     1615 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_study_set_site.py
+-rw-rw-rw-   0        0        0     1457 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_submit_study_basic_info.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.825133 eClinical-1.0.9/src/eclinical/standard/steps/design/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/design/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.908661 eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/__init__.py
+-rw-rw-rw-   0        0        0      931 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/design_download_publish_sql.py
+-rw-rw-rw-   0        0        0      877 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/design_fileids.py
+-rw-rw-rw-   0        0        0      807 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/design_get_last_version.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.917657 eClinical-1.0.9/src/eclinical/standard/steps/portal/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:35:59.992658 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/__init__.py
+-rw-rw-rw-   0        0        0      881 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_create_sponsor.py
+-rw-rw-rw-   0        0        0     1184 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_create_study.py
+-rw-rw-rw-   0        0        0     1214 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_find_sponsor.py
+-rw-rw-rw-   0        0        0     1236 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_find_study.py
+-rw-rw-rw-   0        0        0     1285 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_sponsor_no_start.py
+-rw-rw-rw-   0        0        0     1318 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_startup_sponsor.py
+-rw-rw-rw-   0        0        0     1251 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_startup_study.py
+-rw-rw-rw-   0        0        0     1267 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_study_no_start.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.049663 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/__init__.py
+-rw-rw-rw-   0        0        0     1021 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_create_role.py
+-rw-rw-rw-   0        0        0      823 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_find_role.py
+-rw-rw-rw-   0        0        0     1239 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_get_permission_tree.py
+-rw-rw-rw-   0        0        0     1127 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_set_permissions.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.127667 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/__init__.py
+-rw-rw-rw-   0        0        0     1028 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_associated_usergroup.py
+-rw-rw-rw-   0        0        0     1225 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_create_user.py
+-rw-rw-rw-   0        0        0      776 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_find_user.py
+-rw-rw-rw-   0        0        0      703 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_find_user_role.py
+-rw-rw-rw-   0        0        0     1041 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_study_title.py
+-rw-rw-rw-   0        0        0     1053 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_user_access.py
+-rw-rw-rw-   0        0        0     2096 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_user_append_usergroup.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.300657 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/__init__.py
+-rw-rw-rw-   0        0        0      991 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_add_group_user.py
+-rw-rw-rw-   0        0        0     1197 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_create_usergroup.py
+-rw-rw-rw-   0        0        0     1113 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_find_un_added_user.py
+-rw-rw-rw-   0        0        0      854 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_find_usergroup.py
+-rw-rw-rw-   0        0        0      854 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_get_company_envs.py
+-rw-rw-rw-   0        0        0     1880 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_get_lifecycle_hierarchies.py
+-rw-rw-rw-   0        0        0     1153 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_get_user_group_info.py
+-rw-rw-rw-   0        0        0      754 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_life_cycle.py
+-rw-rw-rw-   0        0        0     2540 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_set_lifecycle_hierarchies.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.340307 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_roles/
+-rw-rw-rw-   0        0        0        0 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_roles/__init__.py
+-rw-rw-rw-   0        0        0     1265 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_roles/portal_find_no_rel_user.py
+-rw-rw-rw-   0        0        0      934 2022-07-01 03:30:38.000000 eClinical-1.0.9/src/eclinical/standard/steps/portal/user_roles/portal_get_user_role.py
+drwxrwxrwx   0        0        0        0 2022-07-01 03:36:00.355892 eClinical-1.0.9/src/eclinical/utils/
+-rw-rw-rw-   0        0        0        0 2022-03-03 10:16:08.000000 eClinical-1.0.9/src/eclinical/utils/__init__.py
+-rw-rw-rw-   0        0        0      697 2022-03-17 06:26:43.000000 eClinical-1.0.9/src/eclinical/utils/ecrypto.py
```

### Comparing `eClinical-1.0.8.4/LICENSE` & `eClinical-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/PKG-INFO` & `eClinical-1.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eClinical
-Version: 1.0.8.4
+Version: 1.0.9
 Summary: 内部工具类
 Home-page: https://github.com/xxxx
 Author: thcpc
 Author-email: pengcheng.chen@edetek.com
 Project-URL: Bug Tracker, https://github.com/xxxx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,7 +22,8 @@
  * @FilePath: \PyPackage\cjen\README.md
 -->
 
 公司使用内部工具类
 
 - 1.0.5 加入第一版脚手架
 - 1.0.8.2 修改了内置的url
+- 1.0.8.9 提供了一步创建sponsor,study,site的工具类
```

### Comparing `eClinical-1.0.8.4/setup.cfg` & `eClinical-1.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 436c 696e 6963 616c 0d0a 7665   = eClinical..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 382e 340d  rsion = 1.0.8.4.
-00000030: 0a61 7574 686f 7220 3d20 7468 6370 630d  .author = thcpc.
-00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 7065 6e67 6368 656e 672e 6368 656e 4065  pengcheng.chen@e
-00000060: 6465 7465 6b2e 636f 6d0d 0a64 6573 6372  detek.com..descr
-00000070: 6970 7469 6f6e 203d 20e5 8685 e983 a8e5  iption = .......
-00000080: b7a5 e585 b7e7 b1bb 0d0a 6c6f 6e67 5f64  ..........long_d
-00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000a0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000c0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000d0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-000000e0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000000f0: 622e 636f 6d2f 7878 7878 0d0a 7072 6f6a  b.com/xxxx..proj
-00000100: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
-00000110: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f78  s://github.com/x
-00000130: 7878 780d 0a63 6c61 7373 6966 6965 7273  xxx..classifiers
-00000140: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-00000150: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000160: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
-00000170: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000180: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000190: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-000001a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001b0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
-000001c0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-000001d0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-000001e0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-000001f0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000200: 6461 7461 203d 2046 616c 7365 0d0a 696e  data = False..in
-00000210: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000220: 200d 0a09 636a 656e 0d0a 0970 7963 7279   ...cjen...pycry
-00000230: 7074 6f64 6f6d 650d 0a70 7974 686f 6e5f  ptodome..python_
-00000240: 7265 7175 6972 6573 203d 203e 3d33 2e39  requires = >=3.9
-00000250: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000260: 6b61 6765 5f64 6174 615d 0d0a 2a20 3d20  kage_data]..* = 
-00000270: 2a2e 7961 6d6c 2c2a 2e74 7874 0d0a 0d0a  *.yaml,*.txt....
-00000280: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000290: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000002a0: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
-000002b0: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-000002c0: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-000002d0: 3d20 0d0a 0965 646b 203d 2065 636c 696e  = ...edk = eclin
-000002e0: 6963 616c 2e73 6361 6666 6f6c 642e 636f  ical.scaffold.co
-000002f0: 6d6d 616e 642e 6564 6b3a 6564 6b5f 636f  mmand.edk:edk_co
-00000300: 6d6d 616e 640d 0a09 6564 6b2d 6d6f 6475  mmand...edk-modu
-00000310: 6c65 203d 2065 636c 696e 6963 616c 2e73  le = eclinical.s
-00000320: 6361 6666 6f6c 642e 636f 6d6d 616e 642e  caffold.command.
-00000330: 6563 6c3a 6563 6c5f 636f 6d6d 616e 640d  ecl:ecl_command.
-00000340: 0a09 6564 6b2d 7365 7276 6963 6520 3d20  ..edk-service = 
-00000350: 6563 6c69 6e69 6361 6c2e 7363 6166 666f  eclinical.scaffo
-00000360: 6c64 2e63 6f6d 6d61 6e64 2e73 633a 7363  ld.command.sc:sc
-00000370: 5f63 6f6d 6d61 6e64 0d0a 0965 646b 2d6d  _command...edk-m
-00000380: 6574 6120 3d20 6563 6c69 6e69 6361 6c2e  eta = eclinical.
-00000390: 7363 6166 666f 6c64 2e63 6f6d 6d61 6e64  scaffold.command
-000003a0: 2e6d 633a 6d63 5f63 6f6d 6d61 6e64 0d0a  .mc:mc_command..
-000003b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000003d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 7273 696f 6e20 3d20 312e 302e 390d 0a61  rsion = 1.0.9..a
+00000030: 7574 686f 7220 3d20 7468 6370 630d 0a61  uthor = thcpc..a
+00000040: 7574 686f 725f 656d 6169 6c20 3d20 7065  uthor_email = pe
+00000050: 6e67 6368 656e 672e 6368 656e 4065 6465  ngcheng.chen@ede
+00000060: 7465 6b2e 636f 6d0d 0a64 6573 6372 6970  tek.com..descrip
+00000070: 7469 6f6e 203d 20e5 8685 e983 a8e5 b7a5  tion = .........
+00000080: e585 b7e7 b1bb 0d0a 6c6f 6e67 5f64 6573  ........long_des
+00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000a0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+000000b0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000c0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+000000d0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
+000000e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000f0: 636f 6d2f 7878 7878 0d0a 7072 6f6a 6563  com/xxxx..projec
+00000100: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
+00000110: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f78 7878  //github.com/xxx
+00000130: 780d 0a63 6c61 7373 6966 6965 7273 203d  x..classifiers =
+00000140: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+00000150: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000160: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+00000170: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000180: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000190: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000001a0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000001b0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+000001c0: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+000001d0: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+000001e0: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+000001f0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000200: 7461 203d 2046 616c 7365 0d0a 696e 7374  ta = False..inst
+00000210: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000220: 0a09 636a 656e 0d0a 0970 7963 7279 7074  ..cjen...pycrypt
+00000230: 6f64 6f6d 650d 0a70 7974 686f 6e5f 7265  odome..python_re
+00000240: 7175 6972 6573 203d 203e 3d33 2e39 0d0a  quires = >=3.9..
+00000250: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000260: 6765 5f64 6174 615d 0d0a 2a20 3d20 2a2e  ge_data]..* = *.
+00000270: 7961 6d6c 2c2a 2e74 7874 0d0a 0d0a 5b6f  yaml,*.txt....[o
+00000280: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000290: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000002a0: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
+000002b0: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
+000002c0: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
+000002d0: 0d0a 0965 646b 203d 2065 636c 696e 6963  ...edk = eclinic
+000002e0: 616c 2e73 6361 6666 6f6c 642e 636f 6d6d  al.scaffold.comm
+000002f0: 616e 642e 6564 6b3a 6564 6b5f 636f 6d6d  and.edk:edk_comm
+00000300: 616e 640d 0a09 6564 6b2d 6d6f 6475 6c65  and...edk-module
+00000310: 203d 2065 636c 696e 6963 616c 2e73 6361   = eclinical.sca
+00000320: 6666 6f6c 642e 636f 6d6d 616e 642e 6563  ffold.command.ec
+00000330: 6c3a 6563 6c5f 636f 6d6d 616e 640d 0a09  l:ecl_command...
+00000340: 6564 6b2d 7365 7276 6963 6520 3d20 6563  edk-service = ec
+00000350: 6c69 6e69 6361 6c2e 7363 6166 666f 6c64  linical.scaffold
+00000360: 2e63 6f6d 6d61 6e64 2e73 633a 7363 5f63  .command.sc:sc_c
+00000370: 6f6d 6d61 6e64 0d0a 0965 646b 2d6d 6574  ommand...edk-met
+00000380: 6120 3d20 6563 6c69 6e69 6361 6c2e 7363  a = eclinical.sc
+00000390: 6166 666f 6c64 2e63 6f6d 6d61 6e64 2e6d  affold.command.m
+000003a0: 633a 6d63 5f63 6f6d 6d61 6e64 0d0a 0d0a  c:mc_command....
+000003b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000003c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000003d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `eClinical-1.0.8.4/src/eClinical.egg-info/PKG-INFO` & `eClinical-1.0.9/src/eClinical.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eClinical
-Version: 1.0.8.4
+Version: 1.0.9
 Summary: 内部工具类
 Home-page: https://github.com/xxxx
 Author: thcpc
 Author-email: pengcheng.chen@edetek.com
 Project-URL: Bug Tracker, https://github.com/xxxx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,7 +22,8 @@
  * @FilePath: \PyPackage\cjen\README.md
 -->
 
 公司使用内部工具类
 
 - 1.0.5 加入第一版脚手架
 - 1.0.8.2 修改了内置的url
+- 1.0.8.9 提供了一步创建sponsor,study,site的工具类
```

### Comparing `eClinical-1.0.8.4/src/eClinical.egg-info/SOURCES.txt` & `eClinical-1.0.9/src/eClinical.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -95,32 +95,35 @@
 src/eclinical/service/data/__init__.py
 src/eclinical/service/data/_sponsor_login_data.py
 src/eclinical/service/data/_study_login_data.py
 src/eclinical/standard/__init__.py
 src/eclinical/standard/base/__init__.py
 src/eclinical/standard/base/container.py
 src/eclinical/standard/base/ok_response.py
+src/eclinical/standard/ctms/__init__.py
+src/eclinical/standard/ctms/ctms_api.py
+src/eclinical/standard/ctms/dto/__init__.py
+src/eclinical/standard/ctms/dto/country.py
+src/eclinical/standard/ctms/dto/menus.py
+src/eclinical/standard/ctms/dto/site_entities.py
+src/eclinical/standard/ctms/dto/sites_of_study.py
+src/eclinical/standard/ctms/dto/studies.py
 src/eclinical/standard/design/__init__.py
-src/eclinical/standard/design/versioning.py
+src/eclinical/standard/design/design_api.py
 src/eclinical/standard/design/dto/__init__.py
 src/eclinical/standard/design/dto/archive_file.py
 src/eclinical/standard/design/dto/version_info.py
 src/eclinical/standard/portal/__init__.py
-src/eclinical/standard/portal/hierarchies.py
-src/eclinical/standard/portal/role.py
-src/eclinical/standard/portal/user.py
-src/eclinical/standard/portal/user_groups.py
-src/eclinical/standard/portal/user_role.py
+src/eclinical/standard/portal/portal_api.py
 src/eclinical/standard/portal/dto/__init__.py
 src/eclinical/standard/portal/dto/company_envs.py
 src/eclinical/standard/portal/dto/envs.py
 src/eclinical/standard/portal/dto/group_user.py
 src/eclinical/standard/portal/dto/hierarchy.py
 src/eclinical/standard/portal/dto/permission_tree.py
-src/eclinical/standard/portal/dto/query_sponsors.py
 src/eclinical/standard/portal/dto/query_studies.py
 src/eclinical/standard/portal/dto/query_user_groups.py
 src/eclinical/standard/portal/dto/querysponsors.py
 src/eclinical/standard/portal/dto/role_list.py
 src/eclinical/standard/portal/dto/role_rel_user.py
 src/eclinical/standard/portal/dto/systems.py
 src/eclinical/standard/portal/dto/user_access.py
@@ -130,14 +133,23 @@
 src/eclinical/standard/portal/dto/users.py
 src/eclinical/standard/portal/dto/hierarchies/__init__.py
 src/eclinical/standard/portal/dto/hierarchies/node.py
 src/eclinical/standard/portal/dto/hierarchies/site.py
 src/eclinical/standard/portal/dto/hierarchies/sponsor.py
 src/eclinical/standard/portal/dto/hierarchies/study.py
 src/eclinical/standard/steps/__init__.py
+src/eclinical/standard/steps/ctms/__init__.py
+src/eclinical/standard/steps/ctms/ctms_all_menu.py
+src/eclinical/standard/steps/ctms/ctms_common_country.py
+src/eclinical/standard/steps/ctms/ctms_create_site_entity.py
+src/eclinical/standard/steps/ctms/ctms_find_site.py
+src/eclinical/standard/steps/ctms/ctms_find_study.py
+src/eclinical/standard/steps/ctms/ctms_find_study_site.py
+src/eclinical/standard/steps/ctms/ctms_study_set_site.py
+src/eclinical/standard/steps/ctms/ctms_submit_study_basic_info.py
 src/eclinical/standard/steps/design/__init__.py
 src/eclinical/standard/steps/design/versioning/__init__.py
 src/eclinical/standard/steps/design/versioning/design_download_publish_sql.py
 src/eclinical/standard/steps/design/versioning/design_fileids.py
 src/eclinical/standard/steps/design/versioning/design_get_last_version.py
 src/eclinical/standard/steps/portal/__init__.py
 src/eclinical/standard/steps/portal/hierarchies/__init__.py
```

### Comparing `eClinical-1.0.8.4/src/eclinical/__init__.py` & `eClinical-1.0.9/src/eclinical/__init__.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/eclinical_cmd.py` & `eClinical-1.0.9/src/eclinical/eclinical_cmd.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/environment/environment.py` & `eClinical-1.0.9/src/eclinical/environment/environment.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/execption.py` & `eClinical-1.0.9/src/eclinical/execption.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/api_spec/api_spec.py` & `eClinical-1.0.9/src/eclinical/record/api_spec/api_spec.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/api_spec/swagger.py` & `eClinical-1.0.9/src/eclinical/record/api_spec/swagger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cjen
 import re
 
 
 class Swagger(cjen.BigTangerine):
     def __init__(self):
-        self.__setattr__("base_url", "http://52.82.79.202:81/")
+        self.__setattr__("base_url", "http://200.200.101.113")
         super().__init__()
 
     @cjen.http.get_mapping(uri="api/{system}/v2/api-docs")
     def doc(self, path_variable, resp=None, **kwargs):
         ...
 
     @classmethod
```

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/api/api_spec.py` & `eClinical-1.0.9/src/eclinical/record/ext/api/api_spec.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/api/swagger.py` & `eClinical-1.0.9/src/eclinical/record/ext/api/swagger.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/common.py` & `eClinical-1.0.9/src/eclinical/record/ext/common.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/eclinical_service.py` & `eClinical-1.0.9/src/eclinical/record/ext/eclinical_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/memcached.py` & `eClinical-1.0.9/src/eclinical/record/ext/memcached.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/ext/proxy.py` & `eClinical-1.0.9/src/eclinical/record/ext/proxy.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/mitm/mitm_process.py` & `eClinical-1.0.9/src/eclinical/record/mitm/mitm_process.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/player.py` & `eClinical-1.0.9/src/eclinical/record/player.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/view/alert_dialog.py` & `eClinical-1.0.9/src/eclinical/record/view/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/record/view/record_ui.py` & `eClinical-1.0.9/src/eclinical/record/view/record_ui.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/command/ecl.py` & `eClinical-1.0.9/src/eclinical/scaffold/command/ecl.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/command/edk.py` & `eClinical-1.0.9/src/eclinical/scaffold/command/edk.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/command/mc.py` & `eClinical-1.0.9/src/eclinical/scaffold/command/mc.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/command/resource/global_conftest.txt` & `eClinical-1.0.9/src/eclinical/scaffold/command/resource/global_conftest.txt`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/command/sc.py` & `eClinical-1.0.9/src/eclinical/scaffold/command/sc.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/files/gen_meta.py` & `eClinical-1.0.9/src/eclinical/scaffold/files/gen_meta.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/files/gen_service.py` & `eClinical-1.0.9/src/eclinical/scaffold/files/gen_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/inputs/component/text.py` & `eClinical-1.0.9/src/eclinical/scaffold/inputs/component/text.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/eclinical_uri.py` & `eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/eclinical_uri.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/inputs/edk/environment_name.py` & `eClinical-1.0.9/src/eclinical/scaffold/inputs/edk/environment_name.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/inputs/mc/meta_attrs.py` & `eClinical-1.0.9/src/eclinical/scaffold/inputs/mc/meta_attrs.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/template/file_operate.py` & `eClinical-1.0.9/src/eclinical/scaffold/template/file_operate.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/template/meta.py` & `eClinical-1.0.9/src/eclinical/scaffold/template/meta.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/scaffold/template/service.py` & `eClinical-1.0.9/src/eclinical/scaffold/template/service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/_login_service.py` & `eClinical-1.0.9/src/eclinical/service/_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/_sponsor_login_service.py` & `eClinical-1.0.9/src/eclinical/service/_sponsor_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/_study_login_service.py` & `eClinical-1.0.9/src/eclinical/service/_study_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/ctms_login_service.py` & `eClinical-1.0.9/src/eclinical/service/ctms_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/data/_sponsor_login_data.py` & `eClinical-1.0.9/src/eclinical/service/data/_sponsor_login_data.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/data/_study_login_data.py` & `eClinical-1.0.9/src/eclinical/service/data/_study_login_data.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/design_login_service.py` & `eClinical-1.0.9/src/eclinical/service/design_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/edc_login_service.py` & `eClinical-1.0.9/src/eclinical/service/edc_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/ediary_login_service.py` & `eClinical-1.0.9/src/eclinical/service/ediary_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/etmf_login_service.py` & `eClinical-1.0.9/src/eclinical/service/etmf_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/iwrs_login_service.py` & `eClinical-1.0.9/src/eclinical/service/iwrs_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/portal_administrator_login_service.py` & `eClinical-1.0.9/src/eclinical/service/portal_administrator_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/portal_login_service.py` & `eClinical-1.0.9/src/eclinical/service/portal_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/service/pv_login_service.py` & `eClinical-1.0.9/src/eclinical/service/pv_login_service.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/design/versioning.py` & `eClinical-1.0.9/src/eclinical/standard/design/design_api.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/company_envs.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/company_envs.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/envs.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/envs.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/group_user.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/group_user.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/node.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/node.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/site.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/site.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/sponsor.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/sponsor.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchies/study.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchies/study.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/hierarchy.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/hierarchy.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/query_studies.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/query_studies.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/query_user_groups.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/query_user_groups.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/querysponsors.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/querysponsors.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/role_list.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/role_list.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/role_rel_user.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/role_rel_user.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/systems.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/systems.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_access.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/user_access.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_group_info.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/user_group_info.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_group_role_rel.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/user_group_role_rel.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/user_roles.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/user_roles.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/portal/dto/users.py` & `eClinical-1.0.9/src/eclinical/standard/portal/dto/users.py`

 * *Files identical despite different names*

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_download_publish_sql.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_find_sponsor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.design.versioning import Versioning
-from eclinical.standard.steps.design.versioning.design_fileids import DesignFileIDS
+from eclinical.standard.scenarios.portal_scenario import PortalScenario
+from eclinical.standard.steps.portal.user_groups.portal_life_cycle import PortalLifeCycle
 
 
-class DesignDownloadPublishSql(StandardStep):
-    Name = "design_download_publish_sql.py"
+class PortalFindSponsor(StandardStep):
+    Name = "portal_find_sponsor"
+    Id = "sponsor_id"
 
-    def __init__(self, service: Versioning, scenario: Scenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def _pre_processor(self):
-        DesignFileIDS(self.service, self.scenario).run()
+    def sponsor(self):
+        return self.scenario.sponsor()
 
-    def _execute(self): self.service.download_file(data=self.data())
+    def _pre_processor(self):
+        PortalLifeCycle(self.service, self.scenario).run()
 
-    def data(self):
-        sql_file_id = self.service.context["archives"].db_spec().get("fileId") - 1
-        return {"fileIds": [sql_file_id]}
+    def _execute(self):
+        super()._execute()
+        self.service.hierarchies_get_sponsor(name=self.sponsor(), path_variable=self.path_variable())
 
     def call_back(self, **kwargs):
-        with open("publish_sql.zip", 'wb') as f:
-            f.write(kwargs.get("file_bytes"))
+        self.service.context[self.Id] = None
+        for sponsor in kwargs.get("query").sponsorExtDtoList():
+            if sponsor.name() == self.sponsor():
+                self.service.context[self.Id] = sponsor.id()
+
+    def life_cycle(self):
+        return self.scenario.life_cycle()
+
+    def path_variable(self):
+        return dict(env_id=self.service.context[self.life_cycle()])
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_fileids.py` & `eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/design_download_publish_sql.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.design.versioning import Versioning
-from eclinical.standard.steps.design.versioning.design_get_last_version import DesignGetLastVersion
+from eclinical.standard.design.design_api import Versioning
+from eclinical.standard.steps.design.versioning.design_fileids import DesignFileIDS
 
 
-# 获取生成文件的fileid
-class DesignFileIDS(StandardStep):
-    Name = "design_fileids.py"
+class DesignDownloadPublishSql(StandardStep):
+    Name = "design_download_publish_sql.py"
 
     def __init__(self, service: Versioning, scenario: Scenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
-        DesignGetLastVersion(self.service, self.scenario).run()
+        DesignFileIDS(self.service, self.scenario).run()
 
-    def _execute(self):  self.service.archive_files(path_variable=self.path_variable())
+    def _execute(self):
+        super()._execute()
+        self.service.download_file(data=self.data())
+
+    def data(self):
+        sql_file_id = self.service.context["archives"].db_spec().get("fileId") - 1
+        return {"fileIds": [sql_file_id]}
 
     def call_back(self, **kwargs):
-        self.service.context["archives"] = kwargs.get("archives")
-
-    def path_variable(self):
-        return dict(currentVersionId=self.service.context["currentVersionId"])
+        with open("publish_sql.zip", 'wb') as f:
+            f.write(kwargs.get("file_bytes"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/design/versioning/design_get_last_version.py` & `eClinical-1.0.9/src/eclinical/standard/steps/design/versioning/design_get_last_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import jsonpath
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.design.versioning import Versioning
+from eclinical.standard.design.design_api import Versioning
 
 
 # 获取最后提交得版本信息
 class DesignGetLastVersion(StandardStep):
     Name = "design_get_last_version"
 
     def __init__(self, service: Versioning, scenario: Scenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+        super().__init__(service, scenario)
+
 
     def call_back(self, **kwargs):
         current = kwargs.get("version_info").current_version()
         if current.get("latest") is True and current.get("status") == 200:
             self.service.context["currentVersionId"] = current.get("id")
         else: raise Exception("The CRF has not Submit")
 
-    def _execute(self): self.service.version_list()
+    def _execute(self):
+        super()._execute()
+        self.service.version_list()
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_create_sponsor.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_create_sponsor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 
 
 class PortalCreateSponsor(StandardStep):
     Name = "portal_create_sponsor.py"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
         PortalFindSponsor(self.service, self.scenario).run()
 
     def ignore(self):
         return self.service.context["sponsor_id"] is not None
 
     def sponsor_name(self): return self.scenario.sponsor()
 
     def data(self):
         return {"name": self.sponsor_name(), "description": "", "active": True}
 
-    def _execute(self): self.service.new_sponsor(data=self.data())
+    def _execute(self):
+        super()._execute()
+        self.service.hierarchies_new_sponsor(data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_create_study.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_create_study.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 from eclinical.standard.steps.portal.hierarchies.portal_find_study import PortalFindStudy
 
 
 class PortalCreateStudy(StandardStep):
     Name = "portal_create_study"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
         PortalFindSponsor(self.service, self.scenario).run()
 
     def ignore(self):
         PortalFindStudy(self.service, self.scenario).run()
         return self.service.context[PortalFindStudy.Id] is not None
 
     def _execute(self):
-        self.service.new_study(data=self.data())
+        super()._execute()
+        self.service.hierarchies_new_study(data=self.data())
 
     def study(self): return self.scenario.study()
 
     def sponsor(self): return self.scenario.sponsor()
 
     def data(self):
         return dict(active=True, description="", name=self.study(),
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_find_sponsor.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_startup_study.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from cjen.sco.scenario import Scenario
+
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user_groups.portal_life_cycle import PortalLifeCycle
+from eclinical.standard.steps.portal.hierarchies.portal_find_study import PortalFindStudy
+from eclinical.standard.steps.portal.hierarchies.portal_study_no_start import PortalStudyNoStart
 
 
-class PortalFindSponsor(StandardStep):
-    Name = "portal_find_sponsor"
-    Id = "sponsor_id"
+class PortalStartupStudy(StandardStep):
+    Name = "portal_startup_study"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def sponsor(self):
-        return self.scenario.sponsor()
 
     def _pre_processor(self):
-        PortalLifeCycle(self.service, self.scenario).run()
+        PortalFindStudy(self.service, self.scenario).run()
+        PortalStudyNoStart(self.service, self.scenario).run()
+
+    def ignore(self):
+        return not self.service.context[PortalStudyNoStart.System]
 
     def _execute(self):
-        self.service.get_sponsor(name=self.sponsor(), path_variable=self.path_variable())
+        super()._execute()
+        self.service.hierarchies_study_startup(
+            data=self.data(),
+            path_variable=self.path_variable())
 
-    def call_back(self, **kwargs):
-        self.service.context[self.Id] = None
-        for sponsor in kwargs.get("query").sponsorExtDtoList():
-            if sponsor.name() == self.sponsor():
-                self.service.context[self.Id] = sponsor.id()
+    def life_cycle(self): return self.scenario.life_cycle()
 
-    def life_cycle(self):
-        return self.scenario.life_cycle()
+    def data(self): return self.service.context[PortalStudyNoStart.System]
 
     def path_variable(self):
-        return dict(env_id=self.service.context[self.life_cycle()])
+        return dict(study_id=self.service.context[PortalFindStudy.Id],
+                    env_id=self.service.context[self.life_cycle()])
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_find_study.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_find_study.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 
 
 class PortalFindStudy(StandardStep):
     Name = "portal_find_study"
     Id = "study_id"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindSponsor(self.service, self.scenario).run()
 
     def sponsor(self):
         return self.scenario.sponsor()
 
@@ -27,16 +26,18 @@
     def call_back(self, **kwargs):
         self.service.context[self.Id] = None
         for study in kwargs.get("query").studies():
             if study.name() == self.study():
                 self.service.context[self.Id] = study.id()
 
     def _execute(self):
-        self.service.get_study(
+        super()._execute()
+        self.service.hierarchies_get_study(
             data=self.data(),
             path_variable=self.path_variable())
 
+
     def data(self):
         return dict(sponsorId=self.service.context[PortalFindSponsor.Id])
 
     def path_variable(self):
         return dict(pageNo=1)
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_sponsor_no_start.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_sponsor_no_start.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from cjen.exceptions import JsonPathNotFoundErr
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 
 
 class PortalSponsorNoStart(StandardStep):
     Name = "portal_sponsor_no_start.py"
     System = "not_startup_sponsor"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         if not self.service.context[PortalFindSponsor.Id]:
             PortalFindSponsor(self.service, self.scenario).run()
 
     def _execute(self):
-        self.service.sponsor_systems(path_variable=self.path_variable())
+        super()._execute()
+        self.service.hierarchies_sponsor_systems(path_variable=self.path_variable())
 
     def life_cycle(self):
         return self.scenario.life_cycle()
 
     def call_back(self, **kwargs):
         try:
             self.service.context[self.System] = [app.id() for app in kwargs.get("systems").no_rel_apps()]
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_startup_sponsor.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_startup_sponsor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 from eclinical.standard.steps.portal.hierarchies.portal_sponsor_no_start import PortalSponsorNoStart
 
 
 class PortalStartSponsor(StandardStep):
     Name = "portal_startup_sponsor.py"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindSponsor(self.service, self.scenario).run()
         PortalSponsorNoStart(self.service, self.scenario).run()
 
     def ignore(self):
         return not self.service.context[PortalSponsorNoStart.System]
 
     def _execute(self):
-        self.service.sponsor_startup(
+        super()._execute()
+        self.service.hierarchies_sponsor_startup(
             data=self.data(),
             path_variable=self.path_variable())
 
     def life_cycle(self): return self.scenario.life_cycle()
 
     def data(self): return self.service.context[PortalSponsorNoStart.System]
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_startup_study.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_set_permissions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.hierarchies.portal_find_study import PortalFindStudy
-from eclinical.standard.steps.portal.hierarchies.portal_study_no_start import PortalStudyNoStart
+from eclinical.standard.steps.portal.role.portal_find_role import PortalFindRole
+from eclinical.standard.steps.portal.role.portal_get_permission_tree import PortalGetPermissionTree
 
 
-class PortalStartupStudy(StandardStep):
-    Name = "portal_startup_study"
+class PortalSetPermissions(StandardStep):
+    Name = "portal_set_permissions.py"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def _pre_processor(self):
-        PortalFindStudy(self.service, self.scenario).run()
-        PortalStudyNoStart(self.service, self.scenario).run()
 
-    def ignore(self):
-        return not self.service.context[PortalStudyNoStart.System]
-
-    def _execute(self):
-        self.service.study_startup(
-            data=self.data(),
-            path_variable=self.path_variable())
-
-    def life_cycle(self): return self.scenario.life_cycle()
+    def _pre_processor(self):
+        PortalFindRole(self.service, self.scenario).run()
+        PortalGetPermissionTree(self.service, self.scenario).run()
 
-    def data(self): return self.service.context[PortalStudyNoStart.System]
+    def data(self):
+        return [dict(permissionId=pid, roleId=self.service.context[PortalFindRole.Id])
+                for pid in self.service.context[PortalGetPermissionTree.IdOfAllPermission]]
 
     def path_variable(self):
-        return dict(study_id=self.service.context[PortalFindStudy.Id],
-                    env_id=self.service.context[self.life_cycle()])
+        return dict(role_id=self.service.context[PortalFindRole.Id])
+
+    def _execute(self):
+        super()._execute()
+        self.service.role_api_set_permissions(path_variable=self.path_variable(), data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/hierarchies/portal_study_no_start.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/hierarchies/portal_study_no_start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from cjen.exceptions import JsonPathNotFoundErr
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_study import PortalFindStudy
 
 
 class PortalStudyNoStart(StandardStep):
     Name = "portal_study_no_start.py"
     System = "not_startup_study"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         if not self.service.context[PortalFindStudy.Id]:
             PortalFindStudy(self.service, self.scenario).run()
 
     def _execute(self):
-        self.service.study_systems(path_variable=self.path_variable())
+        super()._execute()
+        self.service.hierarchies_study_systems(path_variable=self.path_variable())
 
     def life_cycle(self):
         return self.scenario.life_cycle()
 
     def call_back(self, **kwargs):
         try:
             self.service.context[self.System] = [app.id() for app in kwargs.get("systems").no_rel_apps()]
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_create_role.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_create_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.role import Role
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.role.portal_find_role import PortalFindRole
 
 
 class PortalCreateRole(StandardStep):
     Name = "portal_create_role.py"
 
-    def __init__(self, service: Role, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindRole(self.service, self.scenario).run()
 
     def ignore(self): return self.service.context[PortalFindRole.Id] is not None
 
     def category(self): return self.scenario.role().split("/")[0]
@@ -23,8 +22,10 @@
     def code(self): return self.scenario.role()
 
     def subCode(self): return self.scenario.role().split("/")[1]
 
     def data(self):
         return dict(category=self.category(), code=self.code(), subCode=self.subCode(), description="Test", active=True)
 
-    def _execute(self): self.service.api_create_role(data=self.data())
+    def _execute(self):
+        super()._execute()
+        self.service.role_api_create_role(data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_find_role.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_find_role.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.role import Role
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 
 
 class PortalFindRole(StandardStep):
     Name = "portal_find_role.py"
     Id = "role_id"
 
-    def __init__(self, service: Role, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def path_variable(self): return dict(pageNo=1)
 
     def role_name(self):
         return self.scenario.role()
 
     def call_back(self, **kwargs):
         self.service.context[self.Id] = None
         for role in kwargs.get("role_list").all():
             if role.code() == self.role_name():
                 self.service.context[self.Id] = role.id()
 
     def _execute(self):
-        self.service.api_query(path_variable=self.path_variable())
+        super()._execute()
+        self.service.role_api_query(path_variable=self.path_variable())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_get_permission_tree.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/role/portal_get_permission_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.role import Role
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.role.portal_find_role import PortalFindRole
 
 
 class PortalGetPermissionTree(StandardStep):
     Name = "portal_get_permission_tree.py"
     IdOfAllPermission = "all_permissions_ids"
 
-    def __init__(self, service: Role, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
         PortalFindRole(self.service, self.scenario).run()
 
     def path_variable(self):
         return dict(role_id=self.service.context[PortalFindRole.Id])
 
     def _execute(self):
-        self.service.api_all_permission_tree(path_variable=self.path_variable())
+        super()._execute()
+        self.service.role_api_all_permission_tree(path_variable=self.path_variable())
 
     def call_back(self, **kwargs):
         ids = set()
         for system in kwargs.get("pt").systems():
             self.get_permission_id(system, ids)
         self.service.context[self.IdOfAllPermission] = list(ids)
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/role/portal_set_permissions.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_roles/portal_get_user_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+from cjen import BigTangerine
+from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.role import Role
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.role.portal_find_role import PortalFindRole
-from eclinical.standard.steps.portal.role.portal_get_permission_tree import PortalGetPermissionTree
 
 
-class PortalSetPermissions(StandardStep):
-    Name = "portal_set_permissions.py"
+class PortalGetUserRole(StandardStep):
+    Name = "portal_get_user_role.py"
+    Id = "portal_user_role_id"
 
-    def __init__(self, service: Role, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
-
-    def _pre_processor(self):
-        PortalFindRole(self.service, self.scenario).run()
-        PortalGetPermissionTree(self.service, self.scenario).run()
-
-    def data(self):
-        return [dict(permissionId=pid, roleId=self.service.context[PortalFindRole.Id])
-                for pid in self.service.context[PortalGetPermissionTree.IdOfAllPermission]]
+    def __init__(self, service: BigTangerine, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def path_variable(self):
-        return dict(role_id=self.service.context[PortalFindRole.Id])
+        return dict(PageNo=1)
+
+    def role(self):
+        return self.scenario.role()
 
     def _execute(self):
-        self.service.api_set_permissions(path_variable=self.path_variable(), data=self.data())
+        super()._execute()
+        self.service.userrole_api_get_user_roles(path_variable=self.path_variable())
+
+    def call_back(self, **kwargs):
+        self.service.context[self.Id] = None
+        for role in kwargs.get("user_role").list():
+            if role.code() == self.role():
+                self.service.context[self.Id] = role.id()
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_associated_usergroup.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_find_un_added_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
+from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 
 
-class PortalAssociatedUserGroup(StandardStep):
-    Name = "portal_associate_user_group.py"
-    ExistsRels = "exists_user_rels"
+class PortalFindUnAddedUser(StandardStep):
+    Name = "portal_get_un_added_user.py"
+
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
 
     def _pre_processor(self):
-        PortalFindUser(self.service, self.scenario).run()
+        PortalFindUserGroup(self.service, self.scenario).run()
+
+    def call_back(self, **kwargs):
+        self.service.context["user_id"] = None
+        for user in kwargs.get("group_users").list():
+            if user.loginName() == self.user_name():
+                self.service.context["user_id"] = user.id()
 
-    def path_variable(self):
-        return dict(user_id=self.service.context[PortalFindUser.Id])
+    def user_name(self): return self.scenario.user()
 
     def _execute(self):
-        self.service.api_user_group_role_rel(path_variable=self.path_variable())
+        super()._execute()
+        self.service.usergroups_api_get_un_added_user(path_variable=self.path_variable())
 
-    def call_back(self, **kwargs):
-        rels = [dict(roleId=rel.roleId(), userGroupId=rel.userGroupId(), userId=rel.userId()) for rel in kwargs.get("rel").list()]
-        self.service.context[PortalAssociatedUserGroup.ExistsRels] = rels
+    def path_variable(self): return dict(userGroup_id=self.service.context["user_group_id"])
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_create_user.py` & `eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_submit_study_basic_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
-from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
+from eclinical.standard.scenarios.ctms_scenario import CtmsScenario
+from eclinical.standard.steps.ctms.ctms_find_study import CtmsFindStudy
 
 
-class PortalCreateUser(StandardStep):
-    Name = "portal_create_user.py"
+class CtmsSubmitStudyBasicInfo(StandardStep):
+    Name = "ctms_submit_study_basic_info.py"
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: CtmsScenario):
+        super().__init__(service, scenario)
 
-    def _pre_processor(self): PortalFindUser(self.service, self.scenario).run()
+    def _pre_processor(self):
+        CtmsFindStudy(self.service, self.scenario).run()
 
-    def ignore(self):
-        return self.service.context[PortalFindUser.Id] is not None
-
-    def login_name(self): return self.scenario.user()
-
-    def pass_word(self): return self.service.encypt_password("Admin@123")
+    def is_randomized(self):
+        return "IWRS" in self.scenario.apps()
 
     def data(self):
         return {
-            "firstName": self.login_name()[0],
-            "lastName": self.login_name()[1:],
-            "loginName": self.login_name(),
-            "password": self.pass_word(),
-            "phoneNumber": "88888888",
-            "email": f'{self.login_name()}@163.com', "active": True, "etmfAdministrator": False}
-
-    def _execute(self): self.service.api_create_user(data=self.data())
+            "blindMethods": 0,
+            "craReview": False,
+            "daysToResolveQuery": 100,
+            "endDate": 2519827200000,
+            "id": self.service.context[CtmsFindStudy.Info].get("id"),
+            "intervalDays": 10000,
+            "isDraft": False,
+            "mainPurpose": 1,
+            "mandatoryForAttachments": 0,
+            "name": self.service.context[CtmsFindStudy.Info].get("name"),
+            "numOfSite": 3,
+            "numOfSubject": 100,
+            "randomize": self.is_randomized(),
+            "saftyReview": False,
+            "startDate": 1655971679755,
+            "studyPhase": 1,
+            "studyType": 0
+        }
+
+    def _execute(self):
+        super()._execute()
+        self.service.study_management_submit_info(data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_find_user.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_find_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 
 
 class PortalFindUser(StandardStep):
     Name = "portal_find_user.py"
     Id = "user_id"
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def user_name(self):
         return self.scenario.user().upper()
 
     def call_back(self, **kwargs):
         self.service.context[self.Id] = None
         for user in kwargs.get("users").list():
             if user.loginName() == self.user_name():
                 self.service.context[self.Id] = user.id()
 
     def _execute(self):
-        self.service.api_user_query(path_variable=dict(pageNo=1))
+        super()._execute()
+        self.service.user_api_user_query(path_variable=dict(pageNo=1))
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_find_user_role.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_find_user_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 
 
 class PortalFindUserRole(StandardStep):
     Name = "portal_role_list.py"
     Id = "user_role_id"
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def role(self):
         return self.scenario.role()
 
     def _execute(self):
-        self.service.api_role_list()
+        super()._execute()
+        self.service.user_api_role_list()
 
     def call_back(self, **kwargs):
         for r in kwargs.get("role_list").payload():
             if r.code() == self.role():
                 self.service.context[PortalFindUserRole.Id] = r.id()
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_study_title.py` & `eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_find_study_site.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
-from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
-from eclinical.standard.steps.portal.user.portal_user_access import PortalUserAccess
+from eclinical.standard.scenarios.ctms_scenario import CtmsScenario
+
+from eclinical.standard.steps.ctms.ctms_find_study import CtmsFindStudy
+
+
+class CtmsFindStudySite(StandardStep):
+    Name = "ctms_find_study_site.py"
+    Info = "ctms_sites_of_study"
 
+    def __init__(self, service, scenario: CtmsScenario):
+        super().__init__(service, scenario)
+        self.service.context[self.Info] = []
 
-class PortalStudyTitle(StandardStep):
-    Name = "portal_study_title.py"
+    def _pre_processor(self):
+        CtmsFindStudy(self.service, self.scenario).run()
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def ignore(self): return self.service.context[CtmsFindStudy.Info] is None
 
-    def _pre_processor(self): ...
+    def call_back(self, **kwargs):
+        self.service.context[self.Info].extend(kwargs.get("query").list())
 
-    def path_variable(self):
-        return dict(user_id=self.service.context[PortalFindUser.Id])
+    def path_variable(self): return dict(pageNo=1)
 
-    def data(self):
-        return [dict(studyId=study_id, title=f'Title Of {study_id}', userId=self.service.context[PortalFindUser.Id])
-                for study_id in self.service.context[PortalUserAccess.StudiesId]]
+    def data(self): return dict(studyId=self.service.context[CtmsFindStudy.Info].get("id"))
 
     def _execute(self):
-        self.service.api_study_title(path_variable=self.path_variable(), data=self.data())
+        super()._execute()
+        self.service.study_management_site_list(path_variable=self.path_variable(), data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_user_access.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_user_access.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
 
 
 class PortalUserAccess(StandardStep):
     Name = "portal_user_access.py"
     StudiesId = "user_access_permission_studies_id"
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindUser(self.service, self.scenario).run()
 
     def path_variable(self): return {"user_id": self.service.context[PortalFindUser.Id]}
 
-    def _execute(self): self.service.api_user_access(path_variable=self.path_variable())
+    def _execute(self):
+        super()._execute()
+        self.service.user_api_user_access(path_variable=self.path_variable())
 
     def call_back(self, **kwargs):
         id_of_studies = set()
         for user_permission_dto in kwargs.get("user_access").userPermissionDtoList():
             id_of_studies.add(user_permission_dto.studyId())
         self.service.context[self.StudiesId] = list(id_of_studies)
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user/portal_user_append_usergroup.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_user_append_usergroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user import User
-from eclinical.standard.portal.user_groups import UserGroups
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.user.portal_associated_usergroup import PortalAssociatedUserGroup
 from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
 from eclinical.standard.steps.portal.user.portal_find_user_role import PortalFindUserRole
 from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 
 
 class PortalUserAppendUserGroup(StandardStep):
     Name = "portal_user_append_usergroup.py"
 
-    def __init__(self, service: User, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindUserGroup(self.service, self.scenario).run()
         PortalAssociatedUserGroup(self.service, self.scenario).run()
 
     def ignore(self):
         for rels in self.service.context[PortalAssociatedUserGroup.ExistsRels]:
@@ -43,8 +41,9 @@
         rels = self.service.context[PortalAssociatedUserGroup.ExistsRels]
         rels.append(dict(roleId=self.service.context[PortalFindUserRole.Id],
                          userId=self.service.context[PortalFindUser.Id],
                          userGroupId=self.service.context[PortalFindUserGroup.Id]))
         return rels
 
     def _execute(self):
-        self.service.api_append_user_group_role_rel(path_variable=self.path_variable(), data=self.data())
+        super()._execute()
+        self.service.user_api_append_user_group_role_rel(path_variable=self.path_variable(), data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_add_group_user.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_add_group_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.user_groups.portal_find_un_added_user import PortalFindUnAddedUser
 
 
 class PortalAddGroupUser(StandardStep):
     Name = "portal_add_group_user.py"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindUnAddedUser(self.service, self.scenario).run()
 
     def ignore(self): return self.service.context["user_id"] is None
 
     def _execute(self):
-        self.service.api_add_group_user(path_variable=self.path_variable(), data=self.data())
+        super()._execute()
+        self.service.usergroups_api_add_group_user(path_variable=self.path_variable(), data=self.data())
 
     def path_variable(self): return dict(userGroup_id=self.service.context["user_group_id"])
 
     def data(self):
         return [dict(userGroupId=self.service.context["user_group_id"], userId=self.service.context["user_id"])]
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_create_usergroup.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_create_usergroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 from eclinical.standard.steps.portal.user_groups.portal_get_company_envs import PortalGetCompanyEnvs
 
 
 class PortalCreateUserGroup(StandardStep):
     Name = "portal_create_user_group"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
+
 
     def _pre_processor(self):
         PortalFindUserGroup(self.service, self.scenario).run()
         PortalGetCompanyEnvs(self.service, self.scenario).run()
 
     def ignore(self): return self.service.context[PortalFindUserGroup.Id] is not None
 
     def code(self): return self.scenario.user_group()
 
     def _execute(self):
+        super()._execute()
         if self.service.context[PortalFindUserGroup.Id] is None:
-            self.service.create_user_group(data=self.data())
+            self.service.usergroups_create_user_group(data=self.data())
 
-    def data(self): return {"code": self.code(), "active": True, "envIds": self.service.context["envIds"]}
+    def data(self):
+        return {"code": self.code(), "active": True, "envIds": self.service.context[PortalGetCompanyEnvs.Id]}
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_find_un_added_user.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user/portal_study_title.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
-from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 
+from eclinical.standard.scenarios.portal_scenario import PortalScenario
+from eclinical.standard.steps.portal.user.portal_find_user import PortalFindUser
+from eclinical.standard.steps.portal.user.portal_user_access import PortalUserAccess
 
-class PortalFindUnAddedUser(StandardStep):
-    Name = "portal_get_un_added_user.py"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+class PortalStudyTitle(StandardStep):
+    Name = "portal_study_title.py"
 
-    def _pre_processor(self):
-        PortalFindUserGroup(self.service, self.scenario).run()
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def call_back(self, **kwargs):
-        self.service.context["user_id"] = None
-        for user in kwargs.get("group_users").list():
-            if user.loginName() == self.user_name():
-                self.service.context["user_id"] = user.id()
 
-    def _post_processor(self):
-        print("user_id", self.service.context["user_id"])
+    def _pre_processor(self): ...
 
-    def user_name(self): return self.scenario.user()
+    def path_variable(self):
+        return dict(user_id=self.service.context[PortalFindUser.Id])
 
-    def _execute(self): self.service.api_get_un_added_user(path_variable=self.path_variable())
+    def data(self):
+        return [dict(studyId=study_id,
+                     title=f'Title Of {study_id}',
+                     userId=self.service.context[PortalFindUser.Id])
+                for study_id in self.service.context[PortalUserAccess.StudiesId]]
 
-    def path_variable(self): return dict(userGroup_id=self.service.context["user_group_id"])
+    def _execute(self):
+        super()._execute()
+        self.service.user_api_study_title(path_variable=self.path_variable(), data=self.data())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_find_usergroup.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_find_usergroup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 
 
 class PortalFindUserGroup(StandardStep):
     Name = "portal_find_user_group"
     Id = "user_group_id"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def user_group(self):
         return self.scenario.user_group()
 
     def call_back(self, **kwargs):
         self.service.context[self.Id] = None
         for user_group in kwargs.get("query").user_groups():
             if user_group.code() == self.user_group():
                 self.service.context[self.Id] = user_group.id()
 
     def _execute(self):
-        self.service.get_user_group(path_variable=dict(pageNo=1))
+        super()._execute()
+        self.service.usergroups_get_user_group(path_variable=dict(pageNo=1))
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_get_lifecycle_hierarchies.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_get_lifecycle_hierarchies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
 from eclinical.standard.portal.dto.hierarchies.node import Node
 from eclinical.standard.portal.dto.hierarchies.sponsor import Sponsor
-from eclinical.standard.portal.user_groups import UserGroups
+
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 from eclinical.standard.steps.portal.user_groups.portal_get_company_envs import PortalGetCompanyEnvs
 
 
 class PortalGetLifeCycleHierarchies(StandardStep):
     Name = "portal_get_lifecycle_hierarchies.py"
     Tree = "hierarchies"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
         PortalGetCompanyEnvs(self.service, self.scenario).run()
 
     def life_cycle(self):
         return self.scenario.life_cycle()
 
@@ -36,8 +34,9 @@
         return {"life_cycle_id": None}
 
     def call_back(self, **kwargs):
         self.service.context[self.Tree] = Sponsor.trees(kwargs.get("hierarchies").sponsorExtDtoList(),
                                                         self.service.context[PortalFindUserGroup.Id])
 
     def _execute(self):
-        self.service.api_get_lifecycle_hierarchies(path_variable=self.path_variable())
+        super()._execute()
+        self.service.usergroups_api_get_lifecycle_hierarchies(path_variable=self.path_variable())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_get_user_group_info.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_get_user_group_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 
 
 class PortalGetUserGroupInfo(StandardStep):
     Name = "portal_get_user_group_info"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def _pre_processor(self):
         PortalFindUserGroup(self.service, self.scenario).run()
 
-    def life_cycle(self): return self.scenario.life_cycle()
+    def life_cycle(self):
+        return self.scenario.life_cycle()
 
     def call_back(self, **kwargs):
         for company_multiple_env in kwargs.get("query").company_multiple_envs():
             if company_multiple_env.name() == self.life_cycle():
                 self.service.context["company_multiple_env_id"] = company_multiple_env.id()
 
-    def _post_processor(self):
-        print("company_multiple_env_id", self.service.context["company_multiple_env_id"])
+    def _execute(self):
+        super()._execute()
+        self.service.usergroups_user_group_info(path_variable=self.path_variable())
 
-    def _execute(self): self.service.user_group_info(path_variable=self.path_variable())
-
-    def path_variable(self): return dict(userGroup_id=self.service.context["user_group_id"])
+    def path_variable(self):
+        return dict(userGroup_id=self.service.context["user_group_id"])
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_life_cycle.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_life_cycle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.hierarchies import Hierarchies
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 
 
 class PortalLifeCycle(StandardStep):
     Name = "portal_life_cycle"
 
-    def __init__(self, service: Hierarchies, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
     def call_back(self, **kwargs):
         for env in kwargs.get("envs").payload():
             if env.name() == self.life_cycle():
                 self.service.context[self.life_cycle()] = env.id()
 
     def life_cycle(self):
         return self.scenario.life_cycle()
 
     def _execute(self):
-        self.service.get_env_list(life_cycle=self.life_cycle())
+        super()._execute()
+        self.service.hierarchies_get_env_list(life_cycle=self.life_cycle())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_groups/portal_set_lifecycle_hierarchies.py` & `eClinical-1.0.9/src/eclinical/standard/steps/portal/user_groups/portal_set_lifecycle_hierarchies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_groups import UserGroups
 from eclinical.standard.scenarios.portal_scenario import PortalScenario
 from eclinical.standard.steps.portal.hierarchies.portal_find_sponsor import PortalFindSponsor
 from eclinical.standard.steps.portal.user_groups.portal_find_usergroup import PortalFindUserGroup
 from eclinical.standard.steps.portal.user_groups.portal_get_company_envs import PortalGetCompanyEnvs
 from eclinical.standard.steps.portal.user_groups.portal_get_lifecycle_hierarchies import PortalGetLifeCycleHierarchies
 
 
 class PortalSetLifeCycleHierarchies(StandardStep):
     Name = "portal_set_lifecycle_hierarchies.py"
 
-    def __init__(self, service: UserGroups, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: PortalScenario):
+        super().__init__(service, scenario)
 
-    def life_cycle(self): return self.scenario.life_cycle()
+    def life_cycle(self):
+        return self.scenario.life_cycle()
 
-    def user_group(self): return self.scenario.user_group()
+    def user_group(self):
+        return self.scenario.user_group()
 
     def _pre_processor(self):
         PortalGetLifeCycleHierarchies(self.service, self.scenario).run()
 
     def path_variable(self):
         for life_cycle in self.service.context[PortalGetCompanyEnvs.Object]:
             for life_cycle_name, life_cycle_id in life_cycle.items():
                 if life_cycle_name == self.life_cycle():
-                    return {UserGroups.LifeCycleId: life_cycle_id, UserGroups.UserGroupId: self.service.context[PortalFindUserGroup.Id]}
-        return {UserGroups.LifeCycleId: None}
+                    return {"life_cycle_id": life_cycle_id, "userGroup_id": self.service.context[PortalFindUserGroup.Id]}
+        return {"life_cycle_id": None}
 
     def sponsor_name(self):
         return self.scenario.sponsor()
 
     def study_name(self):
         return self.scenario.study()
 
@@ -49,8 +48,9 @@
                             if site.name in self.sites_name():
                                 site.selected(self.service.context[PortalFindUserGroup.Id])
                         study.selected(self.service.context[PortalFindUserGroup.Id])
                 sponsor.selected(self.service.context[PortalFindUserGroup.Id])
         return [sponsor.to_dict() for sponsor in self.service.context["hierarchies"]]
 
     def _execute(self):
-        self.service.api_set_lifecycle_hierarchies(data=self.data(), path_variable=self.path_variable())
+        super()._execute()
+        self.service.usergroups_api_set_lifecycle_hierarchies(data=self.data(), path_variable=self.path_variable())
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/portal_find_no_rel_user.py` & `eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_find_study.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_role import UserRole
-from eclinical.standard.scenarios.portal_scenario import PortalScenario
-from eclinical.standard.steps.portal.user_roles.portal_get_user_role import PortalGetUserRole
+from eclinical.standard.scenarios.ctms_scenario import CtmsScenario
 
 
-class PortalFindNoRelUser(StandardStep):
-    Name = "portal_find_no_rel_user.py"
+class CtmsFindStudy(StandardStep):
+    Name = "ctms_find_study.py"
+    Info = "ctms_study_dto"
 
-    def __init__(self, service: UserRole, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: CtmsScenario):
+        super().__init__(service, scenario)
+        self.service.context[self.Info] = None
 
-    def _pre_processor(self):
-        PortalGetUserRole(self.service, self.scenario).run()
-
-    def path_variable(self):
-        return dict(role_id=self.service.context[PortalGetUserRole.Id])
+    def call_back(self, **kwargs):
+        for study in kwargs.get("studies").list():
+            if study.name() == self.scenario.study():
+                self.service.context[self.Info] = dict(id=study.id(), name=study.name())
 
     def _execute(self):
-        self.service.get_no_relations_users(path_variable=self.path_variable())
+        super()._execute()
+        self.service.study_management_get_study()
```

### Comparing `eClinical-1.0.8.4/src/eclinical/standard/steps/portal/user_roles/portal_get_user_role.py` & `eClinical-1.0.9/src/eclinical/standard/steps/ctms/ctms_all_menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-from cjen.sco.scenario import Scenario
 from cjen.sco.standard_step import StandardStep
 
-from eclinical.standard.portal.user_role import UserRole
-from eclinical.standard.scenarios.portal_scenario import PortalScenario
+from eclinical.standard.scenarios.ctms_scenario import CtmsScenario
 
 
-class PortalGetUserRole(StandardStep):
-    Name = "portal_get_user_role.py"
-    Id = "portal_user_role_id"
+class CtmsAllMenu(StandardStep):
+    Name = "ctms_all_menu.py"
+    Menu = "ctms_all_menu"
 
-    def __init__(self, service: UserRole, scenario: PortalScenario):
-        self.service = service
-        self.scenario = scenario
-        self.service.step_definitions[self.Name] = self
+    def __init__(self, service, scenario: CtmsScenario):
+        super().__init__(service, scenario)
 
-    def _pre_processor(self): ...
 
-    def path_variable(self):
-        return dict(PageNo=1)
 
-    def role(self): return self.scenario.role()
-
-    def _execute(self): self.service.api_get_user_roles(path_variable=self.path_variable())
+    def ignore(self):
+        try:
+            if self.service.context[self.Menu] is not None:
+                return True
+        except Exception as e:
+            return False
 
     def call_back(self, **kwargs):
-        self.service.context[self.Id] = None
-        for role in kwargs.get("user_role").list():
-            if role.code() == self.role():
-                self.service.context[self.Id] = role.id()
+        self.service.context[self.Menu] = kwargs.get("menus").payload()
+
+    def _execute(self):
+        super()._execute()
+        self.service.common_menu()
```

### Comparing `eClinical-1.0.8.4/src/eclinical/utils/ecrypto.py` & `eClinical-1.0.9/src/eclinical/utils/ecrypto.py`

 * *Files identical despite different names*

