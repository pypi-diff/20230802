# Comparing `tmp/sphinx_json_schema_spec-2023.7.3.tar.gz` & `tmp/sphinx_json_schema_spec-2023.8.1.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.7.3.tar` & `sphinx_json_schema_spec-2023.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.flake8
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.readthedocs.yml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/release.yml
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/Makefile
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/index.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/requirements.in
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/README.rst
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/pyproject.toml
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.flake8
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.github/release.yml
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/Makefile
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/index.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/requirements.in
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/README.rst
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.8.1/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.7.3/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/noxfile.py` & `sphinx_json_schema_spec-2023.8.1/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
-@session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
+@session(python=["3.8", "3.9", "3.10", "3.11", "3.12", "pypy3"])
 def tests(session):
     session.install("pytest", ROOT)
     session.run("pytest", *session.posargs, PACKAGE)
 
 
 @session()
 def audit(session):
@@ -70,27 +70,41 @@
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
     with TemporaryDirectory() as tmpdir_str:
         tmpdir = Path(tmpdir_str)
         argv = ["-n", "-T", "-W"]
         if builder != "spelling":
             argv += ["-q"]
+        posargs = session.posargs or [tmpdir / builder]
         session.run(
             "python",
             "-m",
             "sphinx",
             "-b",
             builder,
             DOCS,
-            tmpdir / builder,
             *argv,
+            *posargs,
         )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
     session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
+
+
+@session(default=False)
+def requirements(session):
+    session.install("pip-tools")
+    for each in [DOCS / "requirements.in"]:
+        session.run(
+            "pip-compile",
+            "--resolver",
+            "backtracking",
+            "-U",
+            each.relative_to(ROOT),
+        )
```

### Comparing `sphinx_json_schema_spec-2023.7.3/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.8.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.8.1/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,22 @@
         if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.x"
+          python-version: |
+            3.8
+            3.9
+            3.10
+            3.11
+            3.12
+            pypy3.10
+          allow-prereleases: true
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   packaging:
     needs: ci
```

### Comparing `sphinx_json_schema_spec-2023.7.3/docs/Makefile` & `sphinx_json_schema_spec-2023.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/docs/conf.py` & `sphinx_json_schema_spec-2023.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/docs/index.rst` & `sphinx_json_schema_spec-2023.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/docs/requirements.txt` & `sphinx_json_schema_spec-2023.8.1/docs/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --resolver=backtracking docs/requirements.in
+#    pip-compile --config=pyproject.toml docs/requirements.in
 #
 alabaster==0.7.13
     # via sphinx
 babel==2.12.1
     # via sphinx
 beautifulsoup4==4.12.2
     # via furo
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via sphinx
-fonttools==4.39.4
+fonttools==4.41.1
     # via matplotlib
-furo==2023.5.20
+furo==2023.7.26
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
 kiwisolver==1.4.4
     # via matplotlib
-lxml==4.9.2
+lxml==4.9.3
     # via sphinx-json-schema-spec
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via sphinxext-opengraph
-numpy==1.24.3
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
 packaging==23.1
     # via
     #   matplotlib
     #   sphinx
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
 pygments==2.15.1
     # via
     #   furo
     #   sphinx
@@ -62,23 +62,23 @@
     # via sphinx
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==7.0.1
+sphinx==7.1.2
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-json-schema-spec
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
-sphinx-basic-ng==1.0.0b1
+sphinx-basic-ng==1.0.0b2
     # via furo
 file:.#egg=sphinx_json_schema_spec
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
@@ -90,9 +90,9 @@
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
-urllib3==2.0.2
+urllib3==2.0.4
     # via requests
```

### Comparing `sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.8.1/sphinx_json_schema_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/.gitignore` & `sphinx_json_schema_spec-2023.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/COPYING` & `sphinx_json_schema_spec-2023.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/README.rst` & `sphinx_json_schema_spec-2023.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.3/pyproject.toml` & `sphinx_json_schema_spec-2023.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Sphinx :: Extension",
   "Topic :: Documentation :: Sphinx",
   "Topic :: File Formats :: JSON :: JSON Schema",
 ]
 dynamic = ["version"]
```

### Comparing `sphinx_json_schema_spec-2023.7.3/PKG-INFO` & `sphinx_json_schema_spec-2023.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.7.3
+Version: 2023.8.1
 Summary: Sphinx support for the JSON Schema specifications
 Project-URL: Documentation, https://sphinx-json-schema-spec.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
@@ -14,19 +14,19 @@
 Keywords: data validation,json,json schema,jsonschema,sphinx
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Requires-Python: >=3.8
 Requires-Dist: lxml
 Requires-Dist: sphinx>=5.1.1
```

