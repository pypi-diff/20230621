# Comparing `tmp/newport-motors-py-0.1.1.tar.gz` & `tmp/newport_motors_py-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newport-motors-py-0.1.1.tar", last modified: Wed Jun 21 03:49:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

