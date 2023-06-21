# Comparing `tmp/BaseDT-0.0.9.tar.gz` & `tmp/BaseDT-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.9.tar", last modified: Mon Jun 19 06:05:56 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.1.0.tar", last modified: Wed Jun 21 03:39:22 2023, max compression
```

## Comparing `BaseDT-0.0.9.tar` & `BaseDT-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    35422 2023-06-19 05:49:30.000000 BaseDT-0.0.9/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.0.9/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    15369 2023-06-19 05:48:40.000000 BaseDT-0.0.9/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 BaseDT-0.0.9/BaseDT/utils.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.9/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.9/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-19 06:05:56.000000 BaseDT-0.0.9/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.9/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-19 06:05:56.000000 BaseDT-0.0.9/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-19 06:05:36.000000 BaseDT-0.0.9/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)       32 2023-06-21 03:34:40.000000 BaseDT-0.1.0/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    35422 2023-06-19 05:49:30.000000 BaseDT-0.1.0/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 BaseDT-0.1.0/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.1.0/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 BaseDT-0.1.0/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15667 2023-06-21 03:33:07.000000 BaseDT-0.1.0/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 BaseDT-0.1.0/BaseDT/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1224 2023-06-21 03:31:23.000000 BaseDT-0.1.0/BaseDT/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      383 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-21 03:39:22.000000 BaseDT-0.1.0/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.1.0/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.1.0/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-21 03:39:22.000000 BaseDT-0.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.1.0/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-21 03:39:22.000000 BaseDT-0.1.0/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-21 03:39:15.000000 BaseDT-0.1.0/setup.py
```

### Comparing `BaseDT-0.0.9/BaseDT/data.py` & `BaseDT-0.1.0/BaseDT/data.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.9/BaseDT/data_image.py` & `BaseDT-0.1.0/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.9/BaseDT/dataset.py` & `BaseDT-0.1.0/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.9/BaseDT/io.py` & `BaseDT-0.1.0/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.9/BaseDT/plot.py` & `BaseDT-0.1.0/BaseDT/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,17 +242,20 @@
     'bbox': dict(facecolor='black', alpha=0.5, boxstyle='Round'),
     'verticalalignment': 'top',
     'horizontalalignment': 'left',
 }
 def draw_single_cls(image, result):
     texts = []
     max_length = 12 # 文本长度限制
-    texts.append('Pred_label: {}'.format(result['标签']))
-    texts.append('Pred_score: {:.2f}'.format(result['置信度']))
-    texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
+    if '标签' in result:
+        texts.append('Pred_label: {}'.format(result['标签']))
+    if '置信度' in result:
+        texts.append('Pred_score: {:.2f}'.format(result['置信度']))
+    if '预测结果' in result:
+        texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
     text = '\n'.join(texts)
     #fig = plt.figure()
     image.init_plt()
     img_tmp = image._image
     img_scale = get_adaptive_scale(img_tmp.shape[:2])
     DEFAULT_TEXT_CFG['size'] = int(img_scale * 5)
     pos = np.array([[img_scale*5, img_scale*5]], dtype=int)
@@ -305,29 +308,33 @@
     assert len(dataset_palette) >= num_classes, \
         'The length of palette should not be less than `num_classes`.'
     return dataset_palette
 
 def draw_single_det(image, result, line_width: int =3) -> None:
     assert isinstance(result, list), "Expected 'result' to be a list"
     image.init_plt()
+    if len(result) == 0:
+        return
     bboxes = []
     labels = []
     label_texts = []
     for bbox in result:
         assert isinstance(bbox, dict), "Expected each element in 'result' to be a dictionary"
         assert '坐标' in bbox and '标签' in bbox, "Each dictionary in 'result' should have '坐标' and '标签' keys"
         
         coords = bbox['坐标']
         assert isinstance(coords, dict), "Expected '坐标' to be a dictionary"
         assert all(key in coords for key in ['x1', 'y1', 'x2', 'y2']), "The '坐标' dictionary should have 'x1', 'y1', 'x2', 'y2' keys"
         
         bboxes.append([coords['x1'], coords['y1'], coords['x2'], coords['y2']])
         labels.append(bbox['标签'])
-        label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
-
+        if '预测结果' in bbox:
+            label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
+        else:
+            label_texts.append('{}:{}'.format(bbox['标签'],round(float(bbox['置信度']) * 100, 1)))
     bboxes = np.array(bboxes)
     labels = np.array(labels)
 
 
     max_label = int(max(labels) if len(labels) > 0 else 0)
 
     bbox_palette = get_palette(max_label + 1)
```

### Comparing `BaseDT-0.0.9/BaseDT/utils.py` & `BaseDT-0.1.0/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.9/setup.py` & `BaseDT-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.9',
+    version='0.1.0',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
@@ -96,13 +96,13 @@
     # ],
     # classifiers=[
     #     # 'Operating System :: Linux',
     #     'Programming Language :: Python :: 3.8',
     # ],
     python_requires='>=3.6',
     zip_safe=True,
-    # entry_points= {'console_scripts': ['MMEdu = MMEdu.version:hello',]},
+    entry_points= {'console_scripts': ['BaseDT = BaseDT.version:hello',]},
     # build_scripts
     # dependency_links = [
     #     " https://download.pytorch.org/whl/cu101/torch-1.8.1%2Bcu101-cp38-cp38-linux_x86_64.whl#egg=torch-1.8.1+cu101",
     # ],
 )
```

