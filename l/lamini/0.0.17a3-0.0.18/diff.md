# Comparing `tmp/lamini-0.0.17a3.tar.gz` & `tmp/lamini-0.0.18-4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamini-0.0.17a3.tar", last modified: Wed Jun  7 08:59:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

