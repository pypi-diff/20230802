# Comparing `tmp/tox-poetry-installer-0.9.0.tar.gz` & `tmp/tox_poetry_installer-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-poetry-installer-0.9.0.tar", max compression
+gzip compressed data, was "tox_poetry_installer-1.0.0b1.tar", max compression
```

## Comparing `tox-poetry-installer-0.9.0.tar` & `tox_poetry_installer-1.0.0b1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1059 2022-09-07 20:03:49.587295 tox-poetry-installer-0.9.0/LICENSE.md
--rw-r--r--   0        0        0    23370 2022-09-07 20:03:49.707295 tox-poetry-installer-0.9.0/README.md
--rw-r--r--   0        0        0     1867 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1945 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tests/fixtures.py
--rw-r--r--   0        0        0     2071 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tests/test_installer.py
--rw-r--r--   0        0        0     1219 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/test_metadata.py
--rw-r--r--   0        0        0     2731 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tests/test_transients.py
--rw-r--r--   0        0        0      355 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/__about__.py
--rw-r--r--   0        0        0      153 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/__init__.py
--rw-r--r--   0        0        0     2083 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/_poetry.py
--rw-r--r--   0        0        0     1009 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/constants.py
--rw-r--r--   0        0        0     1491 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/exceptions.py
--rw-r--r--   0        0        0    10426 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/hooks.py
--rw-r--r--   0        0        0     2867 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/installer.py
--rw-r--r--   0        0        0      937 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/logger.py
--rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox-poetry-installer-0.9.0/tox_poetry_installer/py.typed
--rw-r--r--   0        0        0    11705 2022-09-07 19:44:43.594829 tox-poetry-installer-0.9.0/tox_poetry_installer/utilities.py
--rw-r--r--   0        0        0    24911 1970-01-01 00:00:00.000000 tox-poetry-installer-0.9.0/setup.py
--rw-r--r--   0        0        0    24932 1970-01-01 00:00:00.000000 tox-poetry-installer-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-08-02 15:35:10.025059 tox_poetry_installer-1.0.0b1/LICENSE.md
+-rw-r--r--   0        0        0    22187 2023-08-02 15:35:10.209061 tox_poetry_installer-1.0.0b1/README.md
+-rw-r--r--   0        0        0     1909 2023-08-02 15:34:31.652817 tox_poetry_installer-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox_poetry_installer-1.0.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     1932 2023-08-02 15:08:54.718344 tox_poetry_installer-1.0.0b1/tests/fixtures.py
+-rw-r--r--   0        0        0     3292 2023-08-02 15:08:54.718344 tox_poetry_installer-1.0.0b1/tests/test_installer.py
+-rw-r--r--   0        0        0     1219 2022-05-31 03:01:10.435532 tox_poetry_installer-1.0.0b1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2731 2022-05-31 03:01:10.435532 tox_poetry_installer-1.0.0b1/tests/test_transients.py
+-rw-r--r--   0        0        0      357 2023-08-02 15:34:31.653818 tox_poetry_installer-1.0.0b1/tox_poetry_installer/__about__.py
+-rw-r--r--   0        0        0      202 2023-08-02 15:08:54.718344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/__init__.py
+-rw-r--r--   0        0        0     2330 2023-08-02 15:08:54.718344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/_poetry.py
+-rw-r--r--   0        0        0     1009 2022-09-07 19:44:43.594829 tox_poetry_installer-1.0.0b1/tox_poetry_installer/constants.py
+-rw-r--r--   0        0        0     1491 2022-05-31 03:01:10.435532 tox_poetry_installer-1.0.0b1/tox_poetry_installer/exceptions.py
+-rw-r--r--   0        0        0     5779 2023-08-02 15:08:54.719344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/hooks.py
+-rw-r--r--   0        0        0     3288 2023-08-02 15:08:54.719344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/installer.py
+-rw-r--r--   0        0        0      930 2023-08-02 15:08:54.719344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/logger.py
+-rw-r--r--   0        0        0        0 2022-05-31 03:01:10.435532 tox_poetry_installer-1.0.0b1/tox_poetry_installer/py.typed
+-rw-r--r--   0        0        0    11516 2023-08-02 15:08:54.719344 tox_poetry_installer-1.0.0b1/tox_poetry_installer/utilities.py
+-rw-r--r--   0        0        0    23841 1970-01-01 00:00:00.000000 tox_poetry_installer-1.0.0b1/PKG-INFO
```

### Comparing `tox-poetry-installer-0.9.0/LICENSE.md` & `tox_poetry_installer-1.0.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.9.0/README.md` & `tox_poetry_installer-1.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,53 +21,55 @@
   - [References](#references)
     - [Config Options](#configuration-options)
     - [Runtime Options](#runtime-options)
     - [Errors](#errors)
   - [Other Notes](#other-notes)
     - [Unsupported Tox config options](#unsupported-tox-config-options)
     - [Updating locked dependencies in a testenv](#updating-locked-dependencies-in-a-testenv)
-    - [Installing unsafe dependencies](#installing-unsafe-dependencies)
     - [Using with an unmanaged Poetry installation](#using-with-an-unmanaged-poetry-installation)
 - [Developing the Plugin](#developer-documentation)
 - [Road Map](#road-map)
 
 See the
 [Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for
 release history.
 
-*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*
+*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html) and
+[the official Poetry documentation on using Tox](https://python-poetry.org/docs/faq/#is-tox-supported)*
 
 ## Feature Overview
 
 - Manage package versions in exactly one place and with exactly one tool: Poetry.
 - Ensure CI/CD and other automation tools are using the same package versions that you are
   in your local development environment.
-- Add only the packages you need to a Tox test environment, instead of everything in your
-  lockfile.
-- Directly integrate with Poetry, re-using your existing package indexes and credentials
+- Add only the packages or custom groups you need to a Tox test environment, instead of
+  everything in your lockfile.
+- Directly integrate with Poetry, re-using your existing package indexes and credentials,
   with no additional configuration.
 - Wherever possible, built-in Tox config options are always respected and their behavior
   kept consistent.
 - Extremely configurable. Every feature can be disabled or enabled for any given Tox test
   environment.
 - Friendly to other Tox plugins and supports a wide range of environments.
 
 ## User Documentation
 
-*This section is for users looking to integrate the plugin with their project or CI system. For information on contributing to the plugin please see the [Developer Docs](#developer-documentation)*
+*This section is for users looking to integrate the plugin with their project or CI
+system. For information on contributing to the plugin please see the
+[Developer Docs](#developer-documentation)*
 
 ### Installing
 
 The recommended way to install the plugin is to add it to a project using Poetry:
 
 ```bash
-poetry add tox-poetry-installer[poetry] --dev
+poetry add -G dev tox-poetry-installer[poetry]
 ```
 
-> **Note:** Always install the plugin with the `[poetry]` extra, unless you are
+> ℹ️ **Note:** Always install the plugin with the `[poetry]` extra, unless you are
 > [managing the Poetry installation yourself](#externally-managed-poetry-installation).
 
 Alternatively, it can be installed directly to a virtual environment using Pip, though
 this is not recommended:
 
 ```bash
 source somevenv/bin/activate
@@ -76,24 +78,24 @@
 
 Alternatively alternatively, it can be installed using the Tox
 [`requires`](https://tox.readthedocs.io/en/latest/config.html#conf-requires) option by
 adding the below to `tox.ini`, though this is also not recommended:
 
 ```ini
 requires =
-    tox-poetry-installer[poetry] == 0.8.0
+    tox-poetry-installer[poetry] == 0.10.2
 ```
 
 After installing, check that Tox recognizes the plugin by running
 `poetry run tox --version`. The command should give output similar to below:
 
 ```
-3.20.0 imported from .venv/lib64/python3.8/site-packages/tox/__init__.py
+3.20.0 imported from .venv/lib64/python3.10/site-packages/tox/__init__.py
 registered plugins:
-    tox-poetry-installer-0.8.0 at .venv/lib64/python3.8/site-packages/tox_poetry_installer/__init__.py
+    tox-poetry-installer-0.10.2 at .venv/lib64/python3.10/site-packages/tox_poetry_installer/__init__.py
 ```
 
 ### Quick Start
 
 Congratulations! 🎉 Just by installing the plugin your Tox config is already using locked
 dependencies: when Tox builds and installs your project package to a test environment,
 your project package's dependencies will be installed from the lockfile.
@@ -142,31 +144,32 @@
 locked_deps =
     black
     pylint
     mypy
 commands = ...
 ```
 
-> **Note:** Settings configured on the main `testenv` environment are inherited by child
-> test environments (for example, `testenv:foo`). To override this, specify the setting in
-> the child environment with a different value.
+> ℹ️ **Note:** Settings configured on the main `testenv` environment are inherited by
+> child test environments (for example, `testenv:foo`). To override this, specify the
+> setting in the child environment with a different value.
 
 Alternatively, we can skip specifying all of our dependencies for a test environment in
-the Tox config and just install all of our Poetry dev-dependencies automatically:
+the Tox config and install Poetry dependency groups directly:
 
 ```ini
 [testenv]
 description = Some very cool tests
 require_locked_deps = true
-install_dev_deps = true
+poetry_dep_groups =
+    dev
 commands = ...
 ```
 
-> **Note:** Setting `install_dev_deps = true` on an environment that also installs the
-> project package is functionally equivalent to running `poetry install`.
+> ℹ️ **Note:** The `install_dev_deps` configuration option is deprecated. See
+> [Configuration Options](#configuration-options) for more information.
 
 Finally, we can also install an unlocked dependency (a dependency which doesn't take its
 version from the Poetry lockfile) into the test environment alongside the locked ones. We
 need to remove the `require_locked_deps = true` option, otherwise the environment will
 error, and then we can add the unlocked dependency using the built-in
 [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:
 
@@ -186,42 +189,35 @@
 
 ### Configuration Options
 
 All options listed below are Tox environment options and can be applied to one or more
 environment sections of the `tox.ini` file. They cannot be applied to the global Tox
 configuration section.
 
-> **Note:** Settings configured on the main `testenv` environment are inherited by child
-> test environments (for example, `testenv:foo`). To override this, specify the setting in
-> the child environment with a different value.
+> ℹ️ **Note:** Settings configured on the main `testenv` environment are inherited by
+> child test environments (for example, `testenv:foo`). To override this, specify the
+> setting in the child environment with a different value.
 
 | Option                 |  Type   | Default | Description                                                                                                                                                                                                                                                                                                                                                          |
 | :--------------------- | :-----: | :-----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `locked_deps`          |  List   |  `[]`   | Names of packages to install to the test environment from the Poetry lockfile. Transient dependencies (packages required by these dependencies) are automatically included.                                                                                                                                                                                          |
 | `require_locked_deps`  | Boolean |  False  | Whether the plugin should block attempts to install unlocked dependencies to the test environment. If enabled, then the [`tox_testenv_install_deps`](https://tox.readthedocs.io/en/latest/plugins.html#tox.hookspecs.tox_testenv_install_deps) plugin hook will be intercepted and an error will be raised if the test environment has the `deps` option configured. |
-| `install_dev_deps`     | Boolean |  False  | Whether all of the Poetry dev-dependencies should be installed to the test environment.                                                                                                                                                                                                                                                                              |
 | `install_project_deps` | Boolean |  True   | Whether all of the Poetry primary dependencies for the project package should be installed to the test environment.                                                                                                                                                                                                                                                  |
 | `require_poetry`       | Boolean |  False  | Whether Tox should be forced to fail if the plugin cannot import Poetry locally. If `False` then the plugin will be skipped for the test environment if Poetry cannot be imported. If `True` then the plugin will force the environment to error and the Tox run to fail.                                                                                            |
+| `poetry_dep_groups`    |  List   |  `[]`   | Names of Poetry dependency groups specified in `pyproject.toml` to install to the test environment.                                                                                                                                                                                                                                                                  |
 
 ### Runtime Options
 
 All arguments listed below can be passed to the `tox` command to modify runtime behavior
 of the plugin.
 
 | Argument                     |  Type   | Default | Description                                                                                                                                                                                                                                                                          |
 | :--------------------------- | :-----: | :-----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `--parallel-install-threads` | Integer |  `10`   | Number of worker threads to use to install dependencies in parallel. Installing in parallel with more threads can greatly speed up the install process, but can cause race conditions during install. Pass this option with the value `0` to entirely disable parallel installation. |
 
-> **Note:** The `--require-poetry` runtime option is deprecated and will be removed in
-> version 1.0.0. Please set `require_poetry = true` in `tox.ini` for environments that
-> should fail if Poetry is not available.
-
-> **Note:** The `--parallelize-locked-install` option is deprecated and will be removed in
-> version 1.0.0. Please use the `--parallel-install-threads` option.
-
 ### Errors
 
 There are several errors that the plugin can encounter for a test environment when Tox is
 run. If an error is encountered then the status of the test environment that caused the
 error will be set to one of the "Status" values below to indicate what the error was.
 
 | Status/Name                     | Cause                                                                                                                                                                                                                           |
@@ -229,29 +225,29 @@
 | `ExtraNotFoundError`            | Indicates that the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) config option specified an extra that is not configured by Poetry in `pyproject.toml`.                                              |
 | `LockedDepVersionConflictError` | Indicates that an item in the `locked_deps` config option includes a [PEP-508 version specifier](https://www.python.org/dev/peps/pep-0508/#grammar) (ex: `pytest >=6.0, <6.1`).                                                 |
 | `LockedDepNotFoundError`        | Indicates that an item specified in the `locked_deps` config option does not match the name of a package in the Poetry lockfile.                                                                                                |
 | `LockedDepsRequiredError`       | Indicates that a test environment with the `require_locked_deps` config option set to `true` also specified unlocked dependencies using the [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) config option. |
 | `PoetryNotInstalledError`       | Indicates that the `poetry` module could not be imported under the current runtime environment, and `require_poetry = true` was specified.                                                                                      |
 | `RequiresUnsafeDepError`        | Indicates that the package-under-test depends on a package that Poetry has classified as unsafe and cannot be installed.                                                                                                        |
 
-> **Note:** One or more of these errors can be caused by the `pyproject.toml` being out of
-> sync with the Poetry lockfile. If this is the case, than a warning will be logged when Tox
-> is run.
+> ℹ️ **Note:** One or more of these errors can be caused by the `pyproject.toml` being out
+> of sync with the Poetry lockfile. If this is the case, than a warning will be logged
+> when Tox is run.
 
 ### Other Notes
 
 #### Unsupported Tox config options
 
 Below are the built-in Tox config options that are not respected by this plugin. All of
 these options are made obsolete by the Poetry lockfile: either they aren't needed or their
 equivalent functionality is instead taken directly from the package details Poetry stores
 in its lockfile.
 
-> **Note:** The unsupported Tox config options will still apply to unlocked dependencies
-> being installed with the default Tox installation backend.
+> ℹ️ **Note:** The unsupported Tox config options will still apply to unlocked
+> dependencies being installed with the default Tox installation backend.
 
 - [`install_command`](https://tox.readthedocs.io/en/latest/config.html#conf-install_command)
 - [`pip_pre`](https://tox.readthedocs.io/en/latest/config.html#conf-pip_pre)
 - [`download`](https://tox.readthedocs.io/en/latest/config.html#conf-download)
 - [`indexserver`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)
 - [`usedevelop`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)
 
@@ -264,61 +260,44 @@
 
 However, the plugin cannot determine when the lockfile is updated. If a Tox test
 environment has already been created then it will need to be recreated (using Tox's
 built-in
 [`--recreate`](https://tox.readthedocs.io/en/latest/example/basic.html#forcing-re-creation-of-virtual-environments)
 option) for the new version to be found and installed.
 
-> **Note:** To force Tox to always recreate a test environment the
-> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config option
-> can be set.
-
-#### Installing unsafe dependencies
-
-There are several packages that cannot be installed from the lockfile because they are
-excluded by Poetry itself. As a result these packages cannot be installed by this plugin
-either as test environment dependencies passed directly to `locked_deps` or as a transient
-dependency. When one of these packages is encountered by the plugin a warning will be
-logged to the console and
-**the unsafe package will not be installed to the test environment**.
-
-This list can be found in the Poetry source code
-[here](https://github.com/python-poetry/poetry/blob/master/poetry/puzzle/provider.py). As
-of [Poetry 1.1.6](https://github.com/python-poetry/poetry/releases/tag/1.1.6) there are
-four packages classified as "unsafe" by Poetry and excluded from the lockfile:
-
-- `setuptools`
-- `distribute`
-- `pip`
-- `wheel`
+> ℹ️ **Note:** To force Tox to always recreate a test environment the
+> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config
+> option can be set.
 
 #### Using with an unmanaged Poetry installation
 
 In CI/CD systems, automation environments, or other Python environments where the loaded
 site packages are not managed by Poetry, it can be useful to manage the local installation
 of Poetry externally. This also helps to avoid problems that can be caused by the
-`--no-root`, `--no-dev`, or `--remove-untracked` arguments to the `poetry install` command
-which, in some situations, can cause Poetry to uninstall itself if Poetry is specified as
-a dependency of one of the packages it is managing (like this plugin). To support these
-use cases, this plugin specifies the `poetry` package as an optional dependency that can
-be installed using a setuptools extra also named `poetry`.
-
-**Critical Warning: This plugin requires Poetry to function. If the plugin is installed without the `poetry` setuptools extra then Poetry must be installed independently for the plugin to function properly.**
+`--no-root`, `--without dev`, or `--sync` arguments to the `poetry install` command which,
+in some situations, can cause Poetry to uninstall itself if Poetry is specified as a
+dependency of one of the packages it is managing (like this plugin). To support these use
+cases, this plugin specifies the `poetry` package as an optional dependency that can be
+installed using a setuptools extra also named `poetry`.
+
+> ⚠️ **Warning:** This plugin requires Poetry to function. If the plugin is installed
+> without the `poetry` setuptools extra then Poetry must be installed independently for
+> the plugin to function properly.
 
 To skip installing the `poetry` package as a dependency of `tox-poetry-installer`, do not
 specify the `poetry` extra when adding the plugin:
 
 ```bash
 # Adding the package without the "[poetry]" extra specifier so that
 # Poetry is not added as a transient dev-dependency:
-poetry add tox-poetry-installer --dev
+poetry add -G dev tox-poetry-installer
 
 # Adding the package with the "[poetry]" extra specifier, so the Poetry
 # package will be added to the environment and tracked in the lockfile:
-poetry add tox-poetry-installer[poetry] --dev
+poetry add -G dev tox-poetry-installer[poetry]
 ```
 
 Once the plugin is installed- either with or without the Poetry extra- you can validate
 that the plugin will run correctly with the following command. This command checks that
 all three required components (Tox, Poetry, and the plugin itself) are available in the
 current Python environment:
 
@@ -326,38 +305,39 @@
 python -c '\
   import tox;\
   import tox_poetry_installer;\
   from poetry.poetry import Poetry;\
 '
 ```
 
-> **Note:** To force Tox to fail if Poetry is not installed, add the `require_poetry = true`
-> option to the tox `[testenv]` configuration. See the
+> ℹ️ **Note:** To force Tox to fail if Poetry is not installed, add the
+> `require_poetry = true` option to the tox `[testenv]` configuration. See the
 > [Config Options](#configuration-options) for more information.
 
 ## Developer Documentation
 
 All project contributors and participants are expected to adhere to the
-[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
+[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md)
+([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
 
 The `devel` branch has the latest (and potentially unstable) changes. The stable releases
 are tracked on [Github](https://github.com/enpaul/tox-poetry-installer/releases),
 [PyPi](https://pypi.org/project/tox-poetry-installer/#history), and in the
 [Changelog](CHANGELOG.md).
 
 - To report a bug, request a feature, or ask for assistance, please
   [open an issue on the Github repository](https://github.com/enpaul/tox-poetry-installer/issues/new).
 - To report a security concern or code of conduct violation, please contact the project
   author directly at **‌me \[at‌\] enp dot‎ ‌one**.
 - To submit an update, please
   [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
   and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).
 
-Developing this project requires [Python 3.7+](https://www.python.org/downloads/) and
-[Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can
+Developing this project requires [Python 3.10+](https://www.python.org/downloads/) and
+[Poetry 1.4](https://python-poetry.org/docs/#installation) or later. GNU Make can
 optionally be used to quickly setup a local development environment, but this is not
 required.
 
 To setup a local development environment:
 
 ```bash
 # Clone the repository...
@@ -374,51 +354,56 @@
 # Run tests and CI locally
 make test
 
 # See additional make targets
 make help
 ```
 
-> **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To
-> make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,
-> alternatively, [launch an environment shell](https://python-poetry.org/docs/cli/#shell).
+> ℹ️ **Note:** The pre-commit hooks require dependencies in the Poetry environment to run.
+> To make a commit with the pre-commit hooks, you will need to run `poetry run git commit`
+> or, alternatively,
+> [launch an environment shell](https://python-poetry.org/docs/cli/#shell).
 
 ## Road Map
 
 This project is under active development and is classified as beta software, ready for
 production environments on a provisional basis only.
 
 - Beta classification was assigned with
   [v0.6.0](https://github.com/enpaul/tox-poetry-installer/releases/tag/0.6.0)
-- Stable classification will be assigned when the test suite covers an acceptable number of
-  use cases
+- Stable classification will be assigned when the test suite covers an acceptable number
+  of use cases
 
 ### Path to Beta
 
 - [x] Verify that primary package dependencies (from the `.package` env) are installed
   correctly using the Poetry backend.
-- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) Tox
-  configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))
+- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras)
+  Tox configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))
 - [x] Add per-environment Tox configuration option to fall back to default installation
   backend.
-- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using the
-  Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))
-- [x] Add trivial tests to ensure the project metadata is consistent between the pyproject.toml
-  and the module constants.
-- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and improve
-  robustness of the Tox and Poetry module imports to avoid potentially breaking API changes
-  in upstream packages. ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
+- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using
+  the Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))
+- [x] Add trivial tests to ensure the project metadata is consistent between the
+  pyproject.toml and the module constants.
+- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and
+  improve robustness of the Tox and Poetry module imports to avoid potentially breaking
+  API changes in upstream packages.
+  ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
 - [ ] ~Find and implement a way to mitigate the
   [UNSAFE_DEPENDENCIES issue](https://github.com/python-poetry/poetry/issues/1584) in
   Poetry.~ ([#6](https://github.com/enpaul/tox-poetry-installer/issues/6))
-- [x] Fix logging to make proper use of Tox's logging reporter infrastructure ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))
-- [x] Add configuration option for installing all dev-dependencies to a testenv ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))
+- [x] Fix logging to make proper use of Tox's logging reporter infrastructure
+  ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))
+- [x] Add configuration option for installing all dev-dependencies to a testenv
+  ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))
 
 ### Path to Stable
 
 Everything in Beta plus...
 
-- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core` ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
+- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core`
+  ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
 - [x] Add comprehensive unit tests
 - [ ] ~Add tests for each feature version of Tox between 3.8 and 3.20~
 - [x] Add tests for Python-3.6, 3.7, 3.8, and 3.9
 - [x] Add Github Actions based CI
```

### Comparing `tox-poetry-installer-0.9.0/pyproject.toml` & `tox_poetry_installer-1.0.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tox-poetry-installer"
-version = "0.9.0"
+version = "1.0.0b1"
 license = "MIT"
 authors = ["Ethan Paul <24588726+enpaul@users.noreply.github.com>"]
 description = "A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile"
 repository = "https://github.com/enpaul/tox-poetry-installer/"
 packages = [
   {include = "tox_poetry_installer"},
   {include = "tests/*.py", format = "sdist"}
@@ -23,45 +23,46 @@
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.plugins.tox]
 poetry_installer = "tox_poetry_installer"
 
 [tool.poetry.extras]
 poetry = ["poetry", "cleo"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cleo = {version = "^1.0.0a5", optional = true, allow-prereleases = true}
-poetry = {version = "^1.2.0", optional = true}
+cleo = {version = ">=1.0,<3.0", optional = true}
+poetry = {version = "^1.5.0", optional = true}
 poetry-core = "^1.1.0"
-tox = "^3.8.0"
+tox = "^4"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.6.2"
 black = "^22.3.0"
 blacken-docs = "^1.8.0"
-ipython = "^7.18.1"
-mdformat = "^0.6"
-mdformat-gfm = "^0.2"
+ipython = {version = "^8.10.1", python = "^3.8"}
+mdformat = "^0.7"
+mdformat-gfm = "^0.3"
 mypy = "^0.930"
 pre-commit = "^2.7.1"
 pre-commit-hooks = "^3.3.0"
 pylint = "^2.13.0"
 pytest = "^6.0.2"
 pytest-cov = "^2.10.1"
 reorder-python-imports = "^2.3.5"
-safety = "^1.9.0"
+safety = "^2.2.0"
 toml = "^0.10.1"
-tox = "^3.20.0"
+tox = "^4"
 types-toml = "^0.10.1"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tox-poetry-installer-0.9.0/tests/fixtures.py` & `tox_poetry_installer-1.0.0b1/tests/fixtures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 # pylint: disable=missing-module-docstring, missing-function-docstring, unused-argument, too-few-public-methods
 import time
 from pathlib import Path
+from typing import List
 
 import poetry.factory
-import poetry.installation.pip_installer
+import poetry.installation.executor
 import poetry.utils.env
 import pytest
-import tox
-from poetry.core.packages.package import Package as PoetryPackage
+import tox.tox_env.python.virtual_env.runner
+from poetry.installation.operations.operation import Operation
 
 from tox_poetry_installer import utilities
 
 
 TEST_PROJECT_PATH = Path(__file__).parent.resolve() / "test-project"
 
 FAKE_VENV_PATH = Path("nowhere")
 
 
 class MockVirtualEnv:
     """Mock class for the :class:`poetry.utils.env.VirtualEnv` and :class:`tox.venv.VirtualEnv`"""
 
-    class MockTestenvConfig:  # pylint: disable=missing-class-docstring
-        envdir = FAKE_VENV_PATH
-
     def __init__(self, *args, **kwargs):
-        self.envconfig = self.MockTestenvConfig()
+        self.env_dir = FAKE_VENV_PATH
         self.installed = []
 
     @staticmethod
     def is_valid_for_marker(*args, **kwargs):
         return True
 
     @staticmethod
     def get_version_info():
         return (1, 2, 3)
 
 
-class MockPipInstaller:
-    """Mock class for the :class:`poetry.installation.pip_installer.PipInstaller`"""
+class MockExecutor:
+    """Mock class for the :class:`poetry.installation.executor.Executor`"""
 
     def __init__(self, env: MockVirtualEnv, **kwargs):
         self.env = env
 
-    def install(self, package: PoetryPackage):
-        self.env.installed.append(package)
+    def execute(self, operations: List[Operation]):
+        self.env.installed.extend([operation.package for operation in operations])
         time.sleep(1)
 
 
 @pytest.fixture
 def mock_venv(monkeypatch):
     monkeypatch.setattr(utilities, "convert_virtualenv", lambda venv: venv)
+    monkeypatch.setattr(poetry.installation.executor, "Executor", MockExecutor)
     monkeypatch.setattr(
-        poetry.installation.pip_installer, "PipInstaller", MockPipInstaller
+        tox.tox_env.python.virtual_env.runner, "VirtualEnvRunner", MockVirtualEnv
     )
-    monkeypatch.setattr(tox.venv, "VirtualEnv", MockVirtualEnv)
     monkeypatch.setattr(poetry.utils.env, "VirtualEnv", MockVirtualEnv)
 
 
 @pytest.fixture(scope="function")
 def mock_poetry_factory(monkeypatch):
     pypoetry = poetry.factory.Factory().create_poetry(cwd=TEST_PROJECT_PATH)
```

### Comparing `tox-poetry-installer-0.9.0/tests/test_metadata.py` & `tox_poetry_installer-1.0.0b1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.9.0/tests/test_transients.py` & `tox_poetry_installer-1.0.0b1/tests/test_transients.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/_poetry.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/_poetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 import sys
 
 from tox_poetry_installer import exceptions
 
 
 try:
     from cleo.io.null_io import NullIO
+    from poetry.config.config import Config
+    from poetry.core.packages.dependency import Dependency as PoetryDependency
+    from poetry.core.packages.package import Package as PoetryPackage
     from poetry.factory import Factory
-    from poetry.installation.pip_installer import PipInstaller
+    from poetry.installation.executor import Executor
+    from poetry.installation.operations.install import Install
     from poetry.poetry import Poetry
     from poetry.utils.env import VirtualEnv
 except ImportError:
     raise exceptions.PoetryNotInstalledError(
         f"No version of Poetry could be imported under the current environment for '{sys.executable}'"
     ) from None
```

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/constants.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/constants.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/exceptions.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/exceptions.py`

 * *Files identical despite different names*

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/installer.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/installer.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,56 +5,54 @@
 import concurrent.futures
 import contextlib
 import typing
 from datetime import datetime
 from typing import Collection
 from typing import Set
 
-from poetry.core.packages.package import Package as PoetryPackage
-from tox.venv import VirtualEnv as ToxVirtualEnv
+from tox.tox_env.api import ToxEnv as ToxVirtualEnv
 
 from tox_poetry_installer import logger
 from tox_poetry_installer import utilities
 
 if typing.TYPE_CHECKING:
     from tox_poetry_installer import _poetry
 
 
 def install(
     poetry: "_poetry.Poetry",
     venv: ToxVirtualEnv,
-    packages: Collection[PoetryPackage],
+    packages: Collection["_poetry.PoetryPackage"],
     parallels: int = 0,
 ):
     """Install a bunch of packages to a virtualenv
 
     :param poetry: Poetry object the packages were sourced from
     :param venv: Tox virtual environment to install the packages to
     :param packages: List of packages to install to the virtual environment
     :param parallels: Number of parallel processes to use for installing dependency packages, or
                       ``None`` to disable parallelization.
     """
     from tox_poetry_installer import _poetry
 
-    logger.info(
-        f"Installing {len(packages)} packages to environment at {venv.envconfig.envdir}"
-    )
+    logger.info(f"Installing {len(packages)} packages to environment at {venv.env_dir}")
 
-    pip = _poetry.PipInstaller(
+    install_executor = _poetry.Executor(
         env=utilities.convert_virtualenv(venv),
         io=_poetry.NullIO(),
         pool=poetry.pool,
+        config=_poetry.Config(),
     )
 
-    installed: Set[PoetryPackage] = set()
+    installed: Set[_poetry.PoetryPackage] = set()
 
-    def logged_install(dependency: PoetryPackage) -> None:
+    def logged_install(dependency: _poetry.PoetryPackage) -> None:
         start = datetime.now()
         logger.debug(f"Installing {dependency}")
-        pip.install(dependency)
+        install_executor.execute([_poetry.Install(package=dependency)])
         end = datetime.now()
         logger.debug(f"Finished installing {dependency} in {end - start}")
 
     @contextlib.contextmanager
     def _optional_parallelize():
         """A bit of cheat, really
 
@@ -67,15 +65,24 @@
                 max_workers=parallels
             ) as executor:
                 yield executor.submit
         else:
             yield lambda func, arg: func(arg)
 
     with _optional_parallelize() as executor:
+        futures = []
         for dependency in packages:
             if dependency not in installed:
                 installed.add(dependency)
                 logger.debug(f"Queuing {dependency}")
-                executor(logged_install, dependency)
+                future = executor(logged_install, dependency)
+                if future is not None:
+                    futures.append(future)
             else:
                 logger.debug(f"Skipping {dependency}, already installed")
         logger.debug("Waiting for installs to finish...")
+
+        for future in concurrent.futures.as_completed(futures):
+            # Don't actually care about the return value, just waiting on the
+            # future to ensure any exceptions that were raised in the called
+            # function are propagated.
+            future.result()
```

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/logger.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Logging wrappers to reduce duplication elsewhere
 
 Calling ``tox.reporter.something()`` and having to format a string with the prefix
 gets really old fast, but more importantly it also makes the flow of the main code
 more difficult to follow because of the added complexity.
 """
-import tox
+import logging
 
 from tox_poetry_installer import constants
 
 
 def error(message: str):
-    """Wrapper around :func:`tox.reporter.error`"""
-    tox.reporter.error(f"{constants.REPORTER_PREFIX} {message}")
+    """Wrapper around :func:`logging.error` that prefixes the reporter prefix onto the message"""
+    logging.error(f"{constants.REPORTER_PREFIX} {message}")
 
 
 def warning(message: str):
-    """Wrapper around :func:`tox.reporter.warning`"""
-    tox.reporter.warning(f"{constants.REPORTER_PREFIX} {message}")
+    """Wrapper around :func:`logging.warning`"""
+    logging.warning(f"{constants.REPORTER_PREFIX} {message}")
 
 
 def info(message: str):
-    """Wrapper around :func:`tox.reporter.verbosity1`"""
-    tox.reporter.verbosity1(f"{constants.REPORTER_PREFIX} {message}")
+    """Wrapper around :func:`logging.info`"""
+    logging.info(f"{constants.REPORTER_PREFIX} {message}")
 
 
 def debug(message: str):
-    """Wrapper around :func:`tox.reporter.verbosity2`"""
-    tox.reporter.verbosity2(f"{constants.REPORTER_PREFIX} {message}")
+    """Wrapper around :func:`logging.debug`"""
+    logging.debug(f"{constants.REPORTER_PREFIX} {message}")
```

### Comparing `tox-poetry-installer-0.9.0/tox_poetry_installer/utilities.py` & `tox_poetry_installer-1.0.0b1/tox_poetry_installer/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,65 +8,50 @@
 from typing import Dict
 from typing import List
 from typing import Sequence
 from typing import Set
 
 from poetry.core.packages.dependency import Dependency as PoetryDependency
 from poetry.core.packages.package import Package as PoetryPackage
-from tox.action import Action as ToxAction
-from tox.venv import VirtualEnv as ToxVirtualEnv
+from tox.tox_env.api import ToxEnv as ToxVirtualEnv
+from tox.tox_env.package import PackageToxEnv
 
 from tox_poetry_installer import constants
 from tox_poetry_installer import exceptions
 from tox_poetry_installer import logger
 
 if typing.TYPE_CHECKING:
     from tox_poetry_installer import _poetry
 
 
 PackageMap = Dict[str, List[PoetryPackage]]
 
 
-def check_preconditions(venv: ToxVirtualEnv, action: ToxAction) -> "_poetry.Poetry":
+def check_preconditions(venv: ToxVirtualEnv) -> "_poetry.Poetry":
     """Check that the local project environment meets expectations"""
+
     # Skip running the plugin for the provisioning environment. The provisioned environment,
     # for alternative Tox versions and/or the ``requires`` meta dependencies is specially
     # handled by Tox and is out of scope for this plugin. Since one of the ways to install this
     # plugin in the first place is via the Tox provisioning environment, it quickly becomes a
     # chicken-and-egg problem.
-    if action.name == venv.envconfig.config.provision_tox_env:
-        raise exceptions.SkipEnvironment(
-            f"Skipping Tox provisioning env '{action.name}'"
-        )
+    if isinstance(venv, PackageToxEnv):
+        raise exceptions.SkipEnvironment(f"Skipping Tox provisioning env '{venv.name}'")
 
-    # Skip running the plugin for the packaging environment. PEP-517 front ends can handle
-    # that better than we can, so let them do their thing. More to the point: if you're having
-    # problems in the packaging env that this plugin would solve, god help you.
-    if action.name == venv.envconfig.config.isolated_build_env:
-        raise exceptions.SkipEnvironment(
-            f"Skipping isolated packaging build env '{action.name}'"
-        )
-
-    if venv.envconfig.config.option.require_poetry:
+    if venv.options.require_poetry:
         logger.warning(
             "DEPRECATION: The '--require-poetry' runtime option is deprecated and will be "
             "removed in version 1.0.0. Please update test environments that require Poetry to "
             "set the 'require_poetry = true' option in tox.ini"
         )
 
-    if venv.envconfig.config.option.parallelize_locked_install is not None:
-        logger.warning(
-            "DEPRECATION: The '--parallelize-locked-install' option is deprecated and will "
-            "be removed in version 1.0.0. Please use the '--parallel-install-threads' option."
-        )
-
     from tox_poetry_installer import _poetry
 
     try:
-        return _poetry.Factory().create_poetry(venv.envconfig.config.toxinidir)
+        return _poetry.Factory().create_poetry(venv.core["tox_root"])
     # Support running the plugin when the current tox project does not use Poetry for its
     # environment/dependency management.
     #
     # ``RuntimeError`` is dangerous to blindly catch because it can be (and in Poetry's case,
     # is) raised in many different places for different purposes.
     except RuntimeError:
         raise exceptions.SkipEnvironment(
@@ -78,15 +63,15 @@
     """Convert a Tox venv to a Poetry venv
 
     :param venv: Tox ``VirtualEnv`` object representing a tox virtual environment
     :returns: Poetry ``VirtualEnv`` object representing a poetry virtual environment
     """
     from tox_poetry_installer import _poetry
 
-    return _poetry.VirtualEnv(path=Path(venv.envconfig.envdir))
+    return _poetry.VirtualEnv(path=Path(venv.env_dir))
 
 
 def build_package_map(poetry: "_poetry.Poetry") -> PackageMap:
     """Build the mapping of package names to objects
 
     :param poetry: Populated poetry object to load locked packages from
     :returns: Mapping of package names to Poetry package objects
@@ -242,36 +227,54 @@
         dependencies += identify_transients(
             dep_name.lower(), packages, venv, allow_missing=[poetry.package.name]
         )
 
     return dedupe_packages(dependencies)
 
 
-def find_dev_deps(
-    packages: PackageMap, venv: "_poetry.VirtualEnv", poetry: "_poetry.Poetry"
+def find_group_deps(
+    group: str,
+    packages: PackageMap,
+    venv: "_poetry.VirtualEnv",
+    poetry: "_poetry.Poetry",
 ) -> List[PoetryPackage]:
-    """Find the dev dependencies
+    """Find the dependencies belonging to a dependency group
 
     Recursively identify the Poetry dev dependencies
 
+    :param group: Name of the dependency group from the project's ``pyproject.toml``
     :param packages: Mapping of all locked package names to their corresponding package object
     :param venv: Poetry virtual environment to use for package compatibility checks
     :param poetry: Poetry object for the current project
     """
-    dev_group_deps = find_additional_deps(
+    return find_additional_deps(
         packages,
         venv,
         poetry,
         poetry.pyproject.data["tool"]["poetry"]
         .get("group", {})
-        .get("dev", {})
+        .get(group, {})
         .get("dependencies", {})
         .keys(),
     )
 
+
+def find_dev_deps(
+    packages: PackageMap, venv: "_poetry.VirtualEnv", poetry: "_poetry.Poetry"
+) -> List[PoetryPackage]:
+    """Find the dev dependencies
+
+    Recursively identify the Poetry dev dependencies
+
+    :param packages: Mapping of all locked package names to their corresponding package object
+    :param venv: Poetry virtual environment to use for package compatibility checks
+    :param poetry: Poetry object for the current project
+    """
+    dev_group_deps = find_group_deps("dev", packages, venv, poetry)
+
     # Legacy pyproject.toml poetry format:
     legacy_dev_group_deps = find_additional_deps(
         packages,
         venv,
         poetry,
         poetry.pyproject.data["tool"]["poetry"].get("dev-dependencies", {}).keys(),
     )
```

### Comparing `tox-poetry-installer-0.9.0/setup.py` & `tox_poetry_installer-1.0.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,448 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tox-poetry-installer
+Version: 1.0.0b1
+Summary: A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile
+Home-page: https://github.com/enpaul/tox-poetry-installer/
+License: MIT
+Keywords: tox,poetry,plugin
+Author: Ethan Paul
+Author-email: 24588726+enpaul@users.noreply.github.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Framework :: tox
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Provides-Extra: poetry
+Requires-Dist: cleo (>=1.0,<3.0) ; extra == "poetry"
+Requires-Dist: poetry (>=1.5.0,<2.0.0) ; extra == "poetry"
+Requires-Dist: poetry-core (>=1.1.0,<2.0.0)
+Requires-Dist: tox (>=4,<5)
+Project-URL: Repository, https://github.com/enpaul/tox-poetry-installer/
+Description-Content-Type: text/markdown
 
-packages = \
-['tests', 'tests.test-project.test_project', 'tox_poetry_installer']
+# tox-poetry-installer
 
-package_data = \
-{'': ['*'], 'tests': ['test-project/*']}
+A plugin for [Tox](https://tox.readthedocs.io/en/latest/) that lets you install test
+environment dependencies from the [Poetry](https://python-poetry.org/) lockfile.
 
-install_requires = \
-['poetry-core>=1.1.0,<2.0.0', 'tox>=3.8.0,<4.0.0']
-
-extras_require = \
-{'poetry': ['cleo>=1.0.0a5,<2.0.0', 'poetry>=1.2.0,<2.0.0']}
-
-entry_points = \
-{'tox': ['poetry_installer = tox_poetry_installer']}
-
-setup_kwargs = {
-    'name': 'tox-poetry-installer',
-    'version': '0.9.0',
-    'description': 'A plugin for Tox that lets you install test environment dependencies from the Poetry lockfile',
-    'long_description': '# tox-poetry-installer\n\nA plugin for [Tox](https://tox.readthedocs.io/en/latest/) that lets you install test\nenvironment dependencies from the [Poetry](https://python-poetry.org/) lockfile.\n\n[![CI Status](https://github.com/enpaul/tox-poetry-installer/workflows/CI/badge.svg?event=push)](https://github.com/enpaul/tox-poetry-installer/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/tox-poetry-installer)](https://pypi.org/project/tox-poetry-installer/)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/tox-poetry-installer)](https://libraries.io/pypi/tox-poetry-installer)\n[![License](https://img.shields.io/pypi/l/tox-poetry-installer)](https://opensource.org/licenses/MIT)\n[![Python Supported Versions](https://img.shields.io/pypi/pyversions/tox-poetry-installer)](https://www.python.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n⚠️ **This project is beta software and is under active development** ⚠️\n\n## Documentation\n\n- [Feature Overview](#feature-overview)\n- [Using the Plugin](#user-documentation)\n  - [Installing](#installing)\n  - [Quick Start](#quick-start)\n  - [References](#references)\n    - [Config Options](#configuration-options)\n    - [Runtime Options](#runtime-options)\n    - [Errors](#errors)\n  - [Other Notes](#other-notes)\n    - [Unsupported Tox config options](#unsupported-tox-config-options)\n    - [Updating locked dependencies in a testenv](#updating-locked-dependencies-in-a-testenv)\n    - [Installing unsafe dependencies](#installing-unsafe-dependencies)\n    - [Using with an unmanaged Poetry installation](#using-with-an-unmanaged-poetry-installation)\n- [Developing the Plugin](#developer-documentation)\n- [Road Map](#road-map)\n\nSee the\n[Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for\nrelease history.\n\n*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html), [Poetry Tox plugin](https://github.com/tkukushkin/tox-poetry)*\n\n## Feature Overview\n\n- Manage package versions in exactly one place and with exactly one tool: Poetry.\n- Ensure CI/CD and other automation tools are using the same package versions that you are\n  in your local development environment.\n- Add only the packages you need to a Tox test environment, instead of everything in your\n  lockfile.\n- Directly integrate with Poetry, re-using your existing package indexes and credentials\n  with no additional configuration.\n- Wherever possible, built-in Tox config options are always respected and their behavior\n  kept consistent.\n- Extremely configurable. Every feature can be disabled or enabled for any given Tox test\n  environment.\n- Friendly to other Tox plugins and supports a wide range of environments.\n\n## User Documentation\n\n*This section is for users looking to integrate the plugin with their project or CI system. For information on contributing to the plugin please see the [Developer Docs](#developer-documentation)*\n\n### Installing\n\nThe recommended way to install the plugin is to add it to a project using Poetry:\n\n```bash\npoetry add tox-poetry-installer[poetry] --dev\n```\n\n> **Note:** Always install the plugin with the `[poetry]` extra, unless you are\n> [managing the Poetry installation yourself](#externally-managed-poetry-installation).\n\nAlternatively, it can be installed directly to a virtual environment using Pip, though\nthis is not recommended:\n\n```bash\nsource somevenv/bin/activate\npip install tox-poetry-installer\n```\n\nAlternatively alternatively, it can be installed using the Tox\n[`requires`](https://tox.readthedocs.io/en/latest/config.html#conf-requires) option by\nadding the below to `tox.ini`, though this is also not recommended:\n\n```ini\nrequires =\n    tox-poetry-installer[poetry] == 0.8.0\n```\n\nAfter installing, check that Tox recognizes the plugin by running\n`poetry run tox --version`. The command should give output similar to below:\n\n```\n3.20.0 imported from .venv/lib64/python3.8/site-packages/tox/__init__.py\nregistered plugins:\n    tox-poetry-installer-0.8.0 at .venv/lib64/python3.8/site-packages/tox_poetry_installer/__init__.py\n```\n\n### Quick Start\n\nCongratulations! 🎉 Just by installing the plugin your Tox config is already using locked\ndependencies: when Tox builds and installs your project package to a test environment,\nyour project package\'s dependencies will be installed from the lockfile.\n\nNow lets update an example `tox.ini` to install the other test environment dependencies\nfrom the lockfile.\n\nA `testenv` from the example `tox.ini` we\'re starting with is below:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    black == 20.8b1\n    pylint >=2.4.4,<2.7.0\n    mypy <0.800\ncommands = ...\n```\n\nTo update the config so that the testenv dependencies are installed from the lockfile, we\ncan replace the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option with the\n`locked_deps` option provided by the plugin, and then remove the inline version\nspecifiers. With these changes the three testenv dependencies (as well as all of their\ndependencies) will be installed from the lockfile when the test environment is recreated:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\nWe can also add the `require_locked_deps` option to the test environment. This will both\nblock any other install tools (another plugin or Tox itself) from installing dependencies\nto the Tox environment and also cause Tox to fail if the test environment also uses the\nbuilt-in [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\nAlternatively, we can skip specifying all of our dependencies for a test environment in\nthe Tox config and just install all of our Poetry dev-dependencies automatically:\n\n```ini\n[testenv]\ndescription = Some very cool tests\nrequire_locked_deps = true\ninstall_dev_deps = true\ncommands = ...\n```\n\n> **Note:** Setting `install_dev_deps = true` on an environment that also installs the\n> project package is functionally equivalent to running `poetry install`.\n\nFinally, we can also install an unlocked dependency (a dependency which doesn\'t take its\nversion from the Poetry lockfile) into the test environment alongside the locked ones. We\nneed to remove the `require_locked_deps = true` option, otherwise the environment will\nerror, and then we can add the unlocked dependency using the built-in\n[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:\n\n```ini\n[testenv]\ndescription = Some very cool tests\ndeps =\n    pytest >= 5.6.0,<6.0.0\nlocked_deps =\n    black\n    pylint\n    mypy\ncommands = ...\n```\n\n## References\n\n### Configuration Options\n\nAll options listed below are Tox environment options and can be applied to one or more\nenvironment sections of the `tox.ini` file. They cannot be applied to the global Tox\nconfiguration section.\n\n> **Note:** Settings configured on the main `testenv` environment are inherited by child\n> test environments (for example, `testenv:foo`). To override this, specify the setting in\n> the child environment with a different value.\n\n| Option                 |  Type   | Default | Description                                                                                                                                                                                                                                                                                                                                                          |\n| :--------------------- | :-----: | :-----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `locked_deps`          |  List   |  `[]`   | Names of packages to install to the test environment from the Poetry lockfile. Transient dependencies (packages required by these dependencies) are automatically included.                                                                                                                                                                                          |\n| `require_locked_deps`  | Boolean |  False  | Whether the plugin should block attempts to install unlocked dependencies to the test environment. If enabled, then the [`tox_testenv_install_deps`](https://tox.readthedocs.io/en/latest/plugins.html#tox.hookspecs.tox_testenv_install_deps) plugin hook will be intercepted and an error will be raised if the test environment has the `deps` option configured. |\n| `install_dev_deps`     | Boolean |  False  | Whether all of the Poetry dev-dependencies should be installed to the test environment.                                                                                                                                                                                                                                                                              |\n| `install_project_deps` | Boolean |  True   | Whether all of the Poetry primary dependencies for the project package should be installed to the test environment.                                                                                                                                                                                                                                                  |\n| `require_poetry`       | Boolean |  False  | Whether Tox should be forced to fail if the plugin cannot import Poetry locally. If `False` then the plugin will be skipped for the test environment if Poetry cannot be imported. If `True` then the plugin will force the environment to error and the Tox run to fail.                                                                                            |\n\n### Runtime Options\n\nAll arguments listed below can be passed to the `tox` command to modify runtime behavior\nof the plugin.\n\n| Argument                     |  Type   | Default | Description                                                                                                                                                                                                                                                                          |\n| :--------------------------- | :-----: | :-----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `--parallel-install-threads` | Integer |  `10`   | Number of worker threads to use to install dependencies in parallel. Installing in parallel with more threads can greatly speed up the install process, but can cause race conditions during install. Pass this option with the value `0` to entirely disable parallel installation. |\n\n> **Note:** The `--require-poetry` runtime option is deprecated and will be removed in\n> version 1.0.0. Please set `require_poetry = true` in `tox.ini` for environments that\n> should fail if Poetry is not available.\n\n> **Note:** The `--parallelize-locked-install` option is deprecated and will be removed in\n> version 1.0.0. Please use the `--parallel-install-threads` option.\n\n### Errors\n\nThere are several errors that the plugin can encounter for a test environment when Tox is\nrun. If an error is encountered then the status of the test environment that caused the\nerror will be set to one of the "Status" values below to indicate what the error was.\n\n| Status/Name                     | Cause                                                                                                                                                                                                                           |\n| :------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |\n| `ExtraNotFoundError`            | Indicates that the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) config option specified an extra that is not configured by Poetry in `pyproject.toml`.                                              |\n| `LockedDepVersionConflictError` | Indicates that an item in the `locked_deps` config option includes a [PEP-508 version specifier](https://www.python.org/dev/peps/pep-0508/#grammar) (ex: `pytest >=6.0, <6.1`).                                                 |\n| `LockedDepNotFoundError`        | Indicates that an item specified in the `locked_deps` config option does not match the name of a package in the Poetry lockfile.                                                                                                |\n| `LockedDepsRequiredError`       | Indicates that a test environment with the `require_locked_deps` config option set to `true` also specified unlocked dependencies using the [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) config option. |\n| `PoetryNotInstalledError`       | Indicates that the `poetry` module could not be imported under the current runtime environment, and `require_poetry = true` was specified.                                                                                      |\n| `RequiresUnsafeDepError`        | Indicates that the package-under-test depends on a package that Poetry has classified as unsafe and cannot be installed.                                                                                                        |\n\n> **Note:** One or more of these errors can be caused by the `pyproject.toml` being out of\n> sync with the Poetry lockfile. If this is the case, than a warning will be logged when Tox\n> is run.\n\n### Other Notes\n\n#### Unsupported Tox config options\n\nBelow are the built-in Tox config options that are not respected by this plugin. All of\nthese options are made obsolete by the Poetry lockfile: either they aren\'t needed or their\nequivalent functionality is instead taken directly from the package details Poetry stores\nin its lockfile.\n\n> **Note:** The unsupported Tox config options will still apply to unlocked dependencies\n> being installed with the default Tox installation backend.\n\n- [`install_command`](https://tox.readthedocs.io/en/latest/config.html#conf-install_command)\n- [`pip_pre`](https://tox.readthedocs.io/en/latest/config.html#conf-pip_pre)\n- [`download`](https://tox.readthedocs.io/en/latest/config.html#conf-download)\n- [`indexserver`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n- [`usedevelop`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)\n\n#### Updating locked dependencies in a testenv\n\nWhen Poetry updates the version of a package in the lockfile (using either `poetry lock`\nor `poetry update`) then the plugin will automatically use this new version to install the\npackage to a test environment; there is no need to manually update `tox.ini` after\nupdating the Poetry lockfile.\n\nHowever, the plugin cannot determine when the lockfile is updated. If a Tox test\nenvironment has already been created then it will need to be recreated (using Tox\'s\nbuilt-in\n[`--recreate`](https://tox.readthedocs.io/en/latest/example/basic.html#forcing-re-creation-of-virtual-environments)\noption) for the new version to be found and installed.\n\n> **Note:** To force Tox to always recreate a test environment the\n> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config option\n> can be set.\n\n#### Installing unsafe dependencies\n\nThere are several packages that cannot be installed from the lockfile because they are\nexcluded by Poetry itself. As a result these packages cannot be installed by this plugin\neither as test environment dependencies passed directly to `locked_deps` or as a transient\ndependency. When one of these packages is encountered by the plugin a warning will be\nlogged to the console and\n**the unsafe package will not be installed to the test environment**.\n\nThis list can be found in the Poetry source code\n[here](https://github.com/python-poetry/poetry/blob/master/poetry/puzzle/provider.py). As\nof [Poetry 1.1.6](https://github.com/python-poetry/poetry/releases/tag/1.1.6) there are\nfour packages classified as "unsafe" by Poetry and excluded from the lockfile:\n\n- `setuptools`\n- `distribute`\n- `pip`\n- `wheel`\n\n#### Using with an unmanaged Poetry installation\n\nIn CI/CD systems, automation environments, or other Python environments where the loaded\nsite packages are not managed by Poetry, it can be useful to manage the local installation\nof Poetry externally. This also helps to avoid problems that can be caused by the\n`--no-root`, `--no-dev`, or `--remove-untracked` arguments to the `poetry install` command\nwhich, in some situations, can cause Poetry to uninstall itself if Poetry is specified as\na dependency of one of the packages it is managing (like this plugin). To support these\nuse cases, this plugin specifies the `poetry` package as an optional dependency that can\nbe installed using a setuptools extra also named `poetry`.\n\n**Critical Warning: This plugin requires Poetry to function. If the plugin is installed without the `poetry` setuptools extra then Poetry must be installed independently for the plugin to function properly.**\n\nTo skip installing the `poetry` package as a dependency of `tox-poetry-installer`, do not\nspecify the `poetry` extra when adding the plugin:\n\n```bash\n# Adding the package without the "[poetry]" extra specifier so that\n# Poetry is not added as a transient dev-dependency:\npoetry add tox-poetry-installer --dev\n\n# Adding the package with the "[poetry]" extra specifier, so the Poetry\n# package will be added to the environment and tracked in the lockfile:\npoetry add tox-poetry-installer[poetry] --dev\n```\n\nOnce the plugin is installed- either with or without the Poetry extra- you can validate\nthat the plugin will run correctly with the following command. This command checks that\nall three required components (Tox, Poetry, and the plugin itself) are available in the\ncurrent Python environment:\n\n```bash\npython -c \'\\\n  import tox;\\\n  import tox_poetry_installer;\\\n  from poetry.poetry import Poetry;\\\n\'\n```\n\n> **Note:** To force Tox to fail if Poetry is not installed, add the `require_poetry = true`\n> option to the tox `[testenv]` configuration. See the\n> [Config Options](#configuration-options) for more information.\n\n## Developer Documentation\n\nAll project contributors and participants are expected to adhere to the\n[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).\n\nThe `devel` branch has the latest (and potentially unstable) changes. The stable releases\nare tracked on [Github](https://github.com/enpaul/tox-poetry-installer/releases),\n[PyPi](https://pypi.org/project/tox-poetry-installer/#history), and in the\n[Changelog](CHANGELOG.md).\n\n- To report a bug, request a feature, or ask for assistance, please\n  [open an issue on the Github repository](https://github.com/enpaul/tox-poetry-installer/issues/new).\n- To report a security concern or code of conduct violation, please contact the project\n  author directly at **\u200cme \\[at\u200c\\] enp dot\u200e \u200cone**.\n- To submit an update, please\n  [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)\n  and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).\n\nDeveloping this project requires [Python 3.7+](https://www.python.org/downloads/) and\n[Poetry 1.2](https://python-poetry.org/docs/#installation) or later. GNU Make can\noptionally be used to quickly setup a local development environment, but this is not\nrequired.\n\nTo setup a local development environment:\n\n```bash\n# Clone the repository...\n# ...over HTTPS\ngit clone https://github.com/enpaul/tox-poetry-installer.git\n# ...over SSH\ngit clone git@github.com:enpaul/tox-poetry-installer.git\n\ncd tox-poetry-installer/\n\n# Create and configure the local development environment\nmake dev\n\n# Run tests and CI locally\nmake test\n\n# See additional make targets\nmake help\n```\n\n> **Note:** The pre-commit hooks require dependencies in the Poetry environment to run. To\n> make a commit with the pre-commit hooks, you will need to run `poetry run git commit` or,\n> alternatively, [launch an environment shell](https://python-poetry.org/docs/cli/#shell).\n\n## Road Map\n\nThis project is under active development and is classified as beta software, ready for\nproduction environments on a provisional basis only.\n\n- Beta classification was assigned with\n  [v0.6.0](https://github.com/enpaul/tox-poetry-installer/releases/tag/0.6.0)\n- Stable classification will be assigned when the test suite covers an acceptable number of\n  use cases\n\n### Path to Beta\n\n- [x] Verify that primary package dependencies (from the `.package` env) are installed\n  correctly using the Poetry backend.\n- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) Tox\n  configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))\n- [x] Add per-environment Tox configuration option to fall back to default installation\n  backend.\n- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using the\n  Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))\n- [x] Add trivial tests to ensure the project metadata is consistent between the pyproject.toml\n  and the module constants.\n- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and improve\n  robustness of the Tox and Poetry module imports to avoid potentially breaking API changes\n  in upstream packages. ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [ ] ~Find and implement a way to mitigate the\n  [UNSAFE_DEPENDENCIES issue](https://github.com/python-poetry/poetry/issues/1584) in\n  Poetry.~ ([#6](https://github.com/enpaul/tox-poetry-installer/issues/6))\n- [x] Fix logging to make proper use of Tox\'s logging reporter infrastructure ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))\n- [x] Add configuration option for installing all dev-dependencies to a testenv ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))\n\n### Path to Stable\n\nEverything in Beta plus...\n\n- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core` ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))\n- [x] Add comprehensive unit tests\n- [ ] ~Add tests for each feature version of Tox between 3.8 and 3.20~\n- [x] Add tests for Python-3.6, 3.7, 3.8, and 3.9\n- [x] Add Github Actions based CI\n',
-    'author': 'Ethan Paul',
-    'author_email': '24588726+enpaul@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/enpaul/tox-poetry-installer/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+[![CI Status](https://github.com/enpaul/tox-poetry-installer/workflows/CI/badge.svg?event=push)](https://github.com/enpaul/tox-poetry-installer/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/tox-poetry-installer)](https://pypi.org/project/tox-poetry-installer/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/tox-poetry-installer)](https://libraries.io/pypi/tox-poetry-installer)
+[![License](https://img.shields.io/pypi/l/tox-poetry-installer)](https://opensource.org/licenses/MIT)
+[![Python Supported Versions](https://img.shields.io/pypi/pyversions/tox-poetry-installer)](https://www.python.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+⚠️ **This project is beta software and is under active development** ⚠️
+
+## Documentation
+
+- [Feature Overview](#feature-overview)
+- [Using the Plugin](#user-documentation)
+  - [Installing](#installing)
+  - [Quick Start](#quick-start)
+  - [References](#references)
+    - [Config Options](#configuration-options)
+    - [Runtime Options](#runtime-options)
+    - [Errors](#errors)
+  - [Other Notes](#other-notes)
+    - [Unsupported Tox config options](#unsupported-tox-config-options)
+    - [Updating locked dependencies in a testenv](#updating-locked-dependencies-in-a-testenv)
+    - [Using with an unmanaged Poetry installation](#using-with-an-unmanaged-poetry-installation)
+- [Developing the Plugin](#developer-documentation)
+- [Road Map](#road-map)
+
+See the
+[Changelog](https://github.com/enpaul/tox-poetry-installer/blob/devel/CHANGELOG.md) for
+release history.
+
+*See also: [official Tox plugins](https://tox.readthedocs.io/en/latest/plugins.html) and
+[the official Poetry documentation on using Tox](https://python-poetry.org/docs/faq/#is-tox-supported)*
+
+## Feature Overview
+
+- Manage package versions in exactly one place and with exactly one tool: Poetry.
+- Ensure CI/CD and other automation tools are using the same package versions that you are
+  in your local development environment.
+- Add only the packages or custom groups you need to a Tox test environment, instead of
+  everything in your lockfile.
+- Directly integrate with Poetry, re-using your existing package indexes and credentials,
+  with no additional configuration.
+- Wherever possible, built-in Tox config options are always respected and their behavior
+  kept consistent.
+- Extremely configurable. Every feature can be disabled or enabled for any given Tox test
+  environment.
+- Friendly to other Tox plugins and supports a wide range of environments.
+
+## User Documentation
+
+*This section is for users looking to integrate the plugin with their project or CI
+system. For information on contributing to the plugin please see the
+[Developer Docs](#developer-documentation)*
+
+### Installing
+
+The recommended way to install the plugin is to add it to a project using Poetry:
+
+```bash
+poetry add -G dev tox-poetry-installer[poetry]
+```
+
+> ℹ️ **Note:** Always install the plugin with the `[poetry]` extra, unless you are
+> [managing the Poetry installation yourself](#externally-managed-poetry-installation).
+
+Alternatively, it can be installed directly to a virtual environment using Pip, though
+this is not recommended:
+
+```bash
+source somevenv/bin/activate
+pip install tox-poetry-installer
+```
+
+Alternatively alternatively, it can be installed using the Tox
+[`requires`](https://tox.readthedocs.io/en/latest/config.html#conf-requires) option by
+adding the below to `tox.ini`, though this is also not recommended:
+
+```ini
+requires =
+    tox-poetry-installer[poetry] == 0.10.2
+```
+
+After installing, check that Tox recognizes the plugin by running
+`poetry run tox --version`. The command should give output similar to below:
+
+```
+3.20.0 imported from .venv/lib64/python3.10/site-packages/tox/__init__.py
+registered plugins:
+    tox-poetry-installer-0.10.2 at .venv/lib64/python3.10/site-packages/tox_poetry_installer/__init__.py
+```
+
+### Quick Start
+
+Congratulations! 🎉 Just by installing the plugin your Tox config is already using locked
+dependencies: when Tox builds and installs your project package to a test environment,
+your project package's dependencies will be installed from the lockfile.
+
+Now lets update an example `tox.ini` to install the other test environment dependencies
+from the lockfile.
+
+A `testenv` from the example `tox.ini` we're starting with is below:
+
+```ini
+[testenv]
+description = Some very cool tests
+deps =
+    black == 20.8b1
+    pylint >=2.4.4,<2.7.0
+    mypy <0.800
+commands = ...
+```
+
+To update the config so that the testenv dependencies are installed from the lockfile, we
+can replace the built-in
+[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option with the
+`locked_deps` option provided by the plugin, and then remove the inline version
+specifiers. With these changes the three testenv dependencies (as well as all of their
+dependencies) will be installed from the lockfile when the test environment is recreated:
+
+```ini
+[testenv]
+description = Some very cool tests
+locked_deps =
+    black
+    pylint
+    mypy
+commands = ...
+```
+
+We can also add the `require_locked_deps` option to the test environment. This will both
+block any other install tools (another plugin or Tox itself) from installing dependencies
+to the Tox environment and also cause Tox to fail if the test environment also uses the
+built-in [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:
+
+```ini
+[testenv]
+description = Some very cool tests
+require_locked_deps = true
+locked_deps =
+    black
+    pylint
+    mypy
+commands = ...
+```
+
+> ℹ️ **Note:** Settings configured on the main `testenv` environment are inherited by
+> child test environments (for example, `testenv:foo`). To override this, specify the
+> setting in the child environment with a different value.
+
+Alternatively, we can skip specifying all of our dependencies for a test environment in
+the Tox config and install Poetry dependency groups directly:
+
+```ini
+[testenv]
+description = Some very cool tests
+require_locked_deps = true
+poetry_dep_groups =
+    dev
+commands = ...
+```
+
+> ℹ️ **Note:** The `install_dev_deps` configuration option is deprecated. See
+> [Configuration Options](#configuration-options) for more information.
+
+Finally, we can also install an unlocked dependency (a dependency which doesn't take its
+version from the Poetry lockfile) into the test environment alongside the locked ones. We
+need to remove the `require_locked_deps = true` option, otherwise the environment will
+error, and then we can add the unlocked dependency using the built-in
+[`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) option:
+
+```ini
+[testenv]
+description = Some very cool tests
+deps =
+    pytest >= 5.6.0,<6.0.0
+locked_deps =
+    black
+    pylint
+    mypy
+commands = ...
+```
+
+## References
+
+### Configuration Options
+
+All options listed below are Tox environment options and can be applied to one or more
+environment sections of the `tox.ini` file. They cannot be applied to the global Tox
+configuration section.
+
+> ℹ️ **Note:** Settings configured on the main `testenv` environment are inherited by
+> child test environments (for example, `testenv:foo`). To override this, specify the
+> setting in the child environment with a different value.
+
+| Option                 |  Type   | Default | Description                                                                                                                                                                                                                                                                                                                                                          |
+| :--------------------- | :-----: | :-----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `locked_deps`          |  List   |  `[]`   | Names of packages to install to the test environment from the Poetry lockfile. Transient dependencies (packages required by these dependencies) are automatically included.                                                                                                                                                                                          |
+| `require_locked_deps`  | Boolean |  False  | Whether the plugin should block attempts to install unlocked dependencies to the test environment. If enabled, then the [`tox_testenv_install_deps`](https://tox.readthedocs.io/en/latest/plugins.html#tox.hookspecs.tox_testenv_install_deps) plugin hook will be intercepted and an error will be raised if the test environment has the `deps` option configured. |
+| `install_project_deps` | Boolean |  True   | Whether all of the Poetry primary dependencies for the project package should be installed to the test environment.                                                                                                                                                                                                                                                  |
+| `require_poetry`       | Boolean |  False  | Whether Tox should be forced to fail if the plugin cannot import Poetry locally. If `False` then the plugin will be skipped for the test environment if Poetry cannot be imported. If `True` then the plugin will force the environment to error and the Tox run to fail.                                                                                            |
+| `poetry_dep_groups`    |  List   |  `[]`   | Names of Poetry dependency groups specified in `pyproject.toml` to install to the test environment.                                                                                                                                                                                                                                                                  |
+
+### Runtime Options
+
+All arguments listed below can be passed to the `tox` command to modify runtime behavior
+of the plugin.
+
+| Argument                     |  Type   | Default | Description                                                                                                                                                                                                                                                                          |
+| :--------------------------- | :-----: | :-----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `--parallel-install-threads` | Integer |  `10`   | Number of worker threads to use to install dependencies in parallel. Installing in parallel with more threads can greatly speed up the install process, but can cause race conditions during install. Pass this option with the value `0` to entirely disable parallel installation. |
+
+### Errors
+
+There are several errors that the plugin can encounter for a test environment when Tox is
+run. If an error is encountered then the status of the test environment that caused the
+error will be set to one of the "Status" values below to indicate what the error was.
+
+| Status/Name                     | Cause                                                                                                                                                                                                                           |
+| :------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| `ExtraNotFoundError`            | Indicates that the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras) config option specified an extra that is not configured by Poetry in `pyproject.toml`.                                              |
+| `LockedDepVersionConflictError` | Indicates that an item in the `locked_deps` config option includes a [PEP-508 version specifier](https://www.python.org/dev/peps/pep-0508/#grammar) (ex: `pytest >=6.0, <6.1`).                                                 |
+| `LockedDepNotFoundError`        | Indicates that an item specified in the `locked_deps` config option does not match the name of a package in the Poetry lockfile.                                                                                                |
+| `LockedDepsRequiredError`       | Indicates that a test environment with the `require_locked_deps` config option set to `true` also specified unlocked dependencies using the [`deps`](https://tox.readthedocs.io/en/latest/config.html#conf-deps) config option. |
+| `PoetryNotInstalledError`       | Indicates that the `poetry` module could not be imported under the current runtime environment, and `require_poetry = true` was specified.                                                                                      |
+| `RequiresUnsafeDepError`        | Indicates that the package-under-test depends on a package that Poetry has classified as unsafe and cannot be installed.                                                                                                        |
+
+> ℹ️ **Note:** One or more of these errors can be caused by the `pyproject.toml` being out
+> of sync with the Poetry lockfile. If this is the case, than a warning will be logged
+> when Tox is run.
+
+### Other Notes
+
+#### Unsupported Tox config options
+
+Below are the built-in Tox config options that are not respected by this plugin. All of
+these options are made obsolete by the Poetry lockfile: either they aren't needed or their
+equivalent functionality is instead taken directly from the package details Poetry stores
+in its lockfile.
+
+> ℹ️ **Note:** The unsupported Tox config options will still apply to unlocked
+> dependencies being installed with the default Tox installation backend.
+
+- [`install_command`](https://tox.readthedocs.io/en/latest/config.html#conf-install_command)
+- [`pip_pre`](https://tox.readthedocs.io/en/latest/config.html#conf-pip_pre)
+- [`download`](https://tox.readthedocs.io/en/latest/config.html#conf-download)
+- [`indexserver`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)
+- [`usedevelop`](https://tox.readthedocs.io/en/latest/config.html#conf-indexserver)
+
+#### Updating locked dependencies in a testenv
+
+When Poetry updates the version of a package in the lockfile (using either `poetry lock`
+or `poetry update`) then the plugin will automatically use this new version to install the
+package to a test environment; there is no need to manually update `tox.ini` after
+updating the Poetry lockfile.
+
+However, the plugin cannot determine when the lockfile is updated. If a Tox test
+environment has already been created then it will need to be recreated (using Tox's
+built-in
+[`--recreate`](https://tox.readthedocs.io/en/latest/example/basic.html#forcing-re-creation-of-virtual-environments)
+option) for the new version to be found and installed.
+
+> ℹ️ **Note:** To force Tox to always recreate a test environment the
+> [`recreate`](https://tox.readthedocs.io/en/latest/config.html#conf-recreate) config
+> option can be set.
+
+#### Using with an unmanaged Poetry installation
+
+In CI/CD systems, automation environments, or other Python environments where the loaded
+site packages are not managed by Poetry, it can be useful to manage the local installation
+of Poetry externally. This also helps to avoid problems that can be caused by the
+`--no-root`, `--without dev`, or `--sync` arguments to the `poetry install` command which,
+in some situations, can cause Poetry to uninstall itself if Poetry is specified as a
+dependency of one of the packages it is managing (like this plugin). To support these use
+cases, this plugin specifies the `poetry` package as an optional dependency that can be
+installed using a setuptools extra also named `poetry`.
+
+> ⚠️ **Warning:** This plugin requires Poetry to function. If the plugin is installed
+> without the `poetry` setuptools extra then Poetry must be installed independently for
+> the plugin to function properly.
+
+To skip installing the `poetry` package as a dependency of `tox-poetry-installer`, do not
+specify the `poetry` extra when adding the plugin:
+
+```bash
+# Adding the package without the "[poetry]" extra specifier so that
+# Poetry is not added as a transient dev-dependency:
+poetry add -G dev tox-poetry-installer
+
+# Adding the package with the "[poetry]" extra specifier, so the Poetry
+# package will be added to the environment and tracked in the lockfile:
+poetry add -G dev tox-poetry-installer[poetry]
+```
+
+Once the plugin is installed- either with or without the Poetry extra- you can validate
+that the plugin will run correctly with the following command. This command checks that
+all three required components (Tox, Poetry, and the plugin itself) are available in the
+current Python environment:
+
+```bash
+python -c '\
+  import tox;\
+  import tox_poetry_installer;\
+  from poetry.poetry import Poetry;\
+'
+```
+
+> ℹ️ **Note:** To force Tox to fail if Poetry is not installed, add the
+> `require_poetry = true` option to the tox `[testenv]` configuration. See the
+> [Config Options](#configuration-options) for more information.
+
+## Developer Documentation
+
+All project contributors and participants are expected to adhere to the
+[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md)
+([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
+
+The `devel` branch has the latest (and potentially unstable) changes. The stable releases
+are tracked on [Github](https://github.com/enpaul/tox-poetry-installer/releases),
+[PyPi](https://pypi.org/project/tox-poetry-installer/#history), and in the
+[Changelog](CHANGELOG.md).
+
+- To report a bug, request a feature, or ask for assistance, please
+  [open an issue on the Github repository](https://github.com/enpaul/tox-poetry-installer/issues/new).
+- To report a security concern or code of conduct violation, please contact the project
+  author directly at **‌me \[at‌\] enp dot‎ ‌one**.
+- To submit an update, please
+  [fork the repository](https://docs.github.com/en/enterprise/2.20/user/github/getting-started-with-github/fork-a-repo)
+  and [open a pull request](https://github.com/enpaul/tox-poetry-installer/compare).
+
+Developing this project requires [Python 3.10+](https://www.python.org/downloads/) and
+[Poetry 1.4](https://python-poetry.org/docs/#installation) or later. GNU Make can
+optionally be used to quickly setup a local development environment, but this is not
+required.
+
+To setup a local development environment:
+
+```bash
+# Clone the repository...
+# ...over HTTPS
+git clone https://github.com/enpaul/tox-poetry-installer.git
+# ...over SSH
+git clone git@github.com:enpaul/tox-poetry-installer.git
+
+cd tox-poetry-installer/
+
+# Create and configure the local development environment
+make dev
+
+# Run tests and CI locally
+make test
+
+# See additional make targets
+make help
+```
+
+> ℹ️ **Note:** The pre-commit hooks require dependencies in the Poetry environment to run.
+> To make a commit with the pre-commit hooks, you will need to run `poetry run git commit`
+> or, alternatively,
+> [launch an environment shell](https://python-poetry.org/docs/cli/#shell).
+
+## Road Map
+
+This project is under active development and is classified as beta software, ready for
+production environments on a provisional basis only.
+
+- Beta classification was assigned with
+  [v0.6.0](https://github.com/enpaul/tox-poetry-installer/releases/tag/0.6.0)
+- Stable classification will be assigned when the test suite covers an acceptable number
+  of use cases
+
+### Path to Beta
+
+- [x] Verify that primary package dependencies (from the `.package` env) are installed
+  correctly using the Poetry backend.
+- [x] Support the [`extras`](https://tox.readthedocs.io/en/latest/config.html#conf-extras)
+  Tox configuration option ([#4](https://github.com/enpaul/tox-poetry-installer/issues/4))
+- [x] Add per-environment Tox configuration option to fall back to default installation
+  backend.
+- [ ] ~Add warnings when an unsupported Tox configuration option is detected while using
+  the Poetry backend.~ ([#5](https://github.com/enpaul/tox-poetry-installer/issues/5))
+- [x] Add trivial tests to ensure the project metadata is consistent between the
+  pyproject.toml and the module constants.
+- [x] Update to use [poetry-core](https://github.com/python-poetry/poetry-core) and
+  improve robustness of the Tox and Poetry module imports to avoid potentially breaking
+  API changes in upstream packages.
+  ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
+- [ ] ~Find and implement a way to mitigate the
+  [UNSAFE_DEPENDENCIES issue](https://github.com/python-poetry/poetry/issues/1584) in
+  Poetry.~ ([#6](https://github.com/enpaul/tox-poetry-installer/issues/6))
+- [x] Fix logging to make proper use of Tox's logging reporter infrastructure
+  ([#3](https://github.com/enpaul/tox-poetry-installer/issues/3))
+- [x] Add configuration option for installing all dev-dependencies to a testenv
+  ([#14](https://github.com/enpaul/tox-poetry-installer/issues/14))
+
+### Path to Stable
+
+Everything in Beta plus...
+
+- [ ] Fully replace dependency on `poetry` with dependency on `poetry-core`
+  ([#2](https://github.com/enpaul/tox-poetry-installer/issues/2))
+- [x] Add comprehensive unit tests
+- [ ] ~Add tests for each feature version of Tox between 3.8 and 3.20~
+- [x] Add tests for Python-3.6, 3.7, 3.8, and 3.9
+- [x] Add Github Actions based CI
 
-setup(**setup_kwargs)
```

