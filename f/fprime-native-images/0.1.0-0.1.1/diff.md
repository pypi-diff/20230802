# Comparing `tmp/fprime-native-images-0.1.0.tar.gz` & `tmp/fprime-native-images-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-native-images-0.1.0.tar", last modified: Wed Aug  2 00:16:40 2023, max compression
+gzip compressed data, was "fprime-native-images-0.1.1.tar", last modified: Wed Aug  2 01:04:08 2023, max compression
```

## Comparing `fprime-native-images-0.1.0.tar` & `fprime-native-images-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.593058 fprime-native-images-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/.github/workflows/native-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/env-setup
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/java
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/native-images
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/publish
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.593058 fprime-native-images-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/templates/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.096048 fprime-native-images-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/.github/workflows/native-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/env-setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/native-images
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/publish
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.096048 fprime-native-images-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/templates/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/top_level.txt
```

### Comparing `fprime-native-images-0.1.0/.github/workflows/native-build.yml` & `fprime-native-images-0.1.1/.github/workflows/native-build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -98,24 +98,24 @@
           cd ${{ inputs.working-directory }}
           export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
           $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
         shell: bash
       - name: "Archive Native Images"
         uses: actions/upload-artifact@v3
         with:
-          name: build-manylinux_2_28
+          name: build-manylinux_2_28_x86_64
           path: bin/*
           retention-days: 5
           if-no-files-found: error
-  build-native-packages:
+  build-native-wheels:
     needs: [build-native-images-linux]
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        package_tag: ["manylinux_2_28", "jar"]
+        package_tag: ["jar", "manylinux_2_28_x86_64"]
     steps:
       - name: "Checkout repository"
         uses: actions/checkout@v3
         with:
           submodules: recursive
       - name: "Download Package"
         uses: actions/download-artifact@v3
@@ -125,19 +125,38 @@
       - name: "Install Builder"
         run: pip install fprime-native-images twine
         shell: bash
       - name: "Run Builder"
         run: |
           fprime-native-packager ${{ inputs.output-directory }} --package-tag ${{ matrix.package_tag }}
         shell: bash
+      - name: "Archiving Wheels"
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels-${{ matrix.package_tag }}
+          path: packages/dist/*
+          retention-days: 5
+          if-no-files-found: error
+  publish-native-wheels:
+    needs: [build-native-wheels]
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        package_tag: ["jar", "manylinux_2_28_x86_64"]
+    steps:
+      - name: "Download Package"
+        uses: actions/download-artifact@v3
+        with:
+          name: wheels-${{ matrix.package_tag }}
+          path: dist
       - name: Publish distributions to TestPyPI
         env:
           TWINE_PASSWORD: ${{ secrets.TESTPYPI_CREDENTIAL }}
         run: |
-          twine upload -r "$https://test.pypi.org/legacy/" -u "__token__" dist/*
+          twine upload -r testpypi -u "__token__" dist/*
         shell: bash
       - name: Publish distributions to PyPI
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_CREDENTIAL }}
         run: |
           twine upload -u "__token__" dist/*
         shell: bash
```

### Comparing `fprime-native-images-0.1.0/.github/workflows/publish.yml` & `fprime-native-images-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/LICENSE` & `fprime-native-images-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/action.yml` & `fprime-native-images-0.1.1/action.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/env-setup` & `fprime-native-images-0.1.1/env-setup`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/native-images` & `fprime-native-images-0.1.1/native-images`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/publish` & `fprime-native-images-0.1.1/publish`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/pyproject.toml` & `fprime-native-images-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     "Intended Audience :: Developers",
 ]
 dependencies = [
     "Jinja2>=2.11.3",
     "build",
     'importlib-metadata; python_version<"3.8"',
 ]
-version="0.1.0"
+version="0.1.1"
 
 [project.scripts]
 fprime-native-packager="fprime_native_images.__main__:main"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.setuptools.package-data]
-"fprime_native_images.templates" = ["*.j2"]
+"fprime_native_images.templates" = ["*.j2"]
```

### Comparing `fprime-native-images-0.1.0/src/fprime_native_images/__main__.py` & `fprime-native-images-0.1.1/src/fprime_native_images/__main__.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/src/fprime_native_images/package.py` & `fprime-native-images-0.1.1/src/fprime_native_images/package.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.0/src/fprime_native_images/templates/setup.py.j2` & `fprime-native-images-0.1.1/src/fprime_native_images/templates/setup.py.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name="{{ package }}",
     #use_scm_version={"root": "../..", "relative_to": __file__},
-    version="0.1.0",
+    version="0.1.1",
     license="Apache 2.0 License",
     description="FPP distribution package for {{ package }}",
     url="https://github.com/nasa/fprime",
     keywords=["fpp", "fprime", "embedded", "nasa"],
     project_urls={"Issue Tracker": "https://github.com/nasa/fprime/issues"},
     author="Michael Starch",
     author_email="Michael.D.Starch@jpl.nasa.gov",
```

### Comparing `fprime-native-images-0.1.0/src/fprime_native_images.egg-info/SOURCES.txt` & `fprime-native-images-0.1.1/src/fprime_native_images.egg-info/SOURCES.txt`

 * *Files identical despite different names*

