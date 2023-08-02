# Comparing `tmp/PrSpiders-0.5.2.7.tar.gz` & `tmp/PrSpiders-0.5.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.7.tar", last modified: Wed Jul  5 02:49:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

