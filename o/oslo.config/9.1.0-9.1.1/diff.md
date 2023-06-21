# Comparing `tmp/oslo.config-9.1.0.tar.gz` & `tmp/oslo.config-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.config-9.1.0.tar", last modified: Thu Jan  5 10:11:27 2023, max compression
+gzip compressed data, was "oslo.config-9.1.1.tar", last modified: Tue Feb 21 17:25:04 2023, max compression
```

## Comparing `oslo.config-9.1.0.tar` & `oslo.config-9.1.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.406790 oslo.config-9.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-01-05 10:11:00.000000 oslo.config-9.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-01-05 10:11:00.000000 oslo.config-9.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-01-05 10:11:00.000000 oslo.config-9.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-01-05 10:11:00.000000 oslo.config-9.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7876 2023-01-05 10:11:27.000000 oslo.config-9.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-01-05 10:11:00.000000 oslo.config-9.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37223 2023-01-05 10:11:27.000000 oslo.config-9.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-01-05 10:11:00.000000 oslo.config-9.1.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2023-01-05 10:11:00.000000 oslo.config-9.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-01-05 10:11:27.406790 oslo.config-9.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-01-05 10:11:00.000000 oslo.config-9.1.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-01-05 10:11:00.000000 oslo.config-9.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.378786 oslo.config-9.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.382787 oslo.config-9.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.382787 oslo.config-9.1.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12088 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/cli/generator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19768 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/cli/validator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/config-generator.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.382787 oslo.config-9.1.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5825 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/mutable.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/configuration/quickstart.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.382787 oslo.config-9.1.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.386787 oslo.config-9.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/accessing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/command-line.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2629 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/configuration-files.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10451 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/defining.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/deprecating.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4339 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/faq.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/globals.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/helpers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/locations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4469 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/mutable.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/naming.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2028 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/sphinxconfiggen.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1199 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/sphinxext.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3161 2023-01-05 10:11:00.000000 oslo.config-9.1.0/doc/source/reference/styleguide.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.390788 oslo.config-9.1.0/oslo.config.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4326 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-01-05 10:11:27.000000 oslo.config-9.1.0/oslo.config.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.394788 oslo.config-9.1.0/oslo_config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/_list_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   118279 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31831 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/iniparser.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.394788 oslo.config-9.1.0/oslo_config/sources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4802 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/sources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/sources/_environment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5793 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/sources/_uri.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3545 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/sphinxconfiggen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/sphinxext.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.398789 oslo.config-9.1.0/oslo_config/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   200771 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_fixture.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7799 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63898 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6798 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_get_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_iniparser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12374 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_sources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5807 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_sphinxconfiggen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14994 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38078 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/test_validator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.398789 oslo.config-9.1.0/oslo_config/tests/testmods/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/bar_foo_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/baz_qux_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/blaa_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/fbaar_baa_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/fbar_foo_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/tests/testmods/fblaa_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32227 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8693 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-01-05 10:11:00.000000 oslo.config-9.1.0/oslo_config/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.374786 oslo.config-9.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.402789 oslo.config-9.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-HostAddressOpt-6e7e2afe7c7863cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-HostDomain-implement-rfc1033-c985a3054f824e9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-default-config-dirs-03340ff6689afe94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-float-min-max-b1a2e16301c8435c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-missing-config-option-9ee1992eea750200.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-port_type-8704295c6a56265d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/add-reno-71dc832ce29b962f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/config-from-environment-3feba7b4cc747d2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/config-validator-256817f2183994fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/drop-python27-support-87f1b4089d4cc78b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/machine-readable-sample-config-e8f8ba43ababcf99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/positional-arguments-are-required-22ddca72e6f523bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/show-deprecated-reason-361a8eb31e05c97e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/support-choice-descriptions-8b2d0c14fbd16b2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/support-fatal-deprecations-ea0513aa58a395ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/validator-check-defaults-e7b596a2fde781a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/notes/validator-exclude-groups-ad2f046522a3407e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.406790 oslo.config-9.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.406790 oslo.config-9.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:27.406790 oslo.config-9.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7900 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-01-05 10:11:00.000000 oslo.config-9.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-01-05 10:11:00.000000 oslo.config-9.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-01-05 10:11:27.410790 oslo.config-9.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-01-05 10:11:00.000000 oslo.config-9.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-01-05 10:11:00.000000 oslo.config-9.1.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1795 2023-01-05 10:11:00.000000 oslo.config-9.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.622377 oslo.config-9.1.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-02-21 17:24:32.000000 oslo.config-9.1.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-02-21 17:24:32.000000 oslo.config-9.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-02-21 17:24:32.000000 oslo.config-9.1.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-21 17:24:32.000000 oslo.config-9.1.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7876 2023-02-21 17:25:04.000000 oslo.config-9.1.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-02-21 17:24:32.000000 oslo.config-9.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37266 2023-02-21 17:25:04.000000 oslo.config-9.1.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-21 17:24:32.000000 oslo.config-9.1.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2023-02-21 17:24:32.000000 oslo.config-9.1.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-02-21 17:25:04.622377 oslo.config-9.1.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-02-21 17:24:32.000000 oslo.config-9.1.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-02-21 17:24:32.000000 oslo.config-9.1.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.606374 oslo.config-9.1.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.606374 oslo.config-9.1.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.606374 oslo.config-9.1.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12088 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/cli/generator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19768 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/cli/validator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/config-generator.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.606374 oslo.config-9.1.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5825 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/mutable.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/configuration/quickstart.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.606374 oslo.config-9.1.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.610375 oslo.config-9.1.1/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/accessing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/command-line.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2629 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/configuration-files.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10451 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/defining.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/deprecating.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4339 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/faq.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/globals.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/helpers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/locations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4469 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/mutable.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/naming.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2028 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/sphinxconfiggen.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1199 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/sphinxext.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3161 2023-02-21 17:24:32.000000 oslo.config-9.1.1/doc/source/reference/styleguide.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.610375 oslo.config-9.1.1/oslo.config.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4326 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-02-21 17:25:04.000000 oslo.config-9.1.1/oslo.config.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.614375 oslo.config-9.1.1/oslo_config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/_list_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   118279 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31831 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/iniparser.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.614375 oslo.config-9.1.1/oslo_config/sources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4802 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/sources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/sources/_environment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5793 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/sources/_uri.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3545 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/sphinxconfiggen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/sphinxext.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.618376 oslo.config-9.1.1/oslo_config/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   200771 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_fixture.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7799 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63898 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6798 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_get_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_iniparser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12374 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_sources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5807 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_sphinxconfiggen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14994 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38078 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/test_validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.618376 oslo.config-9.1.1/oslo_config/tests/testmods/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/bar_foo_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/baz_qux_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/blaa_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/fbaar_baa_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/fbar_foo_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/tests/testmods/fblaa_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32227 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8693 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-02-21 17:24:32.000000 oslo.config-9.1.1/oslo_config/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.602374 oslo.config-9.1.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.622377 oslo.config-9.1.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-HostAddressOpt-6e7e2afe7c7863cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-HostDomain-implement-rfc1033-c985a3054f824e9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-default-config-dirs-03340ff6689afe94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-float-min-max-b1a2e16301c8435c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-missing-config-option-9ee1992eea750200.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-port_type-8704295c6a56265d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/add-reno-71dc832ce29b962f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/config-from-environment-3feba7b4cc747d2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/config-validator-256817f2183994fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/drop-python27-support-87f1b4089d4cc78b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/machine-readable-sample-config-e8f8ba43ababcf99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/positional-arguments-are-required-22ddca72e6f523bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/show-deprecated-reason-361a8eb31e05c97e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/support-choice-descriptions-8b2d0c14fbd16b2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/support-fatal-deprecations-ea0513aa58a395ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/validator-check-defaults-e7b596a2fde781a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/notes/validator-exclude-groups-ad2f046522a3407e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.622377 oslo.config-9.1.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.622377 oslo.config-9.1.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:04.622377 oslo.config-9.1.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7900 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-21 17:24:32.000000 oslo.config-9.1.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-02-21 17:24:32.000000 oslo.config-9.1.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-02-21 17:25:04.626377 oslo.config-9.1.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-21 17:24:32.000000 oslo.config-9.1.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-02-21 17:24:32.000000 oslo.config-9.1.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2023-02-21 17:24:32.000000 oslo.config-9.1.1/tox.ini
```

### Comparing `oslo.config-9.1.0/.pre-commit-config.yaml` & `oslo.config-9.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/AUTHORS` & `oslo.config-9.1.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/CONTRIBUTING.rst` & `oslo.config-9.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/ChangeLog` & `oslo.config-9.1.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+9.1.1
+-----
+
+* Fix issues related to tox4
+
 9.1.0
 -----
 
 * Make tests backward compat with cliff' older versions
 * Add Python3 antelope unit tests
 * Update master for stable/zed
 * Disable a config test if ran under the root user
```

### Comparing `oslo.config-9.1.0/LICENSE` & `oslo.config-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/PKG-INFO` & `oslo.config-9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.config
-Version: 9.1.0
+Version: 9.1.1
 Summary: Oslo Configuration API
 Home-page: https://docs.openstack.org/oslo.config/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.config-9.1.0/README.rst` & `oslo.config-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/cli/generator.rst` & `oslo.config-9.1.1/doc/source/cli/generator.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/cli/validator.rst` & `oslo.config-9.1.1/doc/source/cli/validator.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/conf.py` & `oslo.config-9.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/configuration/format.rst` & `oslo.config-9.1.1/doc/source/configuration/format.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/configuration/mutable.rst` & `oslo.config-9.1.1/doc/source/configuration/mutable.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/configuration/options.rst` & `oslo.config-9.1.1/doc/source/configuration/options.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/configuration/quickstart.rst` & `oslo.config-9.1.1/doc/source/configuration/quickstart.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/accessing.rst` & `oslo.config-9.1.1/doc/source/reference/accessing.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/command-line.rst` & `oslo.config-9.1.1/doc/source/reference/command-line.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/configuration-files.rst` & `oslo.config-9.1.1/doc/source/reference/configuration-files.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/defining.rst` & `oslo.config-9.1.1/doc/source/reference/defining.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/deprecating.rst` & `oslo.config-9.1.1/doc/source/reference/deprecating.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/faq.rst` & `oslo.config-9.1.1/doc/source/reference/faq.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/helpers.rst` & `oslo.config-9.1.1/doc/source/reference/helpers.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/locations.rst` & `oslo.config-9.1.1/doc/source/reference/locations.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/mutable.rst` & `oslo.config-9.1.1/doc/source/reference/mutable.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/naming.rst` & `oslo.config-9.1.1/doc/source/reference/naming.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/sphinxconfiggen.rst` & `oslo.config-9.1.1/doc/source/reference/sphinxconfiggen.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/sphinxext.rst` & `oslo.config-9.1.1/doc/source/reference/sphinxext.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/doc/source/reference/styleguide.rst` & `oslo.config-9.1.1/doc/source/reference/styleguide.rst`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo.config.egg-info/PKG-INFO` & `oslo.config-9.1.1/oslo.config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.config
-Version: 9.1.0
+Version: 9.1.1
 Summary: Oslo Configuration API
 Home-page: https://docs.openstack.org/oslo.config/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.config-9.1.0/oslo.config.egg-info/SOURCES.txt` & `oslo.config-9.1.1/oslo.config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/_i18n.py` & `oslo.config-9.1.1/oslo_config/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/_list_opts.py` & `oslo.config-9.1.1/oslo_config/_list_opts.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/cfg.py` & `oslo.config-9.1.1/oslo_config/cfg.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/fixture.py` & `oslo.config-9.1.1/oslo_config/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/generator.py` & `oslo.config-9.1.1/oslo_config/generator.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/iniparser.py` & `oslo.config-9.1.1/oslo_config/iniparser.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/sources/__init__.py` & `oslo.config-9.1.1/oslo_config/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/sources/_environment.py` & `oslo.config-9.1.1/oslo_config/sources/_environment.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/sources/_uri.py` & `oslo.config-9.1.1/oslo_config/sources/_uri.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/sphinxconfiggen.py` & `oslo.config-9.1.1/oslo_config/sphinxconfiggen.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/sphinxext.py` & `oslo.config-9.1.1/oslo_config/sphinxext.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_cfg.py` & `oslo.config-9.1.1/oslo_config/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_fixture.py` & `oslo.config-9.1.1/oslo_config/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_generator.py` & `oslo.config-9.1.1/oslo_config/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_get_location.py` & `oslo.config-9.1.1/oslo_config/tests/test_get_location.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_iniparser.py` & `oslo.config-9.1.1/oslo_config/tests/test_iniparser.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_sources.py` & `oslo.config-9.1.1/oslo_config/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_sphinxconfiggen.py` & `oslo.config-9.1.1/oslo_config/tests/test_sphinxconfiggen.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_sphinxext.py` & `oslo.config-9.1.1/oslo_config/tests/test_sphinxext.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_types.py` & `oslo.config-9.1.1/oslo_config/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/test_validator.py` & `oslo.config-9.1.1/oslo_config/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/bar_foo_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/bar_foo_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/baz_qux_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/baz_qux_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/blaa_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/blaa_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/fbaar_baa_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/fbaar_baa_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/fbar_foo_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/fbar_foo_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/tests/testmods/fblaa_opt.py` & `oslo.config-9.1.1/oslo_config/tests/testmods/fblaa_opt.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/types.py` & `oslo.config-9.1.1/oslo_config/types.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/validator.py` & `oslo.config-9.1.1/oslo_config/validator.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/oslo_config/version.py` & `oslo.config-9.1.1/oslo_config/version.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/notes/add-HostAddressOpt-6e7e2afe7c7863cb.yaml` & `oslo.config-9.1.1/releasenotes/notes/add-HostAddressOpt-6e7e2afe7c7863cb.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/notes/add-default-config-dirs-03340ff6689afe94.yaml` & `oslo.config-9.1.1/releasenotes/notes/add-default-config-dirs-03340ff6689afe94.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/notes/config-from-environment-3feba7b4cc747d2b.yaml` & `oslo.config-9.1.1/releasenotes/notes/config-from-environment-3feba7b4cc747d2b.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/notes/support-choice-descriptions-8b2d0c14fbd16b2a.yaml` & `oslo.config-9.1.1/releasenotes/notes/support-choice-descriptions-8b2d0c14fbd16b2a.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/notes/support-fatal-deprecations-ea0513aa58a395ca.yaml` & `oslo.config-9.1.1/releasenotes/notes/support-fatal-deprecations-ea0513aa58a395ca.yaml`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/releasenotes/source/conf.py` & `oslo.config-9.1.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/setup.cfg` & `oslo.config-9.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/setup.py` & `oslo.config-9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/test-requirements.txt` & `oslo.config-9.1.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.config-9.1.0/tox.ini` & `oslo.config-9.1.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 [tox]
 minversion = 3.2.0
-distribute = False
 envlist = py3,pep8
-ignore_basepython_conflict = true
 
 [testenv]
-basepython = python3
-whitelist_externals =
+allowlist_externals =
   find
 setenv =
   OS_STDOUT_CAPTURE={env:OS_STDOUT_CAPTURE:1}
   OS_STDERR_CAPTURE={env:OS_STDERR_CAPTURE:1}
   OS_TEST_TIMEOUT={env:OS_TEST_TIMEOUT:60}
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
@@ -39,15 +36,15 @@
   coverage xml -o cover/coverage.xml
   coverage report --show-missing
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 commands =
   rm -fr doc/build
   sphinx-build -W --keep-going -b html -j auto doc/source doc/build/html {posargs}
 
@@ -56,15 +53,15 @@
   mypy oslo_config
 
 [testenv:bandit]
 commands =
   bandit -r oslo_config -x tests -n5
 
 [testenv:releasenotes]
-whitelist_externals =
+allowlist_externals =
   rm
 deps = {[testenv:docs]deps}
 commands =
   rm -rf releasenotes/build
   sphinx-build -W --keep-going -b html -j auto releasenotes/source releasenotes/build/html {posargs}
 
 [hacking]
```

