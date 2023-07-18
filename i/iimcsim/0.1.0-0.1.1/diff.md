# Comparing `tmp/iimcsim-0.1.0.tar.gz` & `tmp/iimcsim-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.1.0.tar", last modified: Tue Jul 18 20:04:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

