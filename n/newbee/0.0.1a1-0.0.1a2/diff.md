# Comparing `tmp/newbee-0.0.1a1.tar.gz` & `tmp/newbee-0.0.1a2.tar.gz`

## Comparing `newbee-0.0.1a1.tar` & `newbee-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 newbee-0.0.1a1/RELEASE.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 newbee-0.0.1a1/dev/Dockerfile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docker/Dockerfile
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/Makefile
--rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/conf.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/make.bat
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 newbee-0.0.1a1/docs/usage.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 newbee-0.0.1a1/newbee/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 newbee-0.0.1a1/tests/test_newbee.py
--rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 newbee-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 newbee-0.0.1a1/LICENSE
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 newbee-0.0.1a1/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 newbee-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 newbee-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 newbee-0.0.1a2/RELEASE.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 newbee-0.0.1a2/dev/Dockerfile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docker/Dockerfile
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docs/Makefile
+-rwxr-xr-x   0        0        0     4760 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docs/conf.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docs/make.bat
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 newbee-0.0.1a2/docs/usage.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 newbee-0.0.1a2/newbee/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 newbee-0.0.1a2/tests/test_newbee.py
+-rw-r--r--   0        0        0    10128 2020-02-02 00:00:00.000000 newbee-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 newbee-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 newbee-0.0.1a2/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 newbee-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 newbee-0.0.1a2/PKG-INFO
```

### Comparing `newbee-0.0.1a1/.pre-commit-config.yaml` & `newbee-0.0.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/RELEASE.md` & `newbee-0.0.1a2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/.github/workflows/publish.yml` & `newbee-0.0.1a2/.github/workflows/publish.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         file: ./docker/Dockerfile
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/newbee-server:${{  github.ref_name }}
 
     # Build latest if release
     -
       name: Build and push release
-      id: docker_build_release
       if: '!github.event.prerelease'
+      id: docker_build_release
       uses: docker/build-push-action@v4
       with:
         context: .
         file: ./docker/Dockerfile
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/newbee-server:latest
```

### Comparing `newbee-0.0.1a1/.github/workflows/python-package.yml` & `newbee-0.0.1a2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/docs/Makefile` & `newbee-0.0.1a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/docs/conf.py` & `newbee-0.0.1a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/docs/make.bat` & `newbee-0.0.1a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/.gitignore` & `newbee-0.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/LICENSE` & `newbee-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/README.md` & `newbee-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/pyproject.toml` & `newbee-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `newbee-0.0.1a1/PKG-INFO` & `newbee-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newbee
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: newbee
 Project-URL: Source, https://github.com/wh1isper/newbee
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: newbee
 Classifier: Programming Language :: Python :: 3
```

