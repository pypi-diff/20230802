# Comparing `tmp/invenio-theme-2.3.0.tar.gz` & `tmp/invenio-theme-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-2.3.0.tar", last modified: Mon Jul 31 08:05:36 2023, max compression
+gzip compressed data, was "dist/invenio-theme-2.4.0.tar", last modified: Wed Aug  2 16:16:05 2023, max compression
```

## Comparing `invenio-theme-2.3.0.tar` & `invenio-theme-2.4.0.tar`

### file list

```diff
@@ -1,477 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1186 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (122)    39567 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/static/base.png
--rw-r--r--   0 runner    (1001) docker     (122)    27194 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/static/cover.png
--rw-r--r--   0 runner    (1001) docker     (122)    45698 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/static/error.png
--rw-r--r--   0 runner    (1001) docker     (122)    48992 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/static/settings.png
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)    18117 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
--rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   256056 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   266158 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   268604 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
--rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    77192 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    49064 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   253461 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
--rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
--rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/static/
--rw-r--r--   0 runner    (1001) docker     (122)    15178 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-120.png
--rw-r--r--   0 runner    (1001) docker     (122)    20939 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-152.png
--rw-r--r--   0 runner    (1001) docker     (122)    23315 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-167.png
--rw-r--r--   0 runner    (1001) docker     (122)    25366 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-180.png
--rw-r--r--   0 runner    (1001) docker     (122)    93062 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/images/invenio-white.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/static/images/square-placeholder.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (122)      288 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/macros/truncate.html
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/401.html
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/403.html
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/429.html
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/500.html
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/body.html
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1526 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
--rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6411 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5364 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5702 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6101 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5259 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      587 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5434 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5553 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5209 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5964 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5777 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/invenio_theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20464 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/invenio_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:05:36.000000 invenio-theme-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5691 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/tests/test_invenio_theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-07-31 08:05:26.000000 invenio-theme-2.3.0/tests/test_invenio_theme_error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6042 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1186 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10064 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7437 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6995 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    39567 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/static/base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27194 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/static/cover.png
+-rw-r--r--   0 runner    (1001) docker     (122)    45698 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/static/error.png
+-rw-r--r--   0 runner    (1001) docker     (122)    48992 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/static/settings.png
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)    18117 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/js/invenio_theme/base.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   256056 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   266158 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   268604 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    77192 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    49064 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   253461 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/breadcrumb.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/table.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (122)     3065 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/flag.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/icon.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/image.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/input.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/list.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/loader.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/rail.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/reveal.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/step.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/reset.variables
+-rw-r--r--   0 runner    (1001) docker     (122)    15218 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/accordion.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/chatroom.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dimmer.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/embed.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/modal.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/nag.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/popup.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/progress.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/rating.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/shape.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sidebar.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/sticky.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/tab.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/transition.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/ad.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/card.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/comment.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/feed.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.variables
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.overrides
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/statistic.variables
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/header.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/type.scss
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (122)    15178 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-120.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20939 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-152.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23315 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-167.png
+-rw-r--r--   0 runner    (1001) docker     (122)    25366 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-180.png
+-rw-r--r--   0 runner    (1001) docker     (122)    93062 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/images/invenio-white.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/static/images/square-placeholder.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/macros/truncate.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2325 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/401.html
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/403.html
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/429.html
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/500.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/body.html
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/javascript.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1526 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2299 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6411 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5364 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5702 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5508 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6101 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5259 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5270 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5217 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5434 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5804 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5350 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5553 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5209 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5964 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1998 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5992 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5777 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/invenio_theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10064 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20464 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/invenio_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:16:05.000000 invenio-theme-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5691 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/tests/test_invenio_theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-08-02 16:15:59.000000 invenio-theme-2.4.0/tests/test_invenio_theme_error_handler.py
```

### Comparing `invenio-theme-2.3.0/.editorconfig` & `invenio-theme-2.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/.github/workflows/pypi-publish.yml` & `invenio-theme-2.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/.github/workflows/tests.yml` & `invenio-theme-2.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/.tx/config` & `invenio-theme-2.4.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/AUTHORS.rst` & `invenio-theme-2.4.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/CHANGES.rst` & `invenio-theme-2.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.4.0 (released 2023-08-02)
+
+- theme: add some general classes and fixes alignment for labeled fluid buttons
+
 Version 2.3.0 (released 2023-07-31)
 
 - settings page: Improve template for a11y
 
 Version 2.2.0 (released 2023-07-26)
 
 - theme: add general style improvements
```

### Comparing `invenio-theme-2.3.0/CONTRIBUTING.rst` & `invenio-theme-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/LICENSE` & `invenio-theme-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/MANIFEST.in` & `invenio-theme-2.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/PKG-INFO` & `invenio-theme-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme
-Version: 2.3.0
+Version: 2.4.0
 Summary: "Invenio standard theme."
 Home-page: https://github.com/inveniosoftware/invenio-theme
 Author: Invenio Collaboration
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.4.0 (released 2023-08-02)
+        
+        - theme: add some general classes and fixes alignment for labeled fluid buttons
+        
         Version 2.3.0 (released 2023-07-31)
         
         - settings page: Improve template for a11y
         
         Version 2.2.0 (released 2023-07-26)
         
         - theme: add general style improvements
```

### Comparing `invenio-theme-2.3.0/README.rst` & `invenio-theme-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/Makefile` & `invenio-theme-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/conf.py` & `invenio-theme-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/index.rst` & `invenio-theme-2.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/make.bat` & `invenio-theme-2.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/static/base.png` & `invenio-theme-2.4.0/docs/static/base.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/static/cover.png` & `invenio-theme-2.4.0/docs/static/cover.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/static/error.png` & `invenio-theme-2.4.0/docs/static/error.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/docs/static/settings.png` & `invenio-theme-2.4.0/docs/static/settings.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/__init__.py` & `invenio-theme-2.4.0/invenio_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,10 +517,10 @@
     def settings_item_1():
         flash('Testing flashing', category='info')
         return render_template('...')
 """
 
 from .ext import InvenioTheme
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 __all__ = ("__version__", "InvenioTheme")
```

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss` & `invenio-theme-2.4.0/invenio_theme/assets/bootstrap3/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/Media.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/admin.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/templates.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/js/invenio_theme/truncate.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.eot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/navbar/navbar.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/grid.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/collections/message.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/divider.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/header.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/label.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/elements/segment.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.overrides`

 * *Files 2% similar despite different names*

```diff
@@ -453,20 +453,22 @@
 .auto-column-grid {
   // used on a container with two children <div>
   // provides auto adjustment to the content of the left column
   // and auto fills the width on the right
   // [   COL1 (auto fill remaining space)  ] [  COL2 (max-content width)   ]
   display: grid;
   grid-auto-flow: column;
-  grid-auto-columns: auto max-content;
+  grid-template-columns: auto max-content;
+  grid-auto-columns: max-content;
   align-items: center;
-  column-gap: 2rem;
+  column-gap: 1rem;
 
-  @media all and (max-width: @largestMobileScreen) {
+  @media all and (max-width: @largestTabletScreen) {
     grid-auto-flow: row;
+    grid-template-columns: minmax(100%, 100%);
     grid-auto-columns: 100%;
     align-items: flex-start;
     row-gap: 1rem;
   }
 
   > *:nth-child(2) {
     @media all and (min-width: @computerBreakpoint) {
@@ -479,14 +481,18 @@
   justify-content: space-between;
 }
 
 .justify-center {
   justify-content: center;
 }
 
+.justify-end {
+  justify-content: flex-end;
+}
+
 .align-items-start {
   align-items: start;
 }
 
 .align-items-baseline {
   align-items: baseline;
 }
```

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/dropdown.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/modules/search.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme/views/item.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/less/invenio_theme/theme.config.example`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/admin.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/angular.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/body.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/cover.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/input-icon.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/navbar.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/styles.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss` & `invenio-theme-2.4.0/invenio_theme/assets/semantic-ui/scss/invenio_theme/variables.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/config.py` & `invenio-theme-2.4.0/invenio_theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/ext.py` & `invenio-theme-2.4.0/invenio_theme/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/proxies.py` & `invenio-theme-2.4.0/invenio_theme/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-120.png` & `invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-120.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-152.png` & `invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-152.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-167.png` & `invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-167.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/apple-touch-icon-180.png` & `invenio-theme-2.4.0/invenio_theme/static/apple-touch-icon-180.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/favicon.ico` & `invenio-theme-2.4.0/invenio_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/images/invenio-white.svg` & `invenio-theme-2.4.0/invenio_theme/static/images/invenio-white.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/static/images/square-placeholder.png` & `invenio-theme-2.4.0/invenio_theme/static/images/square-placeholder.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/500.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/500.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/admin_header.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/admin_layout.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/breadcrumbs.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/footer.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header_frontpage.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/header_login.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/macros/messages.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/macros/messages.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/macros/truncate.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/macros/truncate.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_admin.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_cover.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/invenio_theme/page_settings.html` & `invenio-theme-2.4.0/invenio_theme/templates/invenio_theme/page_settings.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/admin_layout.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header_frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/macros/messages.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_admin.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_cover.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html` & `invenio-theme-2.4.0/invenio_theme/templates/semantic-ui/invenio_theme/page_settings.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/af/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/da/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/el/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/et/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/it/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/messages.pot` & `invenio-theme-2.4.0/invenio_theme/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/no/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-theme-2.4.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-theme-2.4.0/invenio_theme/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/views.py` & `invenio-theme-2.4.0/invenio_theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme/webpack.py` & `invenio-theme-2.4.0/invenio_theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/invenio_theme.egg-info/PKG-INFO` & `invenio-theme-2.4.0/invenio_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme
-Version: 2.3.0
+Version: 2.4.0
 Summary: "Invenio standard theme."
 Home-page: https://github.com/inveniosoftware/invenio-theme
 Author: Invenio Collaboration
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -48,14 +48,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.4.0 (released 2023-08-02)
+        
+        - theme: add some general classes and fixes alignment for labeled fluid buttons
+        
         Version 2.3.0 (released 2023-07-31)
         
         - settings page: Improve template for a11y
         
         Version 2.2.0 (released 2023-07-26)
         
         - theme: add general style improvements
```

### Comparing `invenio-theme-2.3.0/invenio_theme.egg-info/SOURCES.txt` & `invenio-theme-2.4.0/invenio_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/requirements-devel.txt` & `invenio-theme-2.4.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/setup.cfg` & `invenio-theme-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/tests/conftest.py` & `invenio-theme-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/tests/helpers.py` & `invenio-theme-2.4.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/tests/test_invenio_theme.py` & `invenio-theme-2.4.0/tests/test_invenio_theme.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-2.3.0/tests/test_invenio_theme_error_handler.py` & `invenio-theme-2.4.0/tests/test_invenio_theme_error_handler.py`

 * *Files identical despite different names*

