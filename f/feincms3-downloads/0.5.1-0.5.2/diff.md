# Comparing `tmp/feincms3_downloads-0.5.1.tar.gz` & `tmp/feincms3_downloads-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feincms3_downloads-0.5.1.tar", last modified: Fri Dec  9 16:11:09 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `feincms3_downloads-0.5.1.tar` & `feincms3_downloads-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1077 2022-09-27 15:30:54.000000 feincms3_downloads-0.5.1/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      196 2022-09-27 15:30:54.000000 feincms3_downloads-0.5.1/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1452 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      298 2022-09-27 15:30:54.000000 feincms3_downloads-0.5.1/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/feincms3_downloads/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2022-12-09 16:10:47.000000 feincms3_downloads-0.5.1/feincms3_downloads/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      751 2022-09-27 15:30:54.000000 feincms3_downloads-0.5.1/feincms3_downloads/checks.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.499411 feincms3_downloads-0.5.1/feincms3_downloads/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.499411 feincms3_downloads-0.5.1/feincms3_downloads/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/feincms3_downloads/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      660 2022-12-09 16:10:07.000000 feincms3_downloads-0.5.1/feincms3_downloads/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1008 2022-12-09 16:09:12.000000 feincms3_downloads-0.5.1/feincms3_downloads/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1593 2022-12-09 16:08:58.000000 feincms3_downloads-0.5.1/feincms3_downloads/plugins.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      936 2022-12-09 16:08:58.000000 feincms3_downloads-0.5.1/feincms3_downloads/previews.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.499411 feincms3_downloads-0.5.1/feincms3_downloads/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/feincms3_downloads/templates/plugins/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-09-27 15:30:54.000000 feincms3_downloads-0.5.1/feincms3_downloads/templates/plugins/download.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1452 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      573 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       51 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       19 2022-12-09 16:11:09.000000 feincms3_downloads-0.5.1/feincms3_downloads.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1408 2022-12-09 16:11:09.509411 feincms3_downloads-0.5.1/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-12-09 16:08:58.000000 feincms3_downloads-0.5.1/setup.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.editorconfig
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tox.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/checks.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/plugins.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/previews.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/templates/plugins/download.html
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/admin.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/models.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/settings.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/test_downloads.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/urls.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/views.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/templates/article.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/templates/base.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/LICENSE
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/README.rst
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/PKG-INFO
```

### Comparing `feincms3_downloads-0.5.1/LICENSE` & `feincms3_downloads-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.1/PKG-INFO` & `feincms3_downloads-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
-Name: feincms3_downloads
-Version: 0.5.1
+Name: feincms3-downloads
+Version: 0.5.2
 Summary: Downloads plugin for feincms3
-Home-page: https://github.com/matthiask/feincms3-downloads/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
+Project-URL: Homepage, https://github.com/matthiask/feincms3-downloads/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: MIT
-Platform: OS Independent
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Dist: django>=3.2
+Requires-Dist: feincms3>=4
+Requires-Dist: pillow
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 ==================
 feincms3-downloads
 ==================
 
 .. image:: https://github.com/matthiask/feincms3-downloads/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/matthiask/feincms3-downloads/
```

### Comparing `feincms3_downloads-0.5.1/feincms3_downloads/checks.py` & `feincms3_downloads-0.5.2/feincms3_downloads/checks.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.1/feincms3_downloads/locale/de/LC_MESSAGES/django.mo` & `feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.1/feincms3_downloads/locale/de/LC_MESSAGES/django.po` & `feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.1/feincms3_downloads/plugins.py` & `feincms3_downloads-0.5.2/feincms3_downloads/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import tempfile
 
 from django.core.files.base import ContentFile
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from feincms3.utils import upload_to
 
-import feincms3_downloads.checks  # noqa
+import feincms3_downloads.checks  # noqa: F401
 from feincms3_downloads.previews import preview_as_jpeg
 
 
 class DownloadBase(models.Model):
     file = models.FileField(_("file"), upload_to=upload_to)
     file_size = models.IntegerField(_("file size"), editable=False)
     caption = models.CharField(_("caption"), max_length=100, blank=True)
@@ -21,29 +21,30 @@
         abstract = True
         verbose_name = _("download")
         verbose_name_plural = _("downloads")
 
     def __str__(self):
         return self.file.name
 
+    def save(self, *args, **kwargs):
+        self.file_size = self.file.size
+        super().save(*args, **kwargs)
+        if self.show_preview and not self.preview:
+            generate_preview(source=self.file, preview=self.preview)
+
+    save.alters_data = True
+
     @property
     def basename(self):
         return os.path.basename(self.file.name)
 
     @property
     def caption_or_basename(self):
         return self.caption or self.basename
 
-    def save(self, *args, **kwargs):
-        self.file_size = self.file.size
-        super().save(*args, **kwargs)
-        if self.show_preview and not self.preview:
-            with tempfile.NamedTemporaryFile(
-                suffix=os.path.splitext(self.file.name)[1]
-            ) as f:
-                f.write(self.file.read())
-                f.seek(0)
-                preview = preview_as_jpeg(f.name)
-                if preview:
-                    self.preview.save("preview.jpg", ContentFile(preview), save=True)
 
-    save.alters_data = True
+def generate_preview(*, source, preview, save=True):
+    with tempfile.NamedTemporaryFile(suffix=os.path.splitext(source.name)[1]) as f:
+        f.write(source.read())
+        f.seek(0)
+        if p := preview_as_jpeg(f.name):
+            preview.save("preview.jpg", ContentFile(p), save=save)
```

### Comparing `feincms3_downloads-0.5.1/feincms3_downloads/previews.py` & `feincms3_downloads-0.5.2/feincms3_downloads/previews.py`

 * *Files identical despite different names*

