# Comparing `tmp/cyclonedx-conan-0.2.0.tar.gz` & `tmp/cyclonedx_conan-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx-conan-0.2.0.tar", max compression
+gzip compressed data, was "cyclonedx_conan-0.4.0.tar", max compression
```

## Comparing `cyclonedx-conan-0.2.0.tar` & `cyclonedx_conan-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11341 2021-10-14 12:11:48.270583 cyclonedx-conan-0.2.0/LICENSE
--rw-r--r--   0        0        0      152 2021-10-14 12:11:48.270583 cyclonedx-conan-0.2.0/NOTICE
--rw-r--r--   0        0        0     6817 2021-10-14 12:11:48.270583 cyclonedx-conan-0.2.0/README.md
--rw-r--r--   0        0        0      925 2021-10-14 12:12:15.083967 cyclonedx-conan-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     7030 2021-10-14 12:11:48.270583 cyclonedx-conan-0.2.0/src/command.py
--rw-r--r--   0        0        0     7801 2021-10-14 12:12:26.186929 cyclonedx-conan-0.2.0/setup.py
--rw-r--r--   0        0        0     7699 2021-10-14 12:12:26.187343 cyclonedx-conan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-08-02 11:45:23.505188 cyclonedx_conan-0.4.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-08-02 11:45:23.505188 cyclonedx_conan-0.4.0/NOTICE
+-rw-r--r--   0        0        0     8879 2023-08-02 11:45:23.505188 cyclonedx_conan-0.4.0/README.md
+-rw-r--r--   0        0        0     1046 2023-08-02 11:46:00.081704 cyclonedx_conan-0.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0     9069 2023-08-02 11:45:23.505188 cyclonedx_conan-0.4.0/src/command.py
+-rw-r--r--   0        0        0     9894 1970-01-01 00:00:00.000000 cyclonedx_conan-0.4.0/PKG-INFO
```

### Comparing `cyclonedx-conan-0.2.0/LICENSE` & `cyclonedx_conan-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx-conan-0.2.0/README.md` & `cyclonedx_conan-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,174 @@
 # CycloneDX Conan SBOM Generation Tool
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CycloneDX/cyclonedx-conan/Python%20CI)](https://github.com/CycloneDX/cyclonedx-conan/actions/workflows/ci.yml)
-[![GitHub license](https://img.shields.io/github/license/CycloneDX/cyclonedx-conan)](https://github.com/CycloneDX/cyclonedx-conan/blob/main/LICENSE)
-[![Python Version Support](https://img.shields.io/badge/https://-cyclonedx.org-blue)](https://cyclonedx.org/)
-[![Slack Invite](https://img.shields.io/badge/Slack-Join-blue?logo=slack&labelColor=393939)](https://cyclonedx.org/slack/invite)
-![PyPI Version](https://img.shields.io/pypi/v/cyclonedx-conan?label=PyPI&logo=pypi)
-![Python Version Support](https://img.shields.io/badge/python-3.6+-blue)
-[![Group Discussion](https://img.shields.io/badge/discussion-groups.io-blue)](https://groups.io/g/CycloneDX)
-[![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Follow)](https://twitter.com/CycloneDX_Spec)
+[![shield_pypi-version]][link_pypi]
+[![shield_gh-workflow-test]][link_gh-workflow-test]
+[![shield_license]][license_file]  
+[![shield_website]][link_website]
+[![shield_slack]][link_slack]
+[![shield_groups]][link_discussion]
+[![shield_twitter-follow]][link_twitter]
 
 ----
 
 This project provides a tool for generating CycloneDX bill-of-material JSON documents for C/C++ projects using Conan.
 
 The BOM will contain an aggregate of all your current project's dependencies, including a full dependency graph.
 
 CycloneDX is a lightweight BOM specification that is easily created, human-readable, and simple to parse.
 
 Please note: This tool has only been tested with Conan 1.14 so far.
 
 ## Installation
 
-Install this from [PyPi.org](https://pypi.org/project/cyclonedx-conan/) using your preferred Python package manager.
+Install this from [PyPi.org][link_pypi] using your preferred Python package manager.
 
 Example using `pip`:
-```
+
+```shell
 pip install cyclonedx-conan
 ```
 
 Example using `poetry`:
-```
+
+```shell
 poetry add cyclonedx-conan
 ```
 
 ## Usage
 
 Once installed, you can access the full documentation by running `--help`:
 
 The command line options are aligned to the standard Conan options.
 
-```
+```shellSession
 $ cyclonedx-conan --help
-usage: command.py [-h] [-if INSTALL_FOLDER] [-db [DRY_BUILD]] [-b [BUILD]] [-r REMOTE] [-u] [-l LOCKFILE] [--lockfile-out LOCKFILE_OUT]
-                  [-e ENV_HOST] [-e:b ENV_BUILD] [-e:h ENV_HOST] [-o OPTIONS_HOST] [-o:b OPTIONS_BUILD] [-o:h OPTIONS_HOST]
-                  [-pr PROFILE_HOST] [-pr:b PROFILE_BUILD] [-pr:h PROFILE_HOST] [-s SETTINGS_HOST] [-s:b SETTINGS_BUILD]
-                  [-s:h SETTINGS_HOST] [-c CONF_HOST] [-c:b CONF_BUILD] [-c:h CONF_HOST]
-                  path_or_reference
+usage: cyclonedx-conan [-h] [-if INSTALL_FOLDER] [-db [DRY_BUILD]]
+                       [--output FILE_PATH] [--exclude-dev]
+                       [-b [BUILD]] [-r REMOTE] [-u]
+                       [-l LOCKFILE] [--lockfile-out LOCKFILE_OUT]
+                       [-e ENV_HOST] [-e:b ENV_BUILD] [-e:h ENV_HOST]
+                       [-o OPTIONS_HOST] [-o:b OPTIONS_BUILD]
+                       [-o:h OPTIONS_HOST] [-pr PROFILE_HOST]
+                       [-pr:b PROFILE_BUILD] [-pr:h PROFILE_HOST]
+                       [-s SETTINGS_HOST] [-s:b SETTINGS_BUILD]
+                       [-s:h SETTINGS_HOST] [-c CONF_HOST] [-c:b CONF_BUILD]
+                       [-c:h CONF_HOST]
+                       path_or_reference
 
 CycloneDX SBOM Generator
 
 positional arguments:
-  path_or_reference     Path to a folder containing a recipe (conanfile.py or conanfile.txt) or to a recipe file. e.g.,
-                        ./my_project/conanfile.txt. It could also be a reference
+  path_or_reference     Path to a folder containing a recipe (conanfile.py or conanfile.txt) or to a recipe file.
+                        e.g., ./my_project/conanfile.txt. It could also be a reference
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -if INSTALL_FOLDER, --install-folder INSTALL_FOLDER
                         local folder containing the conaninfo.txt and conanbuildinfo.txt files (from a previous conan install execution).
-                        Defaulted to current folder, unless --profile, -s or -o is specified. If you specify both install-folder and any
-                        setting/option it will raise an error.
+                        Defaulted to current folder, unless --profile, -s or -o is specified.
+                        If you specify both install-folder and any setting/option it will raise an error.
   -db [DRY_BUILD], --dry-build [DRY_BUILD]
                         Apply the --build argument to output the information, as it would be done by the install command
+  --output FILE_PATH
+                        Output file path for your SBOM (set to '-' to output to STDOUT)
+  --exclude-dev         Exclude development dependencies from the BOM
   -b [BUILD], --build [BUILD]
-                        Given a build policy, return an ordered list of packages that would be built from sources during the install
-                        command
+                        Given a build policy, return an ordered list of packages that would be built from sources during the install command
   -r REMOTE, --remote REMOTE
                         Look in the specified remote server
-  -u, --update          Will check if updates of the dependencies exist in the remotes (a new version that satisfies a version range, a
-                        new revision or a newer recipe if not using revisions).
+  -u, --update          Will check if updates of the dependencies exist in the remotes 
+                        (a new version that satisfies a version range, a new revision or a newer recipe if not using revisions).
   -l LOCKFILE, --lockfile LOCKFILE
                         Path to a lockfile
   --lockfile-out LOCKFILE_OUT
                         Filename of the updated lockfile
   -e ENV_HOST, --env ENV_HOST
-                        Environment variables that will be set during the package build (host machine). e.g.: -e CXX=/usr/bin/clang++
+                        Environment variables that will be set during the package build (host machine).
+                        e.g.: -e CXX=/usr/bin/clang++
   -e:b ENV_BUILD, --env:build ENV_BUILD
-                        Environment variables that will be set during the package build (build machine). e.g.: -e:b CXX=/usr/bin/clang++
+                        Environment variables that will be set during the package build (build machine).
+                        e.g.: -e:b CXX=/usr/bin/clang++
   -e:h ENV_HOST, --env:host ENV_HOST
-                        Environment variables that will be set during the package build (host machine). e.g.: -e:h CXX=/usr/bin/clang++
+                        Environment variables that will be set during the package build (host machine).
+                        e.g.: -e:h CXX=/usr/bin/clang++
   -o OPTIONS_HOST, --options OPTIONS_HOST
-                        Define options values (host machine), e.g.: -o Pkg:with_qt=true
+                        Define options values (host machine),
+                        e.g.: -o Pkg:with_qt=true
   -o:b OPTIONS_BUILD, --options:build OPTIONS_BUILD
-                        Define options values (build machine), e.g.: -o:b Pkg:with_qt=true
+                        Define options values (build machine),
+                        e.g.: -o:b Pkg:with_qt=true
   -o:h OPTIONS_HOST, --options:host OPTIONS_HOST
-                        Define options values (host machine), e.g.: -o:h Pkg:with_qt=true
+                        Define options values (host machine),
+                        e.g.: -o:h Pkg:with_qt=true
   -pr PROFILE_HOST, --profile PROFILE_HOST
                         Apply the specified profile to the host machine
   -pr:b PROFILE_BUILD, --profile:build PROFILE_BUILD
                         Apply the specified profile to the build machine
   -pr:h PROFILE_HOST, --profile:host PROFILE_HOST
                         Apply the specified profile to the host machine
   -s SETTINGS_HOST, --settings SETTINGS_HOST
-                        Settings to build the package, overwriting the defaults (host machine). e.g.: -s compiler=gcc
+                        Settings to build the package, overwriting the defaults (host machine).
+                        e.g.: -s compiler=gcc
   -s:b SETTINGS_BUILD, --settings:build SETTINGS_BUILD
-                        Settings to build the package, overwriting the defaults (build machine). e.g.: -s:b compiler=gcc
+                        Settings to build the package, overwriting the defaults (build machine).
+                        e.g.: -s:b compiler=gcc
   -s:h SETTINGS_HOST, --settings:host SETTINGS_HOST
-                        Settings to build the package, overwriting the defaults (host machine). e.g.: -s:h compiler=gcc
+                        Settings to build the package, overwriting the defaults (host machine).
+                        e.g.: -s:h compiler=gcc
   -c CONF_HOST, --conf CONF_HOST
-                        Configuration to build the package, overwriting the defaults (host machine). e.g.: -c
-                        tools.cmake.cmaketoolchain:generator=Xcode
+                        Configuration to build the package, overwriting the defaults (host machine).
+                        e.g.: -c tools.cmake.cmaketoolchain:generator=Xcode
   -c:b CONF_BUILD, --conf:build CONF_BUILD
-                        Configuration to build the package, overwriting the defaults (build machine). e.g.: -c:b
-                        tools.cmake.cmaketoolchain:generator=Xcode
+                        Configuration to build the package, overwriting the defaults (build machine).
+                        e.g.: -c:b tools.cmake.cmaketoolchain:generator=Xcode
   -c:h CONF_HOST, --conf:host CONF_HOST
-                        Configuration to build the package, overwriting the defaults (host machine). e.g.: -c:h
-                        tools.cmake.cmaketoolchain:generator=Xcode
+                        Configuration to build the package, overwriting the defaults (host machine).
+                        e.g.: -c:h tools.cmake.cmaketoolchain:generator=Xcode
 ```
 
-
 ## Python Support
 
 We endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).
 However, some features may not be possible/present in older Python versions due to their lack of support.
 
+## Contributing
+
+Pull requests are welcome. But please read the
+[CycloneDX contributing guidelines](https://github.com/CycloneDX/.github/blob/master/CONTRIBUTING.md) first.
+
+It is generally expected that pull requests will include relevant tests.
+Tests are automatically run on Windows, MacOS and Linux for every pull request.
+
+Thanks to [Gitpod](https://gitpod.io/) there are two really easy ways of
+creating a ready to go development environment with VS Code.
+
+You can open a Gitpod hosted development environment in your browser. Or you
+can start a local instance of the OpenVSCode Server by running the
+`localdev.sh` script (requires Docker).
+
+[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/CycloneDX/cyclonedx-conan)
+
 ## Copyright & License
 
-CycloneDX BOM is Copyright (c) OWASP Foundation. All Rights Reserved.
+CycloneDX BOM is Copyright (c) OWASP Foundation. All Rights Reserved.  
+Permission to modify and redistribute is granted under the terms of the Apache 2.0 license.  
+See the [LICENSE][license_file] file for the full license.
+
+[license_file]: https://github.com/CycloneDX/cyclonedx-conan/blob/main/LICENSE
+[chaneglog_file]: https://github.com/CycloneDX/cyclonedx-conan/blob/main/CHANGELOG.md
+
+[link_gh-workflow-test]: https://github.com/CycloneDX/cyclonedx-conan/actions/workflows/ci.yml?query=branch%3Amain
+[link_pypi]: https://pypi.org/project/cyclonedx-conan/
+[link_website]: https://cyclonedx.org/
+[link_slack]: https://cyclonedx.org/slack/invite
+[link_discussion]: https://groups.io/g/CycloneDX
+[link_twitter]: https://twitter.com/CycloneDX_Spec
+
+[shield_gh-workflow-test]: https://img.shields.io/github/actions/workflow/status/CycloneDX/cyclonedx-conan/ci.yml?branch=main&logo=GitHub&logoColor=white "build"
+[shield_pypi-version]: https://img.shields.io/pypi/v/cyclonedx-conan?logo=pypi&logoColor=white&label=PyPI "PyPI"
+[shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-conan?logo=open%20source%20initiative&logoColor=white "license"
+[shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"
+[shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"
+[shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"
+[shield_twitter-follow]: https://img.shields.io/badge/Twitter-follow-blue?logo=Twitter&logoColor=white "twitter follow"
 
-Permission to modify and redistribute is granted under the terms of the Apache 2.0 license.
```

### Comparing `cyclonedx-conan-0.2.0/pyproject.toml` & `cyclonedx_conan-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [tool.poetry]
 name = "cyclonedx-conan"
-version = "0.2.0"
+version = "0.4.0"
 description = "Creates CycloneDX Software Bill of Materials (SBOM) documents for C/C++ projects using Conan"
 authors = ["Patrick Dwyer <patrick.dwyer@owasp.org>"]
+maintainers = [
+    "Patrick Dwyer <patrick.dwyer@owasp.org>",
+    "Jan Kowalleck <jan.kowalleck@gmail.com>",
+]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/CycloneDX/cyclonedx-conan"
+homepage = "https://github.com/CycloneDX/cyclonedx-conan#readme"
 repository = "https://github.com/CycloneDX/cyclonedx-conan"
 packages = [
     { include = "src" }
 ]
 include = [
     "LICENSE", "NOTICE"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
-conan = "1.41.0"
+conan = "^1.41.0"
 packageurl-python = "^0.9.6"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 cyclonedx-conan = 'src.command:main'
 
@@ -31,8 +35,8 @@
 [tool.semantic_release]
 version_variable = [
     "pyproject.toml:version"
 ]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
```

### Comparing `cyclonedx-conan-0.2.0/setup.py` & `cyclonedx_conan-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,199 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cyclonedx-conan
+Version: 0.4.0
+Summary: Creates CycloneDX Software Bill of Materials (SBOM) documents for C/C++ projects using Conan
+Home-page: https://github.com/CycloneDX/cyclonedx-conan#readme
+License: Apache-2.0
+Author: Patrick Dwyer
+Author-email: patrick.dwyer@owasp.org
+Maintainer: Patrick Dwyer
+Maintainer-email: patrick.dwyer@owasp.org
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: conan (>=1.41.0,<2.0.0)
+Requires-Dist: packageurl-python (>=0.9.6,<0.10.0)
+Project-URL: Repository, https://github.com/CycloneDX/cyclonedx-conan
+Description-Content-Type: text/markdown
+
+# CycloneDX Conan SBOM Generation Tool
+
+[![shield_pypi-version]][link_pypi]
+[![shield_gh-workflow-test]][link_gh-workflow-test]
+[![shield_license]][license_file]  
+[![shield_website]][link_website]
+[![shield_slack]][link_slack]
+[![shield_groups]][link_discussion]
+[![shield_twitter-follow]][link_twitter]
+
+----
+
+This project provides a tool for generating CycloneDX bill-of-material JSON documents for C/C++ projects using Conan.
+
+The BOM will contain an aggregate of all your current project's dependencies, including a full dependency graph.
+
+CycloneDX is a lightweight BOM specification that is easily created, human-readable, and simple to parse.
+
+Please note: This tool has only been tested with Conan 1.14 so far.
+
+## Installation
+
+Install this from [PyPi.org][link_pypi] using your preferred Python package manager.
+
+Example using `pip`:
+
+```shell
+pip install cyclonedx-conan
+```
+
+Example using `poetry`:
+
+```shell
+poetry add cyclonedx-conan
+```
+
+## Usage
+
+Once installed, you can access the full documentation by running `--help`:
+
+The command line options are aligned to the standard Conan options.
+
+```shellSession
+$ cyclonedx-conan --help
+usage: cyclonedx-conan [-h] [-if INSTALL_FOLDER] [-db [DRY_BUILD]]
+                       [--output FILE_PATH] [--exclude-dev]
+                       [-b [BUILD]] [-r REMOTE] [-u]
+                       [-l LOCKFILE] [--lockfile-out LOCKFILE_OUT]
+                       [-e ENV_HOST] [-e:b ENV_BUILD] [-e:h ENV_HOST]
+                       [-o OPTIONS_HOST] [-o:b OPTIONS_BUILD]
+                       [-o:h OPTIONS_HOST] [-pr PROFILE_HOST]
+                       [-pr:b PROFILE_BUILD] [-pr:h PROFILE_HOST]
+                       [-s SETTINGS_HOST] [-s:b SETTINGS_BUILD]
+                       [-s:h SETTINGS_HOST] [-c CONF_HOST] [-c:b CONF_BUILD]
+                       [-c:h CONF_HOST]
+                       path_or_reference
+
+CycloneDX SBOM Generator
+
+positional arguments:
+  path_or_reference     Path to a folder containing a recipe (conanfile.py or conanfile.txt) or to a recipe file.
+                        e.g., ./my_project/conanfile.txt. It could also be a reference
+
+options:
+  -h, --help            show this help message and exit
+  -if INSTALL_FOLDER, --install-folder INSTALL_FOLDER
+                        local folder containing the conaninfo.txt and conanbuildinfo.txt files (from a previous conan install execution).
+                        Defaulted to current folder, unless --profile, -s or -o is specified.
+                        If you specify both install-folder and any setting/option it will raise an error.
+  -db [DRY_BUILD], --dry-build [DRY_BUILD]
+                        Apply the --build argument to output the information, as it would be done by the install command
+  --output FILE_PATH
+                        Output file path for your SBOM (set to '-' to output to STDOUT)
+  --exclude-dev         Exclude development dependencies from the BOM
+  -b [BUILD], --build [BUILD]
+                        Given a build policy, return an ordered list of packages that would be built from sources during the install command
+  -r REMOTE, --remote REMOTE
+                        Look in the specified remote server
+  -u, --update          Will check if updates of the dependencies exist in the remotes 
+                        (a new version that satisfies a version range, a new revision or a newer recipe if not using revisions).
+  -l LOCKFILE, --lockfile LOCKFILE
+                        Path to a lockfile
+  --lockfile-out LOCKFILE_OUT
+                        Filename of the updated lockfile
+  -e ENV_HOST, --env ENV_HOST
+                        Environment variables that will be set during the package build (host machine).
+                        e.g.: -e CXX=/usr/bin/clang++
+  -e:b ENV_BUILD, --env:build ENV_BUILD
+                        Environment variables that will be set during the package build (build machine).
+                        e.g.: -e:b CXX=/usr/bin/clang++
+  -e:h ENV_HOST, --env:host ENV_HOST
+                        Environment variables that will be set during the package build (host machine).
+                        e.g.: -e:h CXX=/usr/bin/clang++
+  -o OPTIONS_HOST, --options OPTIONS_HOST
+                        Define options values (host machine),
+                        e.g.: -o Pkg:with_qt=true
+  -o:b OPTIONS_BUILD, --options:build OPTIONS_BUILD
+                        Define options values (build machine),
+                        e.g.: -o:b Pkg:with_qt=true
+  -o:h OPTIONS_HOST, --options:host OPTIONS_HOST
+                        Define options values (host machine),
+                        e.g.: -o:h Pkg:with_qt=true
+  -pr PROFILE_HOST, --profile PROFILE_HOST
+                        Apply the specified profile to the host machine
+  -pr:b PROFILE_BUILD, --profile:build PROFILE_BUILD
+                        Apply the specified profile to the build machine
+  -pr:h PROFILE_HOST, --profile:host PROFILE_HOST
+                        Apply the specified profile to the host machine
+  -s SETTINGS_HOST, --settings SETTINGS_HOST
+                        Settings to build the package, overwriting the defaults (host machine).
+                        e.g.: -s compiler=gcc
+  -s:b SETTINGS_BUILD, --settings:build SETTINGS_BUILD
+                        Settings to build the package, overwriting the defaults (build machine).
+                        e.g.: -s:b compiler=gcc
+  -s:h SETTINGS_HOST, --settings:host SETTINGS_HOST
+                        Settings to build the package, overwriting the defaults (host machine).
+                        e.g.: -s:h compiler=gcc
+  -c CONF_HOST, --conf CONF_HOST
+                        Configuration to build the package, overwriting the defaults (host machine).
+                        e.g.: -c tools.cmake.cmaketoolchain:generator=Xcode
+  -c:b CONF_BUILD, --conf:build CONF_BUILD
+                        Configuration to build the package, overwriting the defaults (build machine).
+                        e.g.: -c:b tools.cmake.cmaketoolchain:generator=Xcode
+  -c:h CONF_HOST, --conf:host CONF_HOST
+                        Configuration to build the package, overwriting the defaults (host machine).
+                        e.g.: -c:h tools.cmake.cmaketoolchain:generator=Xcode
+```
+
+## Python Support
+
+We endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).
+However, some features may not be possible/present in older Python versions due to their lack of support.
+
+## Contributing
+
+Pull requests are welcome. But please read the
+[CycloneDX contributing guidelines](https://github.com/CycloneDX/.github/blob/master/CONTRIBUTING.md) first.
+
+It is generally expected that pull requests will include relevant tests.
+Tests are automatically run on Windows, MacOS and Linux for every pull request.
+
+Thanks to [Gitpod](https://gitpod.io/) there are two really easy ways of
+creating a ready to go development environment with VS Code.
+
+You can open a Gitpod hosted development environment in your browser. Or you
+can start a local instance of the OpenVSCode Server by running the
+`localdev.sh` script (requires Docker).
+
+[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/CycloneDX/cyclonedx-conan)
+
+## Copyright & License
+
+CycloneDX BOM is Copyright (c) OWASP Foundation. All Rights Reserved.  
+Permission to modify and redistribute is granted under the terms of the Apache 2.0 license.  
+See the [LICENSE][license_file] file for the full license.
+
+[license_file]: https://github.com/CycloneDX/cyclonedx-conan/blob/main/LICENSE
+[chaneglog_file]: https://github.com/CycloneDX/cyclonedx-conan/blob/main/CHANGELOG.md
+
+[link_gh-workflow-test]: https://github.com/CycloneDX/cyclonedx-conan/actions/workflows/ci.yml?query=branch%3Amain
+[link_pypi]: https://pypi.org/project/cyclonedx-conan/
+[link_website]: https://cyclonedx.org/
+[link_slack]: https://cyclonedx.org/slack/invite
+[link_discussion]: https://groups.io/g/CycloneDX
+[link_twitter]: https://twitter.com/CycloneDX_Spec
+
+[shield_gh-workflow-test]: https://img.shields.io/github/actions/workflow/status/CycloneDX/cyclonedx-conan/ci.yml?branch=main&logo=GitHub&logoColor=white "build"
+[shield_pypi-version]: https://img.shields.io/pypi/v/cyclonedx-conan?logo=pypi&logoColor=white&label=PyPI "PyPI"
+[shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-conan?logo=open%20source%20initiative&logoColor=white "license"
+[shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"
+[shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"
+[shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"
+[shield_twitter-follow]: https://img.shields.io/badge/Twitter-follow-blue?logo=Twitter&logoColor=white "twitter follow"
 
-packages = \
-['src']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['conan==1.41.0', 'packageurl-python>=0.9.6,<0.10.0']
-
-entry_points = \
-{'console_scripts': ['cyclonedx-conan = src.command:main']}
-
-setup_kwargs = {
-    'name': 'cyclonedx-conan',
-    'version': '0.2.0',
-    'description': 'Creates CycloneDX Software Bill of Materials (SBOM) documents for C/C++ projects using Conan',
-    'long_description': "# CycloneDX Conan SBOM Generation Tool\n\n[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/CycloneDX/cyclonedx-conan/Python%20CI)](https://github.com/CycloneDX/cyclonedx-conan/actions/workflows/ci.yml)\n[![GitHub license](https://img.shields.io/github/license/CycloneDX/cyclonedx-conan)](https://github.com/CycloneDX/cyclonedx-conan/blob/main/LICENSE)\n[![Python Version Support](https://img.shields.io/badge/https://-cyclonedx.org-blue)](https://cyclonedx.org/)\n[![Slack Invite](https://img.shields.io/badge/Slack-Join-blue?logo=slack&labelColor=393939)](https://cyclonedx.org/slack/invite)\n![PyPI Version](https://img.shields.io/pypi/v/cyclonedx-conan?label=PyPI&logo=pypi)\n![Python Version Support](https://img.shields.io/badge/python-3.6+-blue)\n[![Group Discussion](https://img.shields.io/badge/discussion-groups.io-blue)](https://groups.io/g/CycloneDX)\n[![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Follow)](https://twitter.com/CycloneDX_Spec)\n\n----\n\nThis project provides a tool for generating CycloneDX bill-of-material JSON documents for C/C++ projects using Conan.\n\nThe BOM will contain an aggregate of all your current project's dependencies, including a full dependency graph.\n\nCycloneDX is a lightweight BOM specification that is easily created, human-readable, and simple to parse.\n\nPlease note: This tool has only been tested with Conan 1.14 so far.\n\n## Installation\n\nInstall this from [PyPi.org](https://pypi.org/project/cyclonedx-conan/) using your preferred Python package manager.\n\nExample using `pip`:\n```\npip install cyclonedx-conan\n```\n\nExample using `poetry`:\n```\npoetry add cyclonedx-conan\n```\n\n## Usage\n\nOnce installed, you can access the full documentation by running `--help`:\n\nThe command line options are aligned to the standard Conan options.\n\n```\n$ cyclonedx-conan --help\nusage: command.py [-h] [-if INSTALL_FOLDER] [-db [DRY_BUILD]] [-b [BUILD]] [-r REMOTE] [-u] [-l LOCKFILE] [--lockfile-out LOCKFILE_OUT]\n                  [-e ENV_HOST] [-e:b ENV_BUILD] [-e:h ENV_HOST] [-o OPTIONS_HOST] [-o:b OPTIONS_BUILD] [-o:h OPTIONS_HOST]\n                  [-pr PROFILE_HOST] [-pr:b PROFILE_BUILD] [-pr:h PROFILE_HOST] [-s SETTINGS_HOST] [-s:b SETTINGS_BUILD]\n                  [-s:h SETTINGS_HOST] [-c CONF_HOST] [-c:b CONF_BUILD] [-c:h CONF_HOST]\n                  path_or_reference\n\nCycloneDX SBOM Generator\n\npositional arguments:\n  path_or_reference     Path to a folder containing a recipe (conanfile.py or conanfile.txt) or to a recipe file. e.g.,\n                        ./my_project/conanfile.txt. It could also be a reference\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -if INSTALL_FOLDER, --install-folder INSTALL_FOLDER\n                        local folder containing the conaninfo.txt and conanbuildinfo.txt files (from a previous conan install execution).\n                        Defaulted to current folder, unless --profile, -s or -o is specified. If you specify both install-folder and any\n                        setting/option it will raise an error.\n  -db [DRY_BUILD], --dry-build [DRY_BUILD]\n                        Apply the --build argument to output the information, as it would be done by the install command\n  -b [BUILD], --build [BUILD]\n                        Given a build policy, return an ordered list of packages that would be built from sources during the install\n                        command\n  -r REMOTE, --remote REMOTE\n                        Look in the specified remote server\n  -u, --update          Will check if updates of the dependencies exist in the remotes (a new version that satisfies a version range, a\n                        new revision or a newer recipe if not using revisions).\n  -l LOCKFILE, --lockfile LOCKFILE\n                        Path to a lockfile\n  --lockfile-out LOCKFILE_OUT\n                        Filename of the updated lockfile\n  -e ENV_HOST, --env ENV_HOST\n                        Environment variables that will be set during the package build (host machine). e.g.: -e CXX=/usr/bin/clang++\n  -e:b ENV_BUILD, --env:build ENV_BUILD\n                        Environment variables that will be set during the package build (build machine). e.g.: -e:b CXX=/usr/bin/clang++\n  -e:h ENV_HOST, --env:host ENV_HOST\n                        Environment variables that will be set during the package build (host machine). e.g.: -e:h CXX=/usr/bin/clang++\n  -o OPTIONS_HOST, --options OPTIONS_HOST\n                        Define options values (host machine), e.g.: -o Pkg:with_qt=true\n  -o:b OPTIONS_BUILD, --options:build OPTIONS_BUILD\n                        Define options values (build machine), e.g.: -o:b Pkg:with_qt=true\n  -o:h OPTIONS_HOST, --options:host OPTIONS_HOST\n                        Define options values (host machine), e.g.: -o:h Pkg:with_qt=true\n  -pr PROFILE_HOST, --profile PROFILE_HOST\n                        Apply the specified profile to the host machine\n  -pr:b PROFILE_BUILD, --profile:build PROFILE_BUILD\n                        Apply the specified profile to the build machine\n  -pr:h PROFILE_HOST, --profile:host PROFILE_HOST\n                        Apply the specified profile to the host machine\n  -s SETTINGS_HOST, --settings SETTINGS_HOST\n                        Settings to build the package, overwriting the defaults (host machine). e.g.: -s compiler=gcc\n  -s:b SETTINGS_BUILD, --settings:build SETTINGS_BUILD\n                        Settings to build the package, overwriting the defaults (build machine). e.g.: -s:b compiler=gcc\n  -s:h SETTINGS_HOST, --settings:host SETTINGS_HOST\n                        Settings to build the package, overwriting the defaults (host machine). e.g.: -s:h compiler=gcc\n  -c CONF_HOST, --conf CONF_HOST\n                        Configuration to build the package, overwriting the defaults (host machine). e.g.: -c\n                        tools.cmake.cmaketoolchain:generator=Xcode\n  -c:b CONF_BUILD, --conf:build CONF_BUILD\n                        Configuration to build the package, overwriting the defaults (build machine). e.g.: -c:b\n                        tools.cmake.cmaketoolchain:generator=Xcode\n  -c:h CONF_HOST, --conf:host CONF_HOST\n                        Configuration to build the package, overwriting the defaults (host machine). e.g.: -c:h\n                        tools.cmake.cmaketoolchain:generator=Xcode\n```\n\n\n## Python Support\n\nWe endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).\nHowever, some features may not be possible/present in older Python versions due to their lack of support.\n\n## Copyright & License\n\nCycloneDX BOM is Copyright (c) OWASP Foundation. All Rights Reserved.\n\nPermission to modify and redistribute is granted under the terms of the Apache 2.0 license.",
-    'author': 'Patrick Dwyer',
-    'author_email': 'patrick.dwyer@owasp.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/CycloneDX/cyclonedx-conan',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

