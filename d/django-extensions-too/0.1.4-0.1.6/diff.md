# Comparing `tmp/django-extensions-too-0.1.4.tar.gz` & `tmp/django_extensions_too-0.1.6-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-extensions-too-0.1.4.tar", last modified: Fri Sep  3 16:55:22 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

