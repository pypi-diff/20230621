# Comparing `tmp/erlang_py-2.0.5.tar.gz` & `tmp/erlang_py-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlang_py-2.0.5.tar", last modified: Wed Oct 12 19:57:11 2022, max compression
+gzip compressed data, was "erlang_py-2.0.6.tar", last modified: Wed Jun 21 06:50:53 2023, max compression
```

## Comparing `erlang_py-2.0.5.tar` & `erlang_py-2.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2022-10-12 19:57:11.639712 erlang_py-2.0.5/
--rw-rw-r--   0 george    (1000) george    (1000)     1128 2022-02-20 03:46:41.000000 erlang_py-2.0.5/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)     1657 2022-10-12 19:57:11.639712 erlang_py-2.0.5/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      661 2022-10-12 19:54:44.000000 erlang_py-2.0.5/README.rst
--rwxrwxr-x   0 george    (1000) george    (1000)    32765 2022-10-12 19:53:22.000000 erlang_py-2.0.5/erlang.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2022-10-12 19:57:11.639712 erlang_py-2.0.5/erlang_py.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)     1657 2022-10-12 19:57:11.000000 erlang_py-2.0.5/erlang_py.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      169 2022-10-12 19:57:11.000000 erlang_py-2.0.5/erlang_py.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2022-10-12 19:57:11.000000 erlang_py-2.0.5/erlang_py.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)        7 2022-10-12 19:57:11.000000 erlang_py-2.0.5/erlang_py.egg-info/top_level.txt
--rw-rw-r--   0 george    (1000) george    (1000)       38 2022-10-12 19:57:11.639712 erlang_py-2.0.5/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)     1516 2022-10-12 19:54:35.000000 erlang_py-2.0.5/setup.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 06:50:53.403649 erlang_py-2.0.6/
+-rw-rw-r--   0 george    (1000) george    (1000)     1128 2023-05-20 05:09:41.000000 erlang_py-2.0.6/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)     1660 2023-06-21 06:50:53.403649 erlang_py-2.0.6/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      664 2023-06-21 06:48:30.000000 erlang_py-2.0.6/README.rst
+-rwxrwxr-x   0 george    (1000) george    (1000)    33602 2023-05-20 20:07:54.000000 erlang_py-2.0.6/erlang.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 06:50:53.403649 erlang_py-2.0.6/erlang_py.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)     1660 2023-06-21 06:50:52.000000 erlang_py-2.0.6/erlang_py.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      169 2023-06-21 06:50:52.000000 erlang_py-2.0.6/erlang_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-06-21 06:50:52.000000 erlang_py-2.0.6/erlang_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        7 2023-06-21 06:50:52.000000 erlang_py-2.0.6/erlang_py.egg-info/top_level.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-21 06:50:53.403649 erlang_py-2.0.6/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)     1516 2023-06-21 06:46:02.000000 erlang_py-2.0.6/setup.py
```

### Comparing `erlang_py-2.0.5/LICENSE` & `erlang_py-2.0.6/LICENSE`

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

### Comparing `erlang_py-2.0.5/PKG-INFO` & `erlang_py-2.0.6/erlang_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: erlang_py
-Version: 2.0.5
+Name: erlang-py
+Version: 2.0.6
 Summary: Erlang External Term Format for Python
 Home-page: https://github.com/okeuday/erlang_py
 Author: Michael Truog
 Author-email: mjtruog@protonmail.com
 License: MIT
 Description: Erlang External Term Format for Python
         ======================================
         
         |Build Status|
         
         Provides all encoding and decoding for the Erlang External Term Format
-        (as defined at http://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
+        (as defined at https://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
         single Python module.
         
         Available as a `Python package at
         ``https://pypi.python.org/pypi/erlang_py/`` <https://pypi.python.org/pypi/erlang_py/>`__.
         
         Tests
         -----
@@ -31,16 +31,16 @@
         Michael Truog (mjtruog at protonmail dot com)
         
         License
         -------
         
         MIT License
         
-        .. |Build Status| image:: https://secure.travis-ci.org/okeuday/erlang_py.png?branch=master
-           :target: http://travis-ci.org/okeuday/erlang_py
+        .. |Build Status| image:: https://app.travis-ci.com/okeuday/erlang_py.svg?branch=master
+           :target: https://app.travis-ci.com/okeuday/erlang_py
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `erlang_py-2.0.5/README.rst` & `erlang_py-2.0.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Erlang External Term Format for Python
 ======================================
 
 |Build Status|
 
 Provides all encoding and decoding for the Erlang External Term Format
-(as defined at http://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
+(as defined at https://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
 single Python module.
 
 Available as a `Python package at
 ``https://pypi.python.org/pypi/erlang_py/`` <https://pypi.python.org/pypi/erlang_py/>`__.
 
 Tests
 -----
@@ -23,9 +23,9 @@
 Michael Truog (mjtruog at protonmail dot com)
 
 License
 -------
 
 MIT License
 
-.. |Build Status| image:: https://secure.travis-ci.org/okeuday/erlang_py.png?branch=master
-   :target: http://travis-ci.org/okeuday/erlang_py
+.. |Build Status| image:: https://app.travis-ci.com/okeuday/erlang_py.svg?branch=master
+   :target: https://app.travis-ci.com/okeuday/erlang_py
```

### Comparing `erlang_py-2.0.5/erlang.py` & `erlang_py-2.0.6/erlang.py`

 * *Files 1% similar despite different names*

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
@@ -23,14 +23,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 """
 Erlang External Term Format Encoding/Decoding
 """
+# pylint: disable=too-many-lines
 
 import sys
 import struct
 import zlib
 import copy
 
 if sys.version_info[0] >= 3:
@@ -58,19 +59,19 @@
         """
         bytes ord function
         """
         return ord(character)
 
 __all__ = ['OtpErlangAtom',
            'OtpErlangBinary',
-           'OtpErlangFunction',
            'OtpErlangList',
            'OtpErlangPid',
            'OtpErlangPort',
            'OtpErlangReference',
+           'OtpErlangFunction',
            'binary_to_term',
            'term_to_binary',
            'set_undefined',
            'InputException',
            'OutputException',
            'ParseException']
 
@@ -104,14 +105,16 @@
 _TAG_EXPORT_EXT = 113
 _TAG_NEW_REFERENCE_EXT = 114
 _TAG_SMALL_ATOM_EXT = 115
 _TAG_MAP_EXT = 116
 _TAG_FUN_EXT = 117
 _TAG_ATOM_UTF8_EXT = 118
 _TAG_SMALL_ATOM_UTF8_EXT = 119
+_TAG_V4_PORT_EXT = 120
+_TAG_LOCAL_EXT = 121
 
 # Erlang term classes listed alphabetically
 
 class OtpErlangAtom(object):
     """
     OtpErlangAtom
     """
@@ -193,38 +196,14 @@
             self.__class__.__name__, repr(self.value), repr(self.bits)
         )
     def __hash__(self):
         return hash(self.binary())
     def __eq__(self, other):
         return self.binary() == other.binary()
 
-class OtpErlangFunction(object):
-    """
-    OtpErlangFunction
-    """
-    # pylint: disable=useless-object-inheritance
-    # pylint: disable=too-few-public-methods
-    def __init__(self, tag, value):
-        self.tag = tag
-        self.value = value
-    def binary(self):
-        """
-        return encoded representation
-        """
-        return b_chr(self.tag) + self.value
-    def __repr__(self):
-        return '%s(%s,%s)' % (
-            self.__class__.__name__,
-            repr(self.tag), repr(self.value)
-        )
-    def __hash__(self):
-        return hash(self.binary())
-    def __eq__(self, other):
-        return self.binary() == other.binary()
-
 class OtpErlangList(object):
     """
     OtpErlangList
     """
     # pylint: disable=useless-object-inheritance
     # pylint: disable=too-few-public-methods
     def __init__(self, value, improper=False):
@@ -314,25 +293,31 @@
         self.node = node
         self.id = id_value
         self.creation = creation
     def binary(self):
         """
         return encoded representation
         """
-        creation_size = len(self.creation)
-        if creation_size == 1:
+        id_size = len(self.id)
+        if id_size == 8:
             return (
-                b_chr(_TAG_PORT_EXT) +
+                b_chr(_TAG_V4_PORT_EXT) +
                 self.node.binary() + self.id + self.creation
             )
+        creation_size = len(self.creation)
         if creation_size == 4:
             return (
                 b_chr(_TAG_NEW_PORT_EXT) +
                 self.node.binary() + self.id + self.creation
             )
+        if creation_size == 1:
+            return (
+                b_chr(_TAG_PORT_EXT) +
+                self.node.binary() + self.id + self.creation
+            )
         raise OutputException('unknown port type')
     def __repr__(self):
         return '%s(%s,%s,%s)' % (
             self.__class__.__name__,
             repr(self.node), repr(self.id), repr(self.creation)
         )
     def __hash__(self):
@@ -383,14 +368,38 @@
             repr(self.node), repr(self.id), repr(self.creation)
         )
     def __hash__(self):
         return hash(self.binary())
     def __eq__(self, other):
         return self.binary() == other.binary()
 
+class OtpErlangFunction(object):
+    """
+    OtpErlangFunction
+    """
+    # pylint: disable=useless-object-inheritance
+    # pylint: disable=too-few-public-methods
+    def __init__(self, tag, value):
+        self.tag = tag
+        self.value = value
+    def binary(self):
+        """
+        return encoded representation
+        """
+        return b_chr(self.tag) + self.value
+    def __repr__(self):
+        return '%s(%s,%s)' % (
+            self.__class__.__name__,
+            repr(self.tag), repr(self.value)
+        )
+    def __hash__(self):
+        return hash(self.binary())
+    def __eq__(self, other):
+        return self.binary() == other.binary()
+
 # dependency to support Erlang maps as map keys in python
 
 class frozendict(dict):
     """
     frozendict is under the PSF (Python Software Foundation) License
     (from http://code.activestate.com/recipes/414283-frozen-dictionaries/)
     """
@@ -501,27 +510,33 @@
     if tag == _TAG_SMALL_INTEGER_EXT:
         return (i + 1, b_ord(data[i]))
     if tag == _TAG_INTEGER_EXT:
         return (i + 4, struct.unpack(b'>i', data[i:i + 4])[0])
     if tag == _TAG_FLOAT_EXT:
         value = float(data[i:i + 31].partition(b_chr(0))[0])
         return (i + 31, value)
-    if tag in (_TAG_NEW_PORT_EXT, _TAG_REFERENCE_EXT, _TAG_PORT_EXT):
+    if tag in (_TAG_V4_PORT_EXT, _TAG_NEW_PORT_EXT,
+               _TAG_REFERENCE_EXT, _TAG_PORT_EXT):
         i, node = _binary_to_atom(i, data)
-        id_value = data[i:i + 4]
-        i += 4
-        if tag == _TAG_NEW_PORT_EXT:
+        if tag == _TAG_V4_PORT_EXT:
+            id_value = data[i:i + 8]
+            i += 8
+        else:
+            id_value = data[i:i + 4]
+            i += 4
+        if tag in (_TAG_V4_PORT_EXT, _TAG_NEW_PORT_EXT):
             creation = data[i:i + 4]
             i += 4
         else:
             creation = data[i:i + 1]
             i += 1
             if tag == _TAG_REFERENCE_EXT:
                 return (i, OtpErlangReference(node, id_value, creation))
-        # tag == _TAG_NEW_PORT_EXT or tag == _TAG_PORT_EXT
+        # tag == _TAG_V4_PORT_EXT or tag == _TAG_NEW_PORT_EXT or
+        # tag == _TAG_PORT_EXT
         return (i, OtpErlangPort(node, id_value, creation))
     if tag in (_TAG_NEW_PID_EXT, _TAG_PID_EXT):
         i, node = _binary_to_atom(i, data)
         id_value = data[i:i + 4]
         i += 4
         serial = data[i:i + 4]
         i += 4
@@ -600,23 +615,27 @@
             creation = data[i:i + 1]
             i += 1
         return (i + j, OtpErlangReference(node, data[i: i + j], creation))
     if tag == _TAG_MAP_EXT:
         length = struct.unpack(b'>I', data[i:i + 4])[0]
         i += 4
         pairs = {}
+        def to_immutable(value):
+            if isinstance(value, dict):
+                return frozendict(key)
+            if isinstance(value, list):
+                return OtpErlangList(value)
+            if isinstance(value, tuple):
+                return tuple(to_immutable(v) for v in value)
+            return value
+
         for _ in range(length):
             i, key = _binary_to_term(i, data)
             i, value = _binary_to_term(i, data)
-            if isinstance(key, dict):
-                pairs[frozendict(key)] = value
-            elif isinstance(key, list):
-                pairs[OtpErlangList(key)] = value
-            else:
-                pairs[key] = value
+            pairs[to_immutable(key)] = value
         return (i, pairs)
     if tag == _TAG_FUN_EXT:
         old_i = i
         numfree = struct.unpack(b'>I', data[i:i + 4])[0]
         i += 4
         i, _ = _binary_to_pid(i, data)
         i, _ = _binary_to_atom(i, data)
@@ -666,14 +685,16 @@
         data_uncompressed = zlib.decompress(data_compressed)
         if size_uncompressed != len(data_uncompressed):
             raise ParseException('compression corrupt')
         (i_new, term) = _binary_to_term(0, data_uncompressed)
         if i_new != size_uncompressed:
             raise ParseException('unparsed data')
         return (i + j, term)
+    if tag == _TAG_LOCAL_EXT:
+        raise ParseException('LOCAL_EXT is opaque')
     raise ParseException('invalid tag')
 
 def _binary_to_term_sequence(i, length, data):
     sequence = []
     for _ in range(length):
         i, element = _binary_to_term(i, data)
         sequence.append(element)
@@ -862,16 +883,20 @@
             struct.pack(b'>I', length) + sign + b''.join(value)
         )
     raise OutputException('uint32 overflow')
 
 def _float_to_binary(term):
     return b_chr(_TAG_NEW_FLOAT_EXT) + struct.pack(b'>d', term)
 
-# Elixir use can set to b'nil'
 def set_undefined(value):
+    """
+    Set the 'undefined' atom that is decoded as None
+    (Elixir use may want to use 'nil' instead of 'undefined')
+    """
+    # pylint: disable=global-statement
     assert isinstance(value, bytes)
     global _UNDEFINED
     _UNDEFINED = value
 
 # Exception classes listed alphabetically
 
 class InputException(ValueError):
```

### Comparing `erlang_py-2.0.5/erlang_py.egg-info/PKG-INFO` & `erlang_py-2.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: erlang-py
-Version: 2.0.5
+Name: erlang_py
+Version: 2.0.6
 Summary: Erlang External Term Format for Python
 Home-page: https://github.com/okeuday/erlang_py
 Author: Michael Truog
 Author-email: mjtruog@protonmail.com
 License: MIT
 Description: Erlang External Term Format for Python
         ======================================
         
         |Build Status|
         
         Provides all encoding and decoding for the Erlang External Term Format
-        (as defined at http://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
+        (as defined at https://erlang.org/doc/apps/erts/erl_ext_dist.html) in a
         single Python module.
         
         Available as a `Python package at
         ``https://pypi.python.org/pypi/erlang_py/`` <https://pypi.python.org/pypi/erlang_py/>`__.
         
         Tests
         -----
@@ -31,16 +31,16 @@
         Michael Truog (mjtruog at protonmail dot com)
         
         License
         -------
         
         MIT License
         
-        .. |Build Status| image:: https://secure.travis-ci.org/okeuday/erlang_py.png?branch=master
-           :target: http://travis-ci.org/okeuday/erlang_py
+        .. |Build Status| image:: https://app.travis-ci.com/okeuday/erlang_py.svg?branch=master
+           :target: https://app.travis-ci.com/okeuday/erlang_py
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `erlang_py-2.0.5/setup.py` & `erlang_py-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Erlang',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Distributed Computing',
     ],
-    version='2.0.5',
+    version='2.0.6',
     description='Erlang External Term Format for Python',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Michael Truog',
     author_email='mjtruog@protonmail.com',
     url='https://github.com/okeuday/erlang_py',
 )
```

