# Comparing `tmp/feincms3_downloads-0.5.2.tar.gz` & `tmp/feincms3_downloads-0.5.3.tar.gz`

## Comparing `feincms3_downloads-0.5.2.tar` & `feincms3_downloads-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.editorconfig
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/CHANGELOG.rst
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tox.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/checks.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/plugins.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/previews.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/feincms3_downloads/templates/plugins/download.html
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/admin.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/models.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/settings.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/test_downloads.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/urls.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/views.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/templates/article.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/tests/testapp/templates/base.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/LICENSE
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/README.rst
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/.editorconfig
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tox.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/checks.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/plugins.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/previews.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/feincms3_downloads/templates/plugins/download.html
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/admin.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/models.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/settings.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/test_downloads.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/urls.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/views.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/templates/article.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/tests/testapp/templates/base.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/LICENSE
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/README.rst
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 feincms3_downloads-0.5.3/PKG-INFO
```

### Comparing `feincms3_downloads-0.5.2/.pre-commit-config.yaml` & `feincms3_downloads-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/CHANGELOG.rst` & `feincms3_downloads-0.5.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/.github/workflows/tests.yml` & `feincms3_downloads-0.5.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/feincms3_downloads/checks.py` & `feincms3_downloads-0.5.3/feincms3_downloads/checks.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/feincms3_downloads/plugins.py` & `feincms3_downloads-0.5.3/feincms3_downloads/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,27 +24,35 @@
 
     def __str__(self):
         return self.file.name
 
     def save(self, *args, **kwargs):
         self.file_size = self.file.size
         super().save(*args, **kwargs)
-        if self.show_preview and not self.preview:
-            generate_preview(source=self.file, preview=self.preview)
+        if (
+            self.show_preview
+            and not self.preview
+            and generate_preview(source=self.file, preview=self.preview)
+        ):
+            super().save()
 
     save.alters_data = True
 
     @property
     def basename(self):
         return os.path.basename(self.file.name)
 
     @property
     def caption_or_basename(self):
         return self.caption or self.basename
 
 
-def generate_preview(*, source, preview, save=True):
+def generate_preview(*, source, preview):
     with tempfile.NamedTemporaryFile(suffix=os.path.splitext(source.name)[1]) as f:
+        source.open()
+        source.seek(0)
         f.write(source.read())
         f.seek(0)
         if p := preview_as_jpeg(f.name):
-            preview.save("preview.jpg", ContentFile(p), save=save)
+            preview.save("preview.jpg", ContentFile(p), save=False)
+            return True
+        return False
```

### Comparing `feincms3_downloads-0.5.2/feincms3_downloads/previews.py` & `feincms3_downloads-0.5.3/feincms3_downloads/previews.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.mo` & `feincms3_downloads-0.5.3/feincms3_downloads/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/feincms3_downloads/locale/de/LC_MESSAGES/django.po` & `feincms3_downloads-0.5.3/feincms3_downloads/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/tests/testapp/settings.py` & `feincms3_downloads-0.5.3/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/tests/testapp/test_downloads.py` & `feincms3_downloads-0.5.3/tests/testapp/test_downloads.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/tests/testapp/views.py` & `feincms3_downloads-0.5.3/tests/testapp/views.py`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/LICENSE` & `feincms3_downloads-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/pyproject.toml` & `feincms3_downloads-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feincms3_downloads-0.5.2/PKG-INFO` & `feincms3_downloads-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feincms3-downloads
-Version: 0.5.2
+Version: 0.5.3
 Summary: Downloads plugin for feincms3
 Project-URL: Homepage, https://github.com/matthiask/feincms3-downloads/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

