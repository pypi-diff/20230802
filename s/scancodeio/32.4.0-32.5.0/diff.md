# Comparing `tmp/scancodeio-32.4.0.tar.gz` & `tmp/scancodeio-32.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scancodeio-32.4.0.tar", last modified: Thu Jul 13 14:59:31 2023, max compression
+gzip compressed data, was "scancodeio-32.5.0.tar", last modified: Wed Aug  2 20:07:41 2023, max compression
```

## Comparing `scancodeio-32.4.0.tar` & `scancodeio-32.5.0.tar`

### file list

```diff
@@ -1,463 +1,466 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.353439 scancodeio-32.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.269438 scancodeio-32.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.277438 scancodeio-32.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-13 14:59:16.000000 scancodeio-32.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    36932 2023-07-13 14:59:16.000000 scancodeio-32.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-13 14:59:16.000000 scancodeio-32.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 14:59:16.000000 scancodeio-32.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 14:59:16.000000 scancodeio-32.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-13 14:59:16.000000 scancodeio-32.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-13 14:59:16.000000 scancodeio-32.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-13 14:59:31.353439 scancodeio-32.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-13 14:59:16.000000 scancodeio-32.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docker.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.281438 scancodeio-32.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/application-settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/built-in-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/command-line-interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/custom-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/data-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/distros-os-images.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.285438 scancodeio-32.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   347827 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/license-clarity-scan-summary.png
--rw-r--r--   0 runner    (1001) docker     (123)   113257 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/output-files-download-results.png
--rw-r--r--   0 runner    (1001) docker     (123)    49405 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/output-files-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    59030 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/output-files-xlsx-packages.png
--rw-r--r--   0 runner    (1001) docker     (123)    56604 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/output-files-xlsx-resources.png
--rw-r--r--   0 runner    (1001) docker     (123)   161773 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    45598 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
--rw-r--r--   0 runner    (1001) docker     (123)    78178 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
--rw-r--r--   0 runner    (1001) docker     (123)    47458 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-license-policies-results.png
--rw-r--r--   0 runner    (1001) docker     (123)   148235 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-errors-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-packages-charts.png
--rw-r--r--   0 runner    (1001) docker     (123)   115814 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-packages-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    86303 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-project-details.png
--rw-r--r--   0 runner    (1001) docker     (123)   152148 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-project-form.png
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-project-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    50351 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (123)   165263 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-resources-charts.png
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-resources-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)   191624 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/tutorial-web-ui-run-log-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-archive-action.png
--rw-r--r--   0 runner    (1001) docker     (123)   127740 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-archive-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)   153488 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-create-project.png
--rw-r--r--   0 runner    (1001) docker     (123)    52651 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-delete-action.png
--rw-r--r--   0 runner    (1001) docker     (123)   108653 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-delete-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)    51714 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-project-details.png
--rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-project-list-empty.png
--rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-project-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    52920 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-reset-action.png
--rw-r--r--   0 runner    (1001) docker     (123)    93458 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/images/user-interface-reset-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/output-files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/project-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/rest-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/scanpipe-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/scanpipe-pipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_api_analyze_package_archive.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_cli_analyze_codebase.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_cli_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_license_policies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_vulnerablecode_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_web_ui_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/tutorial_web_ui_review_scan_results.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-13 14:59:16.000000 scancodeio-32.4.0/docs/user-interface.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.269438 scancodeio-32.4.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.269438 scancodeio-32.4.0/etc/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.285438 scancodeio-32.4.0/etc/nginx/conf.d/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/nginx/conf.d/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.285438 scancodeio-32.4.0/etc/nginx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/nginx/examples/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.293438 scancodeio-32.4.0/etc/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/isc.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)  4956245 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/virtualenv.pyz
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 14:59:16.000000 scancodeio-32.4.0/etc/thirdparty/virtualenv.pyz.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-07-13 14:59:16.000000 scancodeio-32.4.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scan.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.293438 scancodeio-32.4.0/scancodeio/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/scan.NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.301438 scancodeio-32.4.0/scancodeio/static/
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   422462 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/ace-1.20.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)   368864 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/ace-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/add-inputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/billboard-3.0.1-datalab.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   465309 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   207302 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bulma-0.9.4.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bulma-toast-2.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/cc-by-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/highlight-10.6.0.css
--rw-r--r--   0 runner    (1001) docker     (123)   133121 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/highlight-10.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/highlight.js-10.6.0.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/html5sortable-0.9.17.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/htmx-1.7.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/htmx-1.7.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/static/ofl-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scancodeio/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.353439 scancodeio-32.4.0/scancodeio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-13 14:59:31.000000 scancodeio-32.4.0/scancodeio.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.301438 scancodeio-32.4.0/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.301438 scancodeio-32.4.0/scanpipe/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.269438 scancodeio-32.4.0/scanpipe/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.305438 scancodeio-32.4.0/scanpipe/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/add-input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/add-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/archive-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/create-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/create-user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/delete-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/list-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/reset-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/show-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/management/commands/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.309438 scancodeio-32.4.0/scanpipe/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0002_run_id_and_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0003_remove_run_run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0004_run_pipeline_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0005_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0008_package_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0011_codebaseresource_is_media.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0012_run_scancodeio_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0013_project_is_archived.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0014_webhooksubscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0018_codebaseresource_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0019_auto_20220804_1836.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0021_codebaseresource_package_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0023_migrate_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0026_run_current_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0028_codebaserelation_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0033_project_notes_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0034_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0035_set_projects_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0036_alter_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102515 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.309438 scancodeio-32.4.0/scanpipe/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/deploy_to_develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/docker_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/find_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/inspect_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/load_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/root_filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/scan_codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipelines/scan_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.313439 scancodeio-32.4.0/scanpipe/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (123)    29336 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/js.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26528 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/pathmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/purldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/scancode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.313439 scancodeio-32.4.0/scanpipe/pipes/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    72249 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/schemas/bom-1.4.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/schemas/jsf-0.82.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    45312 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/schemas/spdx.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/vulnerablecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/pipes/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.269438 scancodeio-32.4.0/scanpipe/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.313439 scancodeio-32.4.0/scanpipe/templates/account/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.313439 scancodeio-32.4.0/scanpipe/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/registration/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.313439 scancodeio-32.4.0/scanpipe/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.317438 scancodeio-32.4.0/scanpipe/templates/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/app_monitoring.html
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/attribution.html
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/dependency_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/dependency_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/error_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.321439 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/dropdown_hoverable.html
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/file_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/filter_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/filter_dropdown_choices_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/filter_sort.html
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/help_dropdown_tooltip.html
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/navbar_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/pagination_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_codebase.html
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_downloads.html
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_inputs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_list_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_pipelines.html
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/resource_status_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/search_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/package_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/package_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/project_charts.html
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/project_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/project_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/project_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/project_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/relation_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/resource_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/resource_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.325439 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/field_default.html
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_default.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_image.html
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tabset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.325439 scancodeio-32.4.0/scanpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.341439 scancodeio-32.4.0/scanpipe/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   218206 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    85041 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (123)    82019 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    86996 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
--rw-r--r--   0 runner    (1001) docker     (123)    87965 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
--rw-r--r--   0 runner    (1001) docker     (123)    88140 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/basic-rootfs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47208 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
--rw-r--r--   0 runner    (1001) docker     (123)  1447917 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/centos.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)  5818290 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/centos_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/codebase/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/codebase/a.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/codebase/b.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/codebase/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/missing_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.273438 scancodeio-32.4.0/scanpipe/tests/data/d2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/
--rw-r--r--   0 runner    (1001) docker     (123)    46892 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
--rw-r--r--   0 runner    (1001) docker     (123)    37100 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/d2d/find_java_packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/d2d/jars/
--rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
--rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.273438 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/from/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/from/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.345439 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    54605 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/debian.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/debian_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)    57175 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    25250 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)   176984 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)    81029 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/flume-ng-node-d2d.json
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/foobar.qcow2.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    62008 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1674755 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)    16287 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/jvm/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/jvm/common.java
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/jvm/no-package.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/package.expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/poor_values.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/toml.json
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/manifests/toml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    30726 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/notice.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/outputs/expected_attribution.html
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/outputs/render_me.html
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/policies.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/scancode/
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/data/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/settings/scancode-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/data/windows-container-rootfs.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.349439 scancodeio-32.4.0/scanpipe/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/profile_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/raise_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/register_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipelines/steps_as_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:31.353439 scancodeio-32.4.0/scanpipe/tests/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_pathmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_rootfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_scancode.py
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/pipes/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/regen_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    33923 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    24121 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37204 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    32068 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    55255 2023-07-13 14:59:16.000000 scancodeio-32.4.0/scanpipe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 14:59:31.357439 scancodeio-32.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-13 14:59:16.000000 scancodeio-32.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.494755 scancodeio-32.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.502755 scancodeio-32.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-08-02 20:07:32.000000 scancodeio-32.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-02 20:07:32.000000 scancodeio-32.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 20:07:32.000000 scancodeio-32.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-02 20:07:32.000000 scancodeio-32.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-08-02 20:07:32.000000 scancodeio-32.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 20:07:32.000000 scancodeio-32.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-02 20:07:41.566756 scancodeio-32.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-02 20:07:32.000000 scancodeio-32.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docker.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.506755 scancodeio-32.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/application-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/built-in-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/command-line-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/custom-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/data-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/distros-os-images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   347827 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/license-clarity-scan-summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113257 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-download-results.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49405 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59030 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-xlsx-packages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56604 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-xlsx-resources.png
+-rw-r--r--   0 runner    (1001) docker     (123)   161773 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45598 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78178 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47458 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-license-policies-results.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148235 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-errors-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-charts.png
+-rw-r--r--   0 runner    (1001) docker     (123)   115814 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86303 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   152148 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-form.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50351 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   165263 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-charts.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)   191624 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-run-log-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-archive-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127740 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-archive-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)   153488 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-create-project.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52651 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-delete-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108653 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-delete-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51714 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-list-empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52920 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-reset-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93458 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-reset-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/output-files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/project-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/rest-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/scanpipe-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/scanpipe-pipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_api_analyze_package_archive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_cli_analyze_codebase.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_cli_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_license_policies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_vulnerablecode_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_web_ui_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_web_ui_review_scan_results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/user-interface.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.494755 scancodeio-32.5.0/etc/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/etc/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/nginx/conf.d/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/etc/nginx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/nginx/examples/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.518755 scancodeio-32.5.0/etc/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/isc.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)  4956245 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-08-02 20:07:32.000000 scancodeio-32.5.0/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scan.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.518755 scancodeio-32.5.0/scancodeio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/scan.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scancodeio/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   422462 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)   368864 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/add-inputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1-datalab.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   465309 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   207302 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/cc-by-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   133121 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight.js-10.6.0.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ofl-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scancodeio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-08-02 20:07:41.000000 scancodeio-32.5.0/scancodeio.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scanpipe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.526755 scancodeio-32.5.0/scanpipe/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/add-input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/add-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/archive-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/create-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/create-user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/delete-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/list-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/reset-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/show-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.530755 scancodeio-32.5.0/scanpipe/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0002_run_id_and_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0003_remove_run_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0004_run_pipeline_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0005_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0008_package_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0011_codebaseresource_is_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0012_run_scancodeio_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0013_project_is_archived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0014_webhooksubscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0018_codebaseresource_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0019_auto_20220804_1836.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0021_codebaseresource_package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0023_migrate_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0026_run_current_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0028_codebaserelation_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0033_project_notes_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0034_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0035_set_projects_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0036_alter_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103111 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.530755 scancodeio-32.5.0/scanpipe/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/deploy_to_develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/docker_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/find_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/inspect_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/load_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/populate_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/root_filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_codebase_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/purldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/scancode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/pipes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    72249 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/bom-1.4.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/jsf-0.82.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45312 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/spdx.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/vulnerablecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/registration/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.538756 scancodeio-32.5.0/scanpipe/templates/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/app_monitoring.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/attribution.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/error_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.542755 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/dropdown_hoverable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/file_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_dropdown_choices_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_sort.html
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/help_dropdown_tooltip.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/navbar_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_codebase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_downloads.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_list_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_status_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/search_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/package_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/package_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_charts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/relation_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.542755 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tabset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.546756 scancodeio-32.5.0/scanpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   218206 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85063 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82019 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    86996 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    87965 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88140 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    47288 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1447917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/centos.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  5818290 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/centos_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/codebase/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/a.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/b.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/missing_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/tests/data/d2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    56205 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    37100 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/
+-rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    54605 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/debian.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/debian_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57175 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25250 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   176984 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81029 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/flume-ng-node-d2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/foobar.qcow2.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    62008 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1674755 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16287 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/jvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/jvm/common.java
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/jvm/no-package.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/package.expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/poor_values.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    30726 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/notice.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/expected_attribution.html
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/render_me.html
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/policies.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/data/scancode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/data/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/settings/scancode-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/windows-container-rootfs.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/profile_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/raise_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/register_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/steps_as_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27970 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_scancode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/regen_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34966 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24121 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90466 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39094 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34599 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-02 20:07:41.570756 scancodeio-32.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-08-02 20:07:32.000000 scancodeio-32.5.0/setup.py
```

### Comparing `scancodeio-32.4.0/.github/workflows/ci.yml` & `scancodeio-32.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/.github/workflows/pypi-release.yml` & `scancodeio-32.5.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/.gitignore` & `scancodeio-32.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/.readthedocs.yaml` & `scancodeio-32.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/CHANGELOG.rst` & `scancodeio-32.5.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,53 @@
 Changelog
 =========
 
-v32.5.0 (unreleased)
+v32.5.0 (2023-08-02)
 --------------------
 
+WARNING: After upgrading the ScanCode.io codebase to this version,
+and following the ``docker compose build``,
+the permissions of the ``/var/scancodeio/`` directory of the Docker volumes require
+to be updated for the new ``app`` user, using:
+``docker compose run -u 0:0 web chown -R app:app /var/scancodeio/``
+
+- Run Docker as non-root user using virtualenv.
+  WARNING: The permissions of the ``/var/scancodeio/`` directory in the Docker volumes
+  require to be updated for the new ``app`` user.
+  https://github.com/nexB/scancode.io/issues/399
+
+- Add column sort and filters in dependency list view.
+  https://github.com/nexB/scancode.io/issues/823
+
+- Add a new ``ScanCodebasePackage`` pipeline to scan a codebase for packages only.
+  https://github.com/nexB/scancode.io/issues/815
+
+- Add new ``outputs`` REST API action that list projects output files including an URL
+  to download the file.
+  https://github.com/nexB/scancode.io/issues/678
+
+- Add support for multiple to/from input files in the ``deploy_to_develop`` pipeline.
+  https://github.com/nexB/scancode.io/issues/813
+
+- Add the ability to delete and download project inputs.
+  Note that the inputs cannot be modified (added or deleted) once a pipeline run as
+  started on the project.
+  https://github.com/nexB/scancode.io/issues/813
+
+- Fix root_filesystem data structure stored on the Project ``extra_data`` field.
+  This was causing a conflict with the expected docker images data structure
+  when generating an XLSX output.
+  https://github.com/nexB/scancode.io/issues/824
+
+- Fix the SPDX output to include missing detailed license texts for LicenseRef.
+  Add ``licensedb_url`` and ``scancode_url`` to the SPDX ``ExtractedLicensingInfo``
+  ``seeAlsos``.
+  Include the ``Package.notice_text`` as the SPDX ``attribution_texts``.
+  https://github.com/nexB/scancode.io/issues/841
+
 v32.4.0 (2023-07-13)
 --------------------
 
 - Add support for license policies and complaince alert for Discovered Packages.
   https://github.com/nexB/scancode.io/issues/151
 
 - Refine the details views and tabs:
```

### Comparing `scancodeio-32.4.0/Dockerfile` & `scancodeio-32.5.0/scanpipe/pipes/compliance.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,52 +16,44 @@
 # OR CONDITIONS OF ANY KIND, either express or implied. No content created from
 # ScanCode.io should be considered or used as legal advice. Consult an Attorney
 # for any legal advice.
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
-FROM --platform=linux/amd64 python:3.11
+from scanpipe.pipes import flag
+from scanpipe.pipes import scancode
 
-LABEL org.opencontainers.image.source=https://github.com/nexB/scancode.io
-LABEL org.opencontainers.image.description="ScanCode.io"
-LABEL org.opencontainers.image.licenses="Apache-2.0"
-
-WORKDIR /app
-
-# Python settings: force unbuffered stdout and stderr (i.e. they are flushed to terminal immediately)
-ENV PYTHONUNBUFFERED 1
-# Python settings: do not write pyc files
-ENV PYTHONDONTWRITEBYTECODE 1
-# Add the workdir in the Python path for scancodeio modules availability in entry points
-ENV PYTHONPATH "${PYTHONPATH}:/app"
-
-# OS requirements as per
-# https://scancode-toolkit.readthedocs.io/en/latest/getting-started/install.html
-RUN apt-get update \
- && apt-get install -y --no-install-recommends \
-       bzip2 \
-       xz-utils \
-       zlib1g \
-       libxml2-dev \
-       libxslt1-dev \
-       libgomp1 \
-       libsqlite3-0 \
-       libgcrypt20 \
-       libpopt0 \
-       libzstd1 \
-       libgpgme11 \
-       libdevmapper1.02.1 \
-       libguestfs-tools \
-       linux-image-amd64 \
-       wait-for-it \
- && apt-get clean \
- && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
-
-RUN mkdir -p /var/scancodeio/static/ \
- && mkdir -p /var/scancodeio/workspace/
-
-# Keep the dependencies installation before the COPY of the app/ for proper caching
-COPY setup.cfg setup.py /app/
-RUN pip install .
+"""
+A common compliance pattern for images is to store known licenses in a /licenses
+directory and the corresponding source code archives, for packages that are
+redistributable in source form, in a /sourcemirror directory; both at the root of
+an image (VM or container image).
 
-COPY . /app
+Usage example within a Pipeline:
+
+def analyze_licenses_and_sources(self):
+    util.flag_compliance_files(self.project)
+    util.analyze_compliance_licenses(self.project)
+"""
+
+
+def flag_compliance_files(project):
+    """Flag compliance files status for the provided `project`."""
+    compliance_dirs = {
+        "/licenses": flag.COMPLIANCE_LICENSES,
+        "/sourcemirror": flag.COMPLIANCE_SOURCEMIRROR,
+    }
+
+    qs = project.codebaseresources.no_status()
+
+    for path, status in compliance_dirs.items():
+        qs.filter(rootfs_path__startswith=path).update(status=status)
+
+
+def analyze_compliance_licenses(project):
+    """Scan compliance licenses status for the provided `project`."""
+    qs = project.codebaseresources.status(flag.COMPLIANCE_LICENSES)
+
+    for codebase_resource in qs:
+        scan_results, scan_errors = scancode.scan_file(codebase_resource.location)
+        codebase_resource.set_scan_results(scan_results)
```

### Comparing `scancodeio-32.4.0/LICENSE` & `scancodeio-32.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/Makefile` & `scancodeio-32.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/NOTICE` & `scancodeio-32.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/PKG-INFO` & `scancodeio-32.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scancodeio
-Version: 32.4.0
+Version: 32.5.0
 Summary: Automate software composition analysis pipelines
 Home-page: https://github.com/nexB/scancode.io
 Author: nexB Inc.
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,scan,license,package,dependency,copyright,filetype,author,extract,licensing,scancode,scanpipe,docker,rootfs,vm,virtual machine,pipeline,code analysis,container
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scancodeio-32.4.0/README.rst` & `scancodeio-32.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docker-compose.yml` & `scancodeio-32.5.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/Makefile` & `scancodeio-32.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/application-settings.rst` & `scancodeio-32.5.0/docs/application-settings.rst`

 * *Files 4% similar despite different names*

```diff
@@ -268,16 +268,34 @@
 
     TIME_ZONE=Europe/Paris
 
 .. note::
     You can view a detailed list of time zones `here.
     <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones>`_
 
+.. _scancodeio_settings_purldb:
+
+PURLDB
+------
+
+Provide the URL and API key of your `PurlDB <https://github.com/nexB/purldb/>`_
+instance.
+
+ ::
+
+    PURLDB_URL=https://your-purldb-domain/
+    PURLDB_API_KEY=apikeyexample
+
+.. _scancodeio_settings_vulnerablecode:
+
 VULNERABLECODE
 --------------
 
-You can either run your own instance of VulnerableCode or connect to the public one.
+You can either run your own instance of
+`VulnerableCode <https://github.com/nexB/vulnerablecode/>`_
+or connect to the public one.
+
 Authentication is provided using an API key that you can obtain by registering at
 https://public.vulnerablecode.io/account/request_api_key/ ::
 
     VULNERABLECODE_URL=https://public.vulnerablecode.io/
-    VULNERABLECODE_API_KEY=c1fa7dc1fd0a408880ba2dfdf63c1124abca9477
+    VULNERABLECODE_API_KEY=apikeyexample
```

### Comparing `scancodeio-32.4.0/docs/command-line-interface.rst` & `scancodeio-32.5.0/docs/command-line-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/conf.py` & `scancodeio-32.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/contributing.rst` & `scancodeio-32.5.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/custom-pipelines.rst` & `scancodeio-32.5.0/docs/custom-pipelines.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/data-models.rst` & `scancodeio-32.5.0/docs/data-models.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/distros-os-images.rst` & `scancodeio-32.5.0/docs/distros-os-images.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/license-clarity-scan-summary.png` & `scancodeio-32.5.0/docs/images/license-clarity-scan-summary.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/output-files-download-results.png` & `scancodeio-32.5.0/docs/images/output-files-download-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/output-files-projects-list.png` & `scancodeio-32.5.0/docs/images/output-files-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/output-files-xlsx-packages.png` & `scancodeio-32.5.0/docs/images/output-files-xlsx-packages.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/output-files-xlsx-resources.png` & `scancodeio-32.5.0/docs/images/output-files-xlsx-resources.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-extra-data.png` & `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-extra-data.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-icon-link.png` & `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-icon-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-find-vulnerabilities-packages-link.png` & `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-packages-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-license-policies-results.png` & `scancodeio-32.5.0/docs/images/tutorial-license-policies-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-errors-list.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-errors-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-packages-charts.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-packages-list.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-project-details.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-project-form.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-form.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-project-list.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-projects-list.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-resources-charts.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-resources-filter.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-filter.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/tutorial-web-ui-run-log-modal.png` & `scancodeio-32.5.0/docs/images/tutorial-web-ui-run-log-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-archive-action.png` & `scancodeio-32.5.0/docs/images/user-interface-archive-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-archive-modal.png` & `scancodeio-32.5.0/docs/images/user-interface-archive-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-create-project.png` & `scancodeio-32.5.0/docs/images/user-interface-create-project.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-delete-action.png` & `scancodeio-32.5.0/docs/images/user-interface-delete-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-delete-modal.png` & `scancodeio-32.5.0/docs/images/user-interface-delete-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-project-details.png` & `scancodeio-32.5.0/docs/images/user-interface-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-project-list-empty.png` & `scancodeio-32.5.0/docs/images/user-interface-project-list-empty.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-project-list.png` & `scancodeio-32.5.0/docs/images/user-interface-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-reset-action.png` & `scancodeio-32.5.0/docs/images/user-interface-reset-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/images/user-interface-reset-modal.png` & `scancodeio-32.5.0/docs/images/user-interface-reset-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/index.rst` & `scancodeio-32.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/installation.rst` & `scancodeio-32.5.0/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,14 @@
     make envfile
     docker compose build
 
 .. warning::
     As the ``docker-compose`` v1 command is officially deprecated by Docker, you will
     only find references to the ``docker compose`` v2 command in this documentation.
 
-.. note::
-    You need to rebuild the image whenever ScanCode.io's source code has been
-    modified or updated::
-
-        docker compose build
-
 Run the App
 ^^^^^^^^^^^
 
 **Run your image** as a container::
 
     docker compose up
 
@@ -80,14 +74,21 @@
 
     **Make sure to allow enough memory to support each CPU processes**.
 
     A good rule of thumb is to allow **1 GB of memory per CPU**.
     For example, if Docker is configured for 8 CPUs, a minimum of 8 GB of memory is
     required.
 
+.. tip::
+    By default, ScanCode.io starts only 1 worker, which means only 1 pipeline will be
+    executed at a time. If you wish to start more workers, use the following command,
+    replacing the number 2 with the desired number of workers::
+
+        docker compose up --scale worker=2
+
 .. warning::
     To access a dockerized ScanCode.io app from a remote location, the ``ALLOWED_HOSTS``
     and ``CSRF_TRUSTED_ORIGINS`` settings need to be provided in your ``.env`` file,
     for example::
 
         ALLOWED_HOSTS=.your-domain.com,localhost,127.0.0.1
         CSRF_TRUSTED_ORIGINS=https://*.your-domain.com,http://127.0.0.1:8001
@@ -100,14 +101,38 @@
 .. tip::
     If you run ScanCode.io on desktop or laptop, it may come handy to pause/unpause
     or suspend your local ScanCode.io system. For this, use these commands::
 
         docker compose pause  # to pause/suspend
         docker compose unpause  # to unpause/resume
 
+Upgrade the App
+^^^^^^^^^^^^^^^
+
+**Update your local** `ScanCode.io repo <https://github.com/nexB/scancode.io>`_,
+and **build the Docker image**::
+
+    cd scancode.io
+    git pull
+    docker compose build
+
+.. warning::
+    The Docker image has been updated to run as a non-root user.
+    If you encounter "permissions" issues while running the ScanCode.io Docker images
+    following the ``docker compose build``, you will need to update the the permissions
+    of the ``/var/scancodeio/`` directory of the Docker volumes using::
+
+        docker compose run -u 0:0 web chown -R app:app /var/scancodeio/
+
+    See also https://github.com/nexB/scancode.io/issues/399
+
+.. note::
+    You need to rebuild the image whenever ScanCode.io's source code has been
+    modified or updated.
+
 Execute a Command
 ^^^^^^^^^^^^^^^^^
 
 .. note::
     Refer to the :ref:`command_line_interface` section for the full list of commands.
 
 A ``scanpipe`` command can be executed through the ``docker compose`` command line
```

### Comparing `scancodeio-32.4.0/docs/introduction.rst` & `scancodeio-32.5.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/make.bat` & `scancodeio-32.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/output-files.rst` & `scancodeio-32.5.0/docs/output-files.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/project-configuration.rst` & `scancodeio-32.5.0/docs/project-configuration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/rest-api.rst` & `scancodeio-32.5.0/docs/rest-api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,24 @@
             "pipeline": "scan_package",
             "execute_now": True,
         }
         files = {"upload_file": open("/path/to/the/archive.zip", "rb")}
         response = requests.post(api_url, data=data, files=files)
         response.json()
 
+    You have the flexibility to explicitly set the filename, content_type, and
+    headers for your uploaded files using the following code:
+
+    .. code-block:: python
+
+        files = {"upload_file": ("inventory.json", file_contents, "application/json")}
+
+    For more information on this topic, refer to the following link:
+    https://docs.python-requests.org/en/latest/user/quickstart/#post-a-multipart-encoded-file
+
 When creating a project, the response will include the project's details URL
 value among the returned data.
 You can make a GET request to this URL, which returns all available information
 about the project, including the status of any pipeline run:
 
 .. code-block:: json
```

### Comparing `scancodeio-32.4.0/docs/scanpipe-concepts.rst` & `scancodeio-32.5.0/docs/scanpipe-concepts.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/scanpipe-pipes.rst` & `scancodeio-32.5.0/docs/scanpipe-pipes.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_api_analyze_package_archive.rst` & `scancodeio-32.5.0/docs/tutorial_api_analyze_package_archive.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_cli_analyze_codebase.rst` & `scancodeio-32.5.0/docs/tutorial_cli_analyze_codebase.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_cli_analyze_docker_image.rst` & `scancodeio-32.5.0/docs/tutorial_cli_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_license_policies.rst` & `scancodeio-32.5.0/docs/tutorial_license_policies.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_vulnerablecode_integration.rst` & `scancodeio-32.5.0/docs/tutorial_vulnerablecode_integration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_web_ui_analyze_docker_image.rst` & `scancodeio-32.5.0/docs/tutorial_web_ui_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/tutorial_web_ui_review_scan_results.rst` & `scancodeio-32.5.0/docs/tutorial_web_ui_review_scan_results.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/docs/user-interface.rst` & `scancodeio-32.5.0/docs/user-interface.rst`

 * *Files 2% similar despite different names*

```diff
@@ -109,18 +109,17 @@
 You can specify a list of items to be ignored during pipeline execution,
 ensuring that only relevant content is considered.
 Furthermore, you have the option to customize the attribution template according to
 your specific requirements.
 
 
 .. tip::
-    Our documentation is treated like code. Make sure to check our
-    `writing guidelines <https://scancode-toolkit.readthedocs.io/en/latest/contribute/contrib_doc.html>`_
-    to help guide new users.
-
+    To generate the project configuration file ``scancode-config.yml``, navigate to the
+    Project Settings UI and click on the **Config file** link in the left section under
+    **Download**.
 
 Archive a Project
 ^^^^^^^^^^^^^^^^^
 
 After a project is complete, you may want to archive it to prevent any further
 modification to that project.
```

### Comparing `scancodeio-32.4.0/etc/nginx/examples/ssl.conf` & `scancodeio-32.5.0/etc/nginx/examples/ssl.conf`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/apache-2.0.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/bsd-new.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/bsd-simplified.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/isc.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/isc.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/lgpl-2.1-plus.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/lgpl-2.1-plus.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/mit.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/python.LICENSE` & `scancodeio-32.5.0/etc/thirdparty/python.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/virtualenv.pyz` & `scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/etc/thirdparty/virtualenv.pyz.ABOUT` & `scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/__init__.py` & `scancodeio-32.5.0/scancodeio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import os
 import subprocess
 import sys
 import warnings
 from pathlib import Path
 
-VERSION = "32.4.0"
+VERSION = "32.5.0"
 
 PROJECT_DIR = Path(__file__).resolve().parent
 ROOT_DIR = PROJECT_DIR.parent
 SCAN_NOTICE = PROJECT_DIR.joinpath("scan.NOTICE").read_text()
 
 
 def get_version(version):
```

### Comparing `scancodeio-32.4.0/scancodeio/auth.py` & `scancodeio-32.5.0/scancodeio/auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/context_processors.py` & `scancodeio-32.5.0/scancodeio/context_processors.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/licenses.py` & `scancodeio-32.5.0/scancodeio/licenses.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/settings.py` & `scancodeio-32.5.0/scancodeio/settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js` & `scancodeio-32.5.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/ace-1.20.0.min.js` & `scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/ace-1.9.5.min.js` & `scancodeio-32.5.0/scancodeio/static/ace-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/add-inputs.js` & `scancodeio-32.5.0/scancodeio/static/add-inputs.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/billboard-3.0.1-datalab.min.css` & `scancodeio-32.5.0/scancodeio/static/billboard-3.0.1-datalab.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/billboard-3.0.1.pkgd.min.js` & `scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bsd-new.LICENSE` & `scancodeio-32.5.0/scancodeio/static/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bsd-simplified.LICENSE` & `scancodeio-32.5.0/scancodeio/static/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bulma-0.9.4.min.css` & `scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT` & `scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bulma-toast-2.4.1.min.js` & `scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT` & `scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/cc-by-4.0.LICENSE` & `scancodeio-32.5.0/scancodeio/static/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/favicon.ico` & `scancodeio-32.5.0/scancodeio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/highlight-10.6.0.css` & `scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/highlight-10.6.0.min.js` & `scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/html5sortable-0.9.17.min.js` & `scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT` & `scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/htmx-1.7.0.min.js` & `scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/main.js` & `scancodeio-32.5.0/scancodeio/static/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -177,29 +177,30 @@
     background.style.cssText = "z-index:100;color:white;text-align:center;padding-top:150px;position:fixed;";
     background.innerHTML = '<div class="fa-5x"><i class="fas fa-circle-notch fa-spin"></i></div>';
     document.body.appendChild(background);
     return background;
 }
 
 // Display and update the `$progress` object on `$form` submitted using XHR
-function displayFormUploadProgress($form, $progress, $form_errors) {
+function displayFormUploadProgress($form, $progress, $form_errors, update_title = false) {
 
     // Prepare an AJAX request to submit the form and track the progress
     let xhr = new XMLHttpRequest();
 
     // Submit the form using initial form attributes
     xhr.open($form.getAttribute('method'), $form.getAttribute('action'), true);
     xhr.setRequestHeader('X-Requested-With', 'XMLHttpRequest');
 
     xhr.upload.addEventListener('progress', function(event) {
         console.log("XHR progress event fired");
         // Compute the progress percentage and set the value on the `progress` element
         if (event.lengthComputable) {
             let percent = (event.loaded / event.total * 100).toFixed();
             $progress.setAttribute('value', percent);
+            if (update_title) document.title = `Uploading: ${percent}% - ScanCode.io`;
         }
     }, false);
 
     xhr.addEventListener('readystatechange', function(event) {
         let target = event.target;
         console.log("XHR readystatechange event fired");
```

### Comparing `scancodeio-32.4.0/scancodeio/static/mit.LICENSE` & `scancodeio-32.5.0/scancodeio/static/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/static/ofl-1.1.LICENSE` & `scancodeio-32.5.0/scancodeio/static/ofl-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/urls.py` & `scancodeio-32.5.0/scancodeio/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/worker.py` & `scancodeio-32.5.0/scancodeio/worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio/wsgi.py` & `scancodeio-32.5.0/scancodeio/wsgi.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scancodeio.egg-info/SOURCES.txt` & `scancodeio-32.5.0/scancodeio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,18 @@
 scanpipe/pipelines/__init__.py
 scanpipe/pipelines/deploy_to_develop.py
 scanpipe/pipelines/docker.py
 scanpipe/pipelines/docker_windows.py
 scanpipe/pipelines/find_vulnerabilities.py
 scanpipe/pipelines/inspect_manifest.py
 scanpipe/pipelines/load_inventory.py
+scanpipe/pipelines/populate_purldb.py
 scanpipe/pipelines/root_filesystems.py
 scanpipe/pipelines/scan_codebase.py
+scanpipe/pipelines/scan_codebase_package.py
 scanpipe/pipelines/scan_package.py
 scanpipe/pipes/__init__.py
 scanpipe/pipes/codebase.py
 scanpipe/pipes/compliance.py
 scanpipe/pipes/cyclonedx.py
 scanpipe/pipes/d2d.py
 scanpipe/pipes/docker.py
@@ -260,14 +262,15 @@
 scanpipe/templates/scanpipe/includes/pagination_header_relations.html
 scanpipe/templates/scanpipe/includes/project_archive_modal.html
 scanpipe/templates/scanpipe/includes/project_codebase.html
 scanpipe/templates/scanpipe/includes/project_delete_modal.html
 scanpipe/templates/scanpipe/includes/project_download_dropdown.html
 scanpipe/templates/scanpipe/includes/project_downloads.html
 scanpipe/templates/scanpipe/includes/project_inputs.html
+scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html
 scanpipe/templates/scanpipe/includes/project_list_table.html
 scanpipe/templates/scanpipe/includes/project_pipelines.html
 scanpipe/templates/scanpipe/includes/project_reset_modal.html
 scanpipe/templates/scanpipe/includes/project_settings_menu.html
 scanpipe/templates/scanpipe/includes/project_summary_level.html
 scanpipe/templates/scanpipe/includes/resource_chart_column.html
 scanpipe/templates/scanpipe/includes/resource_file_viewer.html
```

### Comparing `scancodeio-32.4.0/scanpipe/__init__.py` & `scancodeio-32.5.0/scanpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/api/__init__.py` & `scancodeio-32.5.0/scanpipe/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/api/serializers.py` & `scancodeio-32.5.0/scanpipe/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         """
         Create a new `project` with `upload_file` and `pipeline` as optional.
 
         The `execute_now` parameter can be set to execute the Pipeline on creation.
         Note that even when `execute_now` is True, the pipeline execution is always
         delayed after the actual database save and commit of the Project creation
         process, using the `transaction.on_commit` callback system.
-        This ensure the Project data integrity before running any pipelines.
+        This ensures the Project data integrity before running any pipelines.
         """
         upload_file = validated_data.pop("upload_file", None)
         input_urls = validated_data.pop("input_urls", [])
         pipeline = validated_data.pop("pipeline", None)
         execute_now = validated_data.pop("execute_now", False)
         webhook_url = validated_data.pop("webhook_url", None)
```

### Comparing `scancodeio-32.4.0/scanpipe/api/views.py` & `scancodeio-32.5.0/scanpipe/api/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import json
 
 from django.apps import apps
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models import Q
+from django.http import FileResponse
 
 import django_filters
 from rest_framework import mixins
 from rest_framework import renderers
 from rest_framework import status
 from rest_framework import viewsets
 from rest_framework.decorators import action
@@ -250,15 +251,15 @@
         }
         return Response(message, status=status.HTTP_400_BAD_REQUEST)
 
     @action(detail=True, methods=["get", "post"])
     def add_input(self, request, *args, **kwargs):
         project = self.get_object()
 
-        if not project.can_add_input:
+        if not project.can_change_inputs:
             message = {
                 "status": "Cannot add inputs once a pipeline has started to execute."
             }
             return Response(message, status=status.HTTP_400_BAD_REQUEST)
 
         upload_file = request.data.get("upload_file")
         input_urls = request.data.get("input_urls", [])
@@ -324,14 +325,33 @@
             return Response(error, status=status.HTTP_400_BAD_REQUEST)
         else:
             message = (
                 f"All data, except inputs, for the {project} project have been removed."
             )
             return Response({"status": message})
 
+    @action(detail=True, methods=["get"])
+    def outputs(self, request, *args, **kwargs):
+        project = self.get_object()
+
+        if filename := request.query_params.get("filename"):
+            file_path = project.output_path / filename
+            if file_path.exists():
+                return FileResponse(file_path.open("rb"))
+
+            message = {"status": f"Output file {filename} not found"}
+            return Response(message, status=status.HTTP_400_BAD_REQUEST)
+
+        action_url = self.reverse_action(self.outputs.url_name, args=[project.pk])
+        output_data = [
+            {"filename": output, "download_url": f"{action_url}?filename={output}"}
+            for output in project.output_root
+        ]
+        return Response(output_data)
+
 
 class RunViewSet(mixins.RetrieveModelMixin, viewsets.GenericViewSet):
     """Add actions to the Run viewset."""
 
     queryset = Run.objects.all()
     serializer_class = RunSerializer
```

### Comparing `scancodeio-32.4.0/scanpipe/apps.py` & `scancodeio-32.5.0/scanpipe/apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/filters.py` & `scancodeio-32.5.0/scanpipe/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,18 +43,99 @@
 
 PAGE_VAR = "page"
 EMPTY_VAR = "_EMPTY_"
 ANY_VAR = "_ANY_"
 OTHER_VAR = "_OTHER_"
 
 
+class ParentAllValuesFilter(django_filters.ChoiceFilter):
+    """
+    Similar to ``django_filters.AllValuesFilter`` but using the queryset of the parent
+    ``FilterSet``.
+    """
+
+    @property
+    def field(self):
+        qs = self.parent.queryset.distinct()
+        qs = qs.order_by(self.field_name).values_list(self.field_name, flat=True)
+        self.extra["choices"] = [(o, o) for o in qs]
+        return super().field
+
+
+class StrictBooleanFilter(django_filters.ChoiceFilter):
+    def __init__(self, *args, **kwargs):
+        kwargs["choices"] = (
+            (True, _("Yes")),
+            (False, _("No")),
+        )
+        super().__init__(*args, **kwargs)
+
+
+class BulmaLinkWidget(LinkWidget):
+    """Replace LinkWidget rendering with Bulma CSS classes."""
+
+    extra_css_class = ""
+
+    def render_option(self, name, selected_choices, option_value, option_label):
+        option_value = str(option_value)
+        if option_label == BLANK_CHOICE_DASH[0][1]:
+            option_label = _("All")
+
+        data = self.data.copy()
+        data[name] = option_value
+        selected = data == self.data or option_value in selected_choices
+
+        # Do not include the pagination in the filter query string.
+        data.pop(PAGE_VAR, None)
+
+        css_class = str(self.extra_css_class)
+        if selected:
+            css_class += " is-active"
+
+        try:
+            url = data.urlencode()
+        except AttributeError:
+            url = urlencode(data, doseq=True)
+
+        return self.option_string().format(
+            css_class=css_class,
+            query_string=url,
+            label=str(option_label),
+        )
+
+    def option_string(self):
+        return '<li><a href="?{query_string}" class="{css_class}">{label}</a></li>'
+
+
+class BulmaDropdownWidget(BulmaLinkWidget):
+    extra_css_class = "dropdown-item"
+
+
+class HasValueDropdownWidget(BulmaDropdownWidget):
+    def __init__(self, attrs=None, choices=()):
+        super().__init__(attrs)
+        self.choices = (
+            ("", "All"),
+            (EMPTY_VAR, "None"),
+            (ANY_VAR, "Any"),
+        )
+
+
 class FilterSetUtilsMixin:
     empty_value = EMPTY_VAR
     any_value = ANY_VAR
     other_value = OTHER_VAR
+    dropdown_widget_class = BulmaDropdownWidget
+    dropdown_widget_fields = []
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # Set the widget class for defined ``dropdown_widget_fields``.
+        for field_name in self.dropdown_widget_fields:
+            self.filters[field_name].extra["widget"] = self.dropdown_widget_class
 
     @staticmethod
     def remove_field_from_query_dict(query_dict, field_name, remove_value=None):
         """
         For given `field_name`, returns an encoded URL without the value.
         For multi-value filters, a single value can be removed using `remove_value`.
         This URL can be used to remove a filter value from active filters.
@@ -133,65 +214,21 @@
                 return queryset.less_common(name)
             else:
                 queryset = self.filters[name].filter(queryset, value)
 
         return queryset
 
 
-class BulmaLinkWidget(LinkWidget):
-    """Replace LinkWidget rendering with Bulma CSS classes."""
-
-    extra_css_class = ""
-
-    def render_option(self, name, selected_choices, option_value, option_label):
-        option_value = str(option_value)
-        if option_label == BLANK_CHOICE_DASH[0][1]:
-            option_label = _("All")
-
-        data = self.data.copy()
-        data[name] = option_value
-        selected = data == self.data or option_value in selected_choices
-
-        # Do not include the pagination in the filter query string.
-        data.pop(PAGE_VAR, None)
-
-        css_class = str(self.extra_css_class)
-        if selected:
-            css_class += " is-active"
-
-        try:
-            url = data.urlencode()
-        except AttributeError:
-            url = urlencode(data, doseq=True)
-
-        return self.option_string().format(
-            css_class=css_class,
-            query_string=url,
-            label=str(option_label),
-        )
-
-    def option_string(self):
-        return '<li><a href="?{query_string}" class="{css_class}">{label}</a></li>'
-
-
-class BulmaDropdownWidget(BulmaLinkWidget):
-    extra_css_class = "dropdown-item"
-
-
-class HasValueDropdownWidget(BulmaDropdownWidget):
-    def __init__(self, attrs=None, choices=()):
-        super().__init__(attrs)
-        self.choices = (
-            ("", "All"),
-            (EMPTY_VAR, "None"),
-            (ANY_VAR, "Any"),
-        )
-
-
 class ProjectFilterSet(FilterSetUtilsMixin, django_filters.FilterSet):
+    dropdown_widget_fields = [
+        "sort",
+        "pipeline",
+        "status",
+    ]
+
     search = django_filters.CharFilter(
         label="Search", field_name="name", lookup_expr="icontains"
     )
     sort = django_filters.OrderingFilter(
         label="Sort",
         fields=[
             "created_date",
@@ -211,34 +248,31 @@
             ("-discovereddependencies_count", "Dependencies (+)"),
             ("discovereddependencies_count", "Dependencies (-)"),
             ("-codebaseresources_count", "Resources (+)"),
             ("codebaseresources_count", "Resources (-)"),
             ("-projecterrors_count", "Errors (+)"),
             ("projecterrors_count", "Errors (-)"),
         ),
-        widget=BulmaDropdownWidget,
     )
     pipeline = django_filters.ChoiceFilter(
         label="Pipeline",
         field_name="runs__pipeline_name",
         choices=scanpipe_app.get_pipeline_choices(include_blank=False),
-        widget=BulmaDropdownWidget,
         distinct=True,
     )
     status = django_filters.ChoiceFilter(
         label="Status",
         method="filter_run_status",
         choices=[
             ("not_started", "Not started"),
             ("queued", "Queued"),
             ("running", "Running"),
             ("succeed", "Success"),
             ("failed", "Failure"),
         ],
-        widget=BulmaDropdownWidget,
         distinct=True,
     )
 
     class Meta:
         model = Project
         fields = ["is_archived"]
         exclude = ["page"]
@@ -330,15 +364,15 @@
     def filter(self, qs, value):
         if value == "any":
             return qs.status()
         return super().filter(qs, value)
 
 
 class ResourceFilterSet(FilterSetUtilsMixin, django_filters.FilterSet):
-    dropdown_widget = [
+    dropdown_widget_fields = [
         "status",
         "type",
         "compliance_alert",
         "in_package",
         "relation_map_type",
     ]
 
@@ -403,25 +437,26 @@
             "license_detections",
             "license_clues",
             "percentage_of_license_text",
             "emails",
             "urls",
             "in_package",
             "relation_map_type",
+            "is_binary",
+            "is_text",
+            "is_archive",
+            "is_key_file",
+            "is_media",
         ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if status_filter := self.filters.get("status"):
             status_filter.extra.update({"choices": self.get_status_choices()})
 
-        # Set the `BulmaDropdownWidget`` widget for defined ``dropdown_widget``.
-        for field_name in self.dropdown_widget:
-            self.filters[field_name].extra["widget"] = BulmaDropdownWidget()
-
         license_expression_filer = self.filters["detected_license_expression"]
         license_expression_filer.extra["widget"] = HasValueDropdownWidget()
 
     def get_status_choices(self):
         default_choices = [
             (EMPTY_VAR, "No status"),
             ("any", "Any status"),
@@ -454,35 +489,40 @@
             return qs.filter(~Q(**{f"{self.field_name}__in": EMPTY_VALUES}))
         elif value == "no":
             return qs.filter(**{f"{self.field_name}__in": EMPTY_VALUES})
         return qs
 
 
 class PackageFilterSet(FilterSetUtilsMixin, django_filters.FilterSet):
+    dropdown_widget_fields = [
+        "is_vulnerable",
+        "compliance_alert",
+    ]
+
     search = django_filters.CharFilter(
         label="Search", field_name="name", lookup_expr="icontains"
     )
     sort = django_filters.OrderingFilter(
         label="Sort",
         fields=[
             "declared_license_expression",
             "other_license_expression",
             "compliance_alert",
             "copyright",
             "primary_language",
         ],
     )
     purl = PackageURLFilter(label="Package URL")
-    is_vulnerable = IsVulnerable(
-        field_name="affected_by_vulnerabilities",
-        widget=BulmaDropdownWidget,
-    )
+    is_vulnerable = IsVulnerable(field_name="affected_by_vulnerabilities")
     compliance_alert = django_filters.ChoiceFilter(
         choices=[(EMPTY_VAR, "None")] + CodebaseResource.Compliance.choices,
-        widget=BulmaDropdownWidget,
+    )
+    copyright = django_filters.filters.CharFilter(widget=HasValueDropdownWidget)
+    declared_license_expression = django_filters.filters.CharFilter(
+        widget=HasValueDropdownWidget
     )
 
     class Meta:
         model = DiscoveredPackage
         fields = [
             "search",
             "purl",
@@ -510,26 +550,49 @@
             "other_license_expression_spdx",
             "extracted_license_statement",
             "copyright",
             "is_vulnerable",
             "compliance_alert",
         ]
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        license_expression_filer = self.filters["declared_license_expression"]
-        license_expression_filer.extra["widget"] = HasValueDropdownWidget()
-        self.filters["copyright"].extra["widget"] = HasValueDropdownWidget()
-
 
 class DependencyFilterSet(FilterSetUtilsMixin, django_filters.FilterSet):
+    dropdown_widget_fields = [
+        "type",
+        "scope",
+        "is_runtime",
+        "is_optional",
+        "is_resolved",
+        "datasource_id",
+    ]
+
     search = django_filters.CharFilter(
         label="Search", field_name="name", lookup_expr="icontains"
     )
+    sort = django_filters.OrderingFilter(
+        label="Sort",
+        fields=[
+            "type",
+            "extracted_requirement",
+            "scope",
+            "is_runtime",
+            "is_optional",
+            "is_resolved",
+            "for_package",
+            "datafile_resource",
+            "datasource_id",
+        ],
+    )
     purl = PackageURLFilter(label="Package URL")
+    type = ParentAllValuesFilter()
+    scope = ParentAllValuesFilter()
+    datasource_id = ParentAllValuesFilter()
+    is_runtime = StrictBooleanFilter()
+    is_optional = StrictBooleanFilter()
+    is_resolved = StrictBooleanFilter()
 
     class Meta:
         model = DiscoveredDependency
         fields = [
             "search",
             "purl",
             "dependency_uid",
```

### Comparing `scancodeio-32.4.0/scanpipe/forms.py` & `scancodeio-32.5.0/scanpipe/forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/__init__.py` & `scancodeio-32.5.0/scanpipe/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/add-input.py` & `scancodeio-32.5.0/scanpipe/management/commands/add-input.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def handle(self, *args, **options):
         super().handle(*args, **options)
         inputs_files = options["inputs_files"]
         input_urls = options["input_urls"]
         copy_from = options["copy_codebase"]
 
-        if not self.project.can_add_input:
+        if not self.project.can_change_inputs:
             raise CommandError(
                 "Cannot add inputs once a pipeline has started to execute on a project."
             )
 
         if not (inputs_files or input_urls or copy_from):
             raise CommandError(
                 "Provide inputs with the --input-file, --input-url, or --copy-codebase"
```

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/add-pipeline.py` & `scancodeio-32.5.0/scanpipe/management/commands/add-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/archive-project.py` & `scancodeio-32.5.0/scanpipe/management/commands/archive-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/create-project.py` & `scancodeio-32.5.0/scanpipe/management/commands/create-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/create-user.py` & `scancodeio-32.5.0/scanpipe/management/commands/create-user.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/delete-project.py` & `scancodeio-32.5.0/scanpipe/management/commands/delete-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/execute.py` & `scancodeio-32.5.0/scanpipe/management/commands/execute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/graph.py` & `scancodeio-32.5.0/scanpipe/management/commands/graph.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/list-project.py` & `scancodeio-32.5.0/scanpipe/management/commands/list-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/output.py` & `scancodeio-32.5.0/scanpipe/management/commands/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/reset-project.py` & `scancodeio-32.5.0/scanpipe/management/commands/reset-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/show-pipeline.py` & `scancodeio-32.5.0/scanpipe/management/commands/show-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/management/commands/status.py` & `scancodeio-32.5.0/scanpipe/management/commands/status.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0001_initial.py` & `scancodeio-32.5.0/scanpipe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0002_run_id_and_log.py` & `scancodeio-32.5.0/scanpipe/migrations/0002_run_id_and_log.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0004_run_pipeline_name.py` & `scancodeio-32.5.0/scanpipe/migrations/0004_run_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py` & `scancodeio-32.5.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py` & `scancodeio-32.5.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0008_package_extra_data.py` & `scancodeio-32.5.0/scanpipe/migrations/0008_package_extra_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0013_project_is_archived.py` & `scancodeio-32.5.0/scanpipe/migrations/0013_project_is_archived.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0014_webhooksubscription.py` & `scancodeio-32.5.0/scanpipe/migrations/0014_webhooksubscription.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0019_auto_20220804_1836.py` & `scancodeio-32.5.0/scanpipe/migrations/0019_auto_20220804_1836.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0022_create_discovereddependencies_model.py` & `scancodeio-32.5.0/scanpipe/migrations/0022_create_discovereddependencies_model.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0023_migrate_dependencies.py` & `scancodeio-32.5.0/scanpipe/migrations/0023_migrate_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0028_codebaserelation_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0028_codebaserelation_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py` & `scancodeio-32.5.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py` & `scancodeio-32.5.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py` & `scancodeio-32.5.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0033_project_notes_project_settings.py` & `scancodeio-32.5.0/scanpipe/migrations/0033_project_notes_project_settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0035_set_projects_slug.py` & `scancodeio-32.5.0/scanpipe/migrations/0035_set_projects_slug.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0038_migrate_vulnerability_data.py` & `scancodeio-32.5.0/scanpipe/migrations/0038_migrate_vulnerability_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py` & `scancodeio-32.5.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/models.py` & `scancodeio-32.5.0/scanpipe/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,17 +848,20 @@
             return output_files[-1]
 
     def walk_codebase_path(self):
         """Return files and directories path of the codebase/ directory recursively."""
         return self.codebase_path.rglob("*")
 
     @cached_property
-    def can_add_input(self):
-        """Return True until one pipeline run has started to execute on the project."""
-        return not self.runs.has_start_date().exists()
+    def can_change_inputs(self):
+        """
+        Return True until one pipeline run has started its execution on the project.
+        Always False when the project is archived.
+        """
+        return not self.is_archived and not self.runs.has_start_date().exists()
 
     def add_input_source(self, filename, source, save=False):
         """
         Add given `filename` and `source` to the current project's `input_sources`
         field.
         """
         self.input_sources[filename] = source
@@ -875,27 +878,36 @@
                 f.write(chunk)
 
     def copy_input_from(self, input_location):
         """
         Copy the file at `input_location` to the current project's input/
         directory.
         """
-        from scanpipe.pipes.input import copy_inputs
+        from scanpipe.pipes.input import copy_input
 
-        copy_inputs([input_location], self.input_path)
+        copy_input(input_location, self.input_path)
 
     def move_input_from(self, input_location):
         """
         Move the file at `input_location` to the current project's input/
         directory.
         """
         from scanpipe.pipes.input import move_inputs
 
         move_inputs([input_location], self.input_path)
 
+    def delete_input(self, name):
+        """Delete the provided ``name`` input from disk and from ``input_sources``."""
+        file_path = self.input_path / name
+        file_path.unlink(missing_ok=True)
+
+        if self.input_sources.pop(name, None):
+            self.save(update_fields=["input_sources"])
+            return True
+
     def add_downloads(self, downloads):
         """
         Move the given `downloads` to the current project's input/ directory and
         adds the `input_source` for each entry.
         """
         for downloaded in downloads:
             self.move_input_from(downloaded.path)
@@ -2630,14 +2642,18 @@
 
         checksums = [
             spdx.Checksum(algorithm=algorithm, value=checksum_value)
             for algorithm in ["sha1", "md5"]
             if (checksum_value := getattr(self, algorithm))
         ]
 
+        attribution_texts = []
+        if self.notice_text:
+            attribution_texts.append(self.notice_text)
+
         external_refs = []
 
         if package_url := self.package_url:
             external_refs.append(
                 spdx.ExternalRef(
                     category="PACKAGE-MANAGER",
                     type="purl",
@@ -2653,14 +2669,15 @@
             license_concluded=self.get_declared_license_expression_spdx(),
             copyright_text=self.copyright,
             version=self.version,
             homepage=self.homepage_url,
             filename=self.filename,
             description=self.description,
             release_date=str(self.release_date) if self.release_date else "",
+            attribution_texts=attribution_texts,
             checksums=checksums,
             external_refs=external_refs,
         )
 
     def as_cyclonedx(self):
         """Return this DiscoveredPackage as an CycloneDX Component entry."""
         licenses = []
```

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/__init__.py` & `scancodeio-32.5.0/scanpipe/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/deploy_to_develop.py` & `scancodeio-32.5.0/scanpipe/pipelines/deploy_to_develop.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # Visit https://github.com/nexB/scancode.io for support and download.
 
 from scanpipe.pipelines import Pipeline
 from scanpipe.pipes import d2d
 from scanpipe.pipes import flag
 from scanpipe.pipes import purldb
 from scanpipe.pipes import scancode
-from scanpipe.pipes.scancode import extract_archives
 
 
 class DeployToDevelop(Pipeline):
     """
     Relate deploy and develop code trees.
 
     This pipeline is expecting 2 archive files with "from-" and "to-" filename
@@ -74,32 +73,35 @@
         ".scss",
         ".less",
         ".sass",
         ".soy",
     ]
 
     def get_inputs(self):
-        """Locate the ``from`` and ``to`` archives."""
-        self.from_file, self.to_file = d2d.get_inputs(self.project)
-
-        self.from_path = self.project.codebase_path / d2d.FROM
-        self.to_path = self.project.codebase_path / d2d.TO
+        """Locate the ``from`` and ``to`` input files."""
+        self.from_files, self.to_files = d2d.get_inputs(self.project)
 
     def extract_inputs_to_codebase_directory(self):
         """Extract input files to the project's codebase/ directory."""
+        inputs_with_codebase_path_destination = [
+            (self.from_files, self.project.codebase_path / d2d.FROM),
+            (self.to_files, self.project.codebase_path / d2d.TO),
+        ]
+
         errors = []
-        errors += scancode.extract_archive(self.from_file, self.from_path)
-        errors += scancode.extract_archive(self.to_file, self.to_path)
+        for input_files, codebase_path in inputs_with_codebase_path_destination:
+            for input_file_path in input_files:
+                errors += scancode.extract_archive(input_file_path, codebase_path)
 
         if errors:
             self.add_error("\n".join(errors))
 
     def extract_archives_in_place(self):
         """Extract recursively from* and to* archives in place with extractcode."""
-        extract_errors = extract_archives(
+        extract_errors = scancode.extract_archives(
             self.project.codebase_path,
             recurse=self.env.get("extract_recursively", True),
         )
 
         if extract_errors:
             self.add_error("\n".join(extract_errors))
```

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/docker.py` & `scancodeio-32.5.0/scanpipe/pipelines/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/docker_windows.py` & `scancodeio-32.5.0/scanpipe/pipelines/docker_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/find_vulnerabilities.py` & `scancodeio-32.5.0/scanpipe/pipelines/find_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/inspect_manifest.py` & `scancodeio-32.5.0/scanpipe/pipelines/inspect_manifest.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/load_inventory.py` & `scancodeio-32.5.0/scanpipe/pipelines/load_inventory.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/root_filesystems.py` & `scancodeio-32.5.0/scanpipe/pipelines/root_filesystems.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # OR CONDITIONS OF ANY KIND, either express or implied. No content created from
 # ScanCode.io should be considered or used as legal advice. Consult an Attorney
 # for any legal advice.
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
-import os
-
 from scanpipe.pipelines import Pipeline
 from scanpipe.pipes import flag
 from scanpipe.pipes import rootfs
 from scanpipe.pipes import scancode
 
 
 class RootFS(Pipeline):
@@ -64,21 +62,19 @@
             self.add_error("\n".join(errors))
 
     def find_root_filesystems(self):
         """Find root filesystems in the project's codebase/."""
         self.root_filesystems = list(rootfs.RootFs.from_project_codebase(self.project))
 
     def collect_rootfs_information(self):
-        """Collect and stores rootfs information in the project."""
-        rootfs_data = {}
-        for rfs in self.root_filesystems:
-            rootfs_data["name"] = os.path.basename(rfs.location)
-            rootfs_data["distro"] = rfs.distro.to_dict() if rfs.distro else {}
-
-        self.project.update_extra_data({"images": rootfs_data})
+        """Collect and stores rootfs information on the project."""
+        rootfs_data = [
+            rootfs.get_rootfs_data(root_fs) for root_fs in self.root_filesystems
+        ]
+        self.project.update_extra_data({"root_filesystems": rootfs_data})
 
     def collect_and_create_codebase_resources(self):
         """Collect and label all image files as CodebaseResource."""
         for rfs in self.root_filesystems:
             rootfs.create_codebase_resources(self.project, rfs)
 
     def collect_and_create_system_packages(self):
```

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/scan_codebase.py` & `scancodeio-32.5.0/scanpipe/pipelines/scan_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipelines/scan_package.py` & `scancodeio-32.5.0/scanpipe/pipelines/scan_package.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/__init__.py` & `scancodeio-32.5.0/scanpipe/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/codebase.py` & `scancodeio-32.5.0/scanpipe/pipes/codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/compliance.py` & `scancodeio-32.5.0/scanpipe/tests/test_licenses.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,44 +16,26 @@
 # OR CONDITIONS OF ANY KIND, either express or implied. No content created from
 # ScanCode.io should be considered or used as legal advice. Consult an Attorney
 # for any legal advice.
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
-from scanpipe.pipes import flag
-from scanpipe.pipes import scancode
-
-"""
-A common compliance pattern for images is to store known licenses in a /licenses
-directory and the corresponding source code archives, for packages that are
-redistributable in source form, in a /sourcemirror directory; both at the root of
-an image (VM or container image).
-
-Usage example within a Pipeline:
-
-def analyze_licenses_and_sources(self):
-    util.flag_compliance_files(self.project)
-    util.analyze_compliance_licenses(self.project)
-"""
-
-
-def flag_compliance_files(project):
-    """Flag compliance files status for the provided `project`."""
-    compliance_dirs = {
-        "/licenses": flag.COMPLIANCE_LICENSES,
-        "/sourcemirror": flag.COMPLIANCE_SOURCEMIRROR,
-    }
-
-    qs = project.codebaseresources.no_status()
-
-    for path, status in compliance_dirs.items():
-        qs.filter(rootfs_path__startswith=path).update(status=status)
-
-
-def analyze_compliance_licenses(project):
-    """Scan compliance licenses status for the provided `project`."""
-    qs = project.codebaseresources.status(flag.COMPLIANCE_LICENSES)
-
-    for codebase_resource in qs:
-        scan_results, scan_errors = scancode.scan_file(codebase_resource.location)
-        codebase_resource.set_scan_results(scan_results)
+from django.test import TestCase
+from django.test import override_settings
+from django.urls import reverse
+
+
+@override_settings(SCANCODEIO_REQUIRE_AUTHENTICATION=False)
+class LicensesTest(TestCase):
+    def test_license_list_view(self):
+        url = reverse("license_list")
+        response = self.client.get(url)
+        self.assertEqual(response.status_code, 200)
+
+    def test_license_details_view(self):
+        keys = ["apache-2.0", "abcdefg"]
+        license_url = reverse("license_details", args=(keys[0],))
+        dummy_license_url = reverse("license_details", args=(keys[1],))
+        response = [self.client.get(license_url), self.client.get(dummy_license_url)]
+        self.assertEqual(response[0].status_code, 200)
+        self.assertEqual(response[1].status_code, 404)
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/cyclonedx.py` & `scancodeio-32.5.0/scanpipe/pipes/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/d2d.py` & `scancodeio-32.5.0/scanpipe/pipes/d2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
 from itertools import islice
 from pathlib import Path
 from timeit import default_timer as timer
 
+from django.db.models import Q
+
 from scanpipe import pipes
 from scanpipe.models import CodebaseRelation
 from scanpipe.models import CodebaseResource
 from scanpipe.pipes import flag
 from scanpipe.pipes import get_resource_diff_ratio
 from scanpipe.pipes import js
 from scanpipe.pipes import jvm
@@ -37,25 +39,25 @@
 from scanpipe.pipes import scancode
 
 FROM = "from/"
 TO = "to/"
 
 
 def get_inputs(project):
-    """Locate the ``from`` and ``to`` archives in project inputs directory."""
-    from_file = list(project.inputs("from*"))
-    to_file = list(project.inputs("to*"))
+    """Locate the ``from`` and ``to`` input files in project inputs/ directory."""
+    from_files = list(project.inputs("from*"))
+    to_files = list(project.inputs("to*"))
 
-    if len(from_file) != 1:
-        raise FileNotFoundError("from* archive not found.")
+    if len(from_files) < 1:
+        raise FileNotFoundError("from* input files not found.")
 
-    if len(to_file) != 1:
-        raise FileNotFoundError("to* archive not found.")
+    if len(to_files) < 1:
+        raise FileNotFoundError("to* input files not found.")
 
-    return from_file[0], to_file[0]
+    return from_files, to_files
 
 
 def get_resource_codebase_root(project, resource_path):
     """Return "to" or "from" depending on the resource location in the codebase."""
     relative_path = Path(resource_path).relative_to(project.codebase_path)
     first_part = relative_path.parts[0]
     if first_part in ["to", "from"]:
@@ -610,20 +612,31 @@
         return
 
     filename = package_data.get("filename")
     if not filename:
         # Cannot map anything without the about_resource value.
         return
 
+    ignored_resources = []
+    if extra_data := package_data.get("extra_data"):
+        ignored_resources = extra_data.get("ignored_resources")
+
     # Fetch all resources that are covered by the .ABOUT file.
     codebase_resources = to_resources.filter(path__contains=f"/{filename.lstrip('/')}")
     if not codebase_resources:
         # If there's nothing to map on the ``to/`` do not create the package.
         return
 
+    # Ignore resources for paths in `ignored_resources` attribute
+    if ignored_resources:
+        lookups = Q()
+        for resource_path in ignored_resources:
+            lookups |= Q(**{"path__contains": resource_path})
+        codebase_resources = codebase_resources.filter(~lookups)
+
     # Create the Package using .ABOUT data and assigned related codebase_resources
     pipes.update_or_create_package(project, package_data, codebase_resources)
 
     # Map the .ABOUT file resource to all related resources in the ``to/`` side.
     for to_resource in codebase_resources:
         pipes.make_relation(
             from_resource=about_file_resource,
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/docker.py` & `scancodeio-32.5.0/scanpipe/pipes/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,18 @@
 ]
 Layer = namedtuple("Layer", layer_fields)
 
 
 def get_layers_data(project):
     """Get list of structured layers data from project extra_data field."""
     layers_data = []
+
     images = project.extra_data.get("images", [])
+    if not type(images) == list:
+        return []
 
     for image in images:
         image_id = image.get("image_id")
 
         for layer_index, layer in enumerate(image.get("layers", []), start=1):
             layer_id = layer.get("layer_id")
             layers_data.append(
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/fetch.py` & `scancodeio-32.5.0/scanpipe/pipes/fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/flag.py` & `scancodeio-32.5.0/scanpipe/pipes/flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/input.py` & `scancodeio-32.5.0/scanpipe/pipes/input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/js.py` & `scancodeio-32.5.0/scanpipe/pipes/js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/jvm.py` & `scancodeio-32.5.0/scanpipe/pipes/jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/output.py` & `scancodeio-32.5.0/scanpipe/pipes/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
     """
     Generate and return the SPDX `extracted_licenses` from provided
     `license_expressions` list of expressions.
     """
     licensing = Licensing()
     license_index = get_licenses_by_spdx_key()
     urls_fields = [
+        "licensedb_url",
+        "scancode_url",
         "faq_url",
         "homepage_url",
         "osi_url",
         "ignorable_urls",
         "other_urls",
         "text_urls",
     ]
@@ -526,36 +528,36 @@
     """
     Generate output for the provided ``project`` in SPDX document format.
     The output file is created in the ``project`` "output/" directory.
     Return the path of the generated output file.
     """
     output_file = project.get_output_file_path("results", "spdx.json")
 
-    discovereddependencies_qs = get_queryset(project, "discovereddependency")
-    spdx_packages = [
-        *get_queryset(project, "discoveredpackage"),
-        *discovereddependencies_qs,
-    ]
+    discoveredpackage_qs = get_queryset(project, "discoveredpackage")
+    discovereddependency_qs = get_queryset(project, "discovereddependency")
 
     packages_as_spdx = []
     license_expressions = []
-    for spdx_package in spdx_packages:
-        packages_as_spdx.append(spdx_package.as_spdx())
-        if license_expression := getattr(spdx_package, "license_expression", None):
+    relationships = []
+
+    for package in discoveredpackage_qs:
+        packages_as_spdx.append(package.as_spdx())
+        if license_expression := package.declared_license_expression:
             license_expressions.append(license_expression)
 
-    relationships = [
-        spdx.Relationship(
-            spdx_id=dep.spdx_id,
-            related_spdx_id=dep.for_package.spdx_id,
-            relationship="DEPENDENCY_OF",
-        )
-        for dep in discovereddependencies_qs
-        if dep.for_package
-    ]
+    for dependency in discovereddependency_qs:
+        packages_as_spdx.append(dependency.as_spdx())
+        if dependency.for_package:
+            relationships.append(
+                spdx.Relationship(
+                    spdx_id=dependency.spdx_id,
+                    related_spdx_id=dependency.for_package.spdx_id,
+                    relationship="DEPENDENCY_OF",
+                )
+            )
 
     files_as_spdx = []
     if include_files:
         files_as_spdx = [
             resource.as_spdx()
             for resource in get_queryset(project, "codebaseresource").files()
         ]
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/pathmap.py` & `scancodeio-32.5.0/scanpipe/pipes/pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/purldb.py` & `scancodeio-32.5.0/scanpipe/pipes/purldb.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         return response.json()
     except (requests.RequestException, ValueError, TypeError) as exception:
         logger.debug(f"{label} [Exception] {exception}")
 
 
 def request_post(url, data, timeout=None):
     try:
-        response = session.post(url, json=data, timeout=timeout)
+        response = session.post(url, data=data, timeout=timeout)
         response.raise_for_status()
         return response.json()
     except (requests.RequestException, ValueError, TypeError) as exception:
         logger.debug(f"{label} [Exception] {exception}")
 
 
 def match_package(sha1, timeout=None, api_url=PURLDB_API_URL):
@@ -113,7 +113,17 @@
     """Match list SHA1 in the PurlDB for a single resource file."""
     payload = {"sha1": sha1_list}
     response = request_get(url=f"{api_url}resources/", payload=payload, timeout=timeout)
 
     if response and response.get("count"):
         packages = response["results"]
         return packages
+
+
+def submit_purls(purls, timeout=None, api_url=PURLDB_API_URL):
+    """Submit list PURLs to PurlDB for indexing."""
+    payload = {"package_urls": purls}
+    response = request_post(
+        url=f"{api_url}packages/index_packages/", data=payload, timeout=timeout
+    )
+
+    return response
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/resolve.py` & `scancodeio-32.5.0/scanpipe/pipes/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
         for field_name, value in package_url_data.items():
             if value:
                 package_data[field_name] = value
 
     if about_resource := about_data.get("about_resource"):
         package_data["filename"] = list(about_resource.keys())[0]
 
+    if ignored_resources := about_data.get("ignored_resources"):
+        extra_data = {"ignored_resources": list(ignored_resources.keys())}
+        package_data["extra_data"] = extra_data
+
     if license_expression := about_data.get("license_expression"):
         package_data["declared_license_expression"] = license_expression
 
     if notice_dict := about_data.get("notice_file"):
         package_data["notice_text"] = list(notice_dict.values())[0]
 
     for field_name, value in about_data.items():
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/rootfs.py` & `scancodeio-32.5.0/scanpipe/pipes/rootfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,7 +377,15 @@
     qs.filter(lookup).update(status=flag.IGNORED_DATA_FILE_NO_CLUES)
 
 
 def flag_media_files_as_uninteresting(project):
     """Flag CodebaseResources that are media files to be uninteresting."""
     qs = project.codebaseresources.no_status()
     qs.filter(is_media=True).update(status=flag.IGNORED_MEDIA_FILE)
+
+
+def get_rootfs_data(root_fs):
+    """Return a mapping of rootfs-related data given a ``root_fs``."""
+    return {
+        "name": os.path.basename(root_fs.location),
+        "distro": root_fs.distro.to_dict() if root_fs.distro else {},
+    }
```

### Comparing `scancodeio-32.4.0/scanpipe/pipes/scancode.py` & `scancodeio-32.5.0/scanpipe/pipes/scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/schemas/bom-1.4.schema.json` & `scancodeio-32.5.0/scanpipe/pipes/schemas/bom-1.4.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/schemas/jsf-0.82.schema.json` & `scancodeio-32.5.0/scanpipe/pipes/schemas/jsf-0.82.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/schemas/spdx-schema-2.3.json` & `scancodeio-32.5.0/scanpipe/pipes/schemas/spdx-schema-2.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/schemas/spdx.schema.json` & `scancodeio-32.5.0/scanpipe/pipes/schemas/spdx.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/spdx.py` & `scancodeio-32.5.0/scanpipe/pipes/spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/vulnerablecode.py` & `scancodeio-32.5.0/scanpipe/pipes/vulnerablecode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/pipes/windows.py` & `scancodeio-32.5.0/scanpipe/pipes/windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tasks.py` & `scancodeio-32.5.0/scanpipe/tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/account/profile.html` & `scancodeio-32.5.0/scanpipe/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/registration/login.html` & `scancodeio-32.5.0/scanpipe/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/rest_framework/api.html` & `scancodeio-32.5.0/scanpipe/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/app_monitoring.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/app_monitoring.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/attribution.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/base.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/base.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/dependency_detail.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/dependency_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             </td>
             <td>
               {% if dependency.datafile_resource %}
                 <a href="{{ dependency.datafile_resource.get_absolute_url }}" title="{{ dependency.datafile_resource.path }}">{{ dependency.datafile_resource.name }}</a>
               {% endif %}
             </td>
             <td>
-              {{ dependency.datasource_id }}
+              <a href="?datasource_id={{ dependency.datasource_id }}" class="is-black-link">{{ dependency.datasource_id }}</a>
             </td>
           </tr>
         {% empty %}
           <tr>
             <td colspan="42" class="has-text-centered p-3">
               No Dependencies found. <a href="?">Clear search and filters</a>
             </td>
```

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/error_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/error_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/breadcrumb.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/file_filter.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/file_filter.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/list_view_thead.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_view_thead.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/navbar_header.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/navbar_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/pagination.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/pagination_header.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_codebase.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_codebase.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_downloads.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_downloads.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_inputs.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <article id="inputs-panel" class="panel is-info">
   <p class="panel-heading py-2 is-size-6">
     Inputs
   </p>
   {% for input in inputs_with_source %}
-    <div class="panel-block is-justify-content-space-between dropdown is-hoverable is-up is-cursor-help">
-      <div class="break-all pr-1">
+    <div class="panel-block is-justify-content-space-between is-up">
+      <div class="break-all pr-1 is-cursor-help dropdown is-hoverable">
         <div class="panel-icon pt-1">
           <div class="dropdown-trigger">
             <i class="is-size-6 {% if input.is_file %}fa-regular fa-file{% else %}fa-solid fa-folder{% endif %}" aria-hidden="true" aria-haspopup="true" aria-controls="dropdown-input-{{ file.name|slugify }}"></i>
           </div>
           <div class="dropdown-menu" id="dropdown-input-{{ file.name|slugify }}" role="menu">
             <div class="dropdown-content">
               <div class="dropdown-item">
@@ -21,25 +21,33 @@
                   {% elif input.source %}
                     Downloaded from {{ input.source }}
                   {% endif %}
                   </strong>
               </div>
             </div>
           </div>
-        </div>{{ input.name }}
+        </div>
+        {{ input.name }}
       </div>
-      <div class="is-family-monospace is-size-7">
+      <div class="is-size-7">
         {% if input.is_file %}
-          {{ input.size|filesizeformat }}
+          <span class="mr-2">{{ input.size|filesizeformat }}</span>
+        {% endif %}
+        <a class="is-grey-link is-clickable" href="{% url 'project_download_input' project.slug input.name %}"><i class="fa-solid fa-download"></i></a>
+        {% if project.can_change_inputs %}
+          <a class="modal-button is-grey-link is-clickable ml-1" data-target="modal-inputs-delete" aria-haspopup="true" data-url="{% url 'project_delete_input' project.slug input.name %}" data-filename="{{ input.name }}" href="#"><i class="fa-regular fa-trash-can"></i></a>
         {% endif %}
       </div>
     </div>
   {% endfor %}
   <div class="panel-block">
-    {% if project.can_add_input and not project.is_archived %}
+    {% if project.can_change_inputs %}
       <button class="button is-link is-outlined is-fullwidth modal-button" data-target="add-inputs-modal" aria-haspopup="true">Add inputs</button>
       {% include "scanpipe/includes/add_inputs_modal.html" %}
     {% else %}
       <button class="button is-link is-outlined is-fullwidth" disabled>Add inputs</button>
     {% endif %}
   </div>
-</article>
+</article>
+{% if project.can_change_inputs %}
+  {% include 'scanpipe/includes/project_inputs_delete_modal.html' %}
+{% endif %}
```

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_list_table.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_list_table.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_pipelines.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_pipelines.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/project_summary_level.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_summary_level.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_modal.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_modal_content.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/run_status_tag.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_status_tag.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/includes/search_field.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/search_field.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/package_detail.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/package_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/package_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/package_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/project_charts.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_charts.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/project_detail.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/project_form.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -145,11 +145,11 @@
 
       let progress_container = document.createElement('div');
       progress_container.className = 'container is-max-desktop mt-6 px-6';
       progress_container.appendChild(progress_bar)
       background.appendChild(progress_container);
 
       let form_errors = document.getElementById('form-errors');
-      displayFormUploadProgress(form, progress_bar, form_errors);
+      displayFormUploadProgress(form, progress_bar, form_errors, true);
     });
   </script>
 {% endblock %}
```

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/project_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/project_settings.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_settings.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/relation_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/relation_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/resource_detail.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/resource_list.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_packages.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_packages.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_relations.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_resources.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_resources.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/templates/scanpipe/tabset/tabset.html` & `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tabset.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/__init__.py` & `scancodeio-32.5.0/scanpipe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/alpine_3_15_4.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/archive.zip` & `scancodeio-32.5.0/scanpipe/tests/data/archive.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987373737373737%*

 * *Differences: {"'packages'": "{0: {'attributionTexts': ['NOTICE_TEXT']}, 1: {'attributionTexts': "*

 * *               "['NOTICE_TEXT']}}"}*

```diff
@@ -19,14 +19,17 @@
     ],
     "documentNamespace": "https://scancode.io/spdxdocs/cbd609b2-525a-4052-9860-201b879b20d9",
     "files": [],
     "name": "scancodeio_asgiref",
     "packages": [
         {
             "SPDXID": "SPDXRef-scancodeio-discoveredpackage-8fa7433f-c05e-45b3-960d-60a5423327f7",
+            "attributionTexts": [
+                "NOTICE_TEXT"
+            ],
             "copyrightText": "NOASSERTION",
             "description": "ASGI specs, helper code, and adapters\nasgiref\n=======\n\n.. image:: https://api.travis-ci.org/django/asgiref.svg\n    :target: https://travis-ci.org/django/asgiref\n\n.. image:: https://img.shields.io/pypi/v/asgiref.svg\n    :target: https://pypi.python.org/pypi/asgiref\n\nASGI is a standard for Python asynchronous web apps and servers to communicate\nwith each other, and positioned as an asynchronous successor to WSGI. You can\nread more at https://asgi.readthedocs.io/en/latest/\n\nThis package includes ASGI base libraries, such as:\n\n* Sync-to-async and async-to-sync function wrappers, ``asgiref.sync``\n* Server base classes, ``asgiref.server``\n* A WSGI-to-ASGI adapter, in ``asgiref.wsgi``\n\n\nFunction wrappers\n-----------------\n\nThese allow you to wrap or decorate async or sync functions to call them from\nthe other style (so you can call async functions from a synchronous thread,\nor vice-versa).\n\nIn particular:\n\n* AsyncToSync lets a synchronous subthread stop and wait while the async\n  function is called on the main thread's event loop, and then control is\n  returned to the thread when the async function is finished.\n\n* SyncToAsync lets async code call a synchronous function, which is run in\n  a threadpool and control returned to the async coroutine when the synchronous\n  function completes.\n\nThe idea is to make it easier to call synchronous APIs from async code and\nasynchronous APIs from synchronous code so it's easier to transition code from\none style to the other. In the case of Channels, we wrap the (synchronous)\nDjango view system with SyncToAsync to allow it to run inside the (asynchronous)\nASGI server.\n\nNote that exactly what threads things run in is very specific, and aimed to\nkeep maximum compatibility with old synchronous code. See\n\"Synchronous code & Threads\" below for a full explanation. By default,\n``sync_to_async`` will run all synchronous code in the program in the same\nthread for safety reasons; you can disable this for more performance with\n``@sync_to_async(thread_sensitive=False)``, but make sure that your code does\nnot rely on anything bound to threads (like database connections) when you do.\n\n\nThreadlocal replacement\n-----------------------\n\nThis is a drop-in replacement for ``threading.local`` that works with both\nthreads and asyncio Tasks. Even better, it will proxy values through from a\ntask-local context to a thread-local context when you use ``sync_to_async``\nto run things in a threadpool, and vice-versa for ``async_to_sync``.\n\nIf you instead want true thread- and task-safety, you can set\n``thread_critical`` on the Local object to ensure this instead.\n\n\nServer base classes\n-------------------\n\nIncludes a ``StatelessServer`` class which provides all the hard work of\nwriting a stateless server (as in, does not handle direct incoming sockets\nbut instead consumes external streams or sockets to work out what is happening).\n\nAn example of such a server would be a chatbot server that connects out to\na central chat server and provides a \"connection scope\" per user chatting to\nit. There's only one actual connection, but the server has to separate things\ninto several scopes for easier writing of the code.\n\nYou can see an example of this being used in `frequensgi <https://github.com/andrewgodwin/frequensgi>`_.\n\n\nWSGI-to-ASGI adapter\n--------------------\n\nAllows you to wrap a WSGI application so it appears as a valid ASGI application.\n\nSimply wrap it around your WSGI application like so::\n\n    asgi_application = WsgiToAsgi(wsgi_application)\n\nThe WSGI application will be run in a synchronous threadpool, and the wrapped\nASGI application will be one that accepts ``http`` class messages.\n\nPlease note that not all extended features of WSGI may be supported (such as\nfile handles for incoming POST bodies).\n\n\nDependencies\n------------\n\n``asgiref`` requires Python 3.5 or higher.\n\n\nContributing\n------------\n\nPlease refer to the\n`main Channels contributing docs <https://github.com/django/channels/blob/master/CONTRIBUTING.rst>`_.\n\n\nTesting\n'''''''\n\nTo run tests, make sure you have installed the ``tests`` extra with the package::\n\n    cd asgiref/\n    pip install -e .[tests]\n    pytest\n\n\nBuilding the documentation\n''''''''''''''''''''''''''\n\nThe documentation uses `Sphinx <http://www.sphinx-doc.org>`_::\n\n    cd asgiref/docs/\n    pip install sphinx\n\nTo build the docs, you can use the default tools::\n\n    sphinx-build -b html . _build/html  # or `make html`, if you've got make set up\n    cd _build/html\n    python -m http.server\n\n...or you can use ``sphinx-autobuild`` to run a server and rebuild/reload\nyour documentation changes automatically::\n\n    pip install sphinx-autobuild\n    sphinx-autobuild . _build/html\n\n\nImplementation Details\n----------------------\n\nSynchronous code & threads\n''''''''''''''''''''''''''\n\nThe ``asgiref.sync`` module provides two wrappers that let you go between\nasynchronous and synchronous code at will, while taking care of the rough edges\nfor you.\n\nUnfortunately, the rough edges are numerous, and the code has to work especially\nhard to keep things in the same thread as much as possible. Notably, the\nrestrictions we are working with are:\n\n* All synchronous code called through ``SyncToAsync`` and marked with\n  ``thread_sensitive`` should run in the same thread as each other (and if the\n  outer layer of the program is synchronous, the main thread)\n\n* If a thread already has a running async loop, ``AsyncToSync`` can't run things\n  on that loop if it's blocked on synchronous code that is above you in the\n  call stack.\n\nThe first compromise you get to might be that ``thread_sensitive`` code should\njust run in the same thread and not spawn in a sub-thread, fulfilling the first\nrestriction, but that immediately runs you into the second restriction.\n\nThe only real solution is to essentially have a variant of ThreadPoolExecutor\nthat executes any ``thread_sensitive`` code on the outermost synchronous\nthread - either the main thread, or a single spawned subthread.\n\nThis means you now have two basic states:\n\n* If the outermost layer of your program is synchronous, then all async code\n  run through ``AsyncToSync`` will run in a per-call event loop in arbitary\n  sub-threads, while all ``thread_sensitive`` code will run in the main thread.\n\n* If the outermost layer of your program is asynchronous, then all async code\n  runs on the main thread's event loop, and all ``thread_sensitive`` synchronous\n  code will run in a single shared sub-thread.\n\nCruicially, this means that in both cases there is a thread which is a shared\nresource that all ``thread_sensitive`` code must run on, and there is a chance\nthat this thread is currently blocked on its own ``AsyncToSync`` call. Thus,\n``AsyncToSync`` needs to act as an executor for thread code while it's blocking.\n\nThe ``CurrentThreadExecutor`` class provides this functionality; rather than\nsimply waiting on a Future, you can call its ``run_until_future`` method and\nit will run submitted code until that Future is done. This means that code\ninside the call can then run code on your thread.\n\n\nMaintenance and Security\n------------------------\n\nTo report security issues, please contact security@djangoproject.com. For GPG\nsignatures and more security process information, see\nhttps://docs.djangoproject.com/en/dev/internals/security/.\n\nTo report bugs or request new features, please open a new GitHub issue.\n\nThis repository is part of the Channels project. For the shepherd and maintenance team, please see the\n`main Channels readme <https://github.com/django/channels/blob/master/README.rst>`_.",
             "downloadLocation": "NOASSERTION",
             "externalRefs": [
                 {
                     "referenceCategory": "PACKAGE-MANAGER",
                     "referenceLocator": "pkg:pypi/asgiref@3.3.0",
@@ -38,14 +41,17 @@
             "licenseConcluded": "BSD-3-Clause",
             "licenseDeclared": "BSD-3-Clause",
             "name": "asgiref",
             "versionInfo": "3.3.0"
         },
         {
             "SPDXID": "SPDXRef-scancodeio-discoveredpackage-bef22e34-f8c3-463d-9d3e-46a55c3170e8",
+            "attributionTexts": [
+                "NOTICE_TEXT"
+            ],
             "copyrightText": "NOASSERTION",
             "description": "ASGI specs, helper code, and adapters\nasgiref\n=======\n\n.. image:: https://api.travis-ci.org/django/asgiref.svg\n    :target: https://travis-ci.org/django/asgiref\n\n.. image:: https://img.shields.io/pypi/v/asgiref.svg\n    :target: https://pypi.python.org/pypi/asgiref\n\nASGI is a standard for Python asynchronous web apps and servers to communicate\nwith each other, and positioned as an asynchronous successor to WSGI. You can\nread more at https://asgi.readthedocs.io/en/latest/\n\nThis package includes ASGI base libraries, such as:\n\n* Sync-to-async and async-to-sync function wrappers, ``asgiref.sync``\n* Server base classes, ``asgiref.server``\n* A WSGI-to-ASGI adapter, in ``asgiref.wsgi``\n\n\nFunction wrappers\n-----------------\n\nThese allow you to wrap or decorate async or sync functions to call them from\nthe other style (so you can call async functions from a synchronous thread,\nor vice-versa).\n\nIn particular:\n\n* AsyncToSync lets a synchronous subthread stop and wait while the async\n  function is called on the main thread's event loop, and then control is\n  returned to the thread when the async function is finished.\n\n* SyncToAsync lets async code call a synchronous function, which is run in\n  a threadpool and control returned to the async coroutine when the synchronous\n  function completes.\n\nThe idea is to make it easier to call synchronous APIs from async code and\nasynchronous APIs from synchronous code so it's easier to transition code from\none style to the other. In the case of Channels, we wrap the (synchronous)\nDjango view system with SyncToAsync to allow it to run inside the (asynchronous)\nASGI server.\n\nNote that exactly what threads things run in is very specific, and aimed to\nkeep maximum compatibility with old synchronous code. See\n\"Synchronous code & Threads\" below for a full explanation. By default,\n``sync_to_async`` will run all synchronous code in the program in the same\nthread for safety reasons; you can disable this for more performance with\n``@sync_to_async(thread_sensitive=False)``, but make sure that your code does\nnot rely on anything bound to threads (like database connections) when you do.\n\n\nThreadlocal replacement\n-----------------------\n\nThis is a drop-in replacement for ``threading.local`` that works with both\nthreads and asyncio Tasks. Even better, it will proxy values through from a\ntask-local context to a thread-local context when you use ``sync_to_async``\nto run things in a threadpool, and vice-versa for ``async_to_sync``.\n\nIf you instead want true thread- and task-safety, you can set\n``thread_critical`` on the Local object to ensure this instead.\n\n\nServer base classes\n-------------------\n\nIncludes a ``StatelessServer`` class which provides all the hard work of\nwriting a stateless server (as in, does not handle direct incoming sockets\nbut instead consumes external streams or sockets to work out what is happening).\n\nAn example of such a server would be a chatbot server that connects out to\na central chat server and provides a \"connection scope\" per user chatting to\nit. There's only one actual connection, but the server has to separate things\ninto several scopes for easier writing of the code.\n\nYou can see an example of this being used in `frequensgi <https://github.com/andrewgodwin/frequensgi>`_.\n\n\nWSGI-to-ASGI adapter\n--------------------\n\nAllows you to wrap a WSGI application so it appears as a valid ASGI application.\n\nSimply wrap it around your WSGI application like so::\n\n    asgi_application = WsgiToAsgi(wsgi_application)\n\nThe WSGI application will be run in a synchronous threadpool, and the wrapped\nASGI application will be one that accepts ``http`` class messages.\n\nPlease note that not all extended features of WSGI may be supported (such as\nfile handles for incoming POST bodies).\n\n\nDependencies\n------------\n\n``asgiref`` requires Python 3.5 or higher.\n\n\nContributing\n------------\n\nPlease refer to the\n`main Channels contributing docs <https://github.com/django/channels/blob/master/CONTRIBUTING.rst>`_.\n\n\nTesting\n'''''''\n\nTo run tests, make sure you have installed the ``tests`` extra with the package::\n\n    cd asgiref/\n    pip install -e .[tests]\n    pytest\n\n\nBuilding the documentation\n''''''''''''''''''''''''''\n\nThe documentation uses `Sphinx <http://www.sphinx-doc.org>`_::\n\n    cd asgiref/docs/\n    pip install sphinx\n\nTo build the docs, you can use the default tools::\n\n    sphinx-build -b html . _build/html  # or `make html`, if you've got make set up\n    cd _build/html\n    python -m http.server\n\n...or you can use ``sphinx-autobuild`` to run a server and rebuild/reload\nyour documentation changes automatically::\n\n    pip install sphinx-autobuild\n    sphinx-autobuild . _build/html\n\n\nImplementation Details\n----------------------\n\nSynchronous code & threads\n''''''''''''''''''''''''''\n\nThe ``asgiref.sync`` module provides two wrappers that let you go between\nasynchronous and synchronous code at will, while taking care of the rough edges\nfor you.\n\nUnfortunately, the rough edges are numerous, and the code has to work especially\nhard to keep things in the same thread as much as possible. Notably, the\nrestrictions we are working with are:\n\n* All synchronous code called through ``SyncToAsync`` and marked with\n  ``thread_sensitive`` should run in the same thread as each other (and if the\n  outer layer of the program is synchronous, the main thread)\n\n* If a thread already has a running async loop, ``AsyncToSync`` can't run things\n  on that loop if it's blocked on synchronous code that is above you in the\n  call stack.\n\nThe first compromise you get to might be that ``thread_sensitive`` code should\njust run in the same thread and not spawn in a sub-thread, fulfilling the first\nrestriction, but that immediately runs you into the second restriction.\n\nThe only real solution is to essentially have a variant of ThreadPoolExecutor\nthat executes any ``thread_sensitive`` code on the outermost synchronous\nthread - either the main thread, or a single spawned subthread.\n\nThis means you now have two basic states:\n\n* If the outermost layer of your program is synchronous, then all async code\n  run through ``AsyncToSync`` will run in a per-call event loop in arbitary\n  sub-threads, while all ``thread_sensitive`` code will run in the main thread.\n\n* If the outermost layer of your program is asynchronous, then all async code\n  runs on the main thread's event loop, and all ``thread_sensitive`` synchronous\n  code will run in a single shared sub-thread.\n\nCruicially, this means that in both cases there is a thread which is a shared\nresource that all ``thread_sensitive`` code must run on, and there is a chance\nthat this thread is currently blocked on its own ``AsyncToSync`` call. Thus,\n``AsyncToSync`` needs to act as an executor for thread code while it's blocking.\n\nThe ``CurrentThreadExecutor`` class provides this functionality; rather than\nsimply waiting on a Future, you can call its ``run_until_future`` method and\nit will run submitted code until that Future is done. This means that code\ninside the call can then run code on your thread.\n\n\nMaintenance and Security\n------------------------\n\nTo report security issues, please contact security@djangoproject.com. For GPG\nsignatures and more security process information, see\nhttps://docs.djangoproject.com/en/dev/internals/security/.\n\nTo report bugs or request new features, please open a new GitHub issue.\n\nThis repository is part of the Channels project. For the shepherd and maintenance team, please see the\n`main Channels readme <https://github.com/django/channels/blob/master/README.rst>`_.",
             "downloadLocation": "NOASSERTION",
             "externalRefs": [
                 {
                     "referenceCategory": "PACKAGE-MANAGER",
                     "referenceLocator": "pkg:pypi/asgiref@3.3.0",
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998575498575497%*

 * *Differences: {'20': "{'fields': {'notice_text': 'NOTICE_TEXT'}}",*

 * * '21': "{'fields': {'notice_text': 'NOTICE_TEXT'}}"}*

```diff
@@ -1410,15 +1410,15 @@
                 }
             ],
             "md5": "",
             "missing_resources": [],
             "modified_resources": [],
             "name": "asgiref",
             "namespace": "",
-            "notice_text": "",
+            "notice_text": "NOTICE_TEXT",
             "other_license_detections": [],
             "other_license_expression": "",
             "other_license_expression_spdx": "",
             "package_uid": "pkg:pypi/asgiref@3.3.0?uuid=e60b7109-14eb-47af-9568-09b4b630dca5",
             "parties": [
                 {
                     "email": "foundation@djangoproject.com",
@@ -1540,15 +1540,15 @@
                 }
             ],
             "md5": "",
             "missing_resources": [],
             "modified_resources": [],
             "name": "asgiref",
             "namespace": "",
-            "notice_text": "",
+            "notice_text": "NOTICE_TEXT",
             "other_license_detections": [],
             "other_license_expression": "",
             "other_license_expression_spdx": "",
             "package_uid": "pkg:pypi/asgiref@3.3.0?uuid=f66d2b7c-233e-4a6a-93d8-1d17732704e9",
             "parties": [
                 {
                     "email": "foundation@djangoproject.com",
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_tree.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_tree.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json` & `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/basic-rootfs.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json` & `scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'headers'": "{0: {'extra_data': {replace: OrderedDict([('root_filesystems', "*

 * *              "[OrderedDict([('name', 'basic-rootfs.tar.gz-extract'), ('distro', "*

 * *              "OrderedDict([('os', 'linux'), ('architecture', None), ('name', 'Debian GNU/Linux'), "*

 * *              "('version', '9 (stretch)'), ('identifier', 'debian'), ('id_like', None), "*

 * *              "('version_codename', None), ('version_id', '9'), ('pretty_name', 'Debian GNU/Linux "*

 * *              "9 (stretch)'), ('cpe_name', None), ('home_u […]*

```diff
@@ -731,39 +731,41 @@
                 }
             ]
         }
     ],
     "headers": [
         {
             "extra_data": {
-                "images": {
-                    "distro": {
-                        "architecture": null,
-                        "bug_report_url": "https://bugs.debian.org/",
-                        "build_id": null,
-                        "cpe_name": null,
-                        "documentation_url": null,
-                        "extra_data": {},
-                        "home_url": "https://www.debian.org/",
-                        "id_like": null,
-                        "identifier": "debian",
-                        "logo": null,
-                        "name": "Debian GNU/Linux",
-                        "os": "linux",
-                        "pretty_name": "Debian GNU/Linux 9 (stretch)",
-                        "privacy_policy_url": null,
-                        "support_url": "https://www.debian.org/support",
-                        "variant": null,
-                        "variant_id": null,
-                        "version": "9 (stretch)",
-                        "version_codename": null,
-                        "version_id": "9"
-                    },
-                    "name": "basic-rootfs.tar.gz-extract"
-                }
+                "root_filesystems": [
+                    {
+                        "distro": {
+                            "architecture": null,
+                            "bug_report_url": "https://bugs.debian.org/",
+                            "build_id": null,
+                            "cpe_name": null,
+                            "documentation_url": null,
+                            "extra_data": {},
+                            "home_url": "https://www.debian.org/",
+                            "id_like": null,
+                            "identifier": "debian",
+                            "logo": null,
+                            "name": "Debian GNU/Linux",
+                            "os": "linux",
+                            "pretty_name": "Debian GNU/Linux 9 (stretch)",
+                            "privacy_policy_url": null,
+                            "support_url": "https://www.debian.org/support",
+                            "variant": null,
+                            "variant_id": null,
+                            "version": "9 (stretch)",
+                            "version_codename": null,
+                            "version_id": "9"
+                        },
+                        "name": "basic-rootfs.tar.gz-extract"
+                    }
+                ]
             },
             "input_sources": [],
             "notice": "Generated with ScanCode.io and provided on an \"AS IS\" BASIS, WITHOUT WARRANTIES\nOR CONDITIONS OF ANY KIND, either express or implied.\nNo content created from ScanCode.io should be considered or used as legal advice.\nConsult an Attorney for any legal advice.\nScanCode.io is a free software code scanning tool from nexB Inc. and others\nlicensed under the Apache License version 2.0.\nScanCode is a trademark of nexB Inc.\nVisit https://github.com/nexB/scancode.io for support and download.\n",
             "runs": [
                 {
                     "description": "Analyze a Linux root filesystem, aka rootfs.",
                     "execution_time": null,
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/centos.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/centos.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/centos_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/centos_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json` & `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988425925925926%*

 * *Differences: {"'components'": "{0: {'properties': {insert: [(1, OrderedDict([('name', 'aboutcode:notice_text'), "*

 * *                 "('value', 'NOTICE_TEXT')]))]}}}"}*

```diff
@@ -27,14 +27,18 @@
             "name": "asgiref",
             "properties": [
                 {
                     "name": "aboutcode:homepage_url",
                     "value": "https://github.com/django/asgiref/"
                 },
                 {
+                    "name": "aboutcode:notice_text",
+                    "value": "NOTICE_TEXT"
+                },
+                {
                     "name": "aboutcode:primary_language",
                     "value": "Python"
                 }
             ],
             "purl": "pkg:pypi/asgiref@3.3.0",
             "type": "library",
             "version": "3.3.0"
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json` & `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/missing_schema.json` & `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/missing_schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/cyclonedx/nested.cdx.json` & `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/nested.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/expected.json` & `scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/expected.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9706154185629927%*

 * *Differences: {"'files'": "{2: {'md5': '5db9e5cfad2986d7f1e8cd7633100b16', 'sha1': "*

 * *            "'5a8183c7d9d9dcc56c5c7a57ae6a30003917e810', 'sha256': "*

 * *            "'da45c05ba8f0a7e434759085ac7048a4d51c5cc19b6af1d34f932bcb4ed1ecb1', "*

 * *            "'license_detections': {0: {'matches': {0: {'end_line': 8, 'start_line': 8}, 1: "*

 * *            "{'end_line': 11, 'start_line': 11}, 2: {'end_line': 12, 'start_line': 12}, 3: "*

 * *            "{'end_line': 13, 'start_line': 13}}}}, 'percentage_of_license_text': 18.29, 'urls': "*

 * *    […]*

```diff
@@ -81,94 +81,370 @@
             "license_clues": [],
             "license_detections": [
                 {
                     "identifier": "apache_2_0-6ac1a8f1-4540-e467-4f69-5e1984b60129",
                     "license_expression": "apache-2.0",
                     "matches": [
                         {
-                            "end_line": 6,
+                            "end_line": 8,
                             "license_expression": "apache-2.0",
                             "match_coverage": 100.0,
                             "matched_length": 3,
                             "matched_text": "license_expression: apache-2.0",
                             "matcher": "2-aho",
                             "rule_identifier": "spdx_license_id_apache-2.0_for_apache-2.0.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/spdx_license_id_apache-2.0_for_apache-2.0.RULE",
                             "score": 100.0,
-                            "start_line": 6
+                            "start_line": 8
                         },
                         {
-                            "end_line": 9,
+                            "end_line": 11,
                             "license_expression": "apache-2.0",
                             "match_coverage": 100.0,
                             "matched_length": 3,
                             "matched_text": "  - key: apache-2.0",
                             "matcher": "2-aho",
                             "rule_identifier": "spdx_license_id_apache-2.0_for_apache-2.0.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/spdx_license_id_apache-2.0_for_apache-2.0.RULE",
                             "score": 100.0,
-                            "start_line": 9
+                            "start_line": 11
                         },
                         {
-                            "end_line": 10,
+                            "end_line": 12,
                             "license_expression": "apache-2.0",
                             "match_coverage": 100.0,
                             "matched_length": 5,
                             "matched_text": "    name: Apache License 2.0",
                             "matcher": "2-aho",
                             "rule_identifier": "apache-2.0_1039.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/apache-2.0_1039.RULE",
                             "score": 100.0,
-                            "start_line": 10
+                            "start_line": 12
                         },
                         {
-                            "end_line": 11,
+                            "end_line": 13,
                             "license_expression": "apache-2.0",
                             "match_coverage": 100.0,
                             "matched_length": 4,
                             "matched_text": "    file: apache-2.0.LICENSE",
                             "matcher": "2-aho",
                             "rule_identifier": "apache-2.0_176.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/apache-2.0_176.RULE",
                             "score": 100.0,
-                            "start_line": 11
+                            "start_line": 13
                         }
                     ]
                 }
             ],
-            "md5": "d7c3f25f4159f2d93a3203190816443d",
+            "md5": "5db9e5cfad2986d7f1e8cd7633100b16",
             "name": "flume-ng-node-1.9.0-sources.ABOUT",
             "package_data": [],
             "path": "from/flume-ng-node-1.9.0-sources.ABOUT",
-            "percentage_of_license_text": 22.39,
+            "percentage_of_license_text": 18.29,
             "programming_language": "",
-            "sha1": "4efb1dc6691b759dd5885080f64b5b4fe06bd518",
-            "sha256": "bdebcdfbf7f53eba3fa115801fbebc01429fcba7f07aa76556c0eb0ca9d16336",
+            "sha1": "5a8183c7d9d9dcc56c5c7a57ae6a30003917e810",
+            "sha256": "da45c05ba8f0a7e434759085ac7048a4d51c5cc19b6af1d34f932bcb4ed1ecb1",
             "sha512": "",
             "status": "scanned",
             "tag": "from",
             "type": "file",
             "urls": [
                 {
-                    "end_line": 4,
-                    "start_line": 4,
+                    "end_line": 6,
+                    "start_line": 6,
                     "url": "https://repo1.maven.org/maven2/log4j/log4j/1.2.13/log4j-1.2.13.jar"
                 }
             ]
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
+            "extension": ".jar",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": true,
+            "is_binary": true,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "890f2f18119ee83e5fc63fc438bd2367",
+            "name": "flume-ng-node-1.9.0-sources.jar",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "ca559dc7dbbf551f3f8d848c70bc8b2679dc8cf4",
+            "sha256": "2c41dffc2ae1ea7603f4fb497f8ffecc4c5fec6c52e0033c37764ecdf1866793",
+            "sha512": "",
+            "status": "",
+            "tag": "from",
+            "type": "file",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": ".jar-extract",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "flume-ng-node-1.9.0-sources.jar-extract",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "ignored-directory",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": ".jar-extract",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "flume-ng-node-1.9.0-sources.jar-extract",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "mapped",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": "",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "org",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "ignored-directory",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": "",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "apache",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org/apache",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "ignored-directory",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": "",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "flume",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org/apache/flume",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "ignored-directory",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
+            "extension": "",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": false,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "",
+            "name": "node",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org/apache/flume/node",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "",
+            "sha256": "",
+            "sha512": "",
+            "status": "ignored-directory",
+            "tag": "from",
+            "type": "directory",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "apache-2.0",
+            "detected_license_expression_spdx": "Apache-2.0",
+            "emails": [],
+            "extension": ".java",
+            "extra_data": {
+                "java_package": "org.apache.flume.node"
+            },
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": true,
+            "license_clues": [],
+            "license_detections": [
+                {
+                    "identifier": "apache_2_0-4bde3f57-78aa-4201-96bf-531cba09e7de",
+                    "license_expression": "apache-2.0",
+                    "matches": [
+                        {
+                            "end_line": 17,
+                            "license_expression": "apache-2.0",
+                            "match_coverage": 100.0,
+                            "matched_length": 119,
+                            "matched_text": " * Licensed to the Apache Software Foundation (ASF) under one\n * or more contributor license agreements.  See the NOTICE file\n * distributed with this work for additional information\n * regarding copyright ownership.  The ASF licenses this file\n * to you under the Apache License, Version 2.0 (the\n * \"License\"); you may not use this file except in compliance\n * with the License.  You may obtain a copy of the License at\n *\n * http://www.apache.org/licenses/LICENSE-2.0\n *\n * Unless required by applicable law or agreed to in writing,\n * software distributed under the License is distributed on an\n * \"AS IS\" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\n * KIND, either express or implied.  See the License for the\n * specific language governing permissions and limitations\n * under the License.",
+                            "matcher": "2-aho",
+                            "rule_identifier": "apache-2.0_2.RULE",
+                            "rule_relevance": 100,
+                            "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/apache-2.0_2.RULE",
+                            "score": 100.0,
+                            "start_line": 2
+                        }
+                    ]
+                }
+            ],
+            "md5": "318484f1071022f375cd0fd99e9fe844",
+            "name": "ConfigurationProvider.java",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org/apache/flume/node/ConfigurationProvider.java",
+            "percentage_of_license_text": 92.25,
+            "programming_language": "Java",
+            "sha1": "dde981f3bc981e630b3e8673321c2d152d39761c",
+            "sha256": "6768adff7b9027b50ba16fa24a8ac900a0a24c7df34ed0027547d049a7b6e4e6",
+            "sha512": "",
+            "status": "scanned",
+            "tag": "from",
+            "type": "file",
+            "urls": [
+                {
+                    "end_line": 10,
+                    "start_line": 10,
+                    "url": "http://www.apache.org/licenses/LICENSE-2.0"
+                }
+            ]
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
             "extension": ".NOTICE",
             "extra_data": {},
             "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
@@ -885,17 +1161,15 @@
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": ".class",
             "extra_data": {},
-            "for_packages": [
-                "pkg:maven/log4j/log4j@1.2.13?uuid=fixed-uid-done-for-testing-5642512d1758"
-            ],
+            "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": true,
             "is_key_file": false,
             "is_media": false,
             "is_text": false,
             "license_clues": [],
@@ -1242,15 +1516,19 @@
             "code_view_url": "",
             "copyright": "",
             "datasource_id": "",
             "declared_license_expression": "apache-2.0",
             "declared_license_expression_spdx": "",
             "description": "",
             "download_url": "https://repo1.maven.org/maven2/log4j/log4j/1.2.13/log4j-1.2.13.jar",
-            "extra_data": {},
+            "extra_data": {
+                "ignored_resources": [
+                    "flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/ConfigurationProvider.class"
+                ]
+            },
             "extracted_license_statement": "",
             "file_references": [],
             "holder": "",
             "homepage_url": "",
             "keywords": [],
             "license_detections": [],
             "md5": "",
@@ -1380,19 +1658,14 @@
             "from_resource": "from/flume-ng-node-1.9.0-sources.ABOUT",
             "map_type": "about_file",
             "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/Application.class"
         },
         {
             "from_resource": "from/flume-ng-node-1.9.0-sources.ABOUT",
             "map_type": "about_file",
-            "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/ConfigurationProvider.class"
-        },
-        {
-            "from_resource": "from/flume-ng-node-1.9.0-sources.ABOUT",
-            "map_type": "about_file",
             "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/EnvVarResolverProperties.class"
         },
         {
             "from_resource": "from/flume-ng-node-1.9.0-sources.ABOUT",
             "map_type": "about_file",
             "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/MaterializedConfiguration.class"
         },
@@ -1426,10 +1699,20 @@
             "map_type": "about_file",
             "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/SimpleMaterializedConfiguration.class"
         },
         {
             "from_resource": "from/flume-ng-node-1.9.0-sources.ABOUT",
             "map_type": "about_file",
             "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/StaticZooKeeperConfigurationProvider.class"
+        },
+        {
+            "from_resource": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract",
+            "map_type": "jar_to_source",
+            "to_resource": "to/flume-ng-node-1.9.0.jar"
+        },
+        {
+            "from_resource": "from/flume-ng-node-1.9.0-sources.jar-extract/flume-ng-node-1.9.0-sources.jar-extract/org/apache/flume/node/ConfigurationProvider.java",
+            "map_type": "java_to_class",
+            "to_resource": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/ConfigurationProvider.class"
         }
     ]
 }
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip` & `scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip` & `scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip` & `scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/from/main.js` & `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/from/unmain.js` & `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/unmain.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/main.js.map` & `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map` & `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map` & `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl` & `scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999954753971212%*

 * *Differences: {"'files'": "{0: {'package_data': {0: {'license_detections': {1: {'matches': {0: {'matched_text': "*

 * *            '"- \'License :: OSI Approved :: MIT License\'"}}}}}}}, 5: {\'package_data\': {0: '*

 * *            '{\'license_detections\': {1: {\'matches\': {0: {\'matched_text\': "- \'License :: OSI '*

 * *            'Approved :: MIT License\'"}}}}}}}}',*

 * * "'packages'": '{0: {\'license_detections\': {1: {\'matches\': {0: {\'matched_text\': "- \'License '*

 * *               ':: OSI Approved :: MIT License\'"}}}}}, 1: {\'li […]*

```diff
@@ -274,15 +274,15 @@
                             "license_expression": "mit",
                             "matches": [
                                 {
                                     "end_line": 1,
                                     "license_expression": "mit",
                                     "match_coverage": 100.0,
                                     "matched_length": 5,
-                                    "matched_text": "['License :: OSI Approved :: MIT License']",
+                                    "matched_text": "- 'License :: OSI Approved :: MIT License'",
                                     "matcher": "1-hash",
                                     "rule_identifier": "pypi_mit_license.RULE",
                                     "rule_relevance": 100,
                                     "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/pypi_mit_license.RULE",
                                     "score": 100.0,
                                     "start_line": 1
                                 }
@@ -658,15 +658,15 @@
                             "license_expression": "mit",
                             "matches": [
                                 {
                                     "end_line": 1,
                                     "license_expression": "mit",
                                     "match_coverage": 100.0,
                                     "matched_length": 5,
-                                    "matched_text": "['License :: OSI Approved :: MIT License']",
+                                    "matched_text": "- 'License :: OSI Approved :: MIT License'",
                                     "matcher": "1-hash",
                                     "rule_identifier": "pypi_mit_license.RULE",
                                     "rule_relevance": 100,
                                     "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/pypi_mit_license.RULE",
                                     "score": 100.0,
                                     "start_line": 1
                                 }
@@ -958,15 +958,15 @@
                     "license_expression": "mit",
                     "matches": [
                         {
                             "end_line": 1,
                             "license_expression": "mit",
                             "match_coverage": 100.0,
                             "matched_length": 5,
-                            "matched_text": "['License :: OSI Approved :: MIT License']",
+                            "matched_text": "- 'License :: OSI Approved :: MIT License'",
                             "matcher": "1-hash",
                             "rule_identifier": "pypi_mit_license.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/pypi_mit_license.RULE",
                             "score": 100.0,
                             "start_line": 1
                         }
@@ -1055,15 +1055,15 @@
                     "license_expression": "mit",
                     "matches": [
                         {
                             "end_line": 1,
                             "license_expression": "mit",
                             "match_coverage": 100.0,
                             "matched_length": 5,
-                            "matched_text": "['License :: OSI Approved :: MIT License']",
+                            "matched_text": "- 'License :: OSI Approved :: MIT License'",
                             "matcher": "1-hash",
                             "rule_identifier": "pypi_mit_license.RULE",
                             "rule_relevance": 100,
                             "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/pypi_mit_license.RULE",
                             "score": 100.0,
                             "start_line": 1
                         }
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/debian.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/debian.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/debian_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/debian_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html` & `scancodeio-32.5.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json` & `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json` & `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz` & `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json` & `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz` & `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json` & `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/flume-ng-node-d2d.json` & `scancodeio-32.5.0/scanpipe/tests/data/flume-ng-node-d2d.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/foobar.qcow2.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/foobar.qcow2.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar` & `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar` & `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json` & `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json` & `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json` & `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0.tgz` & `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0.tgz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json` & `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666666%*

 * *Differences: {"'headers'": "{0: {'extra_data': {'spdx_license_list_version': '3.21'}}}"}*

```diff
@@ -393,15 +393,15 @@
         }
     ],
     "headers": [
         {
             "errors": [],
             "extra_data": {
                 "files_count": 3,
-                "spdx_license_list_version": "3.20"
+                "spdx_license_list_version": "3.21"
             },
             "message": null,
             "notice": "Generated with ScanCode and provided on an \"AS IS\" BASIS, WITHOUT WARRANTIES\nOR CONDITIONS OF ANY KIND, either express or implied. No content created from\nScanCode should be considered or used as legal advice. Consult an Attorney\nfor any legal advice.\nScanCode is a free software code scanning tool from nexB Inc. and others.\nVisit https://github.com/nexB/scancode-toolkit/ for support and download.",
             "options": {
                 "--classify": true,
                 "--copyright": true,
                 "--email": true,
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json` & `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/jvm/common.java` & `scancodeio-32.5.0/scanpipe/tests/data/jvm/common.java`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/manifests/package.expected.json` & `scancodeio-32.5.0/scanpipe/tests/data/manifests/package.expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/manifests/package.json` & `scancodeio-32.5.0/scanpipe/tests/data/manifests/package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/manifests/toml.json` & `scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/manifests/toml.spdx.json` & `scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz` & `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json` & `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972098214285715%*

 * *Differences: {"'headers'": "{0: {'extra_data': {'spdx_license_list_version': '3.21'}}}",*

 * * "'summary'": "{'other_license_expressions': {0: {'count': 2}}}"}*

```diff
@@ -782,15 +782,15 @@
         }
     ],
     "headers": [
         {
             "errors": [],
             "extra_data": {
                 "files_count": 6,
-                "spdx_license_list_version": "3.20"
+                "spdx_license_list_version": "3.21"
             },
             "message": null,
             "notice": "Generated with ScanCode and provided on an \"AS IS\" BASIS, WITHOUT WARRANTIES\nOR CONDITIONS OF ANY KIND, either express or implied. No content created from\nScanCode should be considered or used as legal advice. Consult an Attorney\nfor any legal advice.\nScanCode is a free software code scanning tool from nexB Inc. and others.\nVisit https://github.com/nexB/scancode-toolkit/ for support and download.",
             "options": {
                 "--classify": true,
                 "--copyright": true,
                 "--email": true,
@@ -997,14 +997,14 @@
                 "count": 4,
                 "value": null
             }
         ],
         "other_languages": [],
         "other_license_expressions": [
             {
-                "count": 1,
+                "count": 2,
                 "value": null
             }
         ],
         "primary_language": "JavaScript"
     }
 }
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json` & `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'other_license_expressions'": "{0: {'count': 2}}"}*

```diff
@@ -237,13 +237,13 @@
             "count": 4,
             "value": null
         }
     ],
     "other_languages": [],
     "other_license_expressions": [
         {
-            "count": 1,
+            "count": 2,
             "value": null
         }
     ],
     "primary_language": "JavaScript"
 }
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/notice.NOTICE` & `scancodeio-32.5.0/scanpipe/tests/data/notice.NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx` & `scancodeio-32.5.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/outputs/expected_attribution.html` & `scancodeio-32.5.0/scanpipe/tests/data/outputs/expected_attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json` & `scancodeio-32.5.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/scancode/package_assembly_codebase.json` & `scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/data/windows-container-rootfs.tar` & `scancodeio-32.5.0/scanpipe/tests/data/windows-container-rootfs.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipelines/do_nothing.py` & `scancodeio-32.5.0/scanpipe/tests/pipelines/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipelines/profile_step.py` & `scancodeio-32.5.0/scanpipe/tests/pipelines/profile_step.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipelines/raise_exception.py` & `scancodeio-32.5.0/scanpipe/tests/pipelines/raise_exception.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipelines/register_from_file.py` & `scancodeio-32.5.0/scanpipe/tests/pipelines/register_from_file.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipelines/steps_as_attribute.py` & `scancodeio-32.5.0/scanpipe/tests/pipelines/steps_as_attribute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_codebase.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_cyclonedx.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_d2d.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_d2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,27 +42,37 @@
 
     def setUp(self):
         self.project1 = Project.objects.create(name="Analysis")
 
     def test_scanpipe_pipes_d2d_get_inputs(self):
         with self.assertRaises(FileNotFoundError) as error:
             d2d.get_inputs(self.project1)
-        self.assertEqual("from* archive not found.", str(error.exception))
+        self.assertEqual("from* input files not found.", str(error.exception))
 
         _, input_location = tempfile.mkstemp(prefix="from-")
         self.project1.copy_input_from(input_location)
 
         with self.assertRaises(FileNotFoundError) as error:
             d2d.get_inputs(self.project1)
-        self.assertEqual("to* archive not found.", str(error.exception))
+        self.assertEqual("to* input files not found.", str(error.exception))
 
         _, input_location = tempfile.mkstemp(prefix="to-")
         self.project1.copy_input_from(input_location)
 
-        self.assertEqual(2, len(d2d.get_inputs(self.project1)))
+        from_files, to_files = d2d.get_inputs(self.project1)
+        self.assertEqual(1, len(from_files))
+        self.assertEqual(1, len(to_files))
+
+        _, input_location = tempfile.mkstemp(prefix="from-")
+        self.project1.copy_input_from(input_location)
+        _, input_location = tempfile.mkstemp(prefix="to-")
+        self.project1.copy_input_from(input_location)
+        from_files, to_files = d2d.get_inputs(self.project1)
+        self.assertEqual(2, len(from_files))
+        self.assertEqual(2, len(to_files))
 
     def test_scanpipe_pipes_d2d_get_resource_codebase_root(self):
         input_location = self.data_location / "codebase" / "a.txt"
         file_location = copy_input(input_location, self.project1.codebase_path)
         codebase_root = d2d.get_resource_codebase_root(self.project1, file_location)
         self.assertEqual("", codebase_root)
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_docker.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,7 +181,13 @@
         self.assertEqual(5855232, layers_data[0].size)
         self.assertEqual("Author", layers_data[0].author)
         self.assertEqual("Comment", layers_data[0].comment)
         self.assertEqual(layers[0]["archive_location"], layers_data[0].archive_location)
 
         self.assertEqual("img-06a4df-layer-02-fbd7d5", layers_data[1].layer_tag)
         self.assertEqual(layers[1]["archive_location"], layers_data[1].archive_location)
+
+        from_old_rootfs = {
+            "images": {"name": "packageurl-python-main.zip-extract", "distro": {}}
+        }
+        p1.update_extra_data(from_old_rootfs)
+        self.assertEqual([], docker.get_layers_data(p1))
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_fetch.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_fetch.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_flag.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_input.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_js.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_jvm.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_output.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,42 @@
         self.assertResultsEqual(expected_file, results)
 
         # Make sure the output can be generated even if the work_directory was wiped
         shutil.rmtree(project.work_directory)
         output_file = output.to_spdx(project=project)
         self.assertIn(output_file.name, project.output_root)
 
+    def test_scanpipe_pipes_outputs_to_spdx_extracted_licenses(self):
+        project = Project.objects.create(name="Analysis")
+        package_data = dict(package_data1)
+        # ac3filter resolves as LicenseRef-scancode-ac3filter
+        expression = "mit AND ac3filter"
+        package_data["declared_license_expression"] = expression
+        pipes.update_or_create_package(project, package_data)
+
+        output_file = output.to_spdx(project=project, include_files=True)
+        self.assertIn(output_file.name, project.output_root)
+
+        results_json = json.loads(output_file.read_text())
+        # mit is part of the SPDX license list, thus not in hasExtractedLicensingInfos
+        self.assertEqual(1, len(results_json["hasExtractedLicensingInfos"]))
+        license_infos = results_json["hasExtractedLicensingInfos"][0]
+        self.assertEqual("LicenseRef-scancode-ac3filter", license_infos["licenseId"])
+        self.assertEqual("AC3Filter License", license_infos["name"])
+        expected = [
+            "https://scancode-licensedb.aboutcode.org/ac3filter",
+            "https://github.com/nexB/scancode-toolkit/tree/develop/src/"
+            "licensedcode/data/licenses/ac3filter.LICENSE",
+            "http://www.ac3filter.net/wiki/Download_AC3Filter",
+            "http://ac3filter.net",
+            "http://ac3filter.net/forum",
+        ]
+        self.assertEqual(expected, license_infos["seeAlsos"])
+        self.assertTrue(license_infos["extractedText"].startswith("License:"))
+
     def test_scanpipe_pipes_outputs_make_unknown_license_object(self):
         licensing = get_licensing()
         parsed_expression = licensing.parse("some-unknown-license")
 
         self.assertEqual(1, len(parsed_expression.symbols))
         license_symbol = list(parsed_expression.symbols)[0]
         license_object = output.make_unknown_license_object(license_symbol)
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_pathmap.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_pipes.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_pipes.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_resolve.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_resolve.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_rootfs.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_scancode.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_spdx.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/pipes/test_windows.py` & `scancodeio-32.5.0/scanpipe/tests/pipes/test_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/regen_test_data.py` & `scancodeio-32.5.0/scanpipe/tests/regen_test_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_api.py` & `scancodeio-32.5.0/scanpipe/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -703,14 +703,39 @@
 
         run3.set_task_stopped()
         response = self.csrf_client.post(url)
         self.assertEqual(status.HTTP_400_BAD_REQUEST, response.status_code)
         expected = {"status": "Only non started or queued pipelines can be deleted."}
         self.assertEqual(expected, response.data)
 
+    def test_scanpipe_api_project_action_outputs(self):
+        url = reverse("project-outputs", args=[self.project1.uuid])
+        response = self.csrf_client.get(url)
+        self.assertEqual([], response.data)
+
+        output_file = self.project1.get_output_file_path("scan", "txt")
+        output_file.write_text("content")
+        response = self.csrf_client.get(url)
+        download_url = f"http://testserver{url}?filename={output_file.name}"
+        expected = [
+            {
+                "download_url": download_url,
+                "filename": output_file.name,
+            }
+        ]
+        self.assertEqual(expected, response.data)
+
+        response = self.csrf_client.get(download_url)
+        self.assertEqual(b"content", response.getvalue())
+
+        response = self.csrf_client.get(f"http://testserver{url}?filename=NOT_FOUND")
+        self.assertEqual(status.HTTP_400_BAD_REQUEST, response.status_code)
+        expected = {"status": "Output file NOT_FOUND not found"}
+        self.assertEqual(expected, response.data)
+
     def test_scanpipe_api_serializer_get_model_serializer(self):
         self.assertEqual(
             DiscoveredPackageSerializer, get_model_serializer(DiscoveredPackage)
         )
         self.assertEqual(
             DiscoveredDependencySerializer, get_model_serializer(DiscoveredDependency)
         )
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_apps.py` & `scancodeio-32.5.0/scanpipe/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_auth.py` & `scancodeio-32.5.0/scanpipe/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_commands.py` & `scancodeio-32.5.0/scanpipe/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_filters.py` & `scancodeio-32.5.0/scanpipe/tests/test_filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,22 +21,26 @@
 # Visit https://github.com/nexB/scancode.io for support and download.
 
 import uuid
 
 from django.test import TestCase
 from django.utils import timezone
 
+from scanpipe.filters import DependencyFilterSet
 from scanpipe.filters import FilterSetUtilsMixin
 from scanpipe.filters import PackageFilterSet
 from scanpipe.filters import ProjectFilterSet
 from scanpipe.filters import ResourceFilterSet
 from scanpipe.models import CodebaseResource
+from scanpipe.models import DiscoveredDependency
 from scanpipe.models import DiscoveredPackage
 from scanpipe.models import Project
 from scanpipe.models import Run
+from scanpipe.tests import dependency_data1
+from scanpipe.tests import dependency_data2
 from scanpipe.tests import package_data1
 from scanpipe.tests import package_data2
 
 
 class ScanPipeFilterTest(TestCase):
     def setUp(self):
         self.project1 = Project.objects.create(name="Analysis")
@@ -154,7 +158,48 @@
         self.assertEqual(2, len(filterset.qs))
 
         filterset = PackageFilterSet(data={"is_vulnerable": "no"})
         self.assertEqual([p1], list(filterset.qs))
 
         filterset = PackageFilterSet(data={"is_vulnerable": "yes"})
         self.assertEqual([p2], list(filterset.qs))
+
+    def test_scanpipe_filters_dependency_filterset(self):
+        DiscoveredPackage.create_from_data(self.project1, package_data1)
+        CodebaseResource.objects.create(
+            project=self.project1,
+            path="daglib-0.3.2.tar.gz-extract/daglib-0.3.2/PKG-INFO",
+        )
+        CodebaseResource.objects.create(
+            project=self.project1,
+            path="data.tar.gz-extract/Gemfile.lock",
+        )
+        d1 = DiscoveredDependency.create_from_data(self.project1, dependency_data1)
+        d2 = DiscoveredDependency.create_from_data(self.project1, dependency_data2)
+
+        filterset = DependencyFilterSet(data={"is_resolved": ""})
+        self.assertEqual(2, len(filterset.qs))
+        filterset = DependencyFilterSet(data={"is_resolved": True})
+        self.assertEqual([d2], list(filterset.qs))
+        filterset = DependencyFilterSet(data={"is_resolved": False})
+        self.assertEqual([d1], list(filterset.qs))
+
+        filterset = DependencyFilterSet(data={"type": ""})
+        self.assertEqual(2, len(filterset.qs))
+        filterset = DependencyFilterSet(data={"type": "pypi"})
+        self.assertEqual([d1], list(filterset.qs))
+        filterset = DependencyFilterSet(data={"type": "gem"})
+        self.assertEqual([d2], list(filterset.qs))
+
+        filterset = DependencyFilterSet(data={"scope": ""})
+        self.assertEqual(2, len(filterset.qs))
+        filterset = DependencyFilterSet(data={"scope": "install"})
+        self.assertEqual([d1], list(filterset.qs))
+        filterset = DependencyFilterSet(data={"scope": "dependencies"})
+        self.assertEqual([d2], list(filterset.qs))
+
+        filterset = DependencyFilterSet(data={"datasource_id": ""})
+        self.assertEqual(2, len(filterset.qs))
+        filterset = DependencyFilterSet(data={"datasource_id": "pypi_sdist_pkginfo"})
+        self.assertEqual([d1], list(filterset.qs))
+        filterset = DependencyFilterSet(data={"datasource_id": "gemfile_lock"})
+        self.assertEqual([d2], list(filterset.qs))
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_forms.py` & `scancodeio-32.5.0/scanpipe/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_licenses.py` & `scancodeio-32.5.0/scanpipe/tests/test_tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 # OR CONDITIONS OF ANY KIND, either express or implied. No content created from
 # ScanCode.io should be considered or used as legal advice. Consult an Attorney
 # for any legal advice.
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
+from unittest import mock
+
 from django.test import TestCase
-from django.test import override_settings
-from django.urls import reverse
 
+from scanpipe import tasks
+from scanpipe.models import Project
+
+
+class ScanPipeTasksTest(TestCase):
+    @mock.patch("scanpipe.pipelines.Pipeline.execute")
+    def test_scanpipe_tasks_execute_pipeline_task(self, mock_execute):
+        project = Project.objects.create(name="my_project")
+        run = project.add_pipeline("do_nothing")
+
+        mock_execute.return_value = 0, ""
+        tasks.execute_pipeline_task(run.pk)
+        mock_execute.assert_called_once()
 
-@override_settings(SCANCODEIO_REQUIRE_AUTHENTICATION=False)
-class LicensesTest(TestCase):
-    def test_license_list_view(self):
-        url = reverse("license_list")
-        response = self.client.get(url)
-        self.assertEqual(response.status_code, 200)
-
-    def test_license_details_view(self):
-        keys = ["apache-2.0", "abcdefg"]
-        license_url = reverse("license_details", args=(keys[0],))
-        dummy_license_url = reverse("license_details", args=(keys[1],))
-        response = [self.client.get(license_url), self.client.get(dummy_license_url)]
-        self.assertEqual(response[0].status_code, 200)
-        self.assertEqual(response[1].status_code, 404)
+        run.refresh_from_db()
+        self.assertEqual(0, run.task_exitcode)
+        self.assertEqual("", run.task_output)
+        self.assertIsNotNone(run.task_start_date)
+        self.assertIsNotNone(run.task_end_date)
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_models.py` & `scancodeio-32.5.0/scanpipe/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 from scanpipe.models import ProjectError
 from scanpipe.models import Run
 from scanpipe.models import RunInProgressError
 from scanpipe.models import get_project_work_directory
 from scanpipe.models import posix_regex_to_django_regex_lookup
 from scanpipe.pipes.fetch import Download
 from scanpipe.pipes.input import copy_input
-from scanpipe.pipes.input import copy_inputs
 from scanpipe.tests import dependency_data1
 from scanpipe.tests import dependency_data2
 from scanpipe.tests import license_policies_index
 from scanpipe.tests import make_resource_file
 from scanpipe.tests import mocked_now
 from scanpipe.tests import package_data1
 from scanpipe.tests import package_data2
@@ -346,36 +345,59 @@
             return x.get("name")
 
         self.assertEqual(
             sorted(expected, key=sort_by_name), sorted(inputs, key=sort_by_name)
         )
         self.assertEqual({"missing.zip": "uploaded"}, missing_inputs)
 
-    def test_scanpipe_project_model_can_add_input(self):
-        self.assertTrue(self.project1.can_add_input)
+    def test_scanpipe_project_model_can_change_inputs(self):
+        self.assertTrue(self.project1.can_change_inputs)
 
         run = self.project1.add_pipeline("docker")
         self.project1 = Project.objects.get(uuid=self.project1.uuid)
-        self.assertTrue(self.project1.can_add_input)
+        self.assertTrue(self.project1.can_change_inputs)
 
         run.task_start_date = timezone.now()
         run.save()
         self.project1 = Project.objects.get(uuid=self.project1.uuid)
-        self.assertFalse(self.project1.can_add_input)
+        self.assertFalse(self.project1.can_change_inputs)
 
     def test_scanpipe_project_model_add_input_source(self):
         self.assertEqual({}, self.project1.input_sources)
 
         self.project1.add_input_source("filename", "source", save=True)
         self.project1.refresh_from_db()
         self.assertEqual({"filename": "source"}, self.project1.input_sources)
 
+    def test_scanpipe_project_model_delete_input(self):
+        self.assertEqual({}, self.project1.input_sources)
+        self.assertEqual([], list(self.project1.inputs()))
+        deleted = self.project1.delete_input(name="not_existing")
+        self.assertFalse(deleted)
+
+        file_location = self.data_location / "notice.NOTICE"
+        copy_input(file_location, self.project1.input_path)
+        self.project1.add_input_source(
+            filename=file_location.name, source="uploaded", save=True
+        )
+        self.project1.refresh_from_db()
+        self.assertEqual({file_location.name: "uploaded"}, self.project1.input_sources)
+        self.assertEqual(
+            [file_location.name], [path.name for path in self.project1.inputs()]
+        )
+
+        deleted = self.project1.delete_input(name=file_location.name)
+        self.assertTrue(deleted)
+        self.project1.refresh_from_db()
+        self.assertEqual({}, self.project1.input_sources)
+        self.assertEqual([], list(self.project1.inputs()))
+
     def test_scanpipe_project_model_add_downloads(self):
         file_location = self.data_location / "notice.NOTICE"
-        copy_inputs([file_location], self.project1.tmp_path)
+        copy_input(file_location, self.project1.tmp_path)
 
         download = Download(
             uri="https://example.com/filename.zip",
             directory="",
             filename="notice.NOTICE",
             path=self.project1.tmp_path / "notice.NOTICE",
             size="",
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_pipelines.py` & `scancodeio-32.5.0/scanpipe/tests/test_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -894,15 +894,59 @@
 
         run = project1.add_pipeline(pipeline_name)
         pipeline = run.make_pipeline_instance()
 
         exitcode, out = pipeline.execute()
         self.assertEqual(0, exitcode, msg=out)
 
-        self.assertEqual(35, project1.codebaseresources.count())
-        self.assertEqual(30, project1.codebaserelations.count())
+        self.assertEqual(43, project1.codebaseresources.count())
+        self.assertEqual(31, project1.codebaserelations.count())
         self.assertEqual(1, project1.discoveredpackages.count())
         self.assertEqual(0, project1.discovereddependencies.count())
 
         result_file = output.to_json(project1)
         expected_file = data_dir / "expected.json"
         self.assertPipelineResultEqual(expected_file, result_file)
+
+    @mock.patch("scanpipe.pipes.purldb.request_post")
+    @mock.patch("scanpipe.pipes.purldb.is_available")
+    def test_scanpipe_populate_purldb_pipeline_integration_test(
+        self, mock_is_available, mock_request_post
+    ):
+        pipeline_name1 = "load_inventory"
+        pipeline_name2 = "populate_purldb"
+        project1 = Project.objects.create(name="Utility: PurlDB")
+
+        input_location = self.data_location / "asgiref-3.3.0_toolkit_scan.json"
+        project1.copy_input_from(input_location)
+
+        run = project1.add_pipeline(pipeline_name1)
+        pipeline = run.make_pipeline_instance()
+
+        exitcode, out = pipeline.execute()
+        self.assertEqual(0, exitcode, msg=out)
+
+        def mock_request_post_return(url, data, timeout):
+            return {
+                "queued_packages_count": len(data["package_urls"]),
+                "queued_packages": data["package_urls"],
+                "unqueued_packages_count": 1,
+                "unqueued_packages": [],
+                "unsupported_packages_count": 1,
+                "unsupported_packages": [],
+            }
+
+        mock_request_post.side_effect = mock_request_post_return
+        mock_is_available.return_value = True
+
+        run = project1.add_pipeline(pipeline_name2)
+        pipeline = run.make_pipeline_instance()
+
+        exitcode, out = pipeline.execute()
+        self.assertEqual(0, exitcode, msg=out)
+
+        self.assertIn("Populating PurlDB with 2 DiscoveredPackage", run.log)
+        self.assertIn("Successfully queued 2 PURLs for indexing in PurlDB", run.log)
+        self.assertIn("1 PURLs were already present in PurlDB index queue", run.log)
+        self.assertIn("Couldn't index 1 unsupported PURLs", run.log)
+        self.assertIn("Populating PurlDB with 4 DiscoveredDependency", run.log)
+        self.assertIn("Successfully queued 4 PURLs for indexing in PurlDB", run.log)
```

### Comparing `scancodeio-32.4.0/scanpipe/tests/test_views.py` & `scancodeio-32.5.0/scanpipe/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from django.urls import reverse
 
 from scanpipe.models import CodebaseResource
 from scanpipe.models import DiscoveredPackage
 from scanpipe.models import Project
 from scanpipe.pipes import make_relation
 from scanpipe.pipes import update_or_create_dependency
+from scanpipe.pipes.input import copy_input
 from scanpipe.pipes.input import copy_inputs
 from scanpipe.tests import dependency_data1
 from scanpipe.tests import make_resource_file
 from scanpipe.tests import package_data1
 from scanpipe.views import ProjectCodebaseView
 from scanpipe.views import ProjectDetailView
 
@@ -186,14 +187,63 @@
         self.assertContains(response, "Input file(s) added.")
 
         self.assertEqual(["archive.zip"], self.project1.input_files)
         expected = {"archive.zip": "https://example.com/archive.zip"}
         self.project1.refresh_from_db()
         self.assertEqual(expected, self.project1.input_sources)
 
+    def test_scanpipe_views_project_details_download_input_view(self):
+        url = reverse("project_download_input", args=[self.project1.slug, "file.zip"])
+        response = self.client.get(url)
+        self.assertEqual(404, response.status_code)
+
+        file_location = self.data_location / "notice.NOTICE"
+        copy_input(file_location, self.project1.input_path)
+        filename = file_location.name
+        url = reverse("project_download_input", args=[self.project1.slug, filename])
+        response = self.client.get(url)
+        self.assertTrue(response.getvalue().startswith(b"# SPDX-License-Identifier"))
+        self.assertEqual("application/octet-stream", response.headers["Content-Type"])
+        self.assertEqual(
+            'attachment; filename="notice.NOTICE"',
+            response.headers["Content-Disposition"],
+        )
+
+    def test_scanpipe_views_project_details_delete_input_view(self):
+        url = reverse("project_delete_input", args=[self.project1.slug, "file.zip"])
+        response = self.client.get(url)
+        self.assertEqual(405, response.status_code)
+
+        response = self.client.post(url, follow=True)
+        self.assertRedirects(response, self.project1.get_absolute_url())
+        expected = '<div class="message-body">Input file.zip not found.</div>'
+        self.assertContains(response, expected, html=True)
+
+        file_location = self.data_location / "notice.NOTICE"
+        copy_input(file_location, self.project1.input_path)
+        filename = file_location.name
+        self.project1.add_input_source(filename=filename, source="uploaded", save=True)
+
+        self.project1.update(is_archived=True)
+        self.assertFalse(self.project1.can_change_inputs)
+        url = reverse("project_delete_input", args=[self.project1.slug, filename])
+        response = self.client.post(url)
+        self.assertEqual(404, response.status_code)
+
+        self.project1.update(is_archived=False)
+        self.project1 = Project.objects.get(pk=self.project1.pk)
+        self.assertTrue(self.project1.can_change_inputs)
+        response = self.client.post(url, follow=True)
+        self.assertRedirects(response, self.project1.get_absolute_url())
+        expected = f'<div class="message-body">Input {filename} deleted.</div>'
+        self.assertContains(response, expected, html=True)
+        self.project1.refresh_from_db()
+        self.assertEqual({}, self.project1.input_sources)
+        self.assertEqual([], list(self.project1.inputs()))
+
     def test_scanpipe_views_project_details_missing_inputs(self):
         self.project1.add_input_source(
             filename="missing.zip", source="uploaded", save=True
         )
         url = self.project1.get_absolute_url()
         response = self.client.get(url)
         expected = (
```

### Comparing `scancodeio-32.4.0/scanpipe/urls.py` & `scancodeio-32.5.0/scanpipe/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,24 @@
     ),
     path(
         "project/<slug:slug>/delete_pipeline/<uuid:run_uuid>/",
         views.delete_pipeline_view,
         name="project_delete_pipeline",
     ),
     path(
+        "project/<slug:slug>/delete_input/<str:input_name>/",
+        views.delete_input_view,
+        name="project_delete_input",
+    ),
+    path(
+        "project/<slug:slug>/download_input/<str:input_name>/",
+        views.download_input_view,
+        name="project_download_input",
+    ),
+    path(
         "project/add/",
         views.ProjectCreateView.as_view(),
         name="project_add",
     ),
     path(
         "project/<slug:slug>/charts/",
         views.ProjectChartsView.as_view(),
```

### Comparing `scancodeio-32.4.0/scanpipe/views.py` & `scancodeio-32.5.0/scanpipe/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from django.http import JsonResponse
 from django.shortcuts import get_object_or_404
 from django.shortcuts import redirect
 from django.shortcuts import render
 from django.template.defaultfilters import filesizeformat
 from django.urls import reverse_lazy
 from django.views import generic
+from django.views.decorators.http import require_POST
 from django.views.generic.detail import SingleObjectMixin
 from django.views.generic.edit import FormView
 from django.views.generic.edit import UpdateView
 
 import saneyaml
 import xlsxwriter
 from django_filters.views import FilterView
@@ -949,30 +950,56 @@
         raise Http404("Only non started or queued pipelines can be deleted.")
 
     run.delete_task()
     messages.success(request, f"Pipeline {run.pipeline_name} deleted.")
     return redirect(project)
 
 
+@require_POST
+@conditional_login_required
+def delete_input_view(request, slug, input_name):
+    project = get_object_or_404(Project, slug=slug)
+
+    if not project.can_change_inputs:
+        raise Http404("Inputs cannot be deleted on this project.")
+
+    deleted = project.delete_input(name=input_name)
+    if deleted:
+        messages.success(request, f"Input {input_name} deleted.")
+    else:
+        messages.error(request, f"Input {input_name} not found.")
+    return redirect(project)
+
+
+@conditional_login_required
+def download_input_view(request, slug, input_name):
+    project = get_object_or_404(Project, slug=slug)
+
+    file_path = project.input_path / input_name
+    if not file_path.exists():
+        raise Http404(f"{file_path} not found")
+
+    return FileResponse(file_path.open("rb"), as_attachment=True)
+
+
 def project_results_json_response(project, as_attachment=False):
     """
     Return the results as JSON compatible with ScanCode data format.
     The content is returned as a stream of JSON content using the JSONResultsGenerator
     class.
     If `as_attachment` is True, the response will force the download of the file.
     """
     results_generator = output.JSONResultsGenerator(project)
     response = FileResponse(
         streaming_content=results_generator,
         content_type="application/json",
     )
 
-    filename = output.safe_filename(f"scancodeio_{project.name}.json")
-
     if as_attachment:
+        filename = output.safe_filename(f"scancodeio_{project.name}.json")
         response["Content-Disposition"] = f'attachment; filename="{filename}"'
 
     return response
 
 
 class ProjectResultsView(ConditionalLoginRequired, generic.DetailView):
     model = Project
@@ -1128,23 +1155,43 @@
     model = DiscoveredDependency
     filterset_class = DependencyFilterSet
     template_name = "scanpipe/dependency_list.html"
     paginate_by = settings.SCANCODEIO_PAGINATE_BY.get("dependency", 100)
     prefetch_related = ["for_package", "datafile_resource"]
     table_columns = [
         "package_url",
-        "package_type",
+        {
+            "field_name": "type",
+            "label": "Package type",
+            "filter_fieldname": "type",
+        },
         "extracted_requirement",
-        "scope",
-        "is_runtime",
-        "is_optional",
-        "is_resolved",
+        {
+            "field_name": "scope",
+            "filter_fieldname": "scope",
+        },
+        {
+            "field_name": "is_runtime",
+            "filter_fieldname": "is_runtime",
+        },
+        {
+            "field_name": "is_optional",
+            "filter_fieldname": "is_optional",
+        },
+        {
+            "field_name": "is_resolved",
+            "filter_fieldname": "is_resolved",
+        },
         "for_package",
         "datafile_resource",
-        "datasource_id",
+        {
+            "field_name": "datasource_id",
+            "filter_fieldname": "datasource_id",
+            "filter_is_right": True,
+        },
     ]
 
 
 class ProjectErrorListView(
     ConditionalLoginRequired,
     ProjectRelatedViewMixin,
     TableColumnsMixin,
```

### Comparing `scancodeio-32.4.0/setup.cfg` & `scancodeio-32.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scancodeio
-version = 32.4.0
+version = 32.5.0
 license = Apache-2.0
 description = Automate software composition analysis pipelines
 long_description = file:README.rst
 author = nexB Inc.
 author_email = info@aboutcode.org
 url = https://github.com/nexB/scancode.io
 classifiers = 
@@ -46,70 +46,72 @@
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	importlib-metadata==6.1.0
+	importlib-metadata==6.8.0
 	Django==4.2.3
 	django-environ==0.10.0
 	django-crispy-forms==2.0
 	crispy-bootstrap3==2022.1
 	django-filter==23.2
 	djangorestframework==3.14.0
 	psycopg==3.1.9
 	django-probes==1.7.0
 	rq==1.15.1
 	django-rq==2.8.1
 	redis==4.6.0
 	gunicorn==20.1.0
 	container-inspector==32.0.1
-	scancode-toolkit[packages]==32.0.5rc3
+	scancode-toolkit[packages]==32.0.6
 	extractcode[full]==31.0.0
 	commoncode==31.0.2
 	fetchcode-container==1.2.3.210512; sys_platform == "linux"
 	python-inspector==0.9.7
-	aboutcode-toolkit==8.0.0
+	aboutcode-toolkit==9.0.0
 	XlsxWriter==3.1.2
 	openpyxl==3.1.2
 	requests==2.31.0
 	pyinstrument==4.5.0
-	jsonschema==4.17.3
+	jsonschema==4.18.3
 	cyclonedx-python-lib==3.1.5
 	hoppr-cyclonedx-models==0.4.10
 	fontawesomefree==6.4.0
 
 [options.extras_require]
 dev = 
 	flake8==6.0.0
-	black==23.3.0
+	black==23.7.0
 	isort==5.12.0
 	doc8==0.11.2
 	pydocstyle==6.3.0
 	django-debug-toolbar==4.1.0
-	Sphinx==5.0.2
-	sphinx-rtd-theme==1.0.0
+	Sphinx==5.3.0
+	sphinx-rtd-theme==1.2.2
 	sphinx-rtd-dark-mode==1.2.4
-	sphinxcontrib-django==2.2
+	sphinxcontrib-django==2.4
 	bumpver==2023.1124
 	twine==4.0.2
 
 [options.entry_points]
 console_scripts = 
 	scanpipe = scancodeio:command_line
 scancodeio_pipelines = 
 	deploy_to_develop = scanpipe.pipelines.deploy_to_develop:DeployToDevelop
 	docker = scanpipe.pipelines.docker:Docker
 	docker_windows = scanpipe.pipelines.docker_windows:DockerWindows
 	find_vulnerabilities = scanpipe.pipelines.find_vulnerabilities:FindVulnerabilities
 	inspect_manifest = scanpipe.pipelines.inspect_manifest:InspectManifest
 	load_inventory = scanpipe.pipelines.load_inventory:LoadInventory
+	populate_purldb = scanpipe.pipelines.populate_purldb:PopulatePurlDB
 	root_filesystems = scanpipe.pipelines.root_filesystems:RootFS
 	scan_codebase = scanpipe.pipelines.scan_codebase:ScanCodebase
+	scan_codebase_package = scanpipe.pipelines.scan_codebase_package:ScanCodebasePackage
 	scan_package = scanpipe.pipelines.scan_package:ScanPackage
 
 [isort]
 force_single_line = True
 line_length = 88
 known_django = django
 sections = FUTURE,STDLIB,DJANGO,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
@@ -122,15 +124,15 @@
 ignore = E203,W503
 
 [pydocstyle]
 ignore = D1,D203,D205,D212,D400,D415
 
 [bumpver]
 version_pattern = "MAJOR.MINOR.PATCH"
-current_version = "32.4.0"
+current_version = "32.5.0"
 
 [bumpver:file_patterns]
 setup.cfg = 
 	version = {version}
 	current_version = "{version}"
 scancodeio/__init__.py = {version}
```

### Comparing `scancodeio-32.4.0/setup.py` & `scancodeio-32.5.0/setup.py`

 * *Files identical despite different names*

