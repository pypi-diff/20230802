# Comparing `tmp/m3-registry-2.0.4.tar.gz` & `tmp/m3_registry-2.2.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m3-registry-2.0.4.tar", last modified: Mon Feb  6 07:57:09 2017, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

