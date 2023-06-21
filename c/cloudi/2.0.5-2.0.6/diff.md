# Comparing `tmp/cloudi-2.0.5.tar.gz` & `tmp/cloudi-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudi-2.0.5.tar", last modified: Thu Oct 13 01:50:45 2022, max compression
+gzip compressed data, was "cloudi-2.0.6.tar", last modified: Wed Jun 21 09:44:16 2023, max compression
```

## Comparing `cloudi-2.0.5.tar` & `cloudi-2.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2022-10-13 01:50:45.986652 cloudi-2.0.5/
--rw-rw-r--   0 george    (1000) george    (1000)     1128 2022-06-05 01:20:23.000000 cloudi-2.0.5/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)     1531 2022-10-13 01:50:45.986652 cloudi-2.0.5/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      513 2019-01-26 03:43:53.000000 cloudi-2.0.5/README.rst
--rw-rw-r--   0 george    (1000) george    (1000)     4482 2022-10-13 01:47:02.000000 cloudi-2.0.5/assert.cpp
--rw-rw-r--   0 george    (1000) george    (1000)    91486 2022-10-13 01:47:02.000000 cloudi-2.0.5/cloudi.cpp
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2022-10-13 01:50:45.986652 cloudi-2.0.5/cloudi.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)     1531 2022-10-13 01:50:45.000000 cloudi-2.0.5/cloudi.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      254 2022-10-13 01:50:45.000000 cloudi-2.0.5/cloudi.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2022-10-13 01:50:45.000000 cloudi-2.0.5/cloudi.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       17 2022-10-13 01:50:45.000000 cloudi-2.0.5/cloudi.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       29 2022-10-13 01:50:45.000000 cloudi-2.0.5/cloudi.egg-info/top_level.txt
--rwxrwxr-x   0 george    (1000) george    (1000)    35222 2022-10-13 01:46:36.000000 cloudi-2.0.5/cloudi.py
--rwxrwxr-x   0 george    (1000) george    (1000)    15328 2022-10-13 01:46:36.000000 cloudi-2.0.5/cloudi_c.py
--rw-rw-r--   0 george    (1000) george    (1000)    57951 2022-10-13 01:46:39.000000 cloudi-2.0.5/cloudi_py.cpp
--rw-rw-r--   0 george    (1000) george    (1000)       85 2022-10-13 01:50:45.986652 cloudi-2.0.5/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)     1914 2022-10-13 01:48:42.000000 cloudi-2.0.5/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)     2248 2022-10-13 01:47:02.000000 cloudi-2.0.5/timer.cpp
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 09:44:16.838144 cloudi-2.0.6/
+-rw-rw-r--   0 george    (1000) george    (1000)     1128 2023-02-16 05:43:43.000000 cloudi-2.0.6/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)     1685 2023-06-21 09:44:16.838144 cloudi-2.0.6/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      651 2023-06-21 09:43:45.000000 cloudi-2.0.6/README.rst
+-rw-rw-r--   0 george    (1000) george    (1000)     4482 2023-06-21 09:43:13.000000 cloudi-2.0.6/assert.cpp
+-rw-rw-r--   0 george    (1000) george    (1000)     3189 2023-06-21 09:43:13.000000 cloudi-2.0.6/bind.cpp
+-rw-rw-r--   0 george    (1000) george    (1000)    94601 2023-06-21 09:43:13.000000 cloudi-2.0.6/cloudi.cpp
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 09:44:16.838144 cloudi-2.0.6/cloudi.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)     1685 2023-06-21 09:44:16.000000 cloudi-2.0.6/cloudi.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      263 2023-06-21 09:44:16.000000 cloudi-2.0.6/cloudi.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-06-21 09:44:16.000000 cloudi-2.0.6/cloudi.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       17 2023-06-21 09:44:16.000000 cloudi-2.0.6/cloudi.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       29 2023-06-21 09:44:16.000000 cloudi-2.0.6/cloudi.egg-info/top_level.txt
+-rwxrwxr-x   0 george    (1000) george    (1000)    36412 2023-02-18 04:21:58.000000 cloudi-2.0.6/cloudi.py
+-rwxrwxr-x   0 george    (1000) george    (1000)    16507 2023-02-18 04:21:58.000000 cloudi-2.0.6/cloudi_c.py
+-rw-rw-r--   0 george    (1000) george    (1000)    57951 2023-02-18 04:21:54.000000 cloudi-2.0.6/cloudi_py.cpp
+-rw-rw-r--   0 george    (1000) george    (1000)       85 2023-06-21 09:44:16.838144 cloudi-2.0.6/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)     1970 2023-06-21 09:42:40.000000 cloudi-2.0.6/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2248 2023-06-21 09:43:13.000000 cloudi-2.0.6/timer.cpp
```

### Comparing `cloudi-2.0.5/LICENSE` & `cloudi-2.0.6/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2011-2022 Michael Truog <mjtruog at protonmail dot com>
+Copyright (c) 2011-2023 Michael Truog <mjtruog at protonmail dot com>
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `cloudi-2.0.5/PKG-INFO` & `cloudi-2.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: cloudi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python CloudI API
 Home-page: https://cloudi.org
 Author: Michael Truog
 Author-email: mjtruog@protonmail.com
 License: MIT
 Description: ``cloudi_api_python``
         =====================
         
         |Build Status| |PyPI Package Version|
         
         Python `CloudI API <https://cloudi.org/api.html#1_Intro>`__
         
+        Available as a `PyPI package at
+        ``https://pypi.python.org/pypi/cloudi/`` <https://pypi.python.org/pypi/cloudi/>`__.
         
         Author
         ------
         
         Michael Truog (mjtruog at protonmail dot com)
         
         License
         -------
         
         MIT License
         
-        .. |Build Status| image:: https://travis-ci.org/CloudI/cloudi_api_python.png
-           :target: https://travis-ci.org/CloudI/cloudi_api_python
+        .. |Build Status| image:: https://app.travis-ci.com/CloudI/cloudi_api_python.svg?branch=master
+           :target: https://app.travis-ci.com/CloudI/cloudi_api_python
         .. |PyPI Package Version| image:: https://img.shields.io/pypi/v/cloudi.svg?maxAge=2592000
            :target: https://pypi.python.org/pypi/cloudi/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudi-2.0.5/assert.cpp` & `cloudi-2.0.6/assert.cpp`

 * *Files identical despite different names*

### Comparing `cloudi-2.0.5/cloudi.cpp` & `cloudi-2.0.6/cloudi.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //-*-Mode:C++;coding:utf-8;tab-width:4;c-basic-offset:4;indent-tabs-mode:()-*-
 // ex: set ft=cpp fenc=utf-8 sts=4 ts=4 sw=4 et nomod:
 //
 // MIT License
 //
-// Copyright (c) 2011-2022 Michael Truog <mjtruog at protonmail dot com>
+// Copyright (c) 2011-2023 Michael Truog <mjtruog at protonmail dot com>
 //
 // Permission is hereby granted, free of charge, to any person obtaining a
 // copy of this software and associated documentation files (the "Software"),
 // to deal in the Software without restriction, including without limitation
 // the rights to use, copy, modify, merge, publish, distribute, sublicense,
 // and/or sell copies of the Software, and to permit persons to whom the
 // Software is furnished to do so, subject to the following conditions:
@@ -28,14 +28,15 @@
 #undef CLOUDI_HPP // avoid header warning
 #include "cloudi.h"
 #define CLOUDI_HPP
 #include "config.h"
 #include "realloc_ptr.hpp"
 #include "copy_ptr.hpp"
 #include "timer.hpp"
+#include "bind.hpp"
 #include <unistd.h>
 #include <errno.h>
 #include <poll.h>
 #include <ei.h>
 #include <boost/shared_ptr.hpp>
 #include <boost/unordered_map.hpp>
 #include <boost/exception/all.hpp>
@@ -565,33 +566,46 @@
     ::fflush(stderr);
 }
 
 static int poll_request(cloudi_instance_t * api,
                         int timeout,
                         int external);
 
+static int getenv_to_uint32(char const * const name,
+                            uint32_t * const value)
+{
+    char const * const value_str = ::getenv(name);
+    if (value_str == 0)
+        return cloudi_invalid_input;
+    int const value_int = ::atoi(value_str);
+    if (value_int < 0)
+        return cloudi_invalid_input;
+    *value = static_cast<uint32_t>(value_int);
+    return cloudi_success;
+}
+
 int cloudi_initialize(cloudi_instance_t * api,
                       unsigned int const thread_index,
                       void * state)
 {
     if (api == 0)
         return cloudi_out_of_memory;
     char const * const protocol = ::getenv("CLOUDI_API_INIT_PROTOCOL");
     if (protocol == 0)
     {
         std::cerr <<
             "CloudI service execution must occur in CloudI" << std::endl;
         return cloudi_invalid_input;
     }
-    char const * const buffer_size_p = ::getenv("CLOUDI_API_INIT_BUFFER_SIZE");
-    if (buffer_size_p == 0)
-        return cloudi_invalid_input;
+    uint32_t buffer_size;
+    int result = getenv_to_uint32("CLOUDI_API_INIT_BUFFER_SIZE", &buffer_size);
+    if (result)
+        return result;
     ::memset(api, 0, sizeof(cloudi_instance_t));
     api->state = state;
-    uint32_t const buffer_size = ::atoi(buffer_size_p);
     if (::strcmp(protocol, "tcp") == 0)
     {
         api->fd = thread_index + 3;
         api->use_header = 1;
     }
     else if (::strcmp(protocol, "udp") == 0)
     {
@@ -642,16 +656,16 @@
     int index = 0;
     if (api->use_header)
         index = 4;
     if (ei_encode_version(buffer.get<char>(), &index))
         return cloudi_error_ei_encode;
     if (ei_encode_atom(buffer.get<char>(), &index, "init"))
         return cloudi_error_ei_encode;
-    int result = write_exact(api->fd, api->use_header,
-                             buffer.get<char>(), index);
+    result = write_exact(api->fd, api->use_header,
+                         buffer.get<char>(), index);
     if (result)
         return result;
 
     while (cloudi_timeout == (result = poll_request(api, 1000, 0)))
     {
     }
 
@@ -673,21 +687,19 @@
         return api->state;
     }
     return 0;
 }
 
 int cloudi_initialize_thread_count(unsigned int * const thread_count)
 {
-    char const * const value_str = ::getenv("CLOUDI_API_INIT_THREAD_COUNT");
-    if (value_str == 0)
-        return cloudi_invalid_input;
-    int const value = ::atoi(value_str);
-    if (value < 0)
-        return cloudi_invalid_input;
-    *thread_count = static_cast<unsigned int>(value);
+    uint32_t value = 0;
+    int result = getenv_to_uint32("CLOUDI_API_INIT_THREAD_COUNT", &value);
+    if (result)
+        return result;
+    *thread_count = value;
     return cloudi_success;
 }
 
 static int cloudi_subscribe_(cloudi_instance_t * api,
                              char const * const pattern,
                              callback_function const & f)
 {
@@ -1564,25 +1576,34 @@
                                   uint32_t & index,
                                   uint32_t & i)
 {
     i = *reinterpret_cast<uint32_t *>(&buffer[index]);
     index += sizeof(uint32_t);
 }
 
+static void store_incoming_int32(buffer_t const & buffer,
+                                 uint32_t & index,
+                                 int32_t & i)
+{
+    i = *reinterpret_cast<int32_t *>(&buffer[index]);
+    index += sizeof(int32_t);
+}
+
 static void store_incoming_int8(buffer_t const & buffer,
                                 uint32_t & index,
                                 int8_t & i)
 {
     i = *reinterpret_cast<int8_t *>(&buffer[index]);
     index += sizeof(int8_t);
 }
 
 static uint8_t get_incoming_uint8(buffer_t const & buffer,
                                   uint32_t & index)
 {
+    // return value required for safe bit field use
     uint8_t const i = *reinterpret_cast<uint8_t *>(&buffer[index]);
     index += sizeof(uint8_t);
     return i;
 }
 
 static bool handle_events(cloudi_instance_t * api,
                           int external,
@@ -1662,14 +1683,16 @@
     }
     else if (external && ! api->initialization_complete)
     {
         result = polling(api);
         if (result)
             return result;
         api->initialization_complete = 1;
+        if (bind_set(api->bind))
+            return cloudi_invalid_input;
     }
 
     buffer_t & buffer_recv = *reinterpret_cast<buffer_t *>(api->buffer_recv);
     buffer_t & buffer_call = *reinterpret_cast<buffer_t *>(api->buffer_call);
 
     timer & poll_timer = *reinterpret_cast<timer *>(api->poll_timer);
     if (timeout > 0)
@@ -1698,24 +1721,28 @@
         store_incoming_uint32(buffer_recv, index, command);
         switch (command)
         {
             case MESSAGE_INIT:
             {
                 store_incoming_uint32(buffer_recv, index, api->process_index);
                 store_incoming_uint32(buffer_recv, index, api->process_count);
-                store_incoming_uint32(buffer_recv, index, api->process_count_max);
-                store_incoming_uint32(buffer_recv, index, api->process_count_min);
+                store_incoming_uint32(buffer_recv, index,
+                                      api->process_count_max);
+                store_incoming_uint32(buffer_recv, index,
+                                      api->process_count_min);
                 store_incoming_binary(buffer_recv, index, api->prefix);
                 store_incoming_uint32(buffer_recv, index,
                                       api->timeout_initialize);
                 store_incoming_uint32(buffer_recv, index, api->timeout_async);
                 store_incoming_uint32(buffer_recv, index, api->timeout_sync);
-                store_incoming_uint32(buffer_recv, index, api->timeout_terminate);
+                store_incoming_uint32(buffer_recv, index,
+                                      api->timeout_terminate);
                 store_incoming_int8(buffer_recv, index, api->priority_default);
                 api->fatal_exceptions = get_incoming_uint8(buffer_recv, index);
+                store_incoming_int32(buffer_recv, index, api->bind);
                 if (index != api->buffer_recv_index)
                 {
                     assert(! external);
                     if (! handle_events(api, external, index, result))
                         return result;
                 }
                 api->buffer_recv_index = 0;
@@ -2066,14 +2093,40 @@
 
 void cloudi_free_response(cloudi_instance_t * api)
 {
     assert(api->free_response == 0);
     api->free_response = 1;
 }
 
+int cloudi_initialize_process_index(uint32_t * const process_index)
+{
+    return getenv_to_uint32("CLOUDI_API_INIT_PROCESS_INDEX",
+                            process_index);
+}
+int cloudi_initialize_process_count_max(uint32_t * const process_count_max)
+{
+    return getenv_to_uint32("CLOUDI_API_INIT_PROCESS_COUNT_MAX",
+                            process_count_max);
+}
+int cloudi_initialize_process_count_min(uint32_t * const process_count_min)
+{
+    return getenv_to_uint32("CLOUDI_API_INIT_PROCESS_COUNT_MIN",
+                            process_count_min);
+}
+int cloudi_initialize_timeout_initialize(uint32_t * const timeout_initialize)
+{
+    return getenv_to_uint32("CLOUDI_API_INIT_TIMEOUT_INITIALIZE",
+                            timeout_initialize);
+}
+int cloudi_initialize_timeout_terminate(uint32_t * const timeout_terminate)
+{
+    return getenv_to_uint32("CLOUDI_API_INIT_TIMEOUT_TERMINATE",
+                            timeout_terminate);
+}
+
 } // extern C
 
 // C++ API
 namespace CloudI
 {
 
 API::API(unsigned int const thread_index,
@@ -2519,39 +2572,79 @@
 }
 
 uint32_t API::process_index() const
 {
     return m_impl.api()->process_index;
 }
 
+uint32_t API::process_index_()
+{
+    uint32_t process_index;
+    int const result =
+        cloudi_initialize_process_index(&process_index);
+    if (result != return_value::success)
+        throw invalid_input_exception(result);
+    return process_index;
+}
+
 uint32_t API::process_count() const
 {
     return m_impl.api()->process_count;
 }
 
 uint32_t API::process_count_max() const
 {
     return m_impl.api()->process_count_max;
 }
 
+uint32_t API::process_count_max_()
+{
+    uint32_t process_count_max;
+    int const result =
+        cloudi_initialize_process_count_max(&process_count_max);
+    if (result != return_value::success)
+        throw invalid_input_exception(result);
+    return process_count_max;
+}
+
 uint32_t API::process_count_min() const
 {
     return m_impl.api()->process_count_min;
 }
 
+uint32_t API::process_count_min_()
+{
+    uint32_t process_count_min;
+    int const result =
+        cloudi_initialize_process_count_min(&process_count_min);
+    if (result != return_value::success)
+        throw invalid_input_exception(result);
+    return process_count_min;
+}
+
 char const * API::prefix() const
 {
     return m_impl.api()->prefix;
 }
 
 uint32_t API::timeout_initialize() const
 {
     return m_impl.api()->timeout_initialize;
 }
 
+uint32_t API::timeout_initialize_()
+{
+    uint32_t timeout_initialize;
+    int const result =
+        cloudi_initialize_timeout_initialize(&timeout_initialize);
+    if (result != return_value::success)
+        throw invalid_input_exception(result);
+    return timeout_initialize;
+}
+
 uint32_t API::timeout_async() const
 {
     return m_impl.api()->timeout_async;
 }
 
 uint32_t API::timeout_sync() const
 {
@@ -2559,14 +2652,24 @@
 }
 
 uint32_t API::timeout_terminate() const
 {
     return m_impl.api()->timeout_terminate;
 }
 
+uint32_t API::timeout_terminate_()
+{
+    uint32_t timeout_terminate;
+    int const result =
+        cloudi_initialize_timeout_terminate(&timeout_terminate);
+    if (result != return_value::success)
+        throw invalid_input_exception(result);
+    return timeout_terminate;
+}
+
 int8_t API::priority_default() const
 {
     return m_impl.api()->priority_default;
 }
 
 int API::poll(int timeout) const
 {
```

### Comparing `cloudi-2.0.5/cloudi.egg-info/PKG-INFO` & `cloudi-2.0.6/cloudi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: cloudi
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python CloudI API
 Home-page: https://cloudi.org
 Author: Michael Truog
 Author-email: mjtruog@protonmail.com
 License: MIT
 Description: ``cloudi_api_python``
         =====================
         
         |Build Status| |PyPI Package Version|
         
         Python `CloudI API <https://cloudi.org/api.html#1_Intro>`__
         
+        Available as a `PyPI package at
+        ``https://pypi.python.org/pypi/cloudi/`` <https://pypi.python.org/pypi/cloudi/>`__.
         
         Author
         ------
         
         Michael Truog (mjtruog at protonmail dot com)
         
         License
         -------
         
         MIT License
         
-        .. |Build Status| image:: https://travis-ci.org/CloudI/cloudi_api_python.png
-           :target: https://travis-ci.org/CloudI/cloudi_api_python
+        .. |Build Status| image:: https://app.travis-ci.com/CloudI/cloudi_api_python.svg?branch=master
+           :target: https://app.travis-ci.com/CloudI/cloudi_api_python
         .. |PyPI Package Version| image:: https://img.shields.io/pypi/v/cloudi.svg?maxAge=2592000
            :target: https://pypi.python.org/pypi/cloudi/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudi-2.0.5/cloudi.py` & `cloudi-2.0.6/cloudi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 #-*-Mode:python;coding:utf-8;tab-width:4;c-basic-offset:4;indent-tabs-mode:()-*-
 # ex: set ft=python fenc=utf-8 sts=4 ts=4 sw=4 et nomod:
 #
 # MIT License
 #
-# Copyright (c) 2011-2022 Michael Truog <mjtruog at protonmail dot com>
+# Copyright (c) 2011-2023 Michael Truog <mjtruog at protonmail dot com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -86,17 +86,15 @@
     SYNC = -1
 
     def __init__(self, thread_index):
         protocol_str = os.getenv('CLOUDI_API_INIT_PROTOCOL')
         if protocol_str is None:
             sys.stderr.write('CloudI service execution must occur in CloudI\n')
             raise InvalidInputException()
-        buffer_size_str = os.getenv('CLOUDI_API_INIT_BUFFER_SIZE')
-        if buffer_size_str is None:
-            raise InvalidInputException()
+        buffer_size = API.__getenv_to_uint('CLOUDI_API_INIT_BUFFER_SIZE')
         if protocol_str == 'tcp':
             self.__s = socket.fromfd(
                 thread_index + 3, socket.AF_INET, socket.SOCK_STREAM
             )
             self.__use_header = True
         elif protocol_str == 'udp':
             self.__s = socket.fromfd(
@@ -108,15 +106,15 @@
                 thread_index + 3, socket.AF_UNIX, socket.SOCK_STREAM
             )
             self.__use_header = True
         else:
             raise InvalidInputException()
         self.__initialization_complete = False
         self.__terminate = False
-        self.__size = int(buffer_size_str)
+        self.__size = buffer_size
         self.__callbacks = {}
         self.__timeout_terminate = 10 # TIMEOUT_TERMINATE_MIN
         self.__send(term_to_binary(OtpErlangAtom(b'init')))
         (self.__process_index,
          self.__process_count,
          self.__process_count_max,
          self.__process_count_min,
@@ -128,18 +126,15 @@
          self.__fatal_exceptions) = self.__poll_request(None, False)
 
     @staticmethod
     def thread_count():
         """
         returns the thread count from the service configuration
         """
-        thread_count = os.getenv('CLOUDI_API_INIT_THREAD_COUNT')
-        if thread_count is None:
-            raise InvalidInputException()
-        return int(thread_count)
+        return API.__getenv_to_uint('CLOUDI_API_INIT_THREAD_COUNT')
 
     def subscribe(self, pattern, function):
         """
         subscribes to a service name pattern with a callback
         """
         if _function_argc(function) != 10:
             # self + arguments for a member function
@@ -332,44 +327,72 @@
 
     def process_index(self):
         """
         returns the 0-based index of this process in the service instance
         """
         return self.__process_index
 
+    @staticmethod
+    def process_index_():
+        """
+        returns the 0-based index of this process in the service instance
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_INDEX')
+
     def process_count(self):
         """
         returns the current process count based on the service configuration
         """
         return self.__process_count
 
     def process_count_max(self):
         """
         returns the count_process_dynamic maximum count
         """
         return self.__process_count_max
 
+    @staticmethod
+    def process_count_max_():
+        """
+        returns the count_process_dynamic maximum count
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_COUNT_MAX')
+
     def process_count_min(self):
         """
         returns the count_process_dynamic minimum count
         """
         return self.__process_count_min
 
+    @staticmethod
+    def process_count_min_():
+        """
+        returns the count_process_dynamic minimum count
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_COUNT_MIN')
+
     def prefix(self):
         """
         returns the service name pattern prefix from the service configuration
         """
         return self.__prefix
 
     def timeout_initialize(self):
         """
         returns the service initialization timeout
         """
         return self.__timeout_initialize
 
+    @staticmethod
+    def timeout_initialize_():
+        """
+        returns the service initialization timeout
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_TIMEOUT_INITIALIZE')
+
     def timeout_async(self):
         """
         returns the default asynchronous service request send timeout
         """
         return self.__timeout_async
 
     def timeout_sync(self):
@@ -380,14 +403,21 @@
 
     def timeout_terminate(self):
         """
         returns the service termination timeout
         """
         return self.__timeout_terminate
 
+    @staticmethod
+    def timeout_terminate_():
+        """
+        returns the service termination timeout
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_TIMEOUT_TERMINATE')
+
     def priority_default(self):
         """
         returns the default service request send priority
         """
         return self.__priority_default
 
     def __null_response(self, request_type, name, pattern,
@@ -594,20 +624,22 @@
         while True:
             command = struct.unpack(b'=I', data[i:j])[0]
             if command == _MESSAGE_INIT:
                 i, j = j, j + 4 + 4 + 4 + 4 + 4
                 (process_index, process_count,
                  process_count_max, process_count_min,
                  prefix_size) = struct.unpack(b'=IIIII', data[i:j])
-                i, j = j, j + prefix_size + 4 + 4 + 4 + 4 + 1 + 1
+                i, j = j, j + prefix_size + 4 + 4 + 4 + 4 + 1 + 1 + 4
                 (prefix, _, timeout_initialize,
                  timeout_async, timeout_sync, timeout_terminate,
-                 priority_default, fatal_exceptions) = struct.unpack(
-                     '=%dscIIIIbB' % (prefix_size - 1), data[i:j]
+                 priority_default, fatal_exceptions, bind) = struct.unpack(
+                     '=%dscIIIIbBi' % (prefix_size - 1), data[i:j]
                  )
+                if bind >= 0:
+                    raise InvalidInputException()
                 if j != data_size:
                     assert external is False
                     self.__handle_events(external, data, data_size, j)
                 return (process_index, process_count,
                         process_count_max, process_count_min,
                         prefix.decode('utf-8'), timeout_initialize,
                         timeout_sync, timeout_async, timeout_terminate,
@@ -839,14 +871,24 @@
                 data += fragment
                 ready = (len(fragment) == self.__size)
                 if ready:
                     fd_in, _, _ = select.select([self.__s], [], [], 0)
                     ready = (fd_in != [])
         return data
 
+    @staticmethod
+    def __getenv_to_uint(name):
+        value_str = os.getenv(name)
+        if value_str is None:
+            raise InvalidInputException()
+        value = int(value_str)
+        if value < 0:
+            raise InvalidInputException()
+        return value
+
 class InvalidInputException(Exception):
     """
     Invalid Input
     """
     def __init__(self):
         Exception.__init__(self, 'Invalid Input')
```

### Comparing `cloudi-2.0.5/cloudi_c.py` & `cloudi-2.0.6/cloudi_c.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 #-*-Mode:python;coding:utf-8;tab-width:4;c-basic-offset:4;indent-tabs-mode:()-*-
 # ex: set ft=python fenc=utf-8 sts=4 ts=4 sw=4 et nomod:
 #
 # MIT License
 #
-# Copyright (c) 2012-2022 Michael Truog <mjtruog at protonmail dot com>
+# Copyright (c) 2012-2023 Michael Truog <mjtruog at protonmail dot com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
@@ -72,18 +72,15 @@
                                            TerminateException)
 
     @staticmethod
     def thread_count():
         """
         returns the thread count from the service configuration
         """
-        thread_count = os.getenv('CLOUDI_API_INIT_THREAD_COUNT')
-        if thread_count is None:
-            raise InvalidInputException()
-        return int(thread_count)
+        return API.__getenv_to_uint('CLOUDI_API_INIT_THREAD_COUNT')
 
     def subscribe(self, pattern, function):
         """
         subscribes to a service name pattern with a callback
         """
         if _function_argc(function) != 10:
             # self + arguments for a member function
@@ -241,44 +238,72 @@
 
     def process_index(self):
         """
         returns the 0-based index of this process in the service instance
         """
         return self.__api.process_index()
 
+    @staticmethod
+    def process_index_():
+        """
+        returns the 0-based index of this process in the service instance
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_INDEX')
+
     def process_count(self):
         """
         returns the current process count based on the service configuration
         """
         return self.__api.process_count()
 
     def process_count_max(self):
         """
         returns the count_process_dynamic maximum count
         """
         return self.__api.process_count_max()
 
+    @staticmethod
+    def process_count_max_():
+        """
+        returns the count_process_dynamic maximum count
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_COUNT_MAX')
+
     def process_count_min(self):
         """
         returns the count_process_dynamic minimum count
         """
         return self.__api.process_count_min()
 
+    @staticmethod
+    def process_count_min_():
+        """
+        returns the count_process_dynamic minimum count
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_PROCESS_COUNT_MIN')
+
     def prefix(self):
         """
         returns the service name pattern prefix from the service configuration
         """
         return self.__api.prefix()
 
     def timeout_initialize(self):
         """
         returns the service initialization timeout
         """
         return self.__api.timeout_initialize()
 
+    @staticmethod
+    def timeout_initialize_():
+        """
+        returns the service initialization timeout
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_TIMEOUT_INITIALIZE')
+
     def timeout_async(self):
         """
         returns the default asynchronous service request send timeout
         """
         return self.__api.timeout_async()
 
     def timeout_sync(self):
@@ -289,14 +314,21 @@
 
     def timeout_terminate(self):
         """
         returns the service termination timeout
         """
         return self.__api.timeout_terminate()
 
+    @staticmethod
+    def timeout_terminate_():
+        """
+        returns the service termination timeout
+        """
+        return API.__getenv_to_uint('CLOUDI_API_INIT_TIMEOUT_TERMINATE')
+
     def priority_default(self):
         """
         returns the default service request send priority
         """
         return self.__api.priority_default()
 
     def poll(self, timeout=-1):
@@ -362,14 +394,24 @@
     @staticmethod
     def info_key_value_new(pairs, response=True):
         """
         encode service response info key/value data
         """
         return API.__text_pairs_new(pairs, response)
 
+    @staticmethod
+    def __getenv_to_uint(name):
+        value_str = os.getenv(name)
+        if value_str is None:
+            raise InvalidInputException()
+        value = int(value_str)
+        if value < 0:
+            raise InvalidInputException()
+        return value
+
 class InvalidInputException(Exception):
     """
     Invalid Input
     """
     def __init__(self, message=None):
         if message is None:
             message = 'Invalid Input'
```

### Comparing `cloudi-2.0.5/cloudi_py.cpp` & `cloudi-2.0.6/cloudi_py.cpp`

 * *Files identical despite different names*

### Comparing `cloudi-2.0.5/setup.py` & `cloudi-2.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     ext_modules=[
         Extension(
             name='libcloudi_py',
             sources=[
                 'cloudi_py.cpp',
                 'assert.cpp',
                 'timer.cpp',
+                'bind.cpp',
                 'cloudi.cpp',
             ],
             depends=[
                 'config.h',
                 'assert.hpp',
                 'copy_ptr.hpp',
                 'realloc_ptr.hpp',
                 'timer.hpp',
+                'bind.hpp',
                 'cloudi.h',
                 'cloudi.hpp',
             ],
             libraries=[
                 'ei',
                 'rt',
                 'stdc++',
@@ -46,16 +48,16 @@
         'Operating System :: Unix',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: System :: Clustering',
         'Topic :: System :: Distributed Computing',
     ],
-    version='2.0.5',
+    version='2.0.6',
     description='Python CloudI API',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Michael Truog',
     author_email='mjtruog@protonmail.com',
     url='https://cloudi.org',
-    install_requires=['erlang_py==2.0.5'],
+    install_requires=['erlang_py==2.0.6'],
 )
```

### Comparing `cloudi-2.0.5/timer.cpp` & `cloudi-2.0.6/timer.cpp`

 * *Files identical despite different names*

