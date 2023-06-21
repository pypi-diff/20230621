# Comparing `tmp/mosec-0.7.1.tar.gz` & `tmp/mosec-0.7.2-pp38-pypy38_pp73-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosec-0.7.1.tar", last modified: Tue Jun  6 10:01:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

