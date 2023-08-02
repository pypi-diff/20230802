# Comparing `tmp/fprime-native-images-0.1.1.tar.gz` & `tmp/fprime-native-images-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-native-images-0.1.1.tar", last modified: Wed Aug  2 01:04:08 2023, max compression
+gzip compressed data, was "fprime-native-images-0.1.2.tar", last modified: Wed Aug  2 04:54:29 2023, max compression
```

## Comparing `fprime-native-images-0.1.1.tar` & `fprime-native-images-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.096048 fprime-native-images-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/.github/workflows/native-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/env-setup
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/java
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/native-images
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/publish
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.096048 fprime-native-images-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 01:03:57.000000 fprime-native-images-0.1.1/src/fprime_native_images/templates/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:04:08.100048 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 01:04:08.000000 fprime-native-images-0.1.1/src/fprime_native_images.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.662181 fprime-native-images-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/.github/workflows/native-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/env-setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/native-images
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/publish
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.662181 fprime-native-images-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/templates/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/top_level.txt
```

### Comparing `fprime-native-images-0.1.1/.github/workflows/native-build.yml` & `fprime-native-images-0.1.2/.github/workflows/native-build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -102,32 +102,72 @@
       - name: "Archive Native Images"
         uses: actions/upload-artifact@v3
         with:
           name: build-manylinux_2_28_x86_64
           path: bin/*
           retention-days: 5
           if-no-files-found: error
+  build-native-images-non-linux:
+    needs: build-jars
+    strategy:
+      matrix:
+        runner:
+         - runner: "macos-11"
+           tag: "macosx_10_9_universal2"
+         - runner: "odroid"
+           tag: "manylinux_2_28_aarch64"
+    runs-on: ${{ matrix.runner.runner }}
+    steps:
+      - name: "Checkout repository"
+        uses: actions/checkout@v3
+        with:
+          submodules: recursive
+      - name: "Setup Native Image Tools"
+        uses: fprime-community/native-images-action@main
+      - name: "Download JARs"
+        uses: actions/download-artifact@v3
+        with:
+          name: build-jar
+          path: bin
+      - name: "Download Tracing"
+        uses: actions/download-artifact@v3
+        with:
+          name: jar-traces
+          path: ${{ inputs.trace-directory }}
+      - name: "Build Native Images"
+        run: |
+          cd ${{ inputs.working-directory }}
+          export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
+          $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
+        shell: bash
+      - name: "Archive Native Images"
+        uses: actions/upload-artifact@v3
+        with:
+          name: native-images-${{ matrix.runner.tag }}
+          path: bin/*
+          retention-days: 5
+          if-no-files-found: error
   build-native-wheels:
-    needs: [build-native-images-linux]
+    needs: [build-native-images-linux, build-native-images-non-linux]
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        package_tag: ["jar", "manylinux_2_28_x86_64"]
+        package_tag: ["jar", "manylinux_2_28_x86_64", "manylinux_2_28_aarch64", "macosx_10_9_universal2"]
     steps:
       - name: "Checkout repository"
         uses: actions/checkout@v3
         with:
           submodules: recursive
       - name: "Download Package"
         uses: actions/download-artifact@v3
         with:
           name: build-${{ matrix.package_tag }}
           path: ${{ inputs.output-directory }}
       - name: "Install Builder"
-        run: pip install fprime-native-images twine
+        run: pip install fprime-native-images
         shell: bash
       - name: "Run Builder"
         run: |
           fprime-native-packager ${{ inputs.output-directory }} --package-tag ${{ matrix.package_tag }}
         shell: bash
       - name: "Archiving Wheels"
         uses: actions/upload-artifact@v3
@@ -144,14 +184,17 @@
         package_tag: ["jar", "manylinux_2_28_x86_64"]
     steps:
       - name: "Download Package"
         uses: actions/download-artifact@v3
         with:
           name: wheels-${{ matrix.package_tag }}
           path: dist
+      - name: "Install Builder"
+        run: pip install twine
+        shell: bash
       - name: Publish distributions to TestPyPI
         env:
           TWINE_PASSWORD: ${{ secrets.TESTPYPI_CREDENTIAL }}
         run: |
           twine upload -r testpypi -u "__token__" dist/*
         shell: bash
       - name: Publish distributions to PyPI
```

### Comparing `fprime-native-images-0.1.1/.github/workflows/publish.yml` & `fprime-native-images-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/LICENSE` & `fprime-native-images-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/action.yml` & `fprime-native-images-0.1.2/action.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/env-setup` & `fprime-native-images-0.1.2/env-setup`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/native-images` & `fprime-native-images-0.1.2/native-images`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/publish` & `fprime-native-images-0.1.2/publish`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/pyproject.toml` & `fprime-native-images-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Developers",
 ]
 dependencies = [
     "Jinja2>=2.11.3",
     "build",
     'importlib-metadata; python_version<"3.8"',
 ]
-version="0.1.1"
+version="0.1.2"
 
 [project.scripts]
 fprime-native-packager="fprime_native_images.__main__:main"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `fprime-native-images-0.1.1/src/fprime_native_images/__main__.py` & `fprime-native-images-0.1.2/src/fprime_native_images/__main__.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/src/fprime_native_images/jar.py` & `fprime-native-images-0.1.2/src/fprime_native_images/jar.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/src/fprime_native_images/package.py` & `fprime-native-images-0.1.2/src/fprime_native_images/package.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.1/src/fprime_native_images/templates/setup.py.j2` & `fprime-native-images-0.1.2/src/fprime_native_images/templates/setup.py.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name="{{ package }}",
     #use_scm_version={"root": "../..", "relative_to": __file__},
-    version="0.1.1",
+    version="0.1.2",
     license="Apache 2.0 License",
     description="FPP distribution package for {{ package }}",
     url="https://github.com/nasa/fprime",
     keywords=["fpp", "fprime", "embedded", "nasa"],
     project_urls={"Issue Tracker": "https://github.com/nasa/fprime/issues"},
     author="Michael Starch",
     author_email="Michael.D.Starch@jpl.nasa.gov",
```

### Comparing `fprime-native-images-0.1.1/src/fprime_native_images.egg-info/SOURCES.txt` & `fprime-native-images-0.1.2/src/fprime_native_images.egg-info/SOURCES.txt`

 * *Files identical despite different names*

