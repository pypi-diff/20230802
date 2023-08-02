# Comparing `tmp/ufmt-2.1.0.tar.gz` & `tmp/ufmt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufmt-2.1.0.tar", last modified: Mon Mar 27 08:16:06 2023, max compression
+gzip compressed data, was "ufmt-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ufmt-2.1.0.tar` & `ufmt-2.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      180 2022-08-24 05:22:22.088722 ufmt-2.1.0/.flake8
--rw-r--r--   0        0        0     1825 2022-08-24 05:22:22.089380 ufmt-2.1.0/.gitignore
--rw-r--r--   0        0        0       45 2023-03-12 06:58:49.964569 ufmt-2.1.0/.mailmap
--rw-r--r--   0        0        0      202 2022-08-24 05:22:22.089533 ufmt-2.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      156 2023-03-12 07:09:39.616612 ufmt-2.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     6454 2023-03-27 08:03:26.398631 ufmt-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-08-24 05:22:29.431182 ufmt-2.1.0/LICENSE
--rw-r--r--   0        0        0     4486 2022-08-24 05:22:29.435272 ufmt-2.1.0/README.md
--rw-r--r--   0        0        0     1804 2023-03-12 07:19:47.488073 ufmt-2.1.0/action.yml
--rw-r--r--   0        0        0      598 2022-08-24 05:22:22.090743 ufmt-2.1.0/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2022-08-24 05:22:22.091388 ufmt-2.1.0/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2022-08-24 05:22:22.091641 ufmt-2.1.0/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2022-08-24 05:22:22.091821 ufmt-2.1.0/docs/_templates/omnilib.html
--rw-r--r--   0        0        0     1260 2022-08-24 05:22:29.439083 ufmt-2.1.0/docs/api.rst
--rw-r--r--   0        0        0       70 2022-08-24 05:22:29.442268 ufmt-2.1.0/docs/changelog.rst
--rw-r--r--   0        0        0     3259 2022-08-24 05:22:29.445551 ufmt-2.1.0/docs/conf.py
--rw-r--r--   0        0        0       79 2022-08-24 05:22:29.448700 ufmt-2.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     6311 2022-08-24 05:22:29.451708 ufmt-2.1.0/docs/guide.rst
--rw-r--r--   0        0        0      167 2022-08-24 05:22:29.454689 ufmt-2.1.0/docs/index.rst
--rw-r--r--   0        0        0      928 2023-03-12 06:58:49.730504 ufmt-2.1.0/makefile
--rw-r--r--   0        0        0     2414 2023-03-27 04:11:28.005635 ufmt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      693 2022-08-24 05:22:29.480906 ufmt-2.1.0/ufmt/__init__.py
--rw-r--r--   0        0        0       61 2022-08-24 05:22:29.490740 ufmt-2.1.0/ufmt/__main__.py
--rw-r--r--   0        0        0      156 2023-03-27 08:03:26.404938 ufmt-2.1.0/ufmt/__version__.py
--rw-r--r--   0        0        0     4591 2023-03-12 07:35:24.134199 ufmt-2.1.0/ufmt/cli.py
--rw-r--r--   0        0        0     1496 2023-03-27 07:56:43.959770 ufmt-2.1.0/ufmt/config.py
--rw-r--r--   0        0        0    14242 2022-08-24 05:22:29.483128 ufmt-2.1.0/ufmt/core.py
--rw-r--r--   0        0        0        0 2022-08-24 05:22:22.094333 ufmt-2.1.0/ufmt/py.typed
--rw-r--r--   0        0        0      176 2022-08-24 05:22:29.471932 ufmt-2.1.0/ufmt/tests/__init__.py
--rw-r--r--   0        0        0      236 2022-08-24 05:22:29.478841 ufmt-2.1.0/ufmt/tests/__main__.py
--rw-r--r--   0        0        0    17757 2022-09-12 05:44:45.392230 ufmt-2.1.0/ufmt/tests/cli.py
--rw-r--r--   0        0        0     6623 2023-03-27 07:56:43.959899 ufmt-2.1.0/ufmt/tests/config.py
--rw-r--r--   0        0        0    22640 2023-03-27 04:11:28.006833 ufmt-2.1.0/ufmt/tests/core.py
--rw-r--r--   0        0        0     2780 2022-08-24 05:22:29.469756 ufmt-2.1.0/ufmt/tests/util.py
--rw-r--r--   0        0        0     1374 2022-08-24 05:22:29.486971 ufmt-2.1.0/ufmt/types.py
--rw-r--r--   0        0        0     3367 2023-03-12 07:35:24.134583 ufmt-2.1.0/ufmt/util.py
--rw-r--r--   0        0        0     5799 1970-01-01 00:00:00.000000 ufmt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      180 2022-08-24 05:22:22.088722 ufmt-2.2.0/.flake8
+-rw-r--r--   0        0        0     1825 2022-08-24 05:22:22.089380 ufmt-2.2.0/.gitignore
+-rw-r--r--   0        0        0       45 2023-03-12 06:58:49.964569 ufmt-2.2.0/.mailmap
+-rw-r--r--   0        0        0      202 2022-08-24 05:22:22.089533 ufmt-2.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      156 2023-03-12 07:09:39.616612 ufmt-2.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     6882 2023-08-02 04:24:53.289424 ufmt-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      611 2023-08-02 02:55:24.080656 ufmt-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2022-08-24 05:22:29.431182 ufmt-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4486 2023-08-02 02:33:13.073205 ufmt-2.2.0/README.md
+-rw-r--r--   0        0        0     1804 2023-03-12 07:19:47.488073 ufmt-2.2.0/action.yml
+-rw-r--r--   0        0        0      598 2022-08-24 05:22:22.090743 ufmt-2.2.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2022-08-24 05:22:22.091388 ufmt-2.2.0/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2022-08-24 05:22:22.091641 ufmt-2.2.0/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2022-08-24 05:22:22.091821 ufmt-2.2.0/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0     1260 2022-08-24 05:22:29.439083 ufmt-2.2.0/docs/api.rst
+-rw-r--r--   0        0        0       70 2022-08-24 05:22:29.442268 ufmt-2.2.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3259 2022-08-24 05:22:29.445551 ufmt-2.2.0/docs/conf.py
+-rw-r--r--   0        0        0       79 2022-08-24 05:22:29.448700 ufmt-2.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0     6311 2022-08-24 05:22:29.451708 ufmt-2.2.0/docs/guide.rst
+-rw-r--r--   0        0        0      167 2022-08-24 05:22:29.454689 ufmt-2.2.0/docs/index.rst
+-rw-r--r--   0        0        0      928 2023-03-12 06:58:49.730504 ufmt-2.2.0/makefile
+-rw-r--r--   0        0        0     2408 2023-08-02 02:33:13.073329 ufmt-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      693 2022-08-24 05:22:29.480906 ufmt-2.2.0/ufmt/__init__.py
+-rw-r--r--   0        0        0       61 2022-08-24 05:22:29.490740 ufmt-2.2.0/ufmt/__main__.py
+-rw-r--r--   0        0        0      156 2023-08-02 04:24:53.294389 ufmt-2.2.0/ufmt/__version__.py
+-rw-r--r--   0        0        0     4904 2023-08-02 01:40:26.151517 ufmt-2.2.0/ufmt/cli.py
+-rw-r--r--   0        0        0     1496 2023-03-27 07:56:43.959770 ufmt-2.2.0/ufmt/config.py
+-rw-r--r--   0        0        0    14362 2023-08-02 01:40:26.151963 ufmt-2.2.0/ufmt/core.py
+-rw-r--r--   0        0        0        0 2022-08-24 05:22:22.094333 ufmt-2.2.0/ufmt/py.typed
+-rw-r--r--   0        0        0      176 2022-08-24 05:22:29.471932 ufmt-2.2.0/ufmt/tests/__init__.py
+-rw-r--r--   0        0        0      236 2022-08-24 05:22:29.478841 ufmt-2.2.0/ufmt/tests/__main__.py
+-rw-r--r--   0        0        0    18402 2023-08-02 01:40:26.152129 ufmt-2.2.0/ufmt/tests/cli.py
+-rw-r--r--   0        0        0     6623 2023-03-27 07:56:43.959899 ufmt-2.2.0/ufmt/tests/config.py
+-rw-r--r--   0        0        0    22640 2023-03-27 04:11:28.006833 ufmt-2.2.0/ufmt/tests/core.py
+-rw-r--r--   0        0        0     2780 2022-08-24 05:22:29.469756 ufmt-2.2.0/ufmt/tests/util.py
+-rw-r--r--   0        0        0     1412 2023-08-02 01:40:26.152615 ufmt-2.2.0/ufmt/types.py
+-rw-r--r--   0        0        0     3367 2023-03-12 07:35:24.134583 ufmt-2.2.0/ufmt/util.py
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 ufmt-2.2.0/PKG-INFO
```

### Comparing `ufmt-2.1.0/.gitignore` & `ufmt-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/CHANGELOG.md` & `ufmt-2.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 µfmt
 ====
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v2.2.0
+------
+
+Feature release
+
+- New: added `--concurrency` option to control number of parallel jobs (#149)
+- New: `ufmt_paths` accepts `concurrency` option (#149)
+- New: added contributor guide (#159)
+- Fix: return exit code 0 when no files were formatted (#151)
+- Python: dropped support for Python 3.7 (#158)
+
+```text
+$ git shortlog -s v2.1.0...v2.2.0
+     3	Amethyst Reese
+     2	Sergey Goder
+     7	dependabot[bot]
+```
+
+
 v2.1.0
 ------
 
 Feature release
 
 - Better support for 3.10+ syntax, enable LibCST native parser by default (#127)
 - Stronger validation of ufmt config in pyproject.toml (#137)
```

### Comparing `ufmt-2.1.0/LICENSE` & `ufmt-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/README.md` & `ufmt-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 checking or formatting files, without any chance of conflict or intermediate changes
 between the import sorter and the code formatter.
 
 
 Install
 -------
 
-µfmt requires Python 3.7 or newer. You can install it from PyPI:
+µfmt requires Python 3.8 or newer. You can install it from PyPI:
 
 ```shell-session
 $ pip install ufmt
 ```
 
 If you want to prevent unexpected formatting changes that can break your CI workflow,
 make sure to pin your transitive dependencies–including black, µsort, and µfmt–to your
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 producing the smallest diffs possible. Blackened code looks the same regardless
 of the project youâre reading. > Î¼sort is a safe, minimal import sorter. Its
 primary goal is to make no âdangerousâ changes to code, and to make no
 changes on code style. Âµfmt formats files in-memory, first with Âµsort and
 then with black, before writing any changes back to disk. This enables a
 combined, atomic step in CI/CD workflows for checking or formatting files,
 without any chance of conflict or intermediate changes between the import
-sorter and the code formatter. Install ------- Âµfmt requires Python 3.7 or
+sorter and the code formatter. Install ------- Âµfmt requires Python 3.8 or
 newer. You can install it from PyPI: ```shell-session $ pip install ufmt ``` If
 you want to prevent unexpected formatting changes that can break your CI
 workflow, make sure to pin your transitive dependenciesâincluding black,
 Âµsort, and Âµfmtâto your preferred versions. If you use `requirements.txt`,
 this might look like: ```text black==22.6.0 ufmt==2.0.0 usort==1.0.4 ``` Usage
 ----- To format one or more files or directories in place: ```shell-session $
 ufmt format  [ ...] ``` To validate files are formatted correctly, like for CI
```

### Comparing `ufmt-2.1.0/action.yml` & `ufmt-2.2.0/action.yml`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/_static/custom.css` & `ufmt-2.2.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/_static/omnilib.png` & `ufmt-2.2.0/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/_templates/omnilib.html` & `ufmt-2.2.0/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/api.rst` & `ufmt-2.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/conf.py` & `ufmt-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/docs/guide.rst` & `ufmt-2.2.0/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/makefile` & `ufmt-2.2.0/makefile`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/pyproject.toml` & `ufmt-2.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,38 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-requires-python = ">=3.7"
+requires-python = ">= 3.8"
 dependencies = [
     "black>=20.8b0",
     "click>=8.0",
     "libcst>=0.4.0",
     "moreorless>=0.4.0",
     "tomlkit>=0.7.2",
     "trailrunner>=1.2.1",
     "typing-extensions>=4.0",
     "usort>=1.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "attribution==1.6.2",
-    "black==23.1.0",
-    "coverage==7.2.1",
-    "flit==3.7.1",
-    "flake8==5.0.4",
-    "mypy==1.1.1",
-    "usort==1.0.5",
+    "black==23.7.0",
+    "coverage==7.2.7",
+    "flit==3.9.0",
+    "flake8==6.1.0",
+    "mypy==1.4.1",
+    "usort==1.0.7",
 ]
 docs = [
-    "sphinx==6.1.3",
+    "sphinx==7.1.1",
     "sphinx-mdinclude==0.5.3",
 ]
 
 [project.urls]
 Documentation = "https://ufmt.omnilib.dev"
 Github = "https://github.com/omnilib/ufmt"
 Changelog = "https://ufmt.omnilib.dev/en/latest/changelog.html"
@@ -73,23 +73,23 @@
 [tool.coverage.report]
 fail_under = 100
 precision = 1
 show_missing = true
 skip_covered = true
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 # strict = true
 ignore_missing_imports = true
 
 [tool.thx]
 default = ["docs", "test", "lint", "coverage"]
 module = "ufmt"
 srcs = "ufmt"
-python_versions = ["3.7", "3.8", "3.9", "3.10"]
+python_versions = ["3.8", "3.9", "3.10"]
 watch_paths = ["README.md", "docs", "ufmt"]
 
 [tool.thx.jobs]
 deps = "python -m pessimist -c 'python -m {module}.tests' --fast ."
 docs = {run="sphinx-build -ab html docs html", once=true}
 format = {run="python -m ufmt format {srcs}", once=true}
 test = "python -m coverage run -m {module}.tests"
```

### Comparing `ufmt-2.1.0/ufmt/__init__.py` & `ufmt-2.2.0/ufmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/ufmt/cli.py` & `ufmt-2.2.0/ufmt/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,18 +58,14 @@
                 click.secho(f"Would format {result.path}", err=True)
             if diff and result.diff:
                 echo_color_precomputed_diff(result.diff)
 
         else:
             clean += 1
 
-    if empty:
-        click.secho("No files found", fg="yellow", err=True)
-        error += 1
-
     if not quiet:
 
         def f(v: int) -> str:
             return "file" if v == 1 else "files"
 
         reports = []
         if error:
@@ -79,75 +75,87 @@
                 click.style(f"{changed} {f(changed)} would be formatted", bold=True)
             ]
         if written:
             reports += [click.style(f"{written} {f(written)} formatted")]
         if clean:
             reports += [click.style(f"{clean} {f(clean)} already formatted")]
 
-        message = ", ".join(reports)
-        click.secho(f"✨ {message} ✨", err=True)
+        if empty:
+            click.secho("❗️ No files found ❗️", fg="yellow", err=True)
+        else:
+            message = ", ".join(reports)
+            click.secho(f"✨ {message} ✨", err=True)
 
     return (changed + written), error
 
 
 @click.group()
 @click.pass_context
 @click.version_option(__version__, "--version", "-V")
 @click.option(
     "--debug/--quiet",
     "-v/-q",
     is_flag=True,
     default=None,
     help="Enable debug/verbose output",
 )
-def main(ctx: click.Context, debug: Optional[bool]):
+@click.option(
+    "--concurrency",
+    type=int,
+    default=None,
+    help="Override the default concurrency",
+)
+def main(ctx: click.Context, debug: Optional[bool], concurrency: Optional[int]):
     init_logging(debug=debug)
     ctx.obj = Options(
         debug=debug is True,
         quiet=debug is False,
+        concurrency=concurrency,
     )
     enable_libcst_native()
 
 
 @main.command()
 @click.pass_context
 @click.argument(
     "names", type=click.Path(allow_dash=True), nargs=-1, metavar="[PATH] ..."
 )
 def check(ctx: click.Context, names: List[str]):
     """Check formatting of one or more paths"""
     options: Options = ctx.obj
     paths = [Path(name) for name in names] if names else [Path(".")]
-    results = ufmt_paths(paths, dry_run=True)
+    results = ufmt_paths(paths, dry_run=True, concurrency=options.concurrency)
     changed, error = echo_results(results, quiet=options.quiet)
     if changed or error:
         ctx.exit(1)
 
 
 @main.command()
 @click.pass_context
 @click.argument(
     "names", type=click.Path(allow_dash=True), nargs=-1, metavar="[PATH] ..."
 )
 def diff(ctx: click.Context, names: List[str]):
     """Generate diffs for any files that need formatting"""
     options: Options = ctx.obj
     paths = [Path(name) for name in names] if names else [Path(".")]
-    results = ufmt_paths(paths, dry_run=True, diff=True)
+    results = ufmt_paths(
+        paths, dry_run=True, diff=True, concurrency=options.concurrency
+    )
     changed, error = echo_results(results, diff=True, quiet=options.quiet)
     if changed or error:
         ctx.exit(1)
 
 
 @main.command()
 @click.pass_context
 @click.argument(
     "names", type=click.Path(allow_dash=True), nargs=-1, metavar="[PATH] ..."
 )
 def format(ctx: click.Context, names: List[str]):
     """Format one or more paths in place"""
     options: Options = ctx.obj
     paths = [Path(name) for name in names] if names else [Path(".")]
-    results = ufmt_paths(paths)
+    results = ufmt_paths(paths, concurrency=options.concurrency)
     _, error = echo_results(results, quiet=options.quiet)
     if error:
         ctx.exit(1)
```

### Comparing `ufmt-2.1.0/ufmt/config.py` & `ufmt-2.2.0/ufmt/config.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/ufmt/core.py` & `ufmt-2.2.0/ufmt/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
     dry_run: bool = False,
     diff: bool = False,
     return_content: bool = False,
     black_config_factory: Optional[BlackConfigFactory] = None,
     usort_config_factory: Optional[UsortConfigFactory] = None,
     pre_processor: Optional[Processor] = None,
     post_processor: Optional[Processor] = None,
+    concurrency: Optional[int] = None,
 ) -> Generator[Result, None, None]:
     """
     Format one or more paths, recursively, ignoring any files excluded by configuration.
 
     Uses trailrunner to first walk all paths, and then to run :func:`ufmt_file` on each
     matching file found. If more than one eligible file is discovered after walking the
     given paths, all files will be formatted using a process pool for improved
@@ -363,15 +364,17 @@
             usort_config_factory=usort_config_factory,
             pre_processor=pre_processor,
             post_processor=post_processor,
         )
         return
 
     all_paths: List[Path] = []
-    runner = Trailrunner()
+    runner = (
+        Trailrunner() if concurrency is None else Trailrunner(concurrency=concurrency)
+    )
     for path in paths:
         if path == STDIN:
             LOG.warning("Cannot mix stdin ('-') with normal paths, ignoring")
             continue
         config = ufmt_config(path)
         all_paths.extend(runner.walk(path, excludes=config.excludes))
```

### Comparing `ufmt-2.1.0/ufmt/tests/cli.py` & `ufmt-2.2.0/ufmt/tests/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,39 +101,39 @@
 
     @patch("ufmt.cli.ufmt_paths")
     def test_check(self, ufmt_mock):
         with self.subTest("no paths given"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = []
             result = self.runner.invoke(main, ["check"])
-            ufmt_mock.assert_called_with([Path(".")], dry_run=True)
+            ufmt_mock.assert_called_with([Path(".")], dry_run=True, concurrency=None)
             self.assertRegex(result.stderr, r"No files found")
-            self.assertEqual(1, result.exit_code)
+            self.assertEqual(0, result.exit_code)
 
         with self.subTest("already formatted"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=False),
             ]
             result = self.runner.invoke(main, ["check", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True
+                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, concurrency=None
             )
             self.assertEqual(0, result.exit_code)
 
         with self.subTest("needs formatting"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=True),
             ]
             result = self.runner.invoke(main, ["check", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True
+                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, concurrency=None
             )
             self.assertEqual(1, result.exit_code)
 
         with self.subTest("syntax error"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
@@ -145,62 +145,72 @@
                         raw_line=4,
                         raw_column=15,
                     ),
                 ),
             ]
             result = self.runner.invoke(main, ["check", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True
+                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, concurrency=None
             )
             self.assertRegex(
                 result.stderr, r"Error formatting .*frob\.py: Syntax Error @ 4:16"
             )
             self.assertEqual(1, result.exit_code)
 
         with self.subTest("skipped file"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("foo.py"), skipped="special"),
             ]
             result = self.runner.invoke(main, ["check", "foo.py"])
-            ufmt_mock.assert_called_with([Path("foo.py")], dry_run=True)
+            ufmt_mock.assert_called_with(
+                [Path("foo.py")], dry_run=True, concurrency=None
+            )
             self.assertRegex(result.stderr, r"Skipped .*foo\.py: special")
             self.assertEqual(0, result.exit_code)
 
     @patch("ufmt.cli.ufmt_paths")
     def test_diff(self, ufmt_mock):
         with self.subTest("no paths given"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = []
             result = self.runner.invoke(main, ["diff"])
-            ufmt_mock.assert_called_with([Path(".")], dry_run=True, diff=True)
+            ufmt_mock.assert_called_with(
+                [Path(".")], dry_run=True, diff=True, concurrency=None
+            )
             self.assertRegex(result.stderr, r"No files found")
-            self.assertEqual(1, result.exit_code)
+            self.assertEqual(0, result.exit_code)
 
         with self.subTest("already formatted"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=False),
             ]
             result = self.runner.invoke(main, ["diff", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, diff=True
+                [Path("bar.py"), Path("foo/frob.py")],
+                dry_run=True,
+                diff=True,
+                concurrency=None,
             )
             self.assertEqual(0, result.exit_code)
 
         with self.subTest("needs formatting"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=True),
             ]
             result = self.runner.invoke(main, ["diff", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, diff=True
+                [Path("bar.py"), Path("foo/frob.py")],
+                dry_run=True,
+                diff=True,
+                concurrency=None,
             )
             self.assertEqual(1, result.exit_code)
 
         with self.subTest("syntax error"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
@@ -212,69 +222,80 @@
                         raw_line=4,
                         raw_column=15,
                     ),
                 ),
             ]
             result = self.runner.invoke(main, ["diff", "bar.py", "foo/frob.py"])
             ufmt_mock.assert_called_with(
-                [Path("bar.py"), Path("foo/frob.py")], dry_run=True, diff=True
+                [Path("bar.py"), Path("foo/frob.py")],
+                dry_run=True,
+                diff=True,
+                concurrency=None,
             )
             self.assertRegex(
                 result.stderr, r"Error formatting .*frob\.py: Syntax Error @ 4:16"
             )
             self.assertEqual(1, result.exit_code)
 
         with self.subTest("skipped file"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("foo.py"), skipped="special"),
             ]
             result = self.runner.invoke(main, ["diff", "foo.py"])
-            ufmt_mock.assert_called_with([Path("foo.py")], dry_run=True, diff=True)
+            ufmt_mock.assert_called_with(
+                [Path("foo.py")], dry_run=True, diff=True, concurrency=None
+            )
             self.assertRegex(result.stderr, r"Skipped .*foo\.py: special")
             self.assertEqual(0, result.exit_code)
 
         with self.subTest("skipped file quiet"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("foo.py"), skipped="special"),
             ]
             result = self.runner.invoke(main, ["--quiet", "diff", "foo.py"])
-            ufmt_mock.assert_called_with([Path("foo.py")], dry_run=True, diff=True)
+            ufmt_mock.assert_called_with(
+                [Path("foo.py")], dry_run=True, diff=True, concurrency=None
+            )
             self.assertEqual("", result.stderr)
             self.assertEqual(0, result.exit_code)
 
     @patch("ufmt.cli.ufmt_paths")
     def test_format(self, ufmt_mock):
         with self.subTest("no paths given"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = []
             result = self.runner.invoke(main, ["format"])
-            ufmt_mock.assert_called_with([Path(".")])
+            ufmt_mock.assert_called_with([Path(".")], concurrency=None)
             self.assertRegex(result.stderr, r"No files found")
-            self.assertEqual(1, result.exit_code)
+            self.assertEqual(0, result.exit_code)
 
         with self.subTest("already formatted"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=False),
             ]
             result = self.runner.invoke(main, ["format", "bar.py", "foo/frob.py"])
-            ufmt_mock.assert_called_with([Path("bar.py"), Path("foo/frob.py")])
+            ufmt_mock.assert_called_with(
+                [Path("bar.py"), Path("foo/frob.py")], concurrency=None
+            )
             self.assertEqual(0, result.exit_code)
 
         with self.subTest("needs formatting"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(Path("foo/frob.py"), changed=True),
             ]
             result = self.runner.invoke(main, ["format", "bar.py", "foo/frob.py"])
-            ufmt_mock.assert_called_with([Path("bar.py"), Path("foo/frob.py")])
+            ufmt_mock.assert_called_with(
+                [Path("bar.py"), Path("foo/frob.py")], concurrency=None
+            )
             self.assertEqual(0, result.exit_code)
 
         with self.subTest("syntax error"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("bar.py"), changed=False),
                 Result(
@@ -284,27 +305,29 @@
                         lines=("", "", "", "foo bar fizzbuzz hello world"),
                         raw_line=4,
                         raw_column=15,
                     ),
                 ),
             ]
             result = self.runner.invoke(main, ["format", "bar.py", "foo/frob.py"])
-            ufmt_mock.assert_called_with([Path("bar.py"), Path("foo/frob.py")])
+            ufmt_mock.assert_called_with(
+                [Path("bar.py"), Path("foo/frob.py")], concurrency=None
+            )
             self.assertRegex(
                 result.stderr, r"Error formatting .*frob\.py: Syntax Error @ 4:16"
             )
             self.assertEqual(1, result.exit_code)
 
         with self.subTest("skipped file"):
             ufmt_mock.reset_mock()
             ufmt_mock.return_value = [
                 Result(Path("foo.py"), skipped="special"),
             ]
             result = self.runner.invoke(main, ["format", "foo.py"])
-            ufmt_mock.assert_called_with([Path("foo.py")])
+            ufmt_mock.assert_called_with([Path("foo.py")], concurrency=None)
             self.assertRegex(result.stderr, r"Skipped .*foo\.py: special")
             self.assertEqual(0, result.exit_code)
 
     @skipIf(platform.system() == "Windows", "stderr not supported on Windows")
     def test_stdin(self) -> None:
         with self.subTest("check clean"):
             result = self.runner.invoke(
```

### Comparing `ufmt-2.1.0/ufmt/tests/config.py` & `ufmt-2.2.0/ufmt/tests/config.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/ufmt/tests/core.py` & `ufmt-2.2.0/ufmt/tests/core.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/ufmt/tests/util.py` & `ufmt-2.2.0/ufmt/tests/util.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/ufmt/types.py` & `ufmt-2.2.0/ufmt/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 UsortConfigFactory = Callable[[Path], UsortConfig]
 
 
 @dataclass
 class Options:
     debug: bool = False
     quiet: bool = False
+    concurrency: Optional[int] = None
 
 
 class Processor(Protocol):
     def __call__(
         self,
         path: Path,
         content: FileContent,
```

### Comparing `ufmt-2.1.0/ufmt/util.py` & `ufmt-2.2.0/ufmt/util.py`

 * *Files identical despite different names*

### Comparing `ufmt-2.1.0/PKG-INFO` & `ufmt-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ufmt
-Version: 2.1.0
+Version: 2.2.0
 Summary: Safe, atomic formatting with black and µsort
 Author-email: Amethyst Reese <amy@n7.gg>
-Requires-Python: >=3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: black>=20.8b0
@@ -15,21 +15,21 @@
 Requires-Dist: libcst>=0.4.0
 Requires-Dist: moreorless>=0.4.0
 Requires-Dist: tomlkit>=0.7.2
 Requires-Dist: trailrunner>=1.2.1
 Requires-Dist: typing-extensions>=4.0
 Requires-Dist: usort>=1.0
 Requires-Dist: attribution==1.6.2 ; extra == "dev"
-Requires-Dist: black==23.1.0 ; extra == "dev"
-Requires-Dist: coverage==7.2.1 ; extra == "dev"
-Requires-Dist: flit==3.7.1 ; extra == "dev"
-Requires-Dist: flake8==5.0.4 ; extra == "dev"
-Requires-Dist: mypy==1.1.1 ; extra == "dev"
-Requires-Dist: usort==1.0.5 ; extra == "dev"
-Requires-Dist: sphinx==6.1.3 ; extra == "docs"
+Requires-Dist: black==23.7.0 ; extra == "dev"
+Requires-Dist: coverage==7.2.7 ; extra == "dev"
+Requires-Dist: flit==3.9.0 ; extra == "dev"
+Requires-Dist: flake8==6.1.0 ; extra == "dev"
+Requires-Dist: mypy==1.4.1 ; extra == "dev"
+Requires-Dist: usort==1.0.7 ; extra == "dev"
+Requires-Dist: sphinx==7.1.1 ; extra == "docs"
 Requires-Dist: sphinx-mdinclude==0.5.3 ; extra == "docs"
 Project-URL: Changelog, https://ufmt.omnilib.dev/en/latest/changelog.html
 Project-URL: Documentation, https://ufmt.omnilib.dev
 Project-URL: Github, https://github.com/omnilib/ufmt
 Provides-Extra: dev
 Provides-Extra: docs
 
@@ -54,15 +54,15 @@
 checking or formatting files, without any chance of conflict or intermediate changes
 between the import sorter and the code formatter.
 
 
 Install
 -------
 
-µfmt requires Python 3.7 or newer. You can install it from PyPI:
+µfmt requires Python 3.8 or newer. You can install it from PyPI:
 
 ```shell-session
 $ pip install ufmt
 ```
 
 If you want to prevent unexpected formatting changes that can break your CI workflow,
 make sure to pin your transitive dependencies–including black, µsort, and µfmt–to your
```

