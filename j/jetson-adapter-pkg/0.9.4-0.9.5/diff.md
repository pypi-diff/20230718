# Comparing `tmp/jetson-adapter-pkg-0.9.4.tar.gz` & `tmp/jetson_adapter_pkg-0.9.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson-adapter-pkg-0.9.4.tar", last modified: Mon Feb 14 08:14:22 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

