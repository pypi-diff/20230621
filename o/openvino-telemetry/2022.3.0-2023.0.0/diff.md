# Comparing `tmp/openvino-telemetry-2022.3.0.tar.gz` & `tmp/openvino_telemetry-2023.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino-telemetry-2022.3.0.tar", last modified: Fri Dec 16 10:39:00 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

