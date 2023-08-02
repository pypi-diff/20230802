# Comparing `tmp/fprime-native-images-0.0.0.tar.gz` & `tmp/fprime-native-images-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-native-images-0.0.0.tar", last modified: Tue Aug  1 23:15:50 2023, max compression
+gzip compressed data, was "fprime-native-images-0.1.0.tar", last modified: Wed Aug  2 00:16:40 2023, max compression
```

## Comparing `fprime-native-images-0.0.0.tar` & `fprime-native-images-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.249434 fprime-native-images-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/.github/workflows/native-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/env-setup
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/java
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/native-images
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/publish
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.249434 fprime-native-images-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/src/fprime_native_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/src/fprime_native_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/src/fprime_native_images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/src/fprime_native_images/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/src/fprime_native_images/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/src/fprime_native_images/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-01 23:15:41.000000 fprime-native-images-0.0.0/src/fprime_native_images/templates/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:15:50.253434 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 23:15:50.000000 fprime-native-images-0.0.0/src/fprime_native_images.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.593058 fprime-native-images-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/.github/workflows/native-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/env-setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/native-images
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/publish
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.593058 fprime-native-images-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 00:16:32.000000 fprime-native-images-0.1.0/src/fprime_native_images/templates/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:16:40.597058 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 00:16:40.000000 fprime-native-images-0.1.0/src/fprime_native_images.egg-info/top_level.txt
```

### Comparing `fprime-native-images-0.0.0/.github/workflows/native-build.yml` & `fprime-native-images-0.1.0/.github/workflows/native-build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         run: |
           cd ${{ inputs.working-directory }}
           ${{ inputs.build }} ${{ inputs.output-directory }}
         shell: bash
       - name: "Archiving JARs package"
         uses: actions/upload-artifact@v3
         with:
-          name: jar-build
+          name: build-jar
           path: ${{ inputs.output-directory }}
           retention-days: 5
           if-no-files-found: error
       - if: ${{ inputs.trace }}
         name: "Tracing JARs via Unit-Tests"
         run: |
           cd ${{ inputs.working-directory }}
@@ -82,15 +82,15 @@
         with:
           submodules: recursive
       - name: "Setup Native Image Tools"
         uses: fprime-community/native-images-action@main
       - name: "Download JARs"
         uses: actions/download-artifact@v3
         with:
-          name: jar-build
+          name: build-jar
           path: bin
       - name: "Download Tracing"
         uses: actions/download-artifact@v3
         with:
           name: jar-traces
           path: ${{ inputs.trace-directory }}
       - name: "Build Native Images"
@@ -98,18 +98,53 @@
           cd ${{ inputs.working-directory }}
           export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
           $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
         shell: bash
       - name: "Archive Native Images"
         uses: actions/upload-artifact@v3
         with:
-          name: native-images-manylinux_2_28
+          name: build-manylinux_2_28
           path: bin/*
           retention-days: 5
           if-no-files-found: error
+  build-native-packages:
+    needs: [build-native-images-linux]
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        package_tag: ["manylinux_2_28", "jar"]
+    steps:
+      - name: "Checkout repository"
+        uses: actions/checkout@v3
+        with:
+          submodules: recursive
+      - name: "Download Package"
+        uses: actions/download-artifact@v3
+        with:
+          name: build-${{ matrix.package_tag }}
+          path: ${{ inputs.output-directory }}
+      - name: "Install Builder"
+        run: pip install fprime-native-images twine
+        shell: bash
+      - name: "Run Builder"
+        run: |
+          fprime-native-packager ${{ inputs.output-directory }} --package-tag ${{ matrix.package_tag }}
+        shell: bash
+      - name: Publish distributions to TestPyPI
+        env:
+          TWINE_PASSWORD: ${{ secrets.TESTPYPI_CREDENTIAL }}
+        run: |
+          twine upload -r "$https://test.pypi.org/legacy/" -u "__token__" dist/*
+        shell: bash
+      - name: Publish distributions to PyPI
+        env:
+          TWINE_PASSWORD: ${{ secrets.PYPI_CREDENTIAL }}
+        run: |
+          twine upload -u "__token__" dist/*
+        shell: bash
 #  build-native-images-non-linux:
 #    needs: build-jars
 #    strategy:
 #      matrix:
 #        runner: ["macos-11", "odroid"]
 #    runs-on: ${{ matrix.runner }}
 #    steps:
@@ -118,15 +153,15 @@
 #        with:
 #          submodules: recursive
 #      - name: "Setup Native Image Tools"
 #        uses: fprime-community/native-images-action@main
 #      - name: "Download JARs"
 #        uses: actions/download-artifact@v3
 #        with:
-#          name: jar-build
+#          name: build-jar
 #          path: bin
 #      - name: "Download Tracing"
 #        uses: actions/download-artifact@v3
 #        with:
 #          name: jar-traces
 #          path: ${{ inputs.trace-directory }}
 #      - name: "Build Native Images"
```

### Comparing `fprime-native-images-0.0.0/.github/workflows/publish.yml` & `fprime-native-images-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/LICENSE` & `fprime-native-images-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/action.yml` & `fprime-native-images-0.1.0/action.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/env-setup` & `fprime-native-images-0.1.0/env-setup`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/native-images` & `fprime-native-images-0.1.0/native-images`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/publish` & `fprime-native-images-0.1.0/publish`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/pyproject.toml` & `fprime-native-images-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Developers",
 ]
 dependencies = [
     "Jinja2>=2.11.3",
     "build",
     'importlib-metadata; python_version<"3.8"',
 ]
-dynamic = ["version"]
+version="0.1.0"
 
 [project.scripts]
 fprime-native-packager="fprime_native_images.__main__:main"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `fprime-native-images-0.0.0/src/fprime_native_images/__main__.py` & `fprime-native-images-0.1.0/src/fprime_native_images/__main__.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/src/fprime_native_images/package.py` & `fprime-native-images-0.1.0/src/fprime_native_images/package.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.0.0/src/fprime_native_images/templates/setup.py.j2` & `fprime-native-images-0.1.0/src/fprime_native_images/templates/setup.py.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
 setup(
     name="{{ package }}",
-    use_scm_version={"root": "../..", "relative_to": __file__},
+    #use_scm_version={"root": "../..", "relative_to": __file__},
+    version="0.1.0",
     license="Apache 2.0 License",
     description="FPP distribution package for {{ package }}",
     url="https://github.com/nasa/fprime",
     keywords=["fpp", "fprime", "embedded", "nasa"],
     project_urls={"Issue Tracker": "https://github.com/nasa/fprime/issues"},
     author="Michael Starch",
     author_email="Michael.D.Starch@jpl.nasa.gov",
```

### Comparing `fprime-native-images-0.0.0/src/fprime_native_images.egg-info/SOURCES.txt` & `fprime-native-images-0.1.0/src/fprime_native_images.egg-info/SOURCES.txt`

 * *Files identical despite different names*

