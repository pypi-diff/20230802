# Comparing `tmp/invenio-search-ui-2.4.1.tar.gz` & `tmp/invenio-search-ui-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-search-ui-2.4.1.tar", last modified: Thu Apr  6 15:14:18 2023, max compression
+gzip compressed data, was "dist/invenio-search-ui-2.5.0.tar", last modified: Wed Aug  2 16:13:43 2023, max compression
```

## Comparing `invenio-search-ui-2.4.1.tar` & `invenio-search-ui-2.5.0.tar`

### file list

```diff
@@ -1,384 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3734 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/babel-js.ini
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10160 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)    12610 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/app.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js
--rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js
--rw-r--r--   0 runner    (1001) docker     (122)     6957 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/
--rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/context.js
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/defaultComponents.js
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (122)   124321 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     8202 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/searchconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/count.html
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/error.html
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/facets.html
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/loading.html
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/pagination.html
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/range.html
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/results.html
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/selectbox.html
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/togglebutton.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/invenio_search_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     4885 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/invenio_search_ui/search.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/messages-js.pot
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/invenio_search_ui/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/invenio_search_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      522 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2537 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 15:14:18.000000 invenio-search-ui-2.4.1/tests/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/templates/invenio_search_ui/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/templates/invenio_search_ui/base_header.html
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/test_ng_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-06 15:14:13.000000 invenio-search-ui-2.4.1/tests/test_rsk_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3967 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3734 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/babel-js.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10160 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    12610 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/app.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6957 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/context.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/defaultComponents.js
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/
+-rw-r--r--   0 runner    (1001) docker     (122)      898 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (122)      884 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (122)   124321 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8202 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/searchconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/count.html
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/facets.html
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/loading.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/range.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/results.html
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/selectbox.html
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/togglebutton.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/invenio_search_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4885 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/invenio_search_ui/search.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/messages-js.pot
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/invenio_search_ui/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19228 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-02 16:13:42.000000 invenio-search-ui-2.5.0/invenio_search_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      522 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2537 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:13:43.000000 invenio-search-ui-2.5.0/tests/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/templates/invenio_search_ui/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/templates/invenio_search_ui/base_header.html
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/test_ng_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-08-02 16:13:34.000000 invenio-search-ui-2.5.0/tests/test_rsk_templates.py
```

### Comparing `invenio-search-ui-2.4.1/.editorconfig` & `invenio-search-ui-2.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/.github/workflows/pypi-publish.yml` & `invenio-search-ui-2.5.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/.github/workflows/tests.yml` & `invenio-search-ui-2.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/.tx/config` & `invenio-search-ui-2.5.0/.tx/config`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 # Translate python strings
 # 1) Create message catalog:
@@ -21,17 +21,17 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-search-ui-messages]
+[o:inveniosoftware:p:invenio:r:invenio-search-ui-messages]
 file_filter = invenio_search_ui/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_search_ui/translations/messages.pot
 source_lang = en
 type = PO
 
 # Translate JavaScript strings
 # 1) Navigate to the invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/ folder
@@ -56,12 +56,12 @@
 # 9) Pull translations for all languages from Transifex
 #    $ tx pull -a
 # 10) Compile .po files for all languages
 #    $ npm run compile_catalog
 # 11) Convert .po file for a single language
 #    $ npm run compile_catalog lang <lang>
 
-[invenio.invenio-search-ui-messages-js]
+[o:inveniosoftware:p:invenio:r:invenio-search-ui-messages-js]
 file_filter = invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/<lang>/messages.po
 source_file = invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-search-ui-2.4.1/CHANGES.rst` & `invenio-search-ui-2.5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.5.0 (released 2023-08-02)
+
+- search dropdown: add flex to button content
+- pull translations
+
 Version 2.4.1 (released 2023-04-06)
 
 - control maximum search results
 
 Version 2.4.0 (released 2023-03-02)
 
 - remove deprecated flask-babelex dependency and imports
```

### Comparing `invenio-search-ui-2.4.1/CONTRIBUTING.rst` & `invenio-search-ui-2.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/LICENSE` & `invenio-search-ui-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/MANIFEST.in` & `invenio-search-ui-2.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/PKG-INFO` & `invenio-search-ui-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-search-ui
-Version: 2.4.1
+Version: 2.5.0
 Summary: UI for Invenio-Search.
 Home-page: https://github.com/inveniosoftware/invenio-search-ui
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.5.0 (released 2023-08-02)
+        
+        - search dropdown: add flex to button content
+        - pull translations
+        
         Version 2.4.1 (released 2023-04-06)
         
         - control maximum search results
         
         Version 2.4.0 (released 2023-03-02)
         
         - remove deprecated flask-babelex dependency and imports
```

### Comparing `invenio-search-ui-2.4.1/README.rst` & `invenio-search-ui-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/docs/Makefile` & `invenio-search-ui-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/docs/conf.py` & `invenio-search-ui-2.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/docs/customizing.rst` & `invenio-search-ui-2.5.0/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/docs/index.rst` & `invenio-search-ui-2.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/docs/make.bat` & `invenio-search-ui-2.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/__init__.py` & `invenio-search-ui-2.5.0/invenio_search_ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,10 +323,10 @@
         <p>{{ record.metadata.description }}</p>
       </li>
     </ul>
 """
 
 from .ext import InvenioSearchUI
 
-__version__ = "2.4.1"
+__version__ = "2.5.0"
 
 __all__ = ("__version__", "InvenioSearchUI")
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
         } = this.props;
 
         const parsedOptions = this.parsedOptions()
         return ( <
             Dropdown icon = "sort"
             button labeled item trigger = {
                 <
-                span > {
+                span className = "flex align-items-center" > {
                     this.getCurrentlySelectedOption(parsedOptions).text
                 } <
                 Icon name = "dropdown" / >
                 <
                 /span>
             }
             options = {
@@ -86,15 +86,15 @@
             selectOnNavigation = {
                 selectOnNavigation
             }
             selectOnBlur = {
                 false
             }
             size = "large"
-            className = "icon fluid-responsive" /
+            className = "icon fluid-mobile" /
             >
         );
     }
 }
 
 DropdownSort.propTypes = {
     options: PropTypes.array.isRequired,
@@ -138,15 +138,15 @@
             };
         });
 
         return ( <
             Dropdown icon = "filter"
             labeled item button trigger = {
                 <
-                span > {
+                span className = "flex align-items-center" > {
                     filterLabel
                 } <
                 Icon name = "dropdown" / >
                 <
                 /span>
             }
             options = {
@@ -160,15 +160,15 @@
             }
             value = {
                 null
             }
             loading = {
                 loading
             }
-            className = "icon fluid-responsive" {
+            className = "icon fluid-mobile" {
                 ...uiProps
             }
             />
         );
     }
 }
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Afrikaans (http://www.transifex.com/inveniosoftware/invenio/language/af/)\n"
+"Language-Team: Hindi (India) (http://app.transifex.com/inveniosoftware/invenio/language/hi_IN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: af\n"
+"Language: hi_IN\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # 
 # Translators:
-# Bessem Aamira <bessemamira@gmail.com>, 2022
+# Jesús Martín <jesusmartin@sallep.net>, 2017,2022
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (http://www.transifex.com/inveniosoftware/invenio/language/ar/)\n"
+"Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2017,2022\n"
+"Language-Team: Spanish (http://app.transifex.com/inveniosoftware/invenio/language/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ar\n"
-"Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
+"Language: es\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
-msgstr "رتّب"
+msgstr "Ordenar"
 
 msgid "Filter results"
-msgstr "تصفية النتائج "
+msgstr "Filtrar Resultados"
 
 msgid "filters"
-msgstr "تصفيات"
+msgstr "filtros"
 
 msgid "Versions"
-msgstr "الإصدارات"
+msgstr "Versiones"
 
 msgid "View all versions"
-msgstr "الإطلاع على كافة الإصدارات"
+msgstr "Ver todas las versiones"
 
 msgid "Help"
-msgstr "مساعدة"
+msgstr "Ayuda"
 
 msgid "Search guide"
-msgstr "دليل البحث"
+msgstr "Guía de búsqueda"
 
 msgid "Show all sub facets of "
-msgstr "رؤية مزيد من التصفيات الفرعية"
+msgstr "Mostrar todas las subfacetas de"
 
 msgid "Clear selection"
-msgstr "مسح التحدبد"
+msgstr "Borrar selección"
 
 msgid "Clear"
-msgstr "مسح"
+msgstr "Borrar"
 
 msgid "Search records..."
-msgstr "البحث عن تسجيلات..."
+msgstr "Buscar registros..."
 
 msgid "All records"
-msgstr ""
+msgstr "Todos los registros"
 
 msgid "Sort by"
-msgstr "مرتبة حسب"
+msgstr "Ordenado por"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Bulgarian (http://www.transifex.com/inveniosoftware/invenio/language/bg/)\n"
+"Language-Team: Bulgarian (http://app.transifex.com/inveniosoftware/invenio/language/bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Ferran Jorba <Ferran.Jorba@uab.cat>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2018\n"
-"Language-Team: Catalan (http://www.transifex.com/inveniosoftware/invenio/language/ca/)\n"
+"Language-Team: Catalan (http://app.transifex.com/inveniosoftware/invenio/language/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Jiří Kunčar <jiri.kuncar@gmail.com>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2017\n"
-"Language-Team: Czech (http://www.transifex.com/inveniosoftware/invenio/language/cs/)\n"
+"Language-Team: Czech (http://app.transifex.com/inveniosoftware/invenio/language/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Danish (http://www.transifex.com/inveniosoftware/invenio/language/da/)\n"
+"Language-Team: Danish (http://app.transifex.com/inveniosoftware/invenio/language/da/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # chriz_uniba <christina.zeller@uni-bamberg.de>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2021\n"
-"Language-Team: German (http://www.transifex.com/inveniosoftware/invenio/language/de/)\n"
+"Language-Team: German (http://app.transifex.com/inveniosoftware/invenio/language/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Greek (http://www.transifex.com/inveniosoftware/invenio/language/el/)\n"
+"Language-Team: Georgian (http://app.transifex.com/inveniosoftware/invenio/language/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: el\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ka\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Βοήθεια"
+msgstr "დახმარება"
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # 
 # Translators:
-# Jesús Martín <jesusmartin@sallep.net>, 2017,2022
+# Kalven Richie, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2017,2022\n"
-"Language-Team: Spanish (http://www.transifex.com/inveniosoftware/invenio/language/es/)\n"
+"Last-Translator: Kalven Richie, 2022\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/inveniosoftware/invenio/language/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: zh_CN\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
-msgstr "Ordenar"
+msgstr ""
 
 msgid "Filter results"
-msgstr "Filtrar Resultados"
+msgstr "筛选结果"
 
 msgid "filters"
-msgstr "filtros"
+msgstr "筛选"
 
 msgid "Versions"
-msgstr "Versiones"
+msgstr "版本"
 
 msgid "View all versions"
-msgstr "Ver todas las versiones"
+msgstr "查看所有版本"
 
 msgid "Help"
-msgstr "Ayuda"
+msgstr "帮助"
 
 msgid "Search guide"
-msgstr "Guía de búsqueda"
+msgstr "搜索指南"
 
 msgid "Show all sub facets of "
-msgstr "Mostrar todas las subfacetas de"
+msgstr "显示所有的维度"
 
 msgid "Clear selection"
-msgstr "Borrar selección"
+msgstr "清除选择"
 
 msgid "Clear"
-msgstr "Borrar"
+msgstr "清除"
 
 msgid "Search records..."
-msgstr "Buscar registros..."
+msgstr ""
 
 msgid "All records"
-msgstr "Todos los registros"
+msgstr ""
 
 msgid "Sort by"
-msgstr "Ordenado por"
+msgstr "排序方式"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Mart Jantson, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (http://www.transifex.com/inveniosoftware/invenio/language/et/)\n"
+"Language-Team: Estonian (http://app.transifex.com/inveniosoftware/invenio/language/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Estonian (Estonia) (http://www.transifex.com/inveniosoftware/invenio/language/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (http://app.transifex.com/inveniosoftware/invenio/language/et_EE/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Persian (http://www.transifex.com/inveniosoftware/invenio/language/fa/)\n"
+"Language-Team: Persian (http://app.transifex.com/inveniosoftware/invenio/language/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Johnny Mariéthoz <johnny.mariethoz@rero.ch>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Johnny Mariéthoz <johnny.mariethoz@rero.ch>, 2017\n"
-"Language-Team: French (http://www.transifex.com/inveniosoftware/invenio/language/fr/)\n"
+"Language-Team: French (http://app.transifex.com/inveniosoftware/invenio/language/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Galician (http://www.transifex.com/inveniosoftware/invenio/language/gl/)\n"
+"Language-Team: Hungarian (Hungary) (http://app.transifex.com/inveniosoftware/invenio/language/hu_HU/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: gl\n"
+"Language: hu_HU\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Croatian (http://www.transifex.com/inveniosoftware/invenio/language/hr/)\n"
+"Language-Team: Polish (http://app.transifex.com/inveniosoftware/invenio/language/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: hr\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: pl\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Pomoć"
+msgstr "Pomoc"
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Andrea Dömötör, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (http://www.transifex.com/inveniosoftware/invenio/language/hu/)\n"
+"Language-Team: Hungarian (http://app.transifex.com/inveniosoftware/invenio/language/hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Italian (http://www.transifex.com/inveniosoftware/invenio/language/it/)\n"
+"Language-Team: English (Hungary) (http://app.transifex.com/inveniosoftware/invenio/language/en_HU/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: en_HU\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Aiuto"
+msgstr ""
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Japanese (http://www.transifex.com/inveniosoftware/invenio/language/ja/)\n"
+"Language-Team: Japanese (http://app.transifex.com/inveniosoftware/invenio/language/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Georgian (http://www.transifex.com/inveniosoftware/invenio/language/ka/)\n"
+"Language-Team: Italian (http://app.transifex.com/inveniosoftware/invenio/language/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ka\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
 
 msgid "filters"
 msgstr ""
 
 msgid "Versions"
-msgstr ""
+msgstr "Versioni"
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "დახმარება"
+msgstr "Aiuto"
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Lithuanian (http://www.transifex.com/inveniosoftware/invenio/language/lt/)\n"
+"Language-Team: Lithuanian (http://app.transifex.com/inveniosoftware/invenio/language/lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Norwegian (http://www.transifex.com/inveniosoftware/invenio/language/no/)\n"
+"Language-Team: Nepali (http://app.transifex.com/inveniosoftware/invenio/language/ne/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: no\n"
+"Language: ne\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Hjelp"
+msgstr ""
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Polish (http://www.transifex.com/inveniosoftware/invenio/language/pl/)\n"
+"Language-Team: French (Côte d'Ivoire) (http://app.transifex.com/inveniosoftware/invenio/language/fr_CI/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pl\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Language: fr_CI\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Pomoc"
+msgstr ""
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Portuguese (http://www.transifex.com/inveniosoftware/invenio/language/pt/)\n"
+"Language-Team: Portuguese (http://app.transifex.com/inveniosoftware/invenio/language/pt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Romanian (http://www.transifex.com/inveniosoftware/invenio/language/ro/)\n"
+"Language-Team: Romanian (http://app.transifex.com/inveniosoftware/invenio/language/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Russian (http://www.transifex.com/inveniosoftware/invenio/language/ru/)\n"
+"Language-Team: Russian (http://app.transifex.com/inveniosoftware/invenio/language/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Kinyarwanda (http://www.transifex.com/inveniosoftware/invenio/language/rw/)\n"
+"Language-Team: Kinyarwanda (http://app.transifex.com/inveniosoftware/invenio/language/rw/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Ivan Masár <helix84@centrum.sk>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2016\n"
-"Language-Team: Slovak (http://www.transifex.com/inveniosoftware/invenio/language/sk/)\n"
+"Language-Team: Slovak (http://app.transifex.com/inveniosoftware/invenio/language/sk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # 
 # Translators:
 # Sam Arbid, 2022
+# yyones, 2023
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (http://www.transifex.com/inveniosoftware/invenio/language/sv/)\n"
+"Last-Translator: yyones, 2023\n"
+"Language-Team: Swedish (http://app.transifex.com/inveniosoftware/invenio/language/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
@@ -38,17 +39,17 @@
 msgid "Show all sub facets of "
 msgstr "Visa alla underfasetter av "
 
 msgid "Clear selection"
 msgstr "Rensa markering"
 
 msgid "Clear"
-msgstr "Tömma"
+msgstr "Rensa"
 
 msgid "Search records..."
-msgstr "Sök rekord..."
+msgstr "Sök poster..."
 
 msgid "All records"
-msgstr "Alla rekord"
+msgstr "Alla poster"
 
 msgid "Sort by"
 msgstr "Sortera efter"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Ben Translation and Interpreting Services <info@bentercume.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2021\n"
-"Language-Team: Turkish (http://www.transifex.com/inveniosoftware/invenio/language/tr/)\n"
+"Language-Team: Turkish (http://app.transifex.com/inveniosoftware/invenio/language/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Ukrainian (http://www.transifex.com/inveniosoftware/invenio/language/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (http://app.transifex.com/inveniosoftware/invenio/language/uk_UA/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "Допомога"
+msgstr ""
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # 
 # Translators:
-# Kalven Richie, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/inveniosoftware/invenio/language/zh_CN/)\n"
+"Language-Team: German (Austria) (http://app.transifex.com/inveniosoftware/invenio/language/de_AT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_CN\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: de_AT\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
-msgstr "筛选结果"
+msgstr ""
 
 msgid "filters"
-msgstr "筛选"
+msgstr ""
 
 msgid "Versions"
-msgstr "版本"
+msgstr ""
 
 msgid "View all versions"
-msgstr "查看所有版本"
+msgstr ""
 
 msgid "Help"
-msgstr "帮助"
+msgstr ""
 
 msgid "Search guide"
-msgstr "搜索指南"
+msgstr ""
 
 msgid "Show all sub facets of "
-msgstr "显示所有的维度"
+msgstr ""
 
 msgid "Clear selection"
-msgstr "清除选择"
+msgstr ""
 
 msgid "Clear"
-msgstr "清除"
+msgstr ""
 
 msgid "Search records..."
 msgstr ""
 
 msgid "All records"
 msgstr ""
 
 msgid "Sort by"
-msgstr "排序方式"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: InvenioRDM\n"
 "POT-Creation-Date: 2022-10-12T08:17:06.372Z\n"
 "PO-Revision-Date: 2016-10-20 07:42+0000\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/inveniosoftware/invenio/language/zh_TW/)\n"
+"Language-Team: German (Germany) (http://app.transifex.com/inveniosoftware/invenio/language/de_DE/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: de_DE\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Sort"
 msgstr ""
 
 msgid "Filter results"
 msgstr ""
@@ -24,15 +24,15 @@
 msgid "Versions"
 msgstr ""
 
 msgid "View all versions"
 msgstr ""
 
 msgid "Help"
-msgstr "幫助"
+msgstr ""
 
 msgid "Search guide"
 msgstr ""
 
 msgid "Show all sub facets of "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot` & `invenio-search-ui-2.5.0/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/config.py` & `invenio-search-ui-2.5.0/invenio_search_ui/config.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/ext.py` & `invenio-search-ui-2.5.0/invenio_search_ui/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/searchconfig.py` & `invenio-search-ui-2.5.0/invenio_search_ui/searchconfig.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/count.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/count.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/facets.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/facets.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/pagination.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/pagination.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/range.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/range.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/results.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/results.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html` & `invenio-search-ui-2.5.0/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/templates/invenio_search_ui/header.html` & `invenio-search-ui-2.5.0/invenio_search_ui/templates/invenio_search_ui/header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/templates/invenio_search_ui/search.html` & `invenio-search-ui-2.5.0/invenio_search_ui/templates/invenio_search_ui/search.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html` & `invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html` & `invenio-search-ui-2.5.0/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-search-ui 2.1.1*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d31 3920 3133  e: 2016-08-19 13
 000000d0: 3a30 362b 3030 3030 0a4c 6173 742d 5472  :06+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6166  SS>.Language: af
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4166 7269 6b61 616e 7320 2868 7474 7073  Afrikaans (https
-00000130: 3a2f 2f77 7777 2e74 7261 6e73 6966 6578  ://www.transifex
+00000130: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
 00000140: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
 00000150: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
 00000160: 2f61 662f 290a 506c 7572 616c 2d46 6f72  /af/).Plural-For
 00000170: 6d73 3a20 6e70 6c75 7261 6c73 3d32 3b20  ms: nplurals=2; 
 00000180: 706c 7572 616c 3d28 6e20 213d 2031 293b  plural=(n != 1);
 00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/af/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/af/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: bg\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: bg\n"
+"Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Търсене"
+msgstr "Søk"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ca\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: ca\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Cerca"
+msgstr "Caută"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
 "Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-search-ui 2.1.1*

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d31 3920 3133  e: 2016-08-19 13
 000000d0: 3a30 362b 3030 3030 0a4c 6173 742d 5472  :06+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6461  SS>.Language: da
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4461 6e69 7368 2028 6874 7470 733a 2f2f  Danish (https://
-00000130: 7777 772e 7472 616e 7369 6665 782e 636f  www.transifex.co
+00000130: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
 00000140: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
 00000150: 652f 7465 616d 732f 3233 3533 372f 6461  e/teams/23537/da
 00000160: 2f29 0a50 6c75 7261 6c2d 466f 726d 733a  /).Plural-Forms:
 00000170: 206e 706c 7572 616c 733d 323b 2070 6c75   nplurals=2; plu
 00000180: 7261 6c3d 286e 2021 3d20 3129 3b0a 4d49  ral=(n != 1);.MI
 00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/da/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: French (Côte d'Ivoire) (https://app.transifex.com/inveniosoftware/teams/23537/fr_CI/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: da\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fr_CI\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Hermann Schranzhofer <hermann.schranzhofer@tugraz.at>, "
 "2022\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/de/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Hermann Schranzhofer <hermann.schranzhofer@tugraz.at>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Theodoros Theodoropoulos, 2022\n"
 "Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/el/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2016
-# Theodoros Theodoropoulos, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Theodoros Theodoropoulos, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: el\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fa\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Αναζήτηση"
+msgstr "جستجو"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
-msgstr "Φόρτωση..."
+msgstr ""
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/es/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/es/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/et/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/et/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-search-ui 2.1.1*

 * *Files 22% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 000000c0: 653a 2032 3031 362d 3038 2d31 3920 3133  e: 2016-08-19 13
 000000d0: 3a30 362b 3030 3030 0a4c 6173 742d 5472  :06+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 6574  SS>.Language: et
 00000110: 5f45 450a 4c61 6e67 7561 6765 2d54 6561  _EE.Language-Tea
 00000120: 6d3a 2045 7374 6f6e 6961 6e20 2845 7374  m: Estonian (Est
-00000130: 6f6e 6961 2920 2868 7474 7073 3a2f 2f77  onia) (https://w
-00000140: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
+00000130: 6f6e 6961 2920 2868 7474 7073 3a2f 2f61  onia) (https://a
+00000140: 7070 2e74 7261 6e73 6966 6578 2e63 6f6d  pp.transifex.com
 00000150: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
 00000160: 2f74 6561 6d73 2f32 3335 3337 2f65 745f  /teams/23537/et_
 00000170: 4545 2f29 0a50 6c75 7261 6c2d 466f 726d  EE/).Plural-Form
 00000180: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
 00000190: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
 000001a0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001b0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type:
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: fa\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: fa\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: ka\n"
+"Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "جستجو"
+msgstr "ძებნა"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: fr\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Chercher"
+msgstr "Ricerca"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
-msgstr "Chargement..."
+msgstr "Caricamento..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-search-ui 2.1.1*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d31 3920 3133  e: 2016-08-19 13
 000000d0: 3a30 362b 3030 3030 0a4c 6173 742d 5472  :06+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 676c  SS>.Language: gl
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4761 6c69 6369 616e 2028 6874 7470 733a  Galician (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
 00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
 00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
 00000160: 676c 2f29 0a50 6c75 7261 6c2d 466f 726d  gl/).Plural-Form
 00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
 00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
 00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type:
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: hr\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: hr\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: ru\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Pretraži"
+msgstr "Искать"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/it/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # Translations template for invenio-search-ui.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Alizee Pace <alizee.pace@gmail.com>, 2022
+# Tibor Simko <tibor.simko@cern.ch>, 2016
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: ca\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Ricerca"
+msgstr "Cerca"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
-msgstr "Caricamento..."
+msgstr ""
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ja/)\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: no\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
+"teams/23537/no/)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Search"
-msgstr "検索"
+msgstr "Søk"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ka\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: ka\n"
-"Plural-Forms: nplurals=2; plural=(n!=1);\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "ძებნა"
+msgstr "搜尋"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: lt\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/messages-js.pot` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/messages-js.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/messages.pot` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: no\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/no/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/"
+"teams/23537/ro/)\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
+"2:1));\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Search"
-msgstr "Søk"
+msgstr "Caută"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/no/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-search-ui.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: no\n"
+"Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Søk"
+msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: pl\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,19 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-search-ui 2.1.1\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-05-27 08:30+0200\n"
-"PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ro/)\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Search"
-msgstr "Caută"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/teams/23537/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Caută"
+msgstr "Пошук"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: ru\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: hr\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Искать"
+msgstr "Pretraži"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-search-ui 2.1.1*

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 653a 2032 3031 362d 3038 2d31 3920 3133  e: 2016-08-19 13
 000000d0: 3a30 362b 3030 3030 0a4c 6173 742d 5472  :06+0000.Last-Tr
 000000e0: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 000000f0: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 00000100: 5353 3e0a 4c61 6e67 7561 6765 3a20 7277  SS>.Language: rw
 00000110: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
 00000120: 4b69 6e79 6172 7761 6e64 6120 2868 7474  Kinyarwanda (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000130: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000160: 3337 2f72 772f 290a 506c 7572 616c 2d46  37/rw/).Plural-F
 00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
 00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
 00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
 000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
 "Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
+"Last-Translator: Rim Sharif, 2023\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/el/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2016
-# Sam Arbid, 2022
+# Theodoros Theodoropoulos, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Theodoros Theodoropoulos, 2022\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: sv\n"
+"Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Sök"
+msgstr "Αναζήτηση"
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
-msgstr "Sökningen misslyckades."
+msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
-msgstr "Läser in..."
+msgstr "Φόρτωση..."
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2022\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: uk\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/uk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-search-ui.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "Пошук"
+msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
 "Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
-"teams/23537/zh_TW/)\n"
+"Language: ja\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/"
+"teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Search"
-msgstr "搜尋"
+msgstr "検索"
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-search-ui-2.5.0/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-search-ui.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-search-ui
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-search-ui 2.1.1\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-05-27 08:30+0200\n"
 "PO-Revision-Date: 2016-08-19 13:06+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Swedish (Sweden) (https://app.transifex.com/inveniosoftware/teams/23537/sv_SE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.1\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: sv_SE\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_search_ui/templates/invenio_search_ui/header.html:15
 #: invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html:15
 msgid "Search"
-msgstr "搜尋"
+msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:91
 msgid "Search failed."
 msgstr ""
 
 #: invenio_search_ui/templates/invenio_search_ui/search.html:97
 msgid "Loading..."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/views.py` & `invenio-search-ui-2.5.0/invenio_search_ui/views.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui/webpack.py` & `invenio-search-ui-2.5.0/invenio_search_ui/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui.egg-info/PKG-INFO` & `invenio-search-ui-2.5.0/invenio_search_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-search-ui
-Version: 2.4.1
+Version: 2.5.0
 Summary: UI for Invenio-Search.
 Home-page: https://github.com/inveniosoftware/invenio-search-ui
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.5.0 (released 2023-08-02)
+        
+        - search dropdown: add flex to button content
+        - pull translations
+        
         Version 2.4.1 (released 2023-04-06)
         
         - control maximum search results
         
         Version 2.4.0 (released 2023-03-02)
         
         - remove deprecated flask-babelex dependency and imports
```

### Comparing `invenio-search-ui-2.4.1/invenio_search_ui.egg-info/SOURCES.txt` & `invenio-search-ui-2.5.0/invenio_search_ui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 babel-js.ini
 babel.ini
 pyproject.toml
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/i18n-pull.yml
+.github/workflows/i18n-push.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 .tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
@@ -81,42 +83,54 @@
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po
@@ -125,18 +139,20 @@
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/translations.json
+invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/translations.json
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js
 invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js
 invenio_search_ui/static/templates/invenio_search_ui/count.html
@@ -171,49 +187,73 @@
 invenio_search_ui/translations/cs/LC_MESSAGES/messages.po
 invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/da/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/da/LC_MESSAGES/messages.po
 invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/de/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/de/LC_MESSAGES/messages.po
+invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po
+invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po
 invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/el/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/el/LC_MESSAGES/messages.po
+invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po
+invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po
 invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/es/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/es/LC_MESSAGES/messages.po
+invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po
+invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po
 invenio_search_ui/translations/et/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/et/LC_MESSAGES/messages.po
 invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po
 invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/fa/LC_MESSAGES/messages.po
+invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/fr/LC_MESSAGES/messages.po
+invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/gl/LC_MESSAGES/messages.po
+invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/hr/LC_MESSAGES/messages.po
 invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/hu/LC_MESSAGES/messages.po
+invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/it/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/it/LC_MESSAGES/messages.po
 invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/ja/LC_MESSAGES/messages.po
 invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/ka/LC_MESSAGES/messages.po
 invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/lt/LC_MESSAGES/messages.po
+invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/ne/LC_MESSAGES/messages.po
 invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/no/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/no/LC_MESSAGES/messages.po
 invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/pl/LC_MESSAGES/messages.po
 invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po
@@ -230,19 +270,23 @@
 invenio_search_ui/translations/rw/LC_MESSAGES/messages.po
 invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/sk/LC_MESSAGES/messages.po
 invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/sv/LC_MESSAGES/messages.po
+invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/tr/LC_MESSAGES/messages.po
 invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/uk/LC_MESSAGES/messages.po
+invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po
 invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po
 tests/conftest.py
```

### Comparing `invenio-search-ui-2.4.1/requirements-devel.txt` & `invenio-search-ui-2.5.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/run-tests.sh` & `invenio-search-ui-2.5.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/setup.cfg` & `invenio-search-ui-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/conftest.py` & `invenio-search-ui-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/templates/invenio_search_ui/base.html` & `invenio-search-ui-2.5.0/tests/templates/invenio_search_ui/base.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/templates/invenio_search_ui/base_header.html` & `invenio-search-ui-2.5.0/tests/templates/invenio_search_ui/base_header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/test_app.py` & `invenio-search-ui-2.5.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/test_ng_templates.py` & `invenio-search-ui-2.5.0/tests/test_ng_templates.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.4.1/tests/test_rsk_templates.py` & `invenio-search-ui-2.5.0/tests/test_rsk_templates.py`

 * *Files identical despite different names*

