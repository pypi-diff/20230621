# Comparing `tmp/python-gestpay-2.0.0.tar.gz` & `tmp/python_gestpay-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gestpay-2.0.0.tar", last modified: Thu Jun 23 10:49:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

