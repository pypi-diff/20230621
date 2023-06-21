# Comparing `tmp/tablepic-0.0.3.tar.gz` & `tmp/tablepic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepic-0.0.3.tar", last modified: Mon Jun 19 02:58:28 2023, max compression
+gzip compressed data, was "tablepic-0.0.4.tar", last modified: Wed Jun 21 12:53:23 2023, max compression
```

## Comparing `tablepic-0.0.3.tar` & `tablepic-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.147264 tablepic-0.0.3/
--rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.3/LICENSE
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-19 02:58:28.147097 tablepic-0.0.3/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)    15596 2023-06-16 07:44:46.000000 tablepic-0.0.3/README.md
--rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-19 02:56:56.000000 tablepic-0.0.3/pyproject.toml
--rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.3/readme_pypi.md
--rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-19 02:58:28.147349 tablepic-0.0.3/setup.cfg
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.145267 tablepic-0.0.3/src/
--rw-r--r--   0 xinyan     (501) staff       (20)     8232 2023-06-16 07:25:04.000000 tablepic-0.0.3/src/demo.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.146041 tablepic-0.0.3/src/tablepic/
--rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.3/src/tablepic/__init__.py
--rw-r--r--   0 xinyan     (501) staff       (20)    15925 2023-06-16 07:20:40.000000 tablepic-0.0.3/src/tablepic/main.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.146899 tablepic-0.0.3/src/tablepic.egg-info/
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/SOURCES.txt
--rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/dependency_links.txt
--rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/top_level.txt
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.078843 tablepic-0.0.4/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.4/LICENSE
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-21 12:53:23.078691 tablepic-0.0.4/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)    16193 2023-06-20 15:57:19.000000 tablepic-0.0.4/README.md
+-rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-21 12:53:16.000000 tablepic-0.0.4/pyproject.toml
+-rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.4/readme_pypi.md
+-rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-21 12:53:23.078885 tablepic-0.0.4/setup.cfg
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.077299 tablepic-0.0.4/src/
+-rw-r--r--   0 xinyan     (501) staff       (20)     9265 2023-06-20 06:10:03.000000 tablepic-0.0.4/src/demo.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.077701 tablepic-0.0.4/src/tablepic/
+-rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.4/src/tablepic/__init__.py
+-rw-r--r--   0 xinyan     (501) staff       (20)    16949 2023-06-20 04:54:03.000000 tablepic-0.0.4/src/tablepic/main.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-21 12:53:23.078502 tablepic-0.0.4/src/tablepic.egg-info/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/SOURCES.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/dependency_links.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-21 12:53:23.000000 tablepic-0.0.4/src/tablepic.egg-info/top_level.txt
```

### Comparing `tablepic-0.0.3/LICENSE` & `tablepic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.3/PKG-INFO` & `tablepic-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablepic-0.0.3/README.md` & `tablepic-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!--
  * @Author: xinyan
  * @Date: 2023-06-15 15:11:57
  * @LastEditors: xinyan
- * @LastEditTime: 2023-06-16 15:44:45
+ * @LastEditTime: 2023-06-20 23:57:16
  * @Description: file content
 -->
 
 # TablePic
 ## Overview
 This package uses PIL (pillow) to generate a picture that contains a table. It has similar functionality to matplotlib's table, but includes more customization options.
 
@@ -14,14 +14,26 @@
 
 Use pip to install the package.
 
 ```shell
 pip install tablepic
 ```
 
+## Release Note
+### v0.0.4
+In previous versions, the default width of all columns was the same and fixed. If the length of the contents in the table was too long, it would cause overlapping of the content, and the table could not adjust its width according to the contents. In v0.0.4, the recognition of the width and height of the table content was added, automatically setting the appropriate height for each column and row.
+
+Result of version v0.0.4:
+
+![adaptive_width_table](pic/adaptive_width_table.jpg)
+
+Result of version v0.0.3 and before:
+
+![fixed_width_table](pic/fixed_width_table.jpg)
+
 ## Instruction
 
 ### Basic Table
 
 The following code generate a basic table picture, it contains a title and a 10*8 regular table. The table has 1 header row and 9 data rows.
 
 ```python
```

### Comparing `tablepic-0.0.3/pyproject.toml` & `tablepic-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablepic"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Xin Yan", email="slash.xin@gmail.com" },
 ]
 description = "A package can generate a picture which contains a table."
 readme = "readme_pypi.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tablepic-0.0.3/src/demo.py` & `tablepic-0.0.4/src/demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: xinyan
 Date: 2023-06-14 23:43:57
 LastEditors: xinyan
-LastEditTime: 2023-06-16 15:24:58
+LastEditTime: 2023-06-20 14:10:03
 Description: file content
 '''
 import tablepic as tp
 
 
 # ---------------------------------
 # Generate a regular table.
@@ -14,55 +14,55 @@
 
 
 # the title you want to put on the table
 title_list = [{'content': 'This is a title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table1.jpg')
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table1.jpg')
 
 
 # Multiple title.
 title_list = [{'content': 'This is a title.'}, {'content': 'This is a second title.'}, {'content': 'This is a third title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table2.jpg')
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table2.jpg')
 
 
 # Add a footnote
 title_list = [{'content': 'This is a title.'}, {'content': 'This is a second title.'}, {'content': 'This is a third title.'}]
 header_dict = {'content': [f'Header{i+1}' for i in range(8)]}
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(9)]}
 footnote_list = [{'content': 'This is a footnote.'}]
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table3.jpg', footnote_list=footnote_list)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/basic_table3.jpg', footnote_list=footnote_list)
 
 
 # ---------------------------------
 # Generate a cell merged table.
 # ---------------------------------
 
 title_list = [{'content': 'This is a cell merged table'}]
 # 11 header text
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table1.jpg', cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table1.jpg', cell_merge_dict=cell_merge_dict)
 
 
 title_list = [{'content': 'This is a cell merged table for row and column'}]
 # 8 header text
 header_dict = {'content': ['Merge row and column', 'MergedHead2','row\nmerged'] + [f'Header{i+1}' for i in range(5)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[1,2], '0-3':[0,2], '0-6':[1,0]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table2.jpg', cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict, data_dict=data_dict, img_path='./pic/merged_table2.jpg', cell_merge_dict=cell_merge_dict)
 
 
 
 
 # ---------------------------------
 # Change width and height
 # ---------------------------------
@@ -71,18 +71,18 @@
 title_list = [{'content': 'This is a cell merged table and changed the size,'}]
 # 8 header text
 header_dict = {'content': ['Merge row and column', 'MergedHead2','row\nmerged'] + [f'Header{i+1}' for i in range(5)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[1,2], '0-3':[0,2], '0-6':[1,0]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/change_size_table1.jpg',
-                      cell_merge_dict=cell_merge_dict,
-                      cell_width=200, cell_height=80)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/change_size_table1.jpg',
+#                       cell_merge_dict=cell_merge_dict,
+#                       cell_width=200, cell_height=80)
 
 
 
 # ---------------------------------
 # Change font-size
 # ---------------------------------
 
@@ -90,32 +90,32 @@
 title_list = [{'content': 'This is a cell merged table and changed the size,'}]
 # 8 header text
 header_dict = {'content': ['Merge row and column', 'MergedHead2','row merged'] + [f'Header{i+1}' for i in range(5)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[1,2], '0-3':[0,2], '0-6':[1,0]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/change_size_table2.jpg',
-                      cell_merge_dict=cell_merge_dict,
-                      col_width_dict={6:300}, row_height_dict={5:80})
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/change_size_table2.jpg',
+#                       cell_merge_dict=cell_merge_dict,
+#                       col_width_dict={6:300}, row_height_dict={5:80})
 
 
 # Modify the style of the title.
 title_list = [{'content': 'This is a cell merged table', 'font_size': 80, 'color':'#EE00DD', 'height': 100},
     {'content': 'This is a subtitle', 'color':'#0000FF', 'align':'right'}]
 # 11 header text
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)]}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/title_style_table.jpg',
-                      cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/title_style_table.jpg',
+#                       cell_merge_dict=cell_merge_dict)
 
 
 
 
 title_list = [{'content': 'This is a cell merged table'}]
 # Modify the header style.
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)],
@@ -123,17 +123,17 @@
     'bk_color': '#BADC58',
     'align': {0:'left', 2:'right'},
     'fore_color': {0:'#B71540', 1: '#6F1E51', 2:'#546DE5'}}
 # 8 * 8 data content
 data_dict = {'content':[[f'Data{i+j}' for j in range(8)] for i in range(8)]}
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/header_style_table.jpg',
-                      cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/header_style_table.jpg',
+#                       cell_merge_dict=cell_merge_dict)
 
 
 
 title_list = [{'content': 'This is a cell merged table'}]
 # Modify the header style.
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)]}
 # 8 * 8 data content
@@ -141,17 +141,17 @@
     'font_size': 20,
     'bk_color': {'r0': '#78E08F', '3-5': '#686DE0'},
     'fore_color': {'c3': '#EB3B5A'},
     'align': {'3-5': 'right'}
     }
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/data_style_table.jpg',
-                      cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/data_style_table.jpg',
+#                       cell_merge_dict=cell_merge_dict)
 
 
 
 # Change Font
 font_path = '/System/Library/Fonts/Supplemental/Comic Sans MS.ttf'
 
 title_list = [{'content': 'This is a cell merged table'}]
@@ -162,18 +162,18 @@
     'font_size': 20,
     'bk_color': {'r0': '#78E08F', '3-5': '#686DE0'},
     'fore_color': {'c3': '#EB3B5A'},
     'align': {'3-5': 'right'}
     }
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/font_style_table.jpg',
-                      font_path=font_path,
-                      cell_merge_dict=cell_merge_dict)
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/font_style_table.jpg',
+#                       font_path=font_path,
+#                       cell_merge_dict=cell_merge_dict)
 
 
 
 title_list = [{'content': 'This is a cell merged table'}]
 # Modify the header style.
 header_dict = {'content': ['MergedHead1', 'MergedHead2','MergedHead3'] + [f'Header{i+1}' for i in range(8)]}
 # 8 * 8 data content
@@ -181,13 +181,33 @@
     'font_size': 20,
     'bk_color': {'r0': '#78E08F', '3-5': '#686DE0'},
     'fore_color': {'c3': '#EB3B5A'},
     'align': {'3-5': 'right'}
     }
 # cell merged info
 cell_merge_dict = {'0-0':[0,1], '0-2':[0,3], '0-6':[0,1]}
-tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
-                      data_dict=data_dict, img_path='./pic/bk_style_table.jpg',
-                      font_path=font_path,
-                      cell_merge_dict=cell_merge_dict,
-                      pic_bk_color='#DFE4EA',
-                      table_line_color='#2F3542')
+# tp.generate_table_pic(10, 8, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/bk_style_table.jpg',
+#                       font_path=font_path,
+#                       cell_merge_dict=cell_merge_dict,
+#                       pic_bk_color='#DFE4EA',
+#                       table_line_color='#2F3542')
+
+
+# fixed-width table
+title_list = [{'content': 'This is a fixed-width table'}]
+header_dict = {'content': [f'Header{i+1}' for i in range(4)]}
+# 8 * 4 data content
+data_dict = {'content':[[f'Data{i}-0', f'Data{i}-1 this is a long content.', f'Data{i}-2', f'Data{i}-3'] for i in range(9)]}
+# tp.generate_table_pic(10, 4, title_list=title_list, header_dict=header_dict,
+#                       data_dict=data_dict, img_path='./pic/fixed_width_table.jpg')
+
+
+# ------------------- version: v0.0.4 -------------------
+# adaptive-width table
+title_list = [{'content': 'This is a adaptive-width table'}]
+header_dict = {'content': [f'Header{i+1}' for i in range(4)]}
+# 8 * 4 data content
+data_dict = {'content':[[f'Data{i}-0', f'Data{i}-1 this is a long content.', f'Data{i}-2', f'Data{i}-3'] for i in range(9)]}
+tp.generate_table_pic(10, 4, title_list=title_list, header_dict=header_dict,
+                      data_dict=data_dict, img_path='./pic/adaptive_width_table.jpg')
+
```

### Comparing `tablepic-0.0.3/src/tablepic/main.py` & `tablepic-0.0.4/src/tablepic/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: xinyan
 Date: 2023-06-13 17:12:25
 LastEditors: xinyan
-LastEditTime: 2023-06-16 15:20:39
+LastEditTime: 2023-06-20 12:54:03
 Description: file content
 '''
 
 
 import sys
 from PIL import Image, ImageFont, ImageDraw
 
@@ -121,14 +121,30 @@
     elif data_dict[key].get(f'c{j}', None):
         result = data_dict[key].get(f'c{j}')
     else:
         result = v_default
     return result
 
 
+def calculate_cell_width_height(data_dict:dict, font_path:str, cell_width:int, cell_height:int):
+    col_width_dict = {}
+    row_height_dict = {}
+    for i, data_line in enumerate(data_dict['content']):
+        for j, data_content in enumerate(data_line):
+            data_font = get_font(font_path, get_data_info(data_dict, 'font_size', i, j, 20, int))
+            c_w, c_h = 0, 0
+            for item in data_content.split('\n'):
+                w, h = data_font.getbbox(item)[2:]
+                c_w = max(c_w, w) + 20
+            c_h = h * len(data_content.split('\n'))
+            row_height_dict[i] = max(row_height_dict.get(i, cell_height), c_h)
+            col_width_dict[j] = max(col_width_dict.get(j, cell_width), c_w)
+    return col_width_dict, row_height_dict
+
+
 def generate_table_pic(row_num:int, col_num:int, title_list:list, header_dict:dict, data_dict:dict, img_path:str, footnote_list:list=[],
                        cell_width:int=150, cell_height:int=50,  col_width_dict:dict={}, row_height_dict:dict={}, cell_merge_dict:dict={},
                        table_margin:int=20, pic_bk_color='#FFFFFF', table_line_color='#E8EAED', font_path:str=None):
     """
     Generate the table picture.
     :param row_num: int，Number of rows in the table.
     :param col_num: int，Number of columns in the table.
@@ -178,14 +194,18 @@
     :param cell_merge_dict: dict, contains the information of merging cells. For example, {'0-0': [1,0], '0-1': [0, 2]} indicates that the cell at coordinate [0,0] needs to be merged,
         by merging 1 row downward and 0 columns to the right (i.e., not merging columns); the cell at coordinate [0,1] needs to be merged, by merging
         0 rows downward and 1 column to the right.
     :param pic_bk_color: str, optional parameter. Set the background color of the picture, default value is '#FFFFFF'.
     :param table_line_color: str, optional parameter. Set the line color of the table, default value is '#E8EAED'.
     :param font_path: str, optional parameter. Given the font path to set a new font for the text (including title, header, data).
     """
+    # Calculate the width for each column and the height for each row
+    if len(row_height_dict) == 0 or len(col_width_dict) == 0:
+        col_width_dict, row_height_dict = calculate_cell_width_height(data_dict, font_path, cell_width, cell_height)
+
     color_white = '#FFFFFF'
     color_black = '#000000'
     color_default_header_bk = '#CCD6EB'
     title_list = process_title_footnote(title_list, 'title')
     footnote_list = process_title_footnote(footnote_list, 'footnote')
     total_title_height = sum([title['height'] for title in title_list])
     total_footnote_height = sum([footnote['height'] for footnote in footnote_list])
```

### Comparing `tablepic-0.0.3/src/tablepic.egg-info/PKG-INFO` & `tablepic-0.0.4/src/tablepic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

