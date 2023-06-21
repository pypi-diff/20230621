# Comparing `tmp/fabio-2023.4.1.tar.gz` & `tmp/fabio-2023.6.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabio-2023.4.1.tar", last modified: Tue Apr 18 09:38:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

