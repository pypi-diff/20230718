# Comparing `tmp/fast_query_parsers-0.4.0.tar.gz` & `tmp/fast_query_parsers-1.0.0-cp38-abi3-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

