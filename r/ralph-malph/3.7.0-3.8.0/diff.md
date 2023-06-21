# Comparing `tmp/ralph-malph-3.7.0.tar.gz` & `tmp/ralph-malph-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-3.7.0.tar", last modified: Tue Jun 13 16:36:04 2023, max compression
+gzip compressed data, was "ralph-malph-3.8.0.tar", last modified: Wed Jun 21 14:01:33 2023, max compression
```

## Comparing `ralph-malph-3.7.0.tar` & `ralph-malph-3.8.0.tar`

### file list

```diff
@@ -1,176 +1,188 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.348669 ralph-malph-3.7.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/auth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5871 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/oidc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/auth/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16304 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.352669 ralph-malph-3.7.0/src/ralph/backends/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13603 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9315 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9873 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/database/mongo.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/http/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3713 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10463 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/http/lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/mixins.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5310 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/storage/swift.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/backends/stream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/backends/stream/ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21725 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12019 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3000 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7195 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.356669 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.360669 ralph-malph-3.7.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2055 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/ifi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1455 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4079 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/base/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      703 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4575 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.364669 ralph-malph-3.7.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8686 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5263 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6947 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/video/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7328 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5465 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:36:04.000000 ralph-malph-3.7.0/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:36:04.368669 ralph-malph-3.7.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9942 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-13 16:36:03.000000 ralph-malph-3.7.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/api/auth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5871 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/oidc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16304 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13603 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9315 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9873 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/mongo.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/http/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3713 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10463 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/mixins.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5310 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/swift.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21846 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12019 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2066 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3000 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7195 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10009 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8242 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2055 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/ifi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1455 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4079 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4575 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9579 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5263 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7587 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7328 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5925 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9962 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_utils.py
```

### Comparing `ralph-malph-3.7.0/LICENSE.md` & `ralph-malph-3.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/PKG-INFO` & `ralph-malph-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.7.0
+Version: 3.8.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ralph-malph-3.7.0/README.md` & `ralph-malph-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/setup.cfg` & `ralph-malph-3.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ralph-malph
-version = 3.7.0
+version = 3.8.0
 description = The ultimate toolbox for your learning analytics
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/ralph/
 license = MIT
@@ -60,23 +60,23 @@
 	bcrypt>=4.0.0
 	click>=8.1.0
 	click-option-group>=0.5.0
 	sentry-sdk[fastapi]>=1.9.0
 dev = 
 	bandit==1.7.5
 	black==23.3.0
-	cryptography==40.0.1
+	cryptography==41.0.1
 	factory-boy==3.2.1
 	flake8==6.0.0
-	hypothesis==6.78.1
+	hypothesis==6.79.1
 	isort==5.12.0
-	logging-gelf==0.0.26
+	logging-gelf==0.0.31
 	mkdocs==1.4.3
 	mkdocs-click==0.8.0
-	mkdocs-material==9.1.15
+	mkdocs-material==9.1.16
 	mkdocstrings[python-legacy]==0.22.0
 	moto==4.1.11
 	pydocstyle==6.3.0
 	pyfakefs==5.2.2
 	pylint==2.17.4
 	pytest==7.3.2
 	pytest-asyncio==0.21.0
```

### Comparing `ralph-malph-3.7.0/src/ralph/__main__.py` & `ralph-malph-3.8.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/__init__.py` & `ralph-malph-3.8.0/src/ralph/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/auth/basic.py` & `ralph-malph-3.8.0/src/ralph/api/auth/basic.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/auth/oidc.py` & `ralph-malph-3.8.0/src/ralph/api/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/forwarding.py` & `ralph-malph-3.8.0/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/models.py` & `ralph-malph-3.8.0/src/ralph/api/models.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/routers/health.py` & `ralph-malph-3.8.0/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/api/routers/statements.py` & `ralph-malph-3.8.0/src/ralph/api/routers/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/database/base.py` & `ralph-malph-3.8.0/src/ralph/backends/database/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/database/clickhouse.py` & `ralph-malph-3.8.0/src/ralph/backends/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/database/es.py` & `ralph-malph-3.8.0/src/ralph/backends/database/es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/database/mongo.py` & `ralph-malph-3.8.0/src/ralph/backends/database/mongo.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/http/base.py` & `ralph-malph-3.8.0/src/ralph/backends/http/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/http/lrs.py` & `ralph-malph-3.8.0/src/ralph/backends/http/lrs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/mixins.py` & `ralph-malph-3.8.0/src/ralph/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/storage/base.py` & `ralph-malph-3.8.0/src/ralph/backends/storage/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/storage/fs.py` & `ralph-malph-3.8.0/src/ralph/backends/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/storage/ldp.py` & `ralph-malph-3.8.0/src/ralph/backends/storage/ldp.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/storage/s3.py` & `ralph-malph-3.8.0/src/ralph/backends/storage/s3.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/storage/swift.py` & `ralph-malph-3.8.0/src/ralph/backends/storage/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/backends/stream/ws.py` & `ralph-malph-3.8.0/src/ralph/backends/stream/ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/cli.py` & `ralph-malph-3.8.0/src/ralph/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,15 +462,15 @@
     help="Endpoint from which to fetch events (e.g. `/statements`)",
 )
 @click.option(
     "-q",
     "--query",
     type=JSONStringParamType(),
     default=None,
-    help="Query object as a JSON string (database backends ONLY)",
+    help="Query object as a JSON string (database and HTTP backends ONLY)",
 )
 def fetch(backend, archive, chunk_size, target, query, **options):
     """Fetch an archive or records from a configured backend."""
     logger.info(
         (
             "Fetching data from the configured %s backend "
             "(archive: %s | chunk size: %s | target: %s | query: %s)"
@@ -498,15 +498,19 @@
                     json.dumps(document) if isinstance(document, dict) else document,
                     encoding="utf-8",
                 )
             )
     elif backend_type == settings.BACKENDS.STREAM:
         backend.stream(sys.stdout.buffer)
     elif backend_type == settings.BACKENDS.HTTP:
-        for statement in backend.read(target=target, chunk_size=chunk_size):
+        if query is not None:
+            query = backend.query(query=query)
+        for statement in backend.read(
+            target=target, query=query, chunk_size=chunk_size
+        ):
             click.echo(
                 bytes(
                     json.dumps(statement) if isinstance(statement, dict) else statement,
                     encoding="utf-8",
                 )
             )
     elif backend_type is None:
```

### Comparing `ralph-malph-3.7.0/src/ralph/conf.py` & `ralph-malph-3.8.0/src/ralph/conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/exceptions.py` & `ralph-malph-3.8.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/filters.py` & `ralph-malph-3.8.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/converter.py` & `ralph-malph-3.8.0/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/base.py` & `ralph-malph-3.8.0/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/browser.py` & `ralph-malph-3.8.0/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-3.8.0/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/server.py` & `ralph-malph-3.8.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-3.8.0/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-3.8.0/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/selector.py` & `ralph-malph-3.8.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/validator.py` & `ralph-malph-3.8.0/src/ralph/models/validator.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/__init__.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """xAPI pydantic models."""
 
 # flake8: noqa
 
 from .navigation.statements import PageTerminated, PageViewed
 from .video.statements import (
     VideoCompleted,
+    VideoDownloaded,
     VideoEnableClosedCaptioning,
     VideoInitialized,
     VideoPaused,
     VideoPlayed,
     VideoScreenChangeInteraction,
     VideoSeeked,
     VideoTerminated,
```

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/agents.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/agents.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/attachments.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/attachments.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/common.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/common.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/contexts.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/groups.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/groups.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/ifi.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/ifi.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/objects.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/results.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/statements.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/base/unnested_objects.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/base/unnested_objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/video.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/constants/video.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,7 +20,21 @@
         display (dict): Consists of the dictionary `{"en-US": "viewed"}`.
     """
 
     id: Literal[
         "http://id.tincanapi.com/verb/viewed"
     ] = "http://id.tincanapi.com/verb/viewed"
     display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["viewed"]]]
+
+
+class DownloadedVerb(BaseXapiVerb):
+    """Pydantic model for downloaded `verb`.
+
+    Attributes:
+        id (str): Consists of the value `http://id.tincanapi.com/verb/downloaded`.
+        display (dict): Consists of the dictionary `{"en-US": "downloaded"}`.
+    """
+
+    id: Literal[
+        "http://id.tincanapi.com/verb/downloaded"
+    ] = "http://id.tincanapi.com/verb/downloaded"
+    display: Optional[Dict[Literal[LANG_EN_US_DISPLAY], Literal["downloaded"]]]
```

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/video.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/config.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/config.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/video/contexts.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/video/contexts.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from uuid import UUID
 
-from pydantic import Field, NonNegativeFloat
+from pydantic import Field, NonNegativeFloat, PositiveInt
 
 from ..base.contexts import BaseXapiContext, BaseXapiContextContextActivities
 from ..base.unnested_objects import BaseXapiActivity
 from ..concepts.activity_types.scorm_profile import ProfileActivity
 from ..concepts.constants.video import (
     CONTEXT_EXTENSION_CC_ENABLED,
     CONTEXT_EXTENSION_CC_SUBTITLE_LANG,
     CONTEXT_EXTENSION_COMPLETION_THRESHOLD,
     CONTEXT_EXTENSION_FULL_SCREEN,
     CONTEXT_EXTENSION_LENGTH,
+    CONTEXT_EXTENSION_QUALITY,
     CONTEXT_EXTENSION_SCREEN_SIZE,
     CONTEXT_EXTENSION_SESSION_ID,
     CONTEXT_EXTENSION_SPEED,
     CONTEXT_EXTENSION_USER_AGENT,
     CONTEXT_EXTENSION_VIDEO_PLAYBACK_SIZE,
     CONTEXT_EXTENSION_VOLUME,
 )
@@ -128,14 +129,28 @@
 
     length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
     completionThreshold: Optional[float] = Field(
         alias=CONTEXT_EXTENSION_COMPLETION_THRESHOLD
     )
 
 
+class VideoDownloadedContextExtensions(VideoContextExtensions):
+    """Represents the context.extensions field for video `downloaded` xAPI statement.
+
+    Attributes:
+        length (float): Consists of the length of the video.
+        quality (int): Consists of the video resolution or quality of the video.
+        session (uuid): Consists of the ID of the active session.
+    """
+
+    length: NonNegativeFloat = Field(alias=CONTEXT_EXTENSION_LENGTH)
+    quality: PositiveInt = Field(alias=CONTEXT_EXTENSION_QUALITY)
+    session_id: Optional[UUID] = Field(alias=CONTEXT_EXTENSION_SESSION_ID)
+
+
 class VideoEnableClosedCaptioningContextExtensions(VideoContextExtensions):
     """Represents the context.extensions field for video `interacted` xAPI statement.
 
     Attributes:
         ccSubtitleLanguage (str): Consists of the language of subtitle or closed
             captioning.
     """
@@ -228,14 +243,24 @@
     Attributes:
         extensions (dict): See VideoBrowsingContextExtensions.
     """
 
     extensions: VideoBrowsingContextExtensions
 
 
+class VideoDownloadedContext(BaseVideoContext):
+    """Pydantic model for video downloaded `context` property.
+
+    Attributes:
+        extensions (dict): See VideoDownloadedContextExtensions.
+    """
+
+    extensions: VideoDownloadedContextExtensions
+
+
 class VideoEnableClosedCaptioningContext(BaseVideoContext):
     """Pydantic model for video enable closed captioning `context` property.
 
     Attributes:
         extensions (dict): See VideoEnableClosedCaptioningContextExtensions.
     """
```

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/video/results.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/video/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/video/statements.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from ..concepts.activity_types.video import VideoActivity
 from ..concepts.verbs.scorm_profile import (
     CompletedVerb,
     InitializedVerb,
     InteractedVerb,
     TerminatedVerb,
 )
+from ..concepts.verbs.tincan_vocabulary import DownloadedVerb
 from ..concepts.verbs.video import PausedVerb, PlayedVerb, SeekedVerb
 from .contexts import (
     VideoCompletedContext,
+    VideoDownloadedContext,
     VideoEnableClosedCaptioningContext,
     VideoInitializedContext,
     VideoPausedContext,
     VideoPlayedContext,
     VideoScreenChangeInteractionContext,
     VideoSeekedContext,
     VideoTerminatedContext,
@@ -166,14 +168,33 @@
     )
 
     verb: TerminatedVerb = TerminatedVerb()
     result: VideoTerminatedResult
     context: VideoTerminatedContext
 
 
+class VideoDownloaded(BaseVideoStatement):
+    """Pydantic model for video downloaded statement.
+
+    Example: John downloaded (rather than accessed or opened) a video.
+
+    Attributes:
+        verb (dict): See DownloadedVerb.
+        context (dict): See VideoDownloadedContext.
+    """
+
+    __selector__ = selector(
+        object__definition__type="https://w3id.org/xapi/video/activity-type/video",
+        verb__id="http://id.tincanapi.com/verb/downloaded",
+    )
+
+    verb: DownloadedVerb = DownloadedVerb()
+    context: VideoDownloadedContext
+
+
 class VideoEnableClosedCaptioning(BaseVideoStatement):
     """Pydantic model for video enable closed captioning statement.
 
     Example: John interacted with the player to enable closed captioning.
 
     Attributes:
         verb (dict): See InteractedVerb.
```

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/contexts.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/models/xapi/virtual_classroom/statements.py` & `ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/parsers.py` & `ralph-malph-3.8.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph/utils.py` & `ralph-malph-3.8.0/src/ralph/utils.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-3.8.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.7.0
+Version: 3.8.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ralph-malph-3.7.0/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-3.8.0/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,22 @@
 src/ralph/models/edx/enrollment/fields/__init__.py
 src/ralph/models/edx/enrollment/fields/contexts.py
 src/ralph/models/edx/enrollment/fields/events.py
 src/ralph/models/edx/navigational/__init__.py
 src/ralph/models/edx/navigational/statements.py
 src/ralph/models/edx/navigational/fields/__init__.py
 src/ralph/models/edx/navigational/fields/events.py
+src/ralph/models/edx/open_response_assessment/__init__.py
+src/ralph/models/edx/open_response_assessment/statements.py
+src/ralph/models/edx/open_response_assessment/fields/__init__.py
+src/ralph/models/edx/open_response_assessment/fields/events.py
+src/ralph/models/edx/peer_instruction/__init__.py
+src/ralph/models/edx/peer_instruction/statements.py
+src/ralph/models/edx/peer_instruction/fields/__init__.py
+src/ralph/models/edx/peer_instruction/fields/events.py
 src/ralph/models/edx/problem_interaction/__init__.py
 src/ralph/models/edx/problem_interaction/statements.py
 src/ralph/models/edx/problem_interaction/fields/__init__.py
 src/ralph/models/edx/problem_interaction/fields/events.py
 src/ralph/models/edx/textbook_interaction/__init__.py
 src/ralph/models/edx/textbook_interaction/statements.py
 src/ralph/models/edx/textbook_interaction/fields/__init__.py
```

### Comparing `ralph-malph-3.7.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-3.8.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
 bandit==1.7.5
 black==23.3.0
-cryptography==40.0.1
+cryptography==41.0.1
 factory-boy==3.2.1
 flake8==6.0.0
-hypothesis==6.78.1
+hypothesis==6.79.1
 isort==5.12.0
-logging-gelf==0.0.26
+logging-gelf==0.0.31
 mkdocs==1.4.3
 mkdocs-click==0.8.0
-mkdocs-material==9.1.15
+mkdocs-material==9.1.16
 mkdocstrings[python-legacy]==0.22.0
 moto==4.1.11
 pydocstyle==6.3.0
 pyfakefs==5.2.2
 pylint==2.17.4
 pytest==7.3.2
 pytest-asyncio==0.21.0
```

### Comparing `ralph-malph-3.7.0/tests/test_cli.py` & `ralph-malph-3.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_cli_usage.py` & `ralph-malph-3.8.0/tests/test_cli_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,17 @@
         "    --es-client-options KEY=VALUE,KEY=VALUE\n"
         "    --es-index TEXT\n"
         "    --es-hosts VALUE1,VALUE2,VALUE3\n"
         "  -c, --chunk-size INTEGER        Get events by chunks of size #\n"
         "  -t, --target TEXT               Endpoint from which to fetch events (e.g.\n"
         "                                  `/statements`)\n"
         '  -q, --query \'{"KEY": "VALUE", "KEY": "VALUE"}\'\n'
-        "                                  Query object as a JSON string (database\n"
-        "                                  backends ONLY)\n"
+        "                                  Query object as a JSON string (database "
+        "and\n"
+        "                                  HTTP backends ONLY)\n"
     ) in result.output
     logging.warning(result.output)
     result = runner.invoke(cli, ["fetch"])
     assert result.exit_code > 0
     assert (
         "Error: Missing option '-b' / '--backend'. "
         "Choose from:\n\tes,\n\tmongo,\n\tclickhouse,\n\tlrs,\n\tldp,\n\tfs,\n\tswift,"
```

### Comparing `ralph-malph-3.7.0/tests/test_conf.py` & `ralph-malph-3.8.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_dependencies.py` & `ralph-malph-3.8.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_filters.py` & `ralph-malph-3.8.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_logger.py` & `ralph-malph-3.8.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_parsers.py` & `ralph-malph-3.8.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.7.0/tests/test_utils.py` & `ralph-malph-3.8.0/tests/test_utils.py`

 * *Files identical despite different names*

