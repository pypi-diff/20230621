# Comparing `tmp/logbox-1.0.6.tar.gz` & `tmp/logbox-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\matsc\Documents\Coding\py-logger\dist\.tmp-yyvo2sa6\logbox-1.0.6.tar", last modified: Fri Feb 10 08:48:17 2023, max compression
+gzip compressed data, was "logbox-1.0.7.tar", last modified: Wed Jun 21 08:50:42 2023, max compression
```

## Comparing `logbox-1.0.6.tar` & `logbox-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.916540 logbox-1.0.6/
--rw-rw-rw-   0        0        0     1070 2023-01-18 10:02:10.000000 logbox-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       15 2023-01-18 10:02:10.000000 logbox-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      707 2023-02-10 08:48:17.916540 logbox-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-01-18 10:02:10.000000 logbox-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-10 08:48:17.916540 logbox-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-02-10 08:47:44.000000 logbox-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.856096 logbox-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.875033 logbox-1.0.6/src/extension/
--rw-rw-rw-   0        0        0     4147 2023-01-18 10:02:10.000000 logbox-1.0.6/src/extension/windows.cpp
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.898861 logbox-1.0.6/src/logbox/
--rw-rw-rw-   0        0        0      317 2023-02-10 08:47:44.000000 logbox-1.0.6/src/logbox/__init__.py
--rw-rw-rw-   0        0        0     2970 2023-01-31 08:55:05.000000 logbox-1.0.6/src/logbox/_api.py
--rw-rw-rw-   0        0        0     4016 2023-01-31 08:55:05.000000 logbox-1.0.6/src/logbox/_channels.py
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.910866 logbox-1.0.6/src/logbox/_cli/
--rw-rw-rw-   0        0        0      245 2023-01-18 10:02:10.000000 logbox-1.0.6/src/logbox/_cli/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-18 10:02:10.000000 logbox-1.0.6/src/logbox/_cli/_bypass.py
--rw-rw-rw-   0        0        0     4272 2023-01-18 10:02:10.000000 logbox-1.0.6/src/logbox/_codes.py
--rw-rw-rw-   0        0        0     7139 2023-01-31 08:55:05.000000 logbox-1.0.6/src/logbox/_iterators.py
--rw-rw-rw-   0        0        0    22706 2023-02-10 08:47:44.000000 logbox-1.0.6/src/logbox/_logger.py
--rw-rw-rw-   0        0        0    14531 2023-01-18 10:02:10.000000 logbox-1.0.6/src/logbox/_progbars.py
--rw-rw-rw-   0        0        0     1949 2023-01-18 10:02:10.000000 logbox-1.0.6/src/logbox/_timeformat.py
-drwxrwxrwx   0        0        0        0 2023-02-10 08:48:17.906899 logbox-1.0.6/src/logbox.egg-info/
--rw-rw-rw-   0        0        0      707 2023-02-10 08:48:17.000000 logbox-1.0.6/src/logbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-02-10 08:48:17.000000 logbox-1.0.6/src/logbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 08:48:17.000000 logbox-1.0.6/src/logbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-10 08:48:17.000000 logbox-1.0.6/src/logbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.186798 logbox-1.0.7/
+-rw-rw-rw-   0        0        0     1070 2023-06-21 06:45:56.000000 logbox-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-06-21 06:45:56.000000 logbox-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      707 2023-06-21 08:50:42.171170 logbox-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-21 06:45:56.000000 logbox-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 08:50:42.186798 logbox-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-06-21 08:24:26.000000 logbox-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.076718 logbox-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.108202 logbox-1.0.7/src/extension/
+-rw-rw-rw-   0        0        0     4147 2023-06-21 06:45:56.000000 logbox-1.0.7/src/extension/windows.cpp
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.139903 logbox-1.0.7/src/logbox/
+-rw-rw-rw-   0        0        0      317 2023-06-21 08:24:26.000000 logbox-1.0.7/src/logbox/__init__.py
+-rw-rw-rw-   0        0        0     2970 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_api.py
+-rw-rw-rw-   0        0        0     4016 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_channels.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.171170 logbox-1.0.7/src/logbox/_cli/
+-rw-rw-rw-   0        0        0      245 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_cli/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_cli/_bypass.py
+-rw-rw-rw-   0        0        0     4301 2023-06-21 08:40:17.000000 logbox-1.0.7/src/logbox/_codes.py
+-rw-rw-rw-   0        0        0     7139 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_iterators.py
+-rw-rw-rw-   0        0        0    22706 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_logger.py
+-rw-rw-rw-   0        0        0    16502 2023-06-21 08:42:21.000000 logbox-1.0.7/src/logbox/_progbars.py
+-rw-rw-rw-   0        0        0     1949 2023-06-21 06:45:56.000000 logbox-1.0.7/src/logbox/_timeformat.py
+drwxrwxrwx   0        0        0        0 2023-06-21 08:50:42.171170 logbox-1.0.7/src/logbox.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-06-21 08:50:41.000000 logbox-1.0.7/src/logbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-21 08:50:42.000000 logbox-1.0.7/src/logbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 08:50:41.000000 logbox-1.0.7/src/logbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 08:50:41.000000 logbox-1.0.7/src/logbox.egg-info/top_level.txt
```

### Comparing `logbox-1.0.6/LICENSE` & `logbox-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/PKG-INFO` & `logbox-1.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logbox
-Version: 1.0.6
+Version: 1.0.7
 Summary: Toolbox for terminal output and logging to file
 Author: Matthias Nadig
 Author-email: matthias.nadig@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `logbox-1.0.6/setup.py` & `logbox-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 path_package_toplevel = 'src'
 
 ext_module = Extension('logbox._cli._windows',
                        sources=['src/extension/windows.cpp'],)
 
 setup(
     name='logbox',
-    version='1.0.6',
+    version='1.0.7',
     description='Toolbox for terminal output and logging to file',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Matthias Nadig',
     author_email='matthias.nadig@yahoo.com',
     license='MIT',
     package_dir={'': path_package_toplevel},
```

### Comparing `logbox-1.0.6/src/extension/windows.cpp` & `logbox-1.0.7/src/extension/windows.cpp`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox/_api.py` & `logbox-1.0.7/src/logbox/_api.py`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox/_channels.py` & `logbox-1.0.7/src/logbox/_channels.py`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox/_codes.py` & `logbox-1.0.7/src/logbox/_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,14 @@
 CARRIAGE_RETURN = '\r'
 
 PROGBAR_BG_RIGHT = '\033[48;5;251m'
 PROGBAR_BG_LEFT = '\033[48;5;240m'
 PROGBAR_FG_RIGHT = '\033[38;5;16m'
 PROGBAR_FG_LEFT = '\033[38;5;231m'
 
-COLOR_NEGATIVE = '\033[38;5;1m'
-COLOR_NEUTRAL = '\033[38;5;0m'
-COLOR_POSITIVE = '\033[38;5;2m'
-
 PROGBAR_INIT = 0
 PROGBAR_ACTIVE = 1
 PROGBAR_DONE = 2
 
 DEFAULT_STR_INFO = 'Processing step'
 
 
@@ -160,7 +156,11 @@
 if _is_bg_given:
     COLOR_DEFAULT_FONT_BG = _parse_font_color_from_rgb((1, 1, 1))
     RESET += COLOR_DEFAULT_FONT_BG
 else:
     COLOR_DEFAULT_FONT_BG = ''
 
 RED = _parse_font_color_from_rgb((170/255, 0, 0))
+
+COLOR_NEGATIVE = '\033[38;5;1m'
+COLOR_NEUTRAL = '\033[38;5;240m'  # RESET  # '\033[38;5;0m'
+COLOR_POSITIVE = '\033[38;5;2m'
```

### Comparing `logbox-1.0.6/src/logbox/_iterators.py` & `logbox-1.0.7/src/logbox/_iterators.py`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox/_logger.py` & `logbox-1.0.7/src/logbox/_logger.py`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox/_progbars.py` & `logbox-1.0.7/src/logbox/_progbars.py`

 * *Files 9% similar despite different names*

```diff
@@ -241,20 +241,22 @@
 def _check_smaller(val_prev, val_new):
     return np.sign(val_prev - val_new)
 
 
 class ColumnBase:
     def __init__(self,
                  name, type,
+                 layout_leading_line,
                  n_decimals=3,
                  show_change_negative=True, show_change_positive=True, show_change_neutral=True,
                  improvement_case='greater'):
         self.name = name
         self.type = type
         self.n_decimals = n_decimals
+        self.layout_leading_line = layout_leading_line
 
         self.value = 0
 
         if improvement_case == 'greater':
             self.improvement_check = _check_greater
         elif improvement_case == 'smaller':
             self.improvement_check = _check_smaller
@@ -270,73 +272,111 @@
         self.appendix_improve_neg = RESET if show_change_negative else ''
 
     def parse_leading_line(self, value_new):
         improvement = self.improvement_check(self.value, value_new)
         self.value = value_new
 
         if improvement < 0:
-            str_leading_line = self.layout_leading_line.format(self.prefix_improve_neg, value_new,
-                                                               self.appendix_improve_neg)
-        elif improvement == 0:
-            str_leading_line = self.layout_leading_line.format(self.prefix_improve_neu, value_new,
-                                                               self.appendix_improve_neu)
+            str_leading_line = self.layout_leading_line.parse(self.prefix_improve_neg, value_new,
+                                                              self.appendix_improve_neg)
+        elif improvement == 0 or np.isnan(improvement):
+            # This will catch both cases: When value_new is NaN and when self.value (previous value) is NaN
+            str_leading_line = self.layout_leading_line.parse(self.prefix_improve_neu, value_new,
+                                                              self.appendix_improve_neu)
         elif improvement > 0:
-            str_leading_line = self.layout_leading_line.format(self.prefix_improve_pos, value_new,
-                                                               self.appendix_improve_pos)
+            str_leading_line = self.layout_leading_line.parse(self.prefix_improve_pos, value_new,
+                                                              self.appendix_improve_pos)
         else:
             raise RuntimeError(improvement)
 
         return str_leading_line
 
 
 class ColumnOneliner(ColumnBase):
     def __init__(self,
                  name, type,
                  n_decimals=3, leading_chars=3,
                  show_change_negative=True, show_change_positive=True, show_change_neutral=True,
                  improvement_case='greater'):
-        super().__init__(name, type, n_decimals=n_decimals,
+        n_chars_value = _get_length_of_parsed_value(type, leading_chars, n_decimals=n_decimals)
+        delimiter = ': '
+
+        layout_leading_line = LayoutLeadingLine(prefix='{}'.format(name) + delimiter, n_chars_value=n_chars_value, type=type, n_decimals=n_decimals)
+
+        super().__init__(name, type,
+                         layout_leading_line=layout_leading_line, n_decimals=n_decimals,
                          show_change_negative=show_change_negative,
                          show_change_positive=show_change_positive,
                          show_change_neutral=show_change_neutral,
                          improvement_case=improvement_case)
 
-        n_chars_value = _get_length_of_parsed_value(type, leading_chars, n_decimals=n_decimals)
-        self.layout_value = _parse_template_value(n_chars_value, type, n_decimals=self.n_decimals)
+        # self.layout_value = _parse_template_value(n_chars_value, type, n_decimals=self.n_decimals)
 
-        delimiter = ': '
+        #delimiter = ': '
         # self.layout_headline =
-        self.layout_leading_line = '{}'.format(self.name) + delimiter + self.layout_value
+        #self.layout_leading_line = '{}'.format(self.name) + delimiter + self.layout_value
 
 
 class ColumnTable(ColumnBase):
     def __init__(self,
                  name, type,
                  n_decimals=3, leading_chars=3,
                  show_change_negative=True, show_change_positive=True, show_change_neutral=True,
                  improvement_case='greater'):
-        super().__init__(name, type, n_decimals=n_decimals,
+        n_chars_value = _get_length_of_parsed_value(type, leading_chars, n_decimals=n_decimals)
+        n_chars_name = len(self.name)
+        n_chars = max(n_chars_name, n_chars_value)
+        n_chars_value = n_chars - n_chars_value
+
+        layout_leading_line = LayoutLeadingLine(prefix='', n_chars_value=n_chars_value, type=type, n_decimals=n_decimals)
+
+        super().__init__(name, type,
+                         layout_leading_line=layout_leading_line, n_decimals=n_decimals,
                          show_change_negative=show_change_negative,
                          show_change_positive=show_change_positive,
                          show_change_neutral=show_change_neutral,
                          improvement_case=improvement_case)
 
-        n_chars_value = _get_length_of_parsed_value(type, leading_chars, n_decimals=n_decimals)
-        n_chars_name = len(self.name)
-        n_chars = max(n_chars_name, n_chars_value)
-        n_chars_value = n_chars - n_chars_value
-        self.layout_value = _parse_template_value(n_chars_value, type, n_decimals=self.n_decimals)
+        # self.layout_value = _parse_template_value(n_chars_value, type, n_decimals=self.n_decimals)
 
         self.str_headline = '{}'.format(self.name)
-        self.layout_leading_line = self.layout_value
+        # self.layout_leading_line = self.layout_value
 
     def get_headline(self):
         return self.str_headline
 
 
+class LayoutLeadingLine:
+    def __init__(self, prefix, n_chars_value, type, n_decimals):
+        self.layout_value = _parse_template_value(n_chars_value, type, n_decimals=n_decimals)
+        if type == 'float' and n_decimals > 0:
+            self.layout_nan = '-' * (n_chars_value - 1 - n_decimals)
+            self.layout_nan += '.'
+            self.layout_nan += '-' * n_decimals
+            self.layout_nan = '{}' + self.layout_nan + '{}'
+        if type == 'percent':
+            if n_decimals > 0:
+                self.layout_nan = '-' * (n_chars_value - 2 - 1 - n_decimals)
+                self.layout_nan += '.'
+                self.layout_nan += '-' * n_decimals
+            else:
+                self.layout_nan = '-' * (n_chars_value - 2)
+            self.layout_nan = '{}' + self.layout_nan + '{}' + ' %'
+        else:
+            self.layout_nan = '{}' + '-' * n_chars_value + '{}'
+        self.prefix = prefix
+
+    def parse(self, prefix_improvement, value, appendix_improvement):
+        value_parsed = \
+            self.layout_value.format(prefix_improvement, value, appendix_improvement) \
+            if not np.isnan(value) else \
+            self.layout_nan.format(prefix_improvement, appendix_improvement)
+        return self.prefix + value_parsed
+
+
 def _parse_template_value(n_chars, type, n_decimals=3, appendix_percent=' %'):
     if type == 'int':
         str_template_value = '{}{:' + str(n_chars) + 'd}{}'
     elif type == 'float':
         str_template_value = '{}{:' + str(n_chars) + '.' + str(n_decimals) + 'f}{}'
     elif type == 'percent':
         str_template_value = '{}{:' + str(n_chars - len(appendix_percent)) + '.' + str(
```

### Comparing `logbox-1.0.6/src/logbox/_timeformat.py` & `logbox-1.0.7/src/logbox/_timeformat.py`

 * *Files identical despite different names*

### Comparing `logbox-1.0.6/src/logbox.egg-info/PKG-INFO` & `logbox-1.0.7/src/logbox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logbox
-Version: 1.0.6
+Version: 1.0.7
 Summary: Toolbox for terminal output and logging to file
 Author: Matthias Nadig
 Author-email: matthias.nadig@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

