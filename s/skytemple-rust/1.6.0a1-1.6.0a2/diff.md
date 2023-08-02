# Comparing `tmp/skytemple-rust-1.6.0a1.tar.gz` & `tmp/skytemple_rust-1.6.0a2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytemple-rust-1.6.0a1.tar", last modified: Fri Jun  9 19:23:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

