# Comparing `tmp/SparkMinIOHandle-0.0.1.tar.gz` & `tmp/SparkMinIOHandle-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkMinIOHandle-0.0.1.tar", last modified: Wed Jun 21 14:54:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

