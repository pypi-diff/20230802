# Comparing `tmp/memray-1.9.0.tar.gz` & `tmp/memray-1.9.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memray-1.9.0.tar", last modified: Fri Jul 28 17:02:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

