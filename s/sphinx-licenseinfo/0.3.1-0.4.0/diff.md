# Comparing `tmp/sphinx_licenseinfo-0.3.1.tar.gz` & `tmp/sphinx_licenseinfo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_licenseinfo-0.3.1.tar", last modified: Fri Apr  1 18:02:49 2022, max compression
+gzip compressed data, was "sphinx_licenseinfo-0.4.0.tar", last modified: Tue Aug  1 22:22:25 2023, max compression
```

## Comparing `sphinx_licenseinfo-0.3.1.tar` & `sphinx_licenseinfo-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-01 18:02:49.309819 sphinx_licenseinfo-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-01 18:02:49.317819 sphinx_licenseinfo-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-04-01 18:02:49.317819 sphinx_licenseinfo-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-04-01 18:02:49.329819 sphinx_licenseinfo-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-04-01 18:02:49.317819 sphinx_licenseinfo-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license_info.t.html
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license-sprite.png
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license_info.css
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/translators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11162 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-01 18:02:18.021547 sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license-sprite@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-08-01 22:22:25.054066 sphinx_licenseinfo-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-01 22:22:25.066066 sphinx_licenseinfo-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4848 2023-08-01 22:22:25.066066 sphinx_licenseinfo-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6731 2023-08-01 22:22:25.070066 sphinx_licenseinfo-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5338 2023-08-01 22:22:25.066066 sphinx_licenseinfo-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    11217 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license_info.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/translators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license-sprite@2x.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-08-01 22:21:40.053923 sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license_info.t.html
```

### Comparing `sphinx_licenseinfo-0.3.1/LICENSE` & `sphinx_licenseinfo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_licenseinfo-0.3.1/pyproject.toml` & `sphinx_licenseinfo-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "sphinx-licenseinfo"
-version = "0.3.1"
+version = "0.4.0"
 description = "Sphinx directives for showing license information."
 readme = "README.rst"
 keywords = [ "documentation", "license", "sphinx", "sphinx-extension",]
 dynamic = []
 dependencies = [
     "dist-meta>=0.1.2",
-    "docutils==0.16",
+    "docutils>=0.16",
     "domdf-python-tools>=3.0.0",
-    "jinja2<3.1,>=2.11.3",
+    "jinja2>=2.11.3",
     "pychoosealicense>=0.2.0",
-    "sphinx<4.4.0,>=3.2.0",
+    "sphinx<6,>=3.2.0",
+    "sphinx-jinja2-compat>=0.2.0",
     "sphinx-toolbox>=2.13.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
@@ -61,15 +63,15 @@
     "Intended Audience :: Developers",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-python-versions = [ "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "sphinx_licenseinfo"
 additional-files = [
     "include sphinx_licenseinfo/license-sprite.png",
     "include sphinx_licenseinfo/license-sprite@2x.png",
@@ -87,25 +89,25 @@
 package_root = "sphinx_licenseinfo"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx_toolbox_experimental.autosummary_widths",
     "sphinx_toolbox_experimental.needspace",
     "sphinx_toolbox_experimental.missing_xref",
@@ -167,14 +169,17 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.dep_checker]
+allowed_unused = [ "sphinx_jinja2_compat",]
+
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
```

### Comparing `sphinx_licenseinfo-0.3.1/PKG-INFO` & `sphinx_licenseinfo-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-licenseinfo
-Version: 0.3.1
+Version: 0.4.0
 Summary: Sphinx directives for showing license information.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,license,sphinx,sphinx-extension
 Home-page: https://github.com/sphinx-toolbox/sphinx-licenseinfo
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/sphinx-licenseinfo/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/sphinx-licenseinfo
@@ -19,28 +19,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: dist-meta>=0.1.2
-Requires-Dist: docutils==0.16
+Requires-Dist: docutils>=0.16
 Requires-Dist: domdf-python-tools>=3.0.0
-Requires-Dist: jinja2<3.1,>=2.11.3
+Requires-Dist: jinja2>=2.11.3
 Requires-Dist: pychoosealicense>=0.2.0
-Requires-Dist: sphinx<4.4.0,>=3.2.0
+Requires-Dist: sphinx<6,>=3.2.0
+Requires-Dist: sphinx-jinja2-compat>=0.2.0
 Requires-Dist: sphinx-toolbox>=2.13.0
 Description-Content-Type: text/x-rst
 
 
 ===================
 sphinx-licenseinfo
 ===================
@@ -95,16 +97,16 @@
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/sphinx-licenseinfo/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/sphinx-licenseinfo/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/sphinx-licenseinfo/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/sphinx-licenseinfo/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/sphinx-licenseinfo/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/sphinx-licenseinfo/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/sphinx-licenseinfo?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/sphinx-licenseinfo?logo=codefactor
@@ -130,23 +132,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/sphinx-licenseinfo
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/sphinx-licenseinfo
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-licenseinfo/v0.3.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-licenseinfo/v0.4.0
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/sphinx-licenseinfo
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/sphinx-licenseinfo
 	:target: https://pypi.org/project/sphinx-licenseinfo/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `sphinx_licenseinfo-0.3.1/README.rst` & `sphinx_licenseinfo-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/sphinx-licenseinfo/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/sphinx-licenseinfo/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/sphinx-licenseinfo/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/sphinx-licenseinfo/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/sphinx-licenseinfo/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/sphinx-licenseinfo/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/sphinx-licenseinfo?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/sphinx-licenseinfo?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/sphinx-licenseinfo
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/sphinx-licenseinfo
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-licenseinfo/v0.3.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/sphinx-licenseinfo/v0.4.0
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/sphinx-licenseinfo
 	:target: https://github.com/sphinx-toolbox/sphinx-licenseinfo/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/sphinx-licenseinfo
 	:target: https://pypi.org/project/sphinx-licenseinfo/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license_info.t.html` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license_info.t.html`

 * *Files identical despite different names*

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license-sprite.png` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license-sprite.png`

 * *Files identical despite different names*

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license_info.css` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license_info.css`

 * *Files identical despite different names*

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/translators.py` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/translators.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 # this package
 from sphinx_licenseinfo import nodes
 
 __all__ = ["visit_flushright_text", "depart_flushright_text", "visit_license_info", "depart_license_info"]
 
 
-def visit_flushright_text(translator: LaTeXTranslator, node: nodes.flushright_text):
+def visit_flushright_text(translator: LaTeXTranslator, node: nodes.flushright_text) -> None:
 	"""
 	Visit a :class:`~.flushright_text` node and generate LaTeX output.
 
 	:param translator:
 	:param node:
 	"""
 
@@ -68,15 +68,15 @@
 	else:
 		# Sphinx 3.5 adds \sphinxAtStartPar here, but I don't see what it gains.
 		translator.body.append('\n')
 
 	translator.body.append("$POP_TO_HERE$")
 
 
-def depart_flushright_text(translator: LaTeXTranslator, node: nodes.flushright_text):
+def depart_flushright_text(translator: LaTeXTranslator, node: nodes.flushright_text) -> None:
 	"""
 	Depart a :class:`~.flushright_text` node and generate LaTeX output.
 
 	:param translator:
 	:param node:
 	"""
 
@@ -89,15 +89,15 @@
 		else:
 			node_content.append(item.replace('➩', r"{}$\Rightarrow${}"))
 
 	translator.body.extend(reversed(node_content))
 	translator.body.append("\n\\end{flushright}\n")
 
 
-def visit_license_info(translator: HTML5Translator, node: nodes.license_info):
+def visit_license_info(translator: HTML5Translator, node: nodes.license_info) -> None:
 	"""
 	Visit a :class:`~.license_info` node and generate HTML output.
 
 	:param translator:
 	:param node:
 	"""
 
@@ -111,14 +111,14 @@
 	the_description = pychoosealicense.description.as_html(node.license.description)
 	output = license_template.render(license=node.license, description=the_description).split('\n')
 
 	translator.body.extend(output)
 	raise docutils.nodes.SkipNode
 
 
-def depart_license_info(translator: HTML5Translator, node: nodes.license_info):
+def depart_license_info(translator: HTML5Translator, node: nodes.license_info) -> None:
 	"""
 	Depart a :class:`~.license_info` node and generate HTML output.
 
 	:param translator:
 	:param node:
 	"""
```

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/nodes.py` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/__init__.py` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 # this package
 from sphinx_licenseinfo import nodes
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.3.1"
+__version__: str = "0.4.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"ChooseALicenseRole",
 		"LicenseDirective",
 		"LicenseInfoDirective",
 		"setup",
@@ -184,15 +184,15 @@
 				see_more_node
 				)
 
 		license_node += nodes.custom_transition()
 
 		return [license_node]
 
-	def add_rules_list(self, category: str, rules: Iterable[Rule]):
+	def add_rules_list(self, category: str, rules: Iterable[Rule]) -> List[docutils.nodes.Node]:
 		"""
 		Add a heading for a rule category, followed by a bullet-point list of the rules in that category.
 
 		:param category: The category label.
 		:param rules: The rules.
 		"""
 
@@ -244,15 +244,15 @@
 		refuri = f"https://choosealicense.com/licenses/{the_license.spdx_id.lower()}/"
 		reference = docutils.nodes.reference('', '', internal=False, refuri=refuri, classes=["choosealicense"])
 		reference += docutils.nodes.inline(self.title, self.title)
 
 		return [index, target, reference], []
 
 
-def copy_asset_files(app: Sphinx, exception: Optional[Exception] = None):
+def copy_asset_files(app: Sphinx, exception: Optional[Exception] = None) -> None:
 	"""
 	Copy additional stylesheets into the HTML build directory.
 
 	:param app: The Sphinx application.
 	:param exception: Any exception which occurred and caused Sphinx to abort.
 	"""
 
@@ -275,15 +275,15 @@
 	img_dir.maybe_make()
 
 	for filename in ("license-sprite@2x.png", "license-sprite.png"):
 		with importlib_resources.open_binary("sphinx_licenseinfo", filename) as fp2:
 			(css_dir / filename).write_bytes(fp2.read())
 
 
-def _configure(app: Sphinx):
+def _configure(app: Sphinx) -> None:
 
 	assert app.builder is not None
 
 	kwargs = {}
 	translation_handlers = app.registry.translation_handlers
 	translator = app.registry.translators.get(
 			app.builder.name,
@@ -308,15 +308,15 @@
 					return
 
 		kwargs[builder_name_or_format] = (
 				translator.visit_transition,  # type: ignore[attr-defined ]
 				getattr(translator, "depart_transition", lambda *args: None),
 				)
 
-		app.add_node(nodes.custom_transition, **kwargs)  # type: ignore
+		app.add_node(nodes.custom_transition, **kwargs)  # type: ignore[arg-type]
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
 	"""
 	Setup :mod:`sphinx_licenseinfo`.
 
 	:param app: The Sphinx application.
```

### Comparing `sphinx_licenseinfo-0.3.1/sphinx_licenseinfo/license-sprite@2x.png` & `sphinx_licenseinfo-0.4.0/sphinx_licenseinfo/license-sprite@2x.png`

 * *Files identical despite different names*

