# Comparing `tmp/litie-0.2.1.tar.gz` & `tmp/litie-0.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litie-0.2.1.tar", last modified: Tue Jun 20 16:23:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

