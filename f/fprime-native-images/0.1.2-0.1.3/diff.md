# Comparing `tmp/fprime-native-images-0.1.2.tar.gz` & `tmp/fprime-native-images-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-native-images-0.1.2.tar", last modified: Wed Aug  2 04:54:29 2023, max compression
+gzip compressed data, was "fprime-native-images-0.1.3.tar", last modified: Wed Aug  2 17:55:18 2023, max compression
```

## Comparing `fprime-native-images-0.1.2.tar` & `fprime-native-images-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.662181 fprime-native-images-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/.github/workflows/native-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/env-setup
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/java
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/native-images
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/publish
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.662181 fprime-native-images-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 04:54:18.000000 fprime-native-images-0.1.2/src/fprime_native_images/templates/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:54:29.666181 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 04:54:29.000000 fprime-native-images-0.1.2/src/fprime_native_images.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.822933 fprime-native-images-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/.github/workflows/native-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/env-setup
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/native-images
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/publish
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.822933 fprime-native-images-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 17:55:10.000000 fprime-native-images-0.1.3/src/fprime_native_images/templates/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:55:18.826933 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 17:55:18.000000 fprime-native-images-0.1.3/src/fprime_native_images.egg-info/top_level.txt
```

### Comparing `fprime-native-images-0.1.2/.github/workflows/native-build.yml` & `fprime-native-images-0.1.3/.github/workflows/native-build.yml`

 * *Files 25% similar despite different names*

```diff
@@ -138,15 +138,15 @@
           cd ${{ inputs.working-directory }}
           export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
           $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
         shell: bash
       - name: "Archive Native Images"
         uses: actions/upload-artifact@v3
         with:
-          name: native-images-${{ matrix.runner.tag }}
+          name: build-${{ matrix.runner.tag }}
           path: bin/*
           retention-days: 5
           if-no-files-found: error
   build-native-wheels:
     needs: [build-native-images-linux, build-native-images-non-linux]
     runs-on: ubuntu-latest
     strategy:
@@ -173,19 +173,20 @@
         uses: actions/upload-artifact@v3
         with:
           name: wheels-${{ matrix.package_tag }}
           path: packages/dist/*
           retention-days: 5
           if-no-files-found: error
   publish-native-wheels:
+    if: ${{ github.event_name == 'release' }}
     needs: [build-native-wheels]
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        package_tag: ["jar", "manylinux_2_28_x86_64"]
+        package_tag: ["jar", "manylinux_2_28_x86_64", "manylinux_2_28_aarch64", "macosx_10_9_universal2"]
     steps:
       - name: "Download Package"
         uses: actions/download-artifact@v3
         with:
           name: wheels-${{ matrix.package_tag }}
           path: dist
       - name: "Install Builder"
@@ -199,107 +200,7 @@
         shell: bash
       - name: Publish distributions to PyPI
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_CREDENTIAL }}
         run: |
           twine upload -u "__token__" dist/*
         shell: bash
-#  build-native-images-non-linux:
-#    needs: build-jars
-#    strategy:
-#      matrix:
-#        runner: ["macos-11", "odroid"]
-#    runs-on: ${{ matrix.runner }}
-#    steps:
-#      - name: "Checkout repository"
-#        uses: actions/checkout@v3
-#        with:
-#          submodules: recursive
-#      - name: "Setup Native Image Tools"
-#        uses: fprime-community/native-images-action@main
-#      - name: "Download JARs"
-#        uses: actions/download-artifact@v3
-#        with:
-#          name: build-jar
-#          path: bin
-#      - name: "Download Tracing"
-#        uses: actions/download-artifact@v3
-#        with:
-#          name: jar-traces
-#          path: ${{ inputs.trace-directory }}
-#      - name: "Build Native Images"
-#        if: ${{ matrix.runner != "ubuntu-latest" }}
-#        run: |
-#          cd ${{ inputs.working-directory }}
-#          export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
-#          $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
-#        shell: bash
-#      - name: "Build Native Images (Docker)"
-#        if: ${{ matrix.runner == "ubuntu-latest" }}
-#        using: 'docker'
-#        run: |
-#          cd ${{ inputs.working-directory }}
-#          export CLASSPATH="${{ inputs.trace-directory }}/../..:${CLASSPATH}"
-#          $NATIVE_IMAGE_TOOLS_PATH/native-images bin ${{ inputs.tools }}
-#        shell: bash
-#      - name: "Archive Native Images"
-#        uses: actions/upload-artifact@v3
-#        with:
-#          name: native-images-${{ matrix.runner }}
-#          path: bin/*
-#          retention-days: 5
-#          if-no-files-found: error
-
-  #  - run: |
-  #      echo "Build Native Images"
-  #      cd ${{ inputs.working-directory }}
-  #      $GITHUB_ACTION_PATH/native-images "${{ inputs.output-directory }}" ${{ inputs.tools }}
-  #    shell: bash
-
-#
-#
-#  using: "composite"
-#  steps:
-#  - run: |
-#      echo "Setup GraalVM Environment"
-#      $GITHUB_ACTION_PATH/env-setup
-#      echo "ARCH=$( uname -m)" >> $GITHUB_ENV
-#    shell: bash
-#  - run: |
-#      echo "Build JAR files"
-#      cd ${{ inputs.working-directory }}
-#      ${{ inputs.build }} ${{ inputs.output-directory }}
-#    shell: bash
-#  - if: ${{ inputs.trace == 'true' }}
-#    run: |
-#      echo "Trace JAR files via tests"
-#      cd ${{ inputs.working-directory }}
-#      mkdir -p "${{ inputs.trace-directory }}"
-#      export TRACE_METADATA_DIRECTORY="${{ inputs.trace-directory }}"
-#      export PATH="${GITHUB_ACTION_PATH}:${PATH}"
-#      ${{ inputs.test }}
-#      echo "CLASSPATH=${{ inputs.trace-directory }}:${CLASSPATH}" >> $GITHUB_ENV
-#    shell: bash
-#  - run: |
-#      echo "Build Native Images"
-#      cd ${{ inputs.working-directory }}
-#      $GITHUB_ACTION_PATH/native-images "${{ inputs.output-directory }}" ${{ inputs.tools }}
-#    shell: bash
-#  - run: |
-#      echo "Test Native Outputs"
-#      cd ${{ inputs.working-directory }}
-#      ${{ inputs.test }}
-#    shell: bash
-#  - run:  |
-#      echo "Archiving Tools"
-#      tar -czf ${GITHUB_WORKSPACE}/fprime-layout-${ARCH}.tar.gz ${{ inputs.output-directory }}
-#    shell: bash
-#  - if: ${{ github.event_name == 'release' }}
-#    run: |
-#      ${GITHUB_ACTION_PATH}/publish ${GITHUB_WORKSPACE}/fprime-layout-${ARCH}.tar.gz
-#    shell: bash
-#  - if: ${{ github.event_name != 'release' }}
-#    uses: actions/upload-artifact@v3
-#    with:
-#      name: fprime-layout-${{ env.ARCH }}
-#      path: fprime-layout-${{ env.ARCH }}.tar.gz
-#      retention-days: 5
```

### Comparing `fprime-native-images-0.1.2/.github/workflows/publish.yml` & `fprime-native-images-0.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/LICENSE` & `fprime-native-images-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/action.yml` & `fprime-native-images-0.1.3/action.yml`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/env-setup` & `fprime-native-images-0.1.3/env-setup`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/native-images` & `fprime-native-images-0.1.3/native-images`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/publish` & `fprime-native-images-0.1.3/publish`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/pyproject.toml` & `fprime-native-images-0.1.3/pyproject.toml`

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
-version="0.1.2"
+version="0.1.3"
 
 [project.scripts]
 fprime-native-packager="fprime_native_images.__main__:main"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `fprime-native-images-0.1.2/src/fprime_native_images/__main__.py` & `fprime-native-images-0.1.3/src/fprime_native_images/__main__.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/src/fprime_native_images/jar.py` & `fprime-native-images-0.1.3/src/fprime_native_images/jar.py`

 * *Files identical despite different names*

### Comparing `fprime-native-images-0.1.2/src/fprime_native_images/package.py` & `fprime-native-images-0.1.3/src/fprime_native_images/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
+import os
 import platform
 import sys
 import subprocess
 from pathlib import Path
 from typing import List, Union
 
 from jinja2 import Environment, PackageLoader
 
 
-MANY_LINUX_SPECIFIER = "2.28"
-MAC_SPECIFIER = "10.9"
-
-
 def build_packages_from_directory(directory: Path, working: Path, outdir: Path, package_tag: str, extensions: Union[List[str], None] = None):
     """ Build a set of packages around tools found in a directory
 
     Given a directory this will build a PIP package that wraps each tool in that directory. Tools will be filtered by
     the list of extensions, with a default of filter of no-extension and ".exe".
 
     Args:
@@ -33,14 +30,17 @@
     extensions = extensions if extensions else ["", ".exe"]
     for tool in directory.glob("*"):
         if tool.suffix not in extensions:
             print(f"[INFO] Skipping {tool} with unaccepted extension")
             continue
         print(f"[INFO] Building package around {tool} with tag {package_tag}")
         directory = generate_tool_package(tool, environment, working)
+        # Patch for +x ensuring tools are executable
+        st = os.stat(str(tool.resolve()))
+        os.chmod(str(tool.resolve()), st.st_mode | st.S_IEXEC)
         build_wheel(directory, outdir, package_tag)
 
 
 def generate_tool_package(tool: Path, environment: Environment, working: Path) -> Path:
     """ Build a PIP package for a given tool
 
     Builds a package for a given tool using setuptools. This wraps the setup call suplying the given package and given
```

### Comparing `fprime-native-images-0.1.2/src/fprime_native_images/templates/setup.py.j2` & `fprime-native-images-0.1.3/src/fprime_native_images/templates/setup.py.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from setuptools import setup
 setup(
     name="{{ package }}",
-    #use_scm_version={"root": "../..", "relative_to": __file__},
-    version="0.1.2",
+    use_scm_version={"root": "../..", "relative_to": __file__},
     license="Apache 2.0 License",
     description="FPP distribution package for {{ package }}",
     url="https://github.com/nasa/fprime",
     keywords=["fpp", "fprime", "embedded", "nasa"],
     project_urls={"Issue Tracker": "https://github.com/nasa/fprime/issues"},
     author="Michael Starch",
     author_email="Michael.D.Starch@jpl.nasa.gov",
```

### Comparing `fprime-native-images-0.1.2/src/fprime_native_images.egg-info/SOURCES.txt` & `fprime-native-images-0.1.3/src/fprime_native_images.egg-info/SOURCES.txt`

 * *Files identical despite different names*

