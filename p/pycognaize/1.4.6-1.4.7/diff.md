# Comparing `tmp/pycognaize-1.4.6.tar.gz` & `tmp/pycognaize-1.4.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognaize-1.4.6.tar", last modified: Fri Jun 16 09:00:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

