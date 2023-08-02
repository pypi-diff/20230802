# Comparing `tmp/rapidfuzz-3.1.2.tar.gz` & `tmp/rapidfuzz-3.2.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.1.2.tar", last modified: Thu Jul 20 21:25:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

