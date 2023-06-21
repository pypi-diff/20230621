# Comparing `tmp/ogms-0.1.1.tar.gz` & `tmp/ogms-0.1.2-py3.7.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ogms-0.1.1.tar", last modified: Thu Jun  4 07:20:14 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

