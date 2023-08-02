# Comparing `tmp/libcasm-global-2.0.0.tar.gz` & `tmp/libcasm_global-2.0.1-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcasm-global-2.0.0.tar", last modified: Tue Jul 18 20:00:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

